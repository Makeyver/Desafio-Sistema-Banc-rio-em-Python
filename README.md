# Desafio-Sistema-bancário-em-Python
menu = """

[0] Depositar
[1] Sacar
[2] Extrato
[3] Sair

=> """

saldo = 0
limite = 500
extrato = ""
numero_saques = 0
LIMITE-SAQUES = 3

while True:

     opcao = input(menu)

     if opcao == "0":
        valor = float(input("Informe o valor que voce deseja depositar: ":))

        if valor > 0:
        saldo == valor

        extrato == f"Depósito: R$ {valor:.2f}/n"

        else:
            print("Operação falhou! O valor informado é inválido. Tente novamente!")
    
    elif opção == "1":
        valor = float(input("Informe o valor que deseja sacar: "))

        excedeu_saldo = valor > saldo

        excedeu_limite = valor > limite

        excedeu_saques = numero_saques >= LIMITE_SAQUES

        if excedeu-saldo:
            print("Operação falhou! Voce não tem saldo suficiente.")

        elif excedeu-limite:
            print("Operação falhou! O valor do saque excede o limite.")

        elif excedeu-saques:
            print("Operação falhou! Você atingiu o limite de saque diário. Tente amanha!")

        elif valor > 0:
            saldo -= valor
            extrato += f"Saque: R$ {valor:.2f}\n"
            numero-saques += 1
    
    elif opcao == "2":
        print("\n**************** EXTRATO ****************")
        print(Não foram realizadas movimentações neste dia." if not extrato else extrato)
        print(f"\nSaldo: R$ {saldo:.2f}")
        print("*****************************************")

    elif opcao == "3":
        break

    else:
    print("Operação inválida, por favor selecione novamente a operação desejada.")