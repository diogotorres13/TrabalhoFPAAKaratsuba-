# Trabalho FPAA sobre Karatsuba-

## Descrição do Projeto

Este projeto apresenta uma implementação em Python do algoritmo de multiplicação rápida de Karatsuba. Esse método otimiza o processo de multiplicação ao reduzir a quantidade de operações necessárias, dividindo os números em partes menores e resolvendo o problema de forma recursiva.

### Lógica do Algoritmo
1. Se um dos números for menor que 10, retorna a multiplicação direta.
2. Determina o tamanho do maior número e divide ao meio.
3. Divide os números em partes superiores e inferiores.
4. Calcula os produtos intermediários recursivamente.
5. Combina os resultados para obter o produto final.

## Como Executar o Projeto

### Requisitos
- Python 3.x instalado

### Execução
1. Clone o repositório
   ```sh
   git clone https://github.com/diogotorres13/TrabalhoFPAAKaratsuba-.git
   cd TrabalhoFPAAKaratsuba
   ```
2. Execute o script
   ```sh
   python main.py
   ```
3. Insira os números quando solicitado.

## Relatório Técnico

### Complexidade Ciclomática

O fluxo de controle da função karatsuba pode ser descrito por meio de um grafo, composto pelos seguintes elementos:
- Nós (N): correspondem a blocos distintos de código.
- Arestas (E): representam as transições entre os blocos.
- Componentes conexos (P): igual a 1, pois o programa é único.

Fórmula: `V(G) = E - N + 2P`

### Complexidade Assintótica

- Complexidade Temporal: O algoritmo apresenta custo de execução O(n^{\log_2 3}), aproximadamente O(n^{1.585}).
- Complexidade Espacial: O(n), devido ao uso da pilha de chamadas recursivas.

### Análise de Casos
- Melhor caso: O(n), quando os operandos são pequenos.
- Caso médio e pior caso: O(n^{1.585}), em função da decomposição recursiva do problema.
