'''
Faça uma lista de compras com lista
O usuario deve ter a possibilidade de inserir, apagar e listar valores da sua lista
Não permita que o programa quebre com erros de indices inexistentes na lista
'''

import os
compras=[]
opcao = 'I','A','L','S'
opcao_input = ''

while opcao_input != 'S':
    opcao_input = input('Escolha uma opção: [I]nserir, [A]pagar, [L]istar, [S]air: ').upper()

    if opcao_input not in opcao:
        os.system('clear')
        print('Opção invalida')
        continue

    if opcao_input == 'I':
        os.system('clear')
        item = input('Digite o item a ser inserido: ')
        compras.append(item)
        os.system('clear')
        print('Item inserido com sucesso')

    elif opcao_input == 'A':

        try:
            item = int(input('Digite o indicie do item a ser apagado: '))
            if item <= len(compras):
                compras.pop(item)

        except ValueError:
            print('Indicie invalido')

        except:
            continue
        

    elif opcao_input == 'L':
        os.system('clear')
        
        if len(compras) == 0:
            print('Não há nenhum item na lista')
        
        else:

            for indicie, item in enumerate(compras):
                print(f'{indicie} - {item}')
                
    elif opcao_input == 'S':
        os.system('clear')
        print('Saindo...')	

    else:
        os.system('clear')
        print(f'Opção "{opcao_input}" inválida!')
