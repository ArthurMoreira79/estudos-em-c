# Projetos em C

![C](https://img.shields.io/badge/C-A8B9CC?logo=c&logoColor=black)
![License](https://img.shields.io/badge/license-MIT-blue)

Laboratórios de faculdade e estudos pessoais em **linguagem C**, do primeiro programa com `printf` até árvores balanceadas e grafos com milhares de vértices. Os labs são das disciplinas de **Fundamentos de Programação** e **Algoritmos e Estruturas de Dados I e II** (Sistemas de Informação, IFMA).

---

## Destaques

- **Rede de amizades do Facebook** ([AED02 · Lab 7](AED02/Lab%207%20-%20Grafo%20Facebook)): grafo com lista de adjacência que carrega o dataset real do SNAP (4.039 usuários e 88.234 amizades) e responde, para qualquer par de usuários, quantos amigos cada um tem, quais amigos têm em comum e qual o caminho mais curto entre eles, com busca em largura (BFS). Testado com valgrind, sem vazamentos de memória. O relatório explica cada decisão.
- **BST × AVL × Red-Black** ([AED02 · Labs 3 a 5](AED02)): implementação das três árvores e benchmarks com até 1 milhão de elementos, medindo tempo de inserção, altura final e quantidade de rotações de cada tipo (LL, RR, LR, RL).
- **TADs em C** ([AED01](AED01)): lista, fila e árvore implementadas como tipos abstratos de dados, com arquivos `.h` e `.c` separados e programas de teste, aplicados a um cardápio de lanches e a uma fila de pedidos.

---

## Conteúdo

### Algoritmos e Estruturas de Dados II · [`AED02/`](AED02)

| Lab | Tema |
|---|---|
| Lab 1 | Insertion Sort |
| Lab 2 | Merge Sort e comparação de desempenho com o Insertion Sort |
| Lab 3 | Árvores BST e AVL, com benchmark |
| Lab 4 | Instrumentação das rotações da AVL e comparação de tempo e altura com a BST |
| Lab 5 | Árvore Red-Black e relatório comparando BST, AVL e RB |
| Lab 6 | Grafo com lista de adjacência: criação, inserção e remoção de arestas, grafos direcionados e não direcionados |
| Lab 7 | Rede de amizades do Facebook: grau, amigos em comum e caminho mínimo com BFS |

### Algoritmos e Estruturas de Dados I · [`AED01/`](AED01)

| TAD | Tema |
|---|---|
| TAD 1 | Lista, aplicada a um cardápio de lanches lido de arquivo |
| TAD 2 | Fila, aplicada a uma fila de pedidos |
| TAD 3 | Árvore binária de busca e lista encadeada, com um experimento que compara o tempo de busca de um lanche nas duas estruturas |

### Fundamentos de Programação · [`FundProg/`](FundProg)

| Lab | Tema | Programas |
|---|---|---|
| Labs 1 a 3 | Estruturas de repetição | Caixa eletrônico, menu de opções, notas de alunos, campeonato de futebol, fatorial, soma de séries, pirâmide de asteriscos, sincronização de semáforos e validação de senha |
| Lab 4 | Funções, ponteiros e parâmetros | Cofre pirata, descubra o número e tarifa de estacionamento |
| Lab 5 | Estação meteorológica | Análise de temperaturas, alertas de variação, umidade por horário e estatísticas dos sensores |
| Lab 6 | Sistema acadêmico | Cadastro e consulta de alunos |

### Estudos pessoais · [`PraticasC/`](PraticasC)

| Pasta | Tema | Exemplos |
|---|---|---|
| `FundBasicosC` | Fundamentos | Calculadoras (simples, IMC, científica), conversores de unidade e de base, equação do 2º grau, validador de triângulos |
| `ControleDeFluxoC` | Condicionais e laços | Conversor de números romanos, Fibonacci, palíndromos, números primos, pedra-papel-tesoura, jogo de adivinhação |
| `FunçõesC` | Funções e recursão | Torre de Hanói, Fibonacci recursivo, MDC e MMC, combinação e permutação, validador de CPF |

---

## Como compilar

É preciso ter um compilador C, como o GCC. Programas de um arquivo só:

```bash
gcc "PraticasC/FunçõesC/FuncaoTorreHanoi.c" -o hanoi
./hanoi
```

Nos labs com vários arquivos (`.h` e `.c`), compile todos os `.c` da pasta juntos, a partir dela:

```bash
cd "AED02/Lab 7 - Grafo Facebook"
gcc main.c Grafo.c -o programa
./programa
```

---

Feito por [Arthur Moreira](https://github.com/ArthurMoreira79) · Distribuído sob a licença [MIT](LICENSE).
