# Comparação de Algoritmos de Multiplicação de Matrizes

## Descrição

Este projeto tem como objetivo comparar o desempenho de quatro algoritmos de multiplicação de matrizes: **Tradicional**, **Strassen**, **Winograd** e **Karstadt**. O foco está em medir o tempo de execução de cada algoritmo para diferentes tamanhos de matrizes, avaliando sua eficiência em termos de complexidade e tempo.

## Algoritmos Implementados

1. **Algoritmo Tradicional**:
   - Complexidade: O(n³)
   - Realiza a multiplicação direta das matrizes usando multiplicação de elementos e soma.

2. **Algoritmo de Strassen**:
   - Complexidade: O(n².81)
   - Utiliza uma abordagem divide-and-conquer para reduzir o número de multiplicações necessárias.

3. **Algoritmo de Winograd**:
   - Complexidade: Aproximadamente O(n².81) com otimizações adicionais.
   - Baseado no método de Strassen, com otimizações para reduzir o número de operações.

4. **Algoritmo de Karstadt**:
   - Complexidade: Similar ao método tradicional, com otimizações usando paralelização.
   - Implementação customizada para explorar a paralelização nas operações de multiplicação.

## Estrutura do Código

- **traditional_multiplication**: Implementa a multiplicação tradicional de matrizes usando Numpy.
- **strassen_multiplication**: Implementa o algoritmo de Strassen com otimizações para submatrizes pequenas.
- **winograd_multiplication**: Implementa o algoritmo de Winograd, com técnicas de Strassen e otimizações.
- **karstadt_multiplication**: Implementa o algoritmo de Karstadt, focado em paralelização.
- **measure_performance**: Mede o desempenho dos algoritmos para uma gama de tamanhos de matrizes.
- **measure_time**: Função auxiliar para medir o tempo de execução de um algoritmo.

## Como Executar

1. **Instalações Necessárias**:
   - Python 3.6 ou superior.
   - Bibliotecas: `numpy`, `time`, `concurrent.futures`.

2. **Execução dos Testes**:
   - O código está preparado para ser executado em uma interface Jupyter Notebook ou Google Colab.
   - Basta rodar o notebook para observar a comparação dos algoritmos para diferentes tamanhos de matrizes.

## Resultados Esperados

- O tempo de execução para cada algoritmo será impresso no console.
- Espera-se que o Algoritmo Tradicional seja mais lento para matrizes grandes.
- Strassen e Winograd devem apresentar melhor desempenho para matrizes maiores.
- Karstadt pode se destacar em cenários específicos devido à paralelização.

## Referências

- Strassen, V. (1969). Gaussian elimination is not optimal. Numerische Mathematik.
- Winograd, S. (1971). On multiplication of 2x2 matrices. Linear Algebra and its Applications.
- Karstadt, A. (2024). Optimized Matrix Multiplication Techniques.
