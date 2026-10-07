# Quick sort

Trabalho da unidade 2 da disciplina de ALGORITMOS E ESTRUTURA DE DADOS I .

Implementação do código base antes de fazer a parte gráfica e visual com o raylib.

## Sobre o Projeto

Este repositório contém a implementação prática, testes de desempenho e análise do algoritmo de ordenação **Quicksort** desenvolvido na linguagem C.

## Funcionalidades Principais

1. **Geração de Dados Aleatórios (rand e srand)**:
   A massa de dados utilizada para os testes (como conjuntos de 1.000 e 10.000 elementos) é gerada dinamicamente utilizando as funções rand e srand da biblioteca padrão, garantindo variabilidade de dados a cada execução.

2. **Estratégia de Escolha do Pivô**:
   O algoritmo seleciona o pivô utilizando o cálculo do elemento central do subvetor atual.

   * **Exemplo Prático**: Imagine que estamos analisando um subvetor que vai do índice begin = 4 até end = 10 (ou seja, os elementos nas posições 4, 5, 6, 7, 8 e 9):

     * `end - begin = 10 - 4 = 6` elementos.

     * `(end - begin) / 2 = 6 / 2 = 3` posições a partir do início.

     * `begin + 3 = 4 + 3 = 7` (o elemento na posição 7 é escolhido como pivô).

3. **Cronometragem de Desempenho (time.h)**:
   O tempo de execução de cada ordenação é monitorado utilizando recursos da biblioteca `<time.h>` e a função `clock()`, permitindo avaliar o custo computacional de forma rigorosa.

## Como compilar e executar

1. Certifique-se de ter um compilador C instalado (como o GCC).

2. Abra o terminal na pasta do projeto e compile o código modificando o número após `quick_sort` (10, 100, 1000 ou 10000) para executar o `quick_sort` que deseja:

   ```
   gcc quick_sort10.c -o aula
   
   ```

   Execute:

   ```
   ./aula.exe
   
   ```

3. O código vai gerar um FILE "dados10.txt" onde vai criar, de forma aleatória, 10 elementos para que o `quick_sort` possa ser executado.

4. Após a leitura desse FILE criado anteriormente, será gerado um novo FILE "saida10.txt", onde será impressa a saída do código com o processo executado: comparações, passo a passo, tempo executado, quantidade de elementos.
