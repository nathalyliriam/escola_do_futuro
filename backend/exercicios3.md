1. Escreva um programa que mostre na tela a seguinte contagem: 6 7 8 9 10 11
Acabou!
for i in range(6, 12):
    print(i, end=" ")
print("Acabou!")


2. Faça um algoritmo que mostre na tela a seguinte contagem: 10 9 8 7 6 5 4 3
Acabou!
programa {
  funcao inicio() {
    inteiro c = 10
    enquanto (c >= 3) {
      escreva(c + " ")
      c = c - 1 // Decremento
    }
    escreva("Acabou!")
  }
}


3. Crie um aplicativo que mostre na tela a seguinte contagem: 0 3 6 9 12 15 18
Acabou!
for i in range(0, 19, 3):
    print(i, end=" ")
print("Acabou!")


4. Desenvolva um programa que mostre na tela a seguinte contagem: 100 95 90 85 80
... 0 Acabou!
programa {
  funcao inicio() {
    inteiro c = 100
    enquanto (c >= 0) {
      escreva(c + " ")
      c = c - 5 
    }
    escreva("Acabou!")
  }
}


5. Faça um algoritmo que pergunte ao usuário um número inteiro e positivo qualquer e
mostre uma contagem até esse valor: Ex: Digite um valor: 35 Contagem: 1 2 3 4 5
programa {
  funcao inicio() {
    inteiro valor, c = 1
    escreva("Digite um valor: ")
    leia(valor)
    escreva("Contagem: ")
    enquanto (c <= valor) {
      escreva(c + " ")
      c = c + 1
    }
    escreva("Acabou!")
  }
}


6.Desenvolva um algoritmo que mostre uma contagem regressiva de 30 até 1, marcando os números que são divisíveis por 4, exatamente
como mostrado abaixo: 30 29 [28] 27 26 25 [24] 23 22 21 [20] 19 18 17 [16]...

programa {
  funcao inicio() {
    inteiro c = 30
    enquanto (c >= 1) {
      se (c % 4 == 0) {
        escreva("[" + c + "] ")
      } senao {
        escreva(c + " ")
      }
      c = c - 1
    }
    escreva("Acabou!")
  }
}


7. Desenvolva um algoritmo que mostre uma contagem regressiva de 30 até 1,
marcando os números que forem divisíveis por 4, exatamente como mostrado
abaixo: 30 29 [28] 27 26 25 [24] 23 22 21 [20] 19 18 17 [16]...
programa {
  funcao inicio() {
    inteiro contador = 30

    enquanto (contador >= 1) {
      // Verifica se o número é divisível por 4
      se (contador % 4 == 0) {
        escreva("[" , contador , "] ")
      }
      senao {
        escreva(contador , " ")
      }
      
      contador = contador - 1 // Diminui 1 a cada volta
    }
    
    escreva("Acabou!")
  }
}



8. Crie um algoritmo que leia o valor inicial da contagem, o valor final e o incremento,
mostrando em seguida todos os valores no intervalo: Ex: Digite o primeiro Valor: 3
Digite o último Valor: 10 Digite o incremento: 2 Contagem: 3 5 7 9 Acabou!




 9. Crie um programa que calcule e mostre na tela o resultado da soma entre 6 + 8 + 10
12 + 14 + ... + 98 + 100.
\(S_{n}=\frac{n(a_{1}+a_{n})}{2}\)\(S_{48}=\frac{48(6+100)}{2}\)\(S_{48}=24\cdot 106=2544\)

10. Desenvolva um aplicativo que mostre na tela o resultado da expressão 500 + 450 +
400 + 350 + 300 + ... + 50 + 0.
# Inicialização das variáveis
soma = 0
numero = 500

# Estrutura de repetição decrescente
while numero >= 0:
    soma += numero
    numero -= 50

# Exibição do resultado
print(f"O resultado da expressão é: {soma}")


11. Faça um programa que leia 7 números inteiros e no final mostre o somatório entre
soma = 0
cont = 1

while cont <= 7:
    try:
        num = int(input(f"Digite o {cont}º número inteiro: "))
        soma += num
        cont += 1 # Só avança se o número for válido
    except ValueError:
        print("Entrada inválida! Por favor, digite apenas números inteiros.")

print("-" * 30)
print(f"A soma total dos 7 números é: {soma}")

12. Crie um programa que leia 6 números inteiros e no final mostre quantos deles são pares e quantos são ímpares.
    pares = 0
impares = 0

for i in range(1, 7):
    num = int(input(f"Digite o {i}º número inteiro: "))
    
    # Verifica se o número é par
    if num % 2 == 0:
        pares += 1
    else:
        impares += 1

print("-" * 30)
print(f"Total de números PARES: {pares}")
print(f"Total de números ÍMPARES: {impares}")

13.Desenvolva um programa que faça o sorteio de 20 números entre 0 e 10 e mostre na tela: a) Quais foram os números sorteados b)
import random

sorteados = []
acima_cinco = 0

# Realizando os 20 sorteios
for i in range(20):
    num = random.randint(0, 10)
    sorteados.append(num)
    
    # Lógica para o provável item b (contar maiores que 5)
    if num > 5:
        acima_cinco += 1

# Item a) Mostrar os números sorteados
print(f"Números sorteados: {sorteados}")

# Item b) Mostrar a contagem de números acima de 5
print(f"Quantidade de números acima de 5: {acima_cinco}")


 14. Crie um programa que leia 6 números inteiros e no final mostre quantos deles são pares e quantos são ímpares.
 #include <stdio.h>
#include <locale.h>

int main() {
    // Configura o console para aceitar acentos (opcional)
    setlocale(LC_ALL, "Portuguese");

    int numero;
    int pares = 0;
    int impares = 0;

    printf("--- Contador de Pares e Ímpares ---\n\n");

    // Laço para ler 6 números
    for (int i = 1; i <= 6; i++) {
        printf("Digite o %dº número inteiro: ", i);
        scanf("%d", &numero);

        // Verifica se o resto da divisão por 2 é zero
        if (numero % 2 == 0) {
            pares++; // Incrementa contador de pares
        } else {
            impares++; // Incrementa contador de ímpares
        }
    }

    // Exibe os resultados finais
    printf("\n-------------------------------\n");
    printf("Total de números pares: %d\n", pares);
    printf("Total de números ímpares: %d\n", impares);
    printf("-------------------------------\n");

    return 0;
}
15.Crie um algoritmo que leia a idade de 10 pessoas, mostrando no final: a) Qual é a média de idade do grupo b) Quantas pessoas tem mais de 18 anos c) Quantas pessoas tem menos de 5 anos d) Qual foi a maior idade lida
algoritmo "Analise_Grupo_10_Pessoas"
var
   cont, idade, somaIdade, maior18, menor5, maiorIdade: inteiro
   media: real
inicio
   // Inicialização de variáveis
   somaIdade <- 0
   maior18 <- 0
   menor5 <- 0
   maiorIdade <- 0
   
   // Laço para ler a idade de 10 pessoas
   para cont de 1 ate 10 faca
      escreva("Digite a idade da ", cont, "ª pessoa: ")
      leia(idade)
      
      // Acumula a idade para calcular a média depois
      somaIdade <- somaIdade + idade
      
      // b) Conta pessoas com mais de 18 anos
      se (idade > 18) entao
         maior18 <- maior18 + 1
      fimse
      
      // c) Conta pessoas com menos de 5 anos
      se (idade < 5) entao
         menor5 <- menor5 + 1
      fimse
      
      // d) Verifica a maior idade lida
      se (idade > maiorIdade) entao
         maiorIdade <- idade
      fimse
   fimpara
   
   // a) Cálculo da média
   media <- somaIdade / 10
   
   // Exibição dos resultados
   escreval("-----------------------------------------")
   escreval("Média de idade do grupo: ", media:5:2)
   escreval("Pessoas com mais de 18 anos: ", maior18)
   escreval("Pessoas com menos de 5 anos: ", menor5)
   escreval("A maior idade lida foi: ", maiorIdade, " anos")
fimalgoritmo


16.Faça um programa que leia a idade e o sexo de 5 pessoas, mostrando no final: a) Quantos homens foram cadastrados b)
Quantas mulheres foram cadastradas c) A média de idade do grupo d) A média de idade dos homens e) Quantas mulheres têm mais de 20 anos   
  algoritmo "Analise_Grupo_5_Pessoas"
var
   cont, idade, sex: inteiro
   somaIdade, somaIdadeHomens, totalHomens, totalMulheres, mulheresMais20: inteiro
   mediaGrupo, mediaHomens: real
inicio
   // Inicialização
   totalHomens <- 0
   totalMulheres <- 0
   somaIdade <- 0
   somaIdadeHomens <- 0
   mulheresMais20 <- 0

   para cont de 1 ate 5 faca
      escreval("--- ", cont, "ª PESSOA ---")
      escreva("Idade: ")
      leia(idade)
      escreva("Sexo [1] Masc / [2] Fem: ")
      leia(sex)

      somaIdade <- somaIdade + idade

      // Processamento por sexo
      se (sex = 1) entao
         totalHomens <- totalHomens + 1
         somaIdadeHomens <- somaIdadeHomens + idade
      senao
         totalMulheres <- totalMulheres + 1
         se (idade > 20) entao
            mulheresMais20 <- mulheresMais20 + 1
         fimse
      fimse
   fimpara

   // Cálculos das médias
   mediaGrupo <- somaIdade / 5
   se (totalHomens > 0) entao
      mediaHomens <- somaIdadeHomens / totalHomens
   senao
      mediaHomens <- 0
   fimse

   // Resultados
   escreval("================================")
   escreval("a) Total de homens: ", totalHomens)
   escreval("b) Total de mulheres: ", totalMulheres)
   escreval("c) Média de idade do grupo: ", mediaGrupo:5:2)
   escreval("d) Média de idade dos homens: ", mediaHomens:5:2)
   escreval("e) Mulheres com mais de 20 anos: ", mulheresMais20)
fimalgoritmo


17. Crie um programa que leia 6 números inteiros e no final mostre quantos deles são
pares e quantos são ímpares.
algoritmo "ContaParesImpares"
var
   cont, num, pares, impares: inteiro
inicio
   pares <- 0
   impares <- 0

   para cont de 1 ate 6 faca
      escreva("Digite o ", cont, "º número: ")
      leia(num)

      se (num % 2 = 0) entao
         pares <- pares + 1
      senao
         impares <- impares + 1
      fimse
   fimpara

   escreval("---------------------------")
   escreval("Total de números pares: ", pares)
   escreval("Total de números ímpares: ", impares)
fimalgoritmo



18. Desenvolva um programa que faça o sorteio de 20 números entre 0 e 10 e mostre
na tela: a) Quais foram os números sorteados b) Quantos números estão acima de 5
c) Quantos números são divisíveis por 3
algoritmo "Sorteio20Numeros"
var
   cont, num, acima5, div3: inteiro
   listaSorteados: caractere
inicio
   acima5 <- 0
   div3 <- 0
   listaSorteados <- ""

   para cont de 1 ate 20 faca
      // Sorteia entre 0 e 10
      num <- randi(11) 
      listaSorteados <- listaSorteados + dexp(num) + " "

      // b) Conta números acima de 5
      se (num > 5) entao
         acima5 <- acima5 + 1
      fimse

      // c) Conta divisíveis por 3 (incluindo o 0)
      se (num % 3 = 0) entao
         div3 <- div3 + 1
      fimse
   fimpara

   escreval("a) Números sorteados: ", listaSorteados)
   escreval("b) Total de números acima de 5: ", acima5)
   escreval("c) Total de números divisíveis por 3: ", div3)
fimalgoritmo



19. Faça um aplicativo que leia o preço de 8 produtos. No final, mostre na tela qual foi o
maior e qual foi o menor preço digitados.



20. Crie um algoritmo que leia a idade de 10 pessoas, mostrando no final: a) Qual é a
média de idade do grupo b) Quantas pessoas tem mais de 18 anos c) Quantas
pessoas tem menos de 5 anos d) Qual foi a maior idade lida
algoritmo "MaiorMenorPreco"
var
   cont: inteiro
   preco, maior, menor: real
inicio
   // Laço para ler os 8 produtos
   para cont de 1 ate 8 faca
      escreva("Digite o preço do ", cont, "º produto: R$ ")
      leia(preco)

      // Na primeira repetição, o preço lido é tanto o maior quanto o menor
      se (cont = 1) entao
         maior <- preco
         menor <- preco
      senao
         // Verifica se o novo preço é maior que o recordista atual
         se (preco > maior) entao
            maior <- preco
         fimse
         // Verifica se o novo preço é menor que o recordista atual
         se (preco < menor) entao
            menor <- preco
         fimse
      fimse
   fimpara

   escreval("--------------------------------")
   escreval("O MAIOR preço digitado foi: R$ ", maior:5:2)
   escreval("O MENOR preço digitado foi: R$ ", menor:5:2)
fimalgoritmo



21. Faça um programa que leia a idade e o sexo de 5 pessoas, mostrando no final: a)
Quantos homens foram cadastrados b) Quantas mulheres foram cadastradas c) A
média de idade do grupo d) A média de idade dos homens e) Quantas mulheres tem
mais de 20 anos

algoritmo "Analise_Grupo_Completo"
var
   cont, idade, sex: inteiro
   somaIdade, somaIdadeHomens, totH, totM, m20: inteiro
   mediaG, mediaH: real
inicio
   totH <- 0; totM <- 0; somaIdade <- 0; somaIdadeHomens <- 0; m20 <- 0

   para cont de 1 ate 5 faca
      escreval("Dados da ", cont, "ª pessoa:")
      escreva("Idade: ")
      leia(idade)
      escreva("Sexo [1-Masc / 2-Fem]: ")
      leia(sex)

      somaIdade <- somaIdade + idade

      se (sex = 1) entao
         totH <- totH + 1
         somaIdadeHomens <- somaIdadeHomens + idade
      senao
         totM <- totM + 1
         se (idade > 20) entao
            m20 <- m20 + 1
         fimse
      fimse
   fimpara

   mediaG <- somaIdade / 5
   
   // Evita divisão por zero se não houver homens
   se (totH > 0) entao
      mediaH <- somaIdadeHomens / totH
   senao
      mediaH <- 0
   fimse

   escreval("--- RESULTADOS ---")
   escreval("a) Homens cadastrados: ", totH)
   escreval("b) Mulheres cadastradas: ", totM)
   escreval("c) Média de idade do grupo: ", mediaG:5:2)
   escreval("d) Média de idade dos homens: ", mediaH:5:2)
   escreval("e) Mulheres com mais de 20 anos: ", m20)
fimalgoritmo


22. Desenvolva um aplicativo que leia o peso e a altura de 7 pessoas, mostrando no
final: a) Qual foi a média de altura do grupo b) Quantas pessoas pesam mais de
90Kg c) Quantas pessoas que pesam menos de 50Kg tem menos de 1.60m d)
Quantas pessoas que medem mais de 1.90m pesam mais de 100Kg.
algoritmo "AnalisePesoAltura"
var
   cont, p90, p50h160, h190p100: inteiro
   peso, altura, somaH, mediaH: real
inicio
   p90 <- 0; p50h160 <- 0; h190p100 <- 0; somaH <- 0

   para cont de 1 ate 7 faca
      escreval("Pessoa ", cont)
      escreva("Peso (Kg): ")
      leia(peso)
      escreva("Altura (m): ")
      leia(altura)

      somaH <- somaH + altura

      se (peso > 90) entao
         p90 <- p90 + 1
      fimse

      se (peso < 50) e (altura < 1.60) entao
         p50h160 <- p50h160 + 1
      fimse

      se (altura > 1.90) e (peso > 100) entao
         h190p100 <- h190p100 + 1
      fimse
   fimpara

   mediaH <- somaH / 7

   escreval("--------------------------------")
   escreval("a) Média de altura do grupo: ", mediaH:5:2, "m")
   escreval("b) Pessoas com mais de 90Kg: ", p90)
   escreval("c) Pessoas <50Kg e <1.60m: ", p50h160)
   escreval("d) Pessoas >1.90m e >100Kg: ", h190p100)
fimalgoritmo



23. $$DESAFIO$$
Vamos melhorar o jogo. A partir de agora, o
computador vai sortear um número entre 1 e 10 e o jogador vai ter 4 tentativas para
tentar acertar.
algoritmo "JogoAdivinhacaoDesafio"
var
   cont, numSorteado, chute: inteiro
   acertou: logico
inicio
   // O computador sorteia um número entre 1 e 10
   numSorteado <- randi(10) + 1
   acertou <- falso

   escreval("=== JOGO DE ADIVINHAÇÃO ===")
   escreval("Tente acertar o número que sorteei (1 a 10).")
   escreval("Você tem 4 tentativas!")

   para cont de 1 ate 4 faca
      escreva(cont, "ª tentativa: ")
      leia(chute)

      se (chute = numSorteado) entao
         acertou <- verdadeiro
         interrompa // Sai do laço se acertar
      senao
         se (cont < 4) entao
            escreval("Errado! Tente novamente.")
         fimse
      fimse
   fimpara

   // Resultado Final
   se (acertou) entao
      escreval("PARABÉNS! Você acertou o número ", numSorteado, "!")
   senao
      escreval("FIM DE JOGO! Você perdeu. O número era ", numSorteado, ".")
   fimse
fimalgoritmo


