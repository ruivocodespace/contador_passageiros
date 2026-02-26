# 🚍 Contador de Passageiros

## 1. Justificativa

A empresa de transporte do município identificou que, em horários de maior movimento, algumas linhas estavam sobrecarregadas.  
Para ampliar a quantidade de ônibus nas linhas com maior volume de passageiros, é necessário identificar com precisão quais são as mais utilizadas.

Como o investimento em novos veículos é elevado, a empresa precisa de uma forma confiável de análise de dados para apoiar a tomada de decisões estratégicas.

---

## 1.1 Solução Proposta

Desenvolver um algoritmo em Python capaz de:

- Processar um arquivo CSV contendo registros de passageiros por linha.
- Calcular o total de passageiros transportados por linha.
- Ordenar as linhas por volume de passageiros.
- Apresentar os dados consolidados para auxiliar na tomada de decisão.

---

## 2. Fluxograma

Fluxograma desenvolvido com Lucidchart para modelagem da solução:

![Fluxograma](img/fluxograma.png)

---

## 3. O Algoritmo

### 3.1 Linguagem e IDE

- Linguagem: Python  
- IDE: Visual Studio Code  

### 3.2 Infraestrutura Necessária

- Arquivo `out.csv` no mesmo diretório do script.
- Formato do CSV: linha,entrada1:saida1,entrada2:saida2,entrada3:saida3,...
- O algoritmo utiliza apenas o valor de entrada (antes do “:”) para calcular o total de passageiros.

---

### 3.3 Código Fonte

- Arquivo principal: main.py

---

### 3.4 Instruções de Execução

1. Certifique-se de que o arquivo `out.csv` esteja no mesmo diretório do script.
2. Execute o programa com:

```bash
python main.py

---

## 4. Explicação do Algoritmo

O algoritmo foi desenvolvido em Python para processar dados de um transporte público a partir de um arquivo CSV.

### 1️⃣ Leitura dos Dados

- O programa abre o arquivo `out.csv`.
- Cada linha é separada utilizando vírgula como delimitador.
- Os valores numéricos são extraídos antes do caractere “:”.

### 2️⃣ Tratamento e Consolidação

- Os valores são convertidos para inteiros.
- A soma é realizada por linha.
- Caso a linha já exista na estrutura de dados, o valor é acumulado.
- Caso contrário, um novo registro é criado.

### 3️⃣ Organização dos Resultados

- As linhas são ordenadas em ordem decrescente utilizando `sorted()` com `lambda`.

### 4️⃣ Exibição

- O programa exibe a lista final consolidada.
- Mostra também o total geral acumulado de passageiros.

---

## 🧠 Conceitos Aplicados

- Leitura de arquivos
- Manipulação de strings
- List comprehension
- Estruturas de dados (lista de dicionários)
- Ordenação com função lambda
- Processamento e consolidação de dados
- Desenvolvimento colaborativo

---

## 👥 Desenvolvedores

- Peterson Ruivo
- Victor Gabriel

Projeto desenvolvido em colaboração como atividade acadêmica.

---

## 📊 Status

- ✔️ Projeto funcional
- ✔️ Processamento e consolidação de dados implementados
- 🔄 Possíveis melhorias futuras: tratamento de erros do arquivo e uso da biblioteca `csv`
  
