# JogoDeAdivinhacao
#Projeto para rodar na linha de comando que ao iniciar, irá gerar, armazenar, porem não exibir um valor aleatório entre um valor mínimo e máximo definido.

from random import randint

numero = randint(1,11)

print("Olá, este é um jogo de adivinhação de 0 a 10.")

correto = False
chutes = 0

while not correto:
    deducao = int(input("Digite um número: "))
    chutes += 1
    if deducao == numero:
        correto = True

print("Isso mesmo! Você é bom(a) de adivinhação!")
print("Número de palpites: {0}".format(chutes))
