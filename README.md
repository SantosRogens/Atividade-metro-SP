# Atividade-metro-SP
👤 Integrante

Rogens Brasileiro Alcantara dos Santos

📌 Sobre o projeto

Atividade_Metro é um sistema acadêmico de planejamento de rotas do metrô de São Paulo desenvolvido em Python.

O projeto representa três linhas do metrô como um grafo e permite encontrar rotas entre estações utilizando algoritmos de busca. O sistema também considera estações de integração, bloqueios, regras de inferência, interpretação de pedidos em linguagem natural e visualização da rota.

🎯 Objetivos

Representar as linhas do metrô utilizando um grafo;

Identificar automaticamente as estações de integração;

Encontrar rotas entre estações;

Utilizar BFS e DFS;

Considerar estações bloqueadas;

Identificar transferências entre linhas;

Aplicar regras de inferência;

Interpretar solicitações em linguagem natural;

Apresentar visualmente a rota;

Validar o funcionamento por meio de testes automatizados.

🧠 Tecnologias utilizadas

Python 3

Google Colab

Jupyter Notebook

ipywidgets

Grafos

BFS (Breadth-First Search)

DFS (Depth-First Search)

Lógica proposicional

Regras de inferência

🚇 Linhas utilizadas

Linha 1-Azul

Tucuruvi → Parada Inglesa → Jardim São Paulo → Santana → Carandiru → Portuguesa-Tietê → Armênia → Tiradentes → Luz → São Bento → Sé → Japão-Liberdade → São Joaquim → Vergueiro → Paraíso → Ana Rosa → Vila Mariana → Santa Cruz → Praça da Árvore → Saúde → São Judas → Conceição → Jabaquara

Linha 2-Verde

Vila Madalena → Sumaré → Clínicas → Consolação → Trianon-Masp → Brigadeiro → Paraíso → Ana Rosa → Chácara Klabin → Santos-Imigrantes → Alto do Ipiranga → Sacomã → Tamanduateí → Vila Prudente

Linha 3-Vermelha

Palmeiras-Barra Funda → Marechal Deodoro → Santa Cecília → República → Anhangabaú → Sé → Pedro II → Brás → Bresser-Mooca → Belém → Tatuapé → Carrão → Penha → Vila Matilde → Guilhermina-Esperança → Patriarca-Vila Ré → Artur Alvim → Corinthians-Itaquera

🔗 Estações de integração

As integrações são deduzidas automaticamente pelo sistema, verificando quais estações pertencem a mais de uma linha.

As integrações encontradas são:

Sé

Paraíso

Ana Rosa

🔎 Algoritmos de busca

BFS

O BFS realiza uma busca em largura e é utilizado para encontrar uma rota com menor número de trechos em um grafo não ponderado.

DFS

O DFS realiza uma busca em profundidade e também está disponível no sistema para comparação.

🚧 Estações bloqueadas

O sistema permite informar estações fechadas. Durante a busca, as estações bloqueadas são evitadas pelo algoritmo.

🧩 Regras de inferência

O projeto implementa as regras R1 até R7.

A regra R6 identifica automaticamente uma estação como integração quando ela pertence a duas linhas diferentes:

∀e ∀l1 ∀l2 (pertence(e,l1) ∧ pertence(e,l2) ∧ l1 ≠ l2 → integracao(e))

Também foi implementada uma regra adicional R7 relacionada ao tratamento de bloqueios e desvios de rota.

🖥️ Interface

A interface utiliza ipywidgets e permite:

Informar origem;

Informar destino;

Escolher BFS ou DFS;

Solicitar acessibilidade;

Informar estações fechadas;

Informar elevadores em manutenção;

Interpretar pedidos em linguagem natural;

Calcular a rota;

Visualizar a rota no mapa.

🗺️ Visualização

As linhas são apresentadas utilizando suas respectivas cores:

Linha 1-Azul: #1e88e5

Linha 2-Verde: #2e7d32

Linha 3-Vermelha: #d32f2f

🧪 Testes

O projeto possui a função:

rodar_testes()

Ela executa testes automatizados utilizando assert para verificar a estrutura do grafo, integrações, rotas, bloqueios, interpretador e tabela-verdade.

📋 Casos obrigatórios

Caso 1

Tucuruvi → Corinthians-Itaquera

22 paradas

1 transferência

Transferência em Sé

Caso 2

Vila Madalena → Jabaquara

14 paradas

1 transferência

Caso 3

Palmeiras-Barra Funda → Vila Prudente

16 paradas

2 transferências

Caso 4

Tucuruvi → Brás, com Sé fechada

Nenhuma rota

Caso 5

Vila Madalena → Jabaquara, com Paraíso fechado

Nenhuma rota

Caso 6

Vila Prudente → Jabaquara, com Paraíso fechado

13 paradas

Rota alternativa via Ana Rosa

▶️ Como executar

Abra o arquivo Atividade_Metro.ipynb no Google Colab e execute as células em ordem.

📓 Arquivo principal

Atividade_Metro.ipynb

A versão entregue utiliza o interpretador offline e não depende de APIs externas ou chaves de acesso.

👨‍💻 Integrante

Rogens Brasileiro Alcantara dos Santos

Projeto desenvolvido para fins acadêmicos.
