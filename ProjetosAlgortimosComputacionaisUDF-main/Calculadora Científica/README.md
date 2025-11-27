# 🧮 Calculadora Científica - Algoritmos Computacionais

Este repositório contém o projeto de uma **Calculadora Científica** desenvolvido para a disciplina de **Algoritmos Computacionais** do UDF.

O projeto demonstra a aplicação de lógica, estruturas de controle avançadas e o uso da biblioteca matemática para criar uma ferramenta de cálculo completa e funcional via terminal.

---

## 🛠️ Tecnologia e Compilador

| Componente | Detalhe |
| :--- | :--- |
| **Linguagem de Programação** | C / C++ (Linguagem padrão para a disciplina) |
| **Compilador Utilizado** | **GCC** (GNU Compiler Collection) ou **G++** |
| **Biblioteca Externa** | `math.h` (ou `cmath` em C++) para funções trigonométricas e logarítmicas. |

---

## 🧠 Explicação Detalhada do Algoritmo

O código da calculadora não apenas realiza operações, mas também gerencia a complexidade das operações científicas e do fluxo de execução.

### 1. Estrutura e Fluxo (Loop Principal)
O programa é construído em torno de um **loop infinito** ou **loop de menu**, que permite ao usuário executar várias operações sem reiniciar o programa. Dentro deste loop, o código executa as seguintes etapas:
* **Apresentação do Menu:** Exibe as opções (soma, seno, raiz quadrada, sair, etc.).
* **Leitura da Entrada:** Recebe do usuário o comando e os números necessários.
* **Tratamento de Erros:** Verifica entradas inválidas ou condições matemáticas impossíveis (ex: raiz quadrada de número negativo).

### 2. Tratamento de Operações
As operações são categorizadas e tratadas de forma diferente:

* **Operações Binárias:** Exigem dois operandos (ex: $5 + 3$). O código utiliza o comando `switch/case` (ou `if/else` encadeado) para resolver operações como adição, subtração, multiplicação e divisão.
* **Operações Unárias:** Exigem apenas um operando (ex: $\sin(30^\circ)$ ou $\sqrt{25}$). O código invoca diretamente as funções da biblioteca matemática (`sin()`, `cos()`, `log()`, `sqrt()`).
* **Divisão por Zero:** Uma verificação condicional (`if`) previne a execução de uma divisão por zero, retornando uma mensagem de erro em vez de travar o programa.

### 3. Funções Científicas
A capacidade científica é dada pela inclusão da biblioteca matemática. O projeto demonstra a capacidade de chamar e utilizar corretamente funções para:
* **Trigonometria:** Cálculo de **seno**, **cosseno** e **tangente** (geralmente esperando ângulos em radianos).
* **Potenciação e Radiciação:** Funções como `pow()` e `sqrt()`.
* **Logaritmos:** Cálculo de logaritmos na base $e$ (`log()`) e na base 10 (`log10()`).

---

## ▶️ Como Rodar o Código

Para executar esta calculadora, você deve compilar o código-fonte usando o compilador **GCC** ou **G++** em seu terminal.

### 1. Clonar o Repositório

Abra seu terminal (ou Prompt de Comando) e clone o repositório, navegando diretamente para a pasta do projeto:

```bash
git clone [https://github.com/dinizgustavo085-maker/ProjetosAlgortimosComputacionaisUDF.git](https://github.com/dinizgustavo085-maker/ProjetosAlgortimosComputacionaisUDF.git)
cd ProjetosAlgortimosComputacionaisUDF/Calculadora\ Cient%C3%ADfica
