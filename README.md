# Projeto-de-Procura-
Projeto no de âmbito Inteligência Articial, algortimos

# Índice

1. [Resultados](#resultados)
2. [Conclusão](#conclusão)

## Resultados

Grafo A 
Sem verificação de repetições 
 ![image](https://github.com/Becas26/Projeto-de-Procura-/assets/102540581/a18dcd1a-111f-4f1a-9e93-405a82b3964c)


Com verificação de repetições 

![image](https://github.com/Becas26/Projeto-de-Procura-/assets/102540581/64d3712f-9d3e-4054-ae4a-85d0385dd4fc)
 
(Otimalidade dos resultados por ordem de eficácia do 1º ou 4º lugar) 


![image](https://github.com/Becas26/Projeto-de-Procura-/assets/102540581/f86c8fc7-4ed6-4c52-b815-426f97e34493)

![image](https://github.com/Becas26/Projeto-de-Procura-/assets/102540581/7f7c6cce-5701-4547-8959-c241f2d55e21)

![image](https://github.com/Becas26/Projeto-de-Procura-/assets/102540581/6bb5aeb9-e86c-4b07-83b6-9d2ec5251b20)

![image](https://github.com/Becas26/Projeto-de-Procura-/assets/102540581/73cea67d-78d3-4ffd-a35b-df2ca2d7e4fa)

## Conclusão

A comparação entre as versões "Com verificação de repetições" e "Sem verificação de repetições" dos algoritmos apresenta resultados interessantes.  
De um ponto de vista geral, os resultados mostram uma diferença no número de nós expandidos e na utilização de memória quando a verificação de repetição é desativada. Isso é especialmente visível no algoritmo UCS e no A*, que mostram um aumento considerável no número de nós expandidos.  

O algoritmo BFS (Breadth-First Search) demonstra uma utilização de memória maior em comparação com outros algoritmos, o que faz sentido já que o BFS mantém uma fila de todos os nós expandidos. O tempo médio e o número de nós expandidos são consistentes em ambas as variações, dado que o grafo em questão não tem muitas repetições ou caminhos redundantes. A otimalidade é 4, pois foi o que gastou mais memória, demorou mais tempo e não encontrou o caminho mais ótimo.  

O DFS (Depth-First Search), em contrapartida, tem o menor número de nós expandidos e a utilização de memória também é inferior, dado que só mantém uma pilha dos nós ao longo do caminho de busca atual. A sua otimalidade é 3 pois foi o algoritmo que apesar de demonstrar o melhor tempo de execução e a melhor memória (empatada com A). Não encontrou, porém, o caminho mais ótimo. É de notar que o DFS pode deparar-se com o primeiro resultado que encontra, que pode não ser o melhor como aconteceu, por isso depende do grafo, apesar de poder executar com melhor tempo.  

O UCS (Uniform Cost Search) e o A* (com heurística 1), têm números quase idênticos de nós expandidos na variação "Com verificação de repetições". Aqui observamos a diferença entre nós expandidos com ou sem verificação (17-18 vs 31-30). O A* tem ligeiramente menor utilização de memória, o que sugere que a heurística usada é eficaz na redução do espaço de busca, contudo demora mais tempo, indicando que não é a mais ótima. A otimalidade do UCS é 1, a melhor, ligeiramente superior ao A, considerando o balanço entre o tempo e a memória, favorecendo o tempo. UCS e A foram os únicos algoritmos a encontrar o melhor caminho com custo de 12. Executando o A* com heurísticas diferentes mudarão este resultado, ao nível dos nós expandidos, memória e tempo.  

O A* apresenta um acréscimo na utilização de memória na variação "Sem verificação de repetições", dado que o algoritmo vai deixar de percorrer caminhos que incluam nós repetidos. A sua ótimalidade é 2, pois é o mais ótimo a seguir ao UCS como explicado anteriormente. Executando com a heurística 3 (feita por nós), os nós visitados são apenas 7 e tanto a memória como tempo são inferiores fazendo a otimalidade 1.  

Em suma, os resultados sugerem que a verificação de repetições pode ser fundamental para a otimalidade com grafos mais complexos, com caminhos redundantes e ciclos. No entanto, para problemas com estruturas de grafo mais simples, a verificação pode não ser tão crítica. A escolha do algoritmo e a decisão de usar a verificação de repetição deve, portanto, ser cuidadosamente ponderada com base nas especificidades do problema e das restrições de recursos. No que diz respeito ao algoritmo melhor para escolher, observamos que para grafos simples, algoritmos como BFS e DFS são melhores pois não têm tanto overhead, acabando por terminar mais rapidamente. Concluímos também que para A* a heurística é muito importante. No caso da heurística 1, apesar de decente não era a mais ótima para o problema. A* pode ser o melhor algoritmo em muitos casos, dependendo da heurística escolhida. Para o grafo A o melhor algoritmo é o uniforme. 

