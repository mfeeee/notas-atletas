# notas-atletas

Este repositório contém um script JavaScript simples para calcular a média de notas de atletas, desconsiderando a maior e a menor nota de cada conjunto para uma avaliação mais justa.

## ✨ Funcionalidades

O script processa uma lista de atletas, onde cada um possui um conjunto de notas. Para cada atleta, ele realiza os seguintes passos:

1.  **Cria uma cópia das notas originais:** Isso garante que a lista de notas do objeto `atleta` não seja alterada durante o processo de ordenação.
2.  **Ordena as notas:** As notas são ordenadas em ordem crescente numérica. Isso é feito usando o método `sort()` com uma função de comparação `(a, b) => a - b`, que assegura que números sejam comparados corretamente (e não como strings). Após a ordenação, a menor nota estará na primeira posição e a maior nota estará na última.
3.  **Remove a maior e a menor nota:** Utiliza o método `slice(1, 4)` na matriz de notas já ordenada. Isso cria uma nova matriz contendo apenas as notas intermediárias, desconsiderando o primeiro elemento (a menor nota) e o último elemento (a maior nota).
4.  **Calcula a média:** A soma das notas restantes (as "válidas") é calculada e dividida pelo número dessas notas.
5.  **Exibe os resultados:** O nome do atleta, suas notas originais e a média válida calculada são exibidos no console.
