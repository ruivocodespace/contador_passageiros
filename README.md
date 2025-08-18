# Contador-de-Passageiros

## 1. Justificativa

O sistema de Contador de Passageiros foi desenvolvido para facilitar a análise do fluxo de pessoas em linhas de ônibus.
Ele permite organizar e somar os dados de forma automatizada, evitando erros que ocorreriam se os cálculos fossem feitos manualmente.
Com isso, é possível identificar quais linhas são mais utilizadas, auxiliando no planejamento do transporte público, na melhoria da frota e na tomada de decisões estratégicas.

## 2. Fluxograma
(imagem ou diagrama)

## 3. Algoritmo
     #Lista de onibus conhecidas
        buss_list = []
        with open('out.csv', 'r') as arquivo:
        for linha in arquivo:
        #separa os elementos pelas ','
        str_arr = linha.strip().split(",")
        
        #Pega os elementos a partir da segunda posição
        valores = [int(item.split(':')[0]) for item in str_arr[1:]]
        soma = sum(valores)
        
        found = False
        for linha in buss_list:
            if linha["line"] == str_arr[0]:
                found = True
                linha["pass"] += soma
        if not found:
            buss_list.append({"line": str_arr[0], "pass": soma})
            
        # Ordena a lista de dicionários pelo campo "pass".
        buss_list = sorted(buss_list, key=lambda x: x["pass"], reverse=True)
        
        print(buss_list)
