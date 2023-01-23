# JOKENPÔ
from time import sleep
import random

def iniciar():
    global nome
    print('\033[1;34m-=\033[m' * 5)
    print('\033[1;34m JoKenPô\033[m')
    print('\033[1;34m-=\033[m' * 5)

    nome = input('Digite seu nome: ')
    nome = nome.upper()
    if nome == "":
        nome = 'HUMANO'
        return nome

def jogar():
    jkp = ['PEDRA',
       'PAPEL',
       'TESOURA']

    esc = (str(input('Pedra, Papel ou Tesoura? ').upper().strip()))
    while esc != 'PEDRA' and esc != 'PAPEL' and esc != 'TESOURA':
        print('Tente novamente...')
        esc = (str(input('Pedra, Papel ou Tesoura? ').upper().strip()))

# PC
    print('Jo', end='')
    sleep(1)
    print('Ken', end='')
    sleep(1)
    print('Pô!')
    pc = random.choice(jkp)
    print('{} escolheu {}.'.format(nome, esc))
    print('COMPUTADOR escolheu {}.'.format(pc))

# PC PERDE
    if (esc == 'PEDRA' and pc == "TESOURA") or (esc == 'PAPEL' and pc == 'PEDRA') or (
            esc == 'TESOURA' and pc == 'PAPEL'):
        print('Você ganhou!!\n')

    elif esc == pc:
        print('Empatou!\n')
# PC GANHA:
    else:
        print('Você perdeu!!\n')

    sleep(1)
    novo = (input('Tentar novamente?\n 1) SIM\n 2) NÃO\n Digite sua resposta: '))
    while novo != '1' and novo != '2':

        print('Não entendi...')
        sleep(1)
        novo = (input('Tentar novamente\n 1) SIM\n 2) NÃO\n Digite sua resposta: '))

    if novo == '1':
        jogar()

    else:
        print(' FIM DE JOGO\n Desenvolvido por @liliansom(Github).')

if __name__ == "__main__":
    iniciar()
    jogar()

