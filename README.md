# Estagi-rio-Ribeir-o-preto
# 1) Observe o trecho de código abaixo:

int INDICE = 13, SOMA = 0, K = 0;

enquanto K < INDICE faça

{

K = K + 1;

SOMA = SOMA + K;

}

imprimir(SOMA);



# Ao final do processamento, qual será o valor da variável SOMA? 91

# 2) Dado a sequência de Fibonacci, onde se inicia por 0 e 1 e o próximo valor sempre será a soma dos 2 valores anteriores (exemplo: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34...), escreva um programa na linguagem que desejar onde, informado um número, ele calcule a sequência de Fibonacci e retorne uma mensagem avisando se o número informado pertence ou não a sequência.
#  IMPORTANTE: Esse número pode ser informado através de qualquer entrada de sua preferência ou pode ser previamente definido no código;


def verifica_fibonacci(num):
    fibonacci = [0, 1]
    while fibonacci[-1] < num:
        fibonacci.append(fibonacci[-1] + fibonacci[-2])
    if num in fibonacci:
        return f"O número {num} pertence à sequência de Fibonacci."
    else:
        return f"O número {num} não pertence à sequência de Fibonacci."

numero = int(input("Digite um número: "))
print(verifica_fibonacci(numero))

3) Descubra a lógica e complete o próximo elemento:

a) 1, 3, 5, 7, ___
  R: 1, 3, 5, 7, 9, 11, 13...

b) 2, 4, 8, 16, 32, 64, ____
  R: 2, 4, 8, 16, 32, 64, 120, 240, 480...

c) 0, 1, 4, 9, 16, 25, 36, ____
  R: 0, 1, 4, 9, 16, 25, 36, 49, 64

d) 4, 16, 36, 64, ____
  R : 4, 16, 36, 64, 100

e) 1, 1, 2, 3, 5, 8, ____
R: 1, 1, 2, 3, 5, 8, 13

f) 2,10, 12, 16, 17, 18, 19, ____
 R: 2,10, 12, 16, 17, 18, 19, 20

# 4) Você está em uma sala com três interruptores, cada um conectado a uma lâmpada em uma sala diferente. Você não pode ver as lâmpadas da sala em que está, mas pode ligar e desligar os interruptores quantas vezes quiser. Seu objetivo é descobrir qual interruptor controla qual lâmpada.
# Como você faria para descobrir, usando apenas duas idas até uma das salas das lâmpadas, qual interruptor controla cada lâmpada?
R: Ligava duas lampadas e iria conferir, depois desligava uma das que eu tinha ligado e volta pra ver qual desligou, assim sabendo qual é qual.

# 5) Escreva um programa que inverta os caracteres de um string.
# IMPORTANTE:
# a) Essa string pode ser informada através de qualquer entrada de sua preferência ou pode ser previamente definida no código;
# b) Evite usar funções prontas, como, por exemplo, reverse;

def inverte_caracteres(string):
    inverso = ''
    for i in range(len(string)):
        inverso = string[i] + inverso
    return inverso

string = input("Digite uma string: ")
print(inverte_caracteres(string))

