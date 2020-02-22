
![LOGO IPS](https://files.fm/thumb_show.php?i=yred9d27)  

# PROGRAMAÇÃO I

# COMPUTADORES, ALGORITMOS e PROGRAMAS


## Computador

Um computador  é uma artefacto que podem diferir em  tamanho, aparência e custo,  mas que partilham  partilham quatro características fundamentais: são **automáticos, universais, electrónicos e digitais** e caracteriza-se  actualmente por por ser um sistema digital programável através de uma sequência de instruções guardadas em memória.

>Charles Babbage projectou o primeiro computador mecânico capaz de desempenhar automaticamente sequências de operações. O Computador erá conhecido como o **difference engine** e usava apenas elementos mecânicos e podia ser programado para construir tabelas matemáticas.

### Automático

Um computador é referido como sendo automático porque uma vez que tenha acesso a informação necessária, trabalha por si só, sem a intervenção humana.  isto é, uma vez o trabalho começado, ele será levado até ao final sem a intervenção humana. Para isso, o computador recebe um **programa** (um conjunto de instruções que diz como resolver o problema). O programa é escrito numa linguagem que pode ser compreendida pelo computador, ou seja uma **Linguagem de Programação**.


### Universal

Pode efectuar qualquer tarefa cuja solução possa ser expressa através de um programa.

### Electrónico

É composto por  componentes  responsáveis pela grande velocidade das operações efectuadas por um computador.

### Digital

Toda a informação contida num computador é expressa por duas grandezas discretas, normalmente referidas como sendo **0** e **1** ou **falso** e **verdadeiro**.

> 
Por exemplo, num computador o símbolo **“J”**, poder ́a ser representado por **1001010.**
>


#### O primeiro computador completamente automático foi construído em 1944 - Harvard Mark I:
* 18 por 2,5 metros
* 5 toneladas, 
* 760.000 partes e centenas de kilometros de cabos 9 bytes de memória
* 3 segundos para fazer adição ou subtração

## Algoritmo

 Um algoritmo é uma sequência finita de instruções bem definidas e não ambíguas, cada uma das quais pode ser executada mecanicamente num período de tempo finito com uma quantidade de esforço finita. A compreensão do conceito de algoritmo é relevante porque um programa corresponde a um algoritmo escrito numa linguagem que é entendida pelo computador, chamada uma linguagem de programação.

>
**Sequência finita de instruções** quer dizer que existe uma ordem pela qual as instruções aparecem no algoritmo, e que estas instruções são em numero finito.
>


O significado de cada uma das instruções é claro, não havendo lugar para múltiplas interpretações do significado de uma instrução.


>
A execução das instruções não requer imaginação por parte do executante.
>

Um algoritmo está sempre associado com um dado objectivo, ou seja, com a solução de um dado problema. A execução das instruções do algoritmo garante que o seu objectivo é atingido.


### Exemplo de um algoritmo



#### **Rebuçado de ovos**

* 500 g de açúcar; 
* 2 colheres de sopa de amêndoas peladas e raladas; 
* 5 gemas de ovos; 
* 250 g de açúcar para a cobertura; e farinha.

> Leva-se o açúcar ao lume com um copo de ́agua e deixa-se ferver até fazer ponto de pérola. Junta-se a amêndoa e deixa-se ferver um pouco. Retira-se do calor e adicionam-se as gemas. Leva-se o preparado novamente ao lume e deixa-se ferver até se ver o fundo do tacho. Deixa-se arrefecer completamente. Em seguida, com a ajuda de um pouco de farinha, molda-se a massa de ovos em bolas. Leva-se o restante açúcar ao lume com 1 dl de agua e deixa-se ferver até fazer ponto de rebuçado. Passam-se as bolas de ovos por este açúcar e põem-se a secar sobre uma pedra untada, após o que se embrulham em papel celofane de varias cores.


## Programa e linguagem de programação

Um algoritmo, escrito de modo a poder ser executado por um computador, tem o nome de programa. Por sua vez uma linguagem de programação é uma linguagem utilizada para escrever programas de computador. Existem muitos tipos de linguagens de programação. De acordo com as afinidades que estas apresentam com o modo como os humanos resolvem problemas, podem ser classificadas em linguagens máquina, linguagens “Assembly” e linguagens de alto nível.

### Exemplo de um programa em linguagem máquina

```Binary
01001000 01100101 01101100 01101100 01101111 00100000 
01010111 01101111 01110010 01101100 01100100
```

>
Códigos numéricos associados a operações básicas  
Linguagem específica de cada micro-processador  
Única linguagem directamente executável pelo computador  
Difícil escrever programas diretamente em código máquina  
Concebida para facilitar a implementação usando circuitos eletrónicos

### Exemplo de um programa em assembly

```python
;------------------------------------------------------------
FibonacciByMemory PROC 
; Receives: ECX as input n 
; Returns: EAX as nth Fibonacci number calculated
;------------------------------------------------------------
   mov   eax,1         
   mov   previous,0         
   mov   current,0         
L1:
   add eax,previous       ; eax = current + previous      
   mov edx, current       ; previous = current
   mov previous, edx
   mov current, eax
loop   L1
   ret
FibonacciByMemory ENDP
```

>
>Representação do código máquina usando mnemónicas   
Mais legível do que a linguagem máquina   
Pode ser traduzida automaticamente para código máquina   
Continua a ser específica para cada micro-processador   
Exige programação lenta, fastidiosa e susceptível a erros  
Usada apenas em contextos muito específicos



### Exemplo de um programa  em Python

_Programa Hello Word_

```python
# This program prints Hello, world!
print('Hello, world!')
```

### Exemplo de um programa em C

_Programa Hello Word_

```python
#include <stdio.h>
int main() {
   // printf() displays the string inside quotation
   printf("Hello, World!");
   return 0;
}
```

>
Mais próximas da formulação matemática dos problemas  
Permitem o desenvolvimento de programas mais rápido  
Facilitam a deteção e a correção de erros  
Permitem desenvolver programas independentes do processador específico em cada computador


## Exercícios práticos
1. Faça um algoritmo para fritar um ovo.
1. Faça um algoritmo para planear um fim-de-semana
1. Pedir o valor base do salário e o valor de vendas. Em seguida calcule o valor do salário tendo em conta que o salário é base + 4% das vendas. Apresente o valor do salário.
1. Pedir 4 notas e calcular média ponderada com pesos 2, 3, 4 e 6 respetivamente. Caso a média seja menor que 7 exibir "reprovado" juntamente com o valor da média, caso contrário exibir “Aprovado" juntamente com o valor da média.
1. Solicite os valores A e B.  Se A for igual a B calcule a soma de A com B, caso contrário calcule o produto.
1. Pedir o tempo de serviço e salário de um funcionário, caso o tempo for menor que 10 anos o aumento será de 10%, caso contrário o aumento será de 25%
1. Pedir 4 notas e calcular média ponderada com pesos 2, 3, 4 e 6 respetivamente. Caso a média seja menor que 7 exibir "reprovado" juntamente com o valor da média, caso contrário exibir “Aprovado" juntamente com o valor da média
1. Solicite um valor X em seguida apresente os  X primeiros valores inteiros.
1. Faça um algoritmo para planear um fim-de-semana.
1. A imobiliária Remus vende apenas terrenos retangulares. Faça um algoritmo para ler as dimensões de um terreno e depois exibir a área do terreno. 
1. A padaria SuperPão vende uma certa quantidade de papos secos e uma quantidade de broas em cada dia. Cada papo seco custa 0,15 Euros e  cada  broa custa 1,50 Euros . No final do dia, o dono quer saber quanto arrecadou com a venda dos pães, e quanto deve guardar numa conta de poupança \(10% do total arrecadado\). Com base nestes fatos, faça um algoritmo para ler as quantidades de papos e de broas, e depois calcular os dados solicitados. 
1. Escreva um algoritmo para ler o nome e a idade de uma pessoa, e exibir quantos dias de vida ela possui. Considere sempre anos completos, e que um ano possui 365 dias. Ex: uma pessoa com 19 anos possui 6935 dias de vida.
1. Um condutor deseja colocar no seu tanque X euros de gasolina. Escreva um algoritmo para ler o preço do litro da gasolina e o valor que deve ser pago, e exibir quantos litros ele armazenou no tanque. 
1. Entrar com o dia e o mês de uma data e informar quantos dias se passaram desde o início do ano. Esqueça a questão dos anos bissextos e considere sempre que um mês possui 30 dias. 
1. Uma fábrica de camisas produz os tamanhos pequeno, médio e grande, cada uma sendo vendida respectivamente por 30, 45 e 75 Euros. Faça um algoritmo em que o utilizador forneça a quantidade de camisas pequenas, médias e grandes referentes a uma venda, e informe quanto será o valor arrecadado.
1. Faça um algoritmo para ler o salário de um funcionário e aumentá-lo em 15%. Após o aumento, desconte 8% de impostos. Imprima o salário inicial, o salário com o aumento e o salário final. 
1. Alguns países medem temperaturas em graus Celsius, e outros em graus Fahrenheit. Faça um algoritmo para ler uma temperatura Celsius e imprimi-Ia em Fahrenheit \(pesquise como fazer este tipo de conversão\). 
1. A empresa Sorus paga Euros 50,00 por hora normal de trabalho, e Euros 90,00 por hora extra. Faça um algoritmo para calcular e imprimir o salário bruto e o salário líquido de um determinado funcionário. Considere que o salário líquido é igual ao salário bruto descontando-se 25% de impostos. 
1. Faça um algoritmo que receba duas notas, calcule e mostre a média ponderada dessas notas, considerando peso 2 para a primeira nota e peso 3 para a segunda nota.


##  Exercícios laboratoriais
1. Faça um algoritmo que receba o preço de um produto, calcule e mostre o novo preço, sabendo-se que este sofreu um desconto de 10%. 
1. Faça um algoritmo que receba o peso de uma pessoa, calcule e mostre: o novo peso se a pessoa engordar 15% sobre o peso digitado e o novo peso se a pessoa emagrecer 20% sobre o peso digitado. 
1. Faça um algoritmo permite calcular o máximo divisor comum – mdc\(m,n\) – entre dois números inteiros.  
1. Faça um algoritmo para receber um número qualquer e informar na tela se é par ou ímpar. 
1. Faça um algoritmo que leia dois valores inteiros A e B se os valores forem iguais deverá se somar os dois, caso contrário multiplique A por B. Ao final de qualquer um dos cálculos mostrar seu conteúdo na tela. 
1. Encontrar o dobro de um número caso ele seja positivo e o seu triplo caso seja negativo, imprimindo o resultado. 
1. Escreva um algoritmo que leia dois valores e mostre-os em ordem decrescente. 
1. Escreva um algoritmo que leia três valores e mostre-os em ordem decrescente. 
1. Escreva um algoritmo que leia dois valores e mostre-os em ordem crescente. 
1. Escreva um algoritmo que leia três valores e mostre-os em ordem crescente. 
1. O IMC – Índice de Massa Corporal é um critério da Organização Mundial de Saúde para dar uma indicação sobre a condição de peso de uma pessoa adulta. A fórmula é IMC = peso / \(altura \)2  Elabore um algoritmo que leia o peso e a altura de um adulto e mostre sua condição de acordo com  os seguintes valores: Abaixo de 18,5 Abaixo do peso;  Entre 18,5 e 25 Peso normal:  Entre 25 e 30 Acima do peso e  Acima de 30 obeso.
1. Escreva um algoritmo que leia 3 notas obtidas por um aluno nas 3 verificações e a média dos exercícios que fazem parte da avaliação, e calcule a média de aproveitamento, utilizando a seguinte fórmula. Nota Final := \(nota1 + nota 2  _2 + nota 3_  3 \)/6
1. Imprima todos os números pares no intervalo de 1 a 30. 
1. Imprima o somatório de todos os números inteiros no intervalo de 0 \(zero\) a N. Onde N deve ser um número inteiro maior ou igual a zero e será escolhido pelo utilizador. 
1. Desenvolver um algoritmo que efetue a soma de todos os números ímpares que são múltiplos de três e que se encontram no conjunto dos números de 1 até 500. 
1. Desenvolver um algoritmo que leia a altura de 15 pessoas. Este programa deverá calcular e mostrar: A menor altura do grupo e a maior altura do grupo; 
1. Desenvolver um algoritmo que leia um número não determinado de valores e calcule e escreva a média aritmética dos valores lidos, a quantidade de valores positivos, a quantidade de valores negativos e o percentual de valores negativos e positivos. 
1. Escrever um algoritmo que gera e escreve os números ímpares entre 100 e 200. 
1. Escreva um algoritmo que leia um valor inicial A e imprima a sequência de valores do cálculo de A! e o seu resultado. Ex: 5! = 5 X 4 X 3 X 2 X 1 = 120 
