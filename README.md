# Modelagem-Matemática

Aqui está o passo a passo da construção do Projeto, assim como ideias tomadas, analises desde o inicio do problema, como foi tomada as decisão e ideias desenvolvidas.

# 1. conjuntos e índices
P = {1,2, ..., n} produtos a serem produzidos;
T = {1,2, ..., n} periodo de tempo.

# 2. parâmetros
dc = demanda conhecida para cada produto p no período t;  
cp = capacidade produtiva limitada em cada período;  
ca = capacidade de armazenamento limitada;  
cup = custo unitário de produção;
cue = custo unitário de estoque;
cpp = custo de preparação da produção;
ch = custo de hora extra;
cmh = capacidade máxima de horas extras;
p = penalidade por falta de produtos;
ne = nivel do estoque inicial.

# 3. variáveis de decisão
xij = quantidade de produtos p que serão produzidos no periodo t
yij = capacidade do estoque ao fim do periodo t
zi = quantidade de horas extras para cada periodo t
// com i relacionado com os produtos e j com o tempo (pode ser p e t)

# 4. função objetivo
vair ser um somátorio com x e y e um para z, do tipo:
min Z = Σ (j=1 até n) Σ (i=1 até n) (xij*cup + yij*cue) + Σ (i=1 até n) zi

5. restrições de capacidade
