# ***Contador de Passageiros***

## 1. Justificativa
> A empresa de transporte do seu município, identificou que em horários de maior
movimento, algumas linhas estavam sobrecarregadas e por isso deseja ampliar a
quantidade de ônibus nestas linhas que têm maior volume de passageiros.
Porém, para tal, necessita de uma forma confiável, devido ao valor alto de
investimento em uma unidade de transporte, estabelecer quais linhas poderão receber
esse investimento.
### 1.1 Solução 
> Desenvolver um algoritmo que calcule a quantidade de usuários que circulam no ônibus de uma linha por viagem realizada nos horários de pico, utilizando o kit fornecido conforme contexto do problema.

## 2. fluxograma
![Fluxograma](img/fluxograma.png)


## 3. O Algoritmo
## 📝 Explicação do Algoritmo

O algoritmo foi desenvolvido em **Python** para processar os dados de um arquivo `CSV` contendo informações sobre as linhas de ônibus e a quantidade de passageiros registrados.  

Ele funciona em 4 etapas principais:  

1) **Leitura dos dados**  
   - O programa abre o arquivo `out.csv` e lê todas as linhas.  
   - Cada linha contém o nome da linha de ônibus e os valores correspondentes aos passageiros que entraram.  

2) **Tratamento e soma dos passageiros**  
   - Os valores são convertidos para números e somados.  
   - Se a linha de ônibus já existir na lista, o programa adiciona os novos passageiros ao total acumulado.  
   - Caso contrário, cria um novo registro para essa linha.  

3) **Organização das linhas**  
   - Todas as linhas são ordenadas em ordem decrescente, da que teve mais passageiros para a que teve menos.  

4) **Exibição dos resultados**  
   - Mostra o total de passageiros de cada linha.  
   - Calcula e exibe o **total geral de passageiros** transportados.  

Dessa forma, o algoritmo permite identificar quais linhas tiveram maior movimentação de passageiros e também o volume total registrado.  
Utilizamos o Visual Studio Code para desenvolve-lo.
