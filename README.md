# Calculadora2
Segundo exercício_ Calculadora

def calculadora():
    while True:
        print("1: Soma")
        print("2: Subtração")
        print("3: Multiplicação")
        print("4: Divisão")
        print("0: Sair")
        
        operacao = int(input("Digite o número para a operação correspondente: "))
        
        if operacao == 0:
            print("Saindo...")
            break
        elif operacao >= 1 and operacao <= 4:
            num1 = float(input("Digite o primeiro número: "))
            num2 = float(input("Digite o segundo número: "))
            
            if operacao == 1:
                resultado = num1 + num2
            elif operacao == 2:
                resultado = num1 - num2
            elif operacao == 3:
                resultado = num1 * num2
            elif operacao == 4:
                if num2 != 0:
                    resultado = num1 / num2
                else:
                    print("Não é possível dividir por zero!")
                    continue
            
            print("Resultado:", resultado)
        else:
            print("Essa opção não existe!")

calculadora()
