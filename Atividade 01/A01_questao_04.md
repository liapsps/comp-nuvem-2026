---------------------------------------------------------------------------
Q04: ESTUDOS DE CASO - GOOGLE CLOUD (GCP)
ALUNO: Ana Julia Chaves Souto da Costa
---------------------------------------------------------------------------

Para esta questão, analisei como grandes empresas utilizam o Google Cloud 
para resolver problemas de escala e processamento de dados.

1. SNAP INC. (SNAPCHAT)
A Snap Inc., dona do Snapchat, é um dos maiores usuários globais do Google 
Cloud. O desafio deles é processar bilhões de "Snaps" (fotos e vídeos) 
diariamente com baixa latência para usuários no mundo todo.

Como o provedor foi utilizado:
A empresa utiliza quase todo o ecossistema do GCP. O destaque vai para o 
Google App Engine, que permite que eles rodem o backend do aplicativo 
sem se preocupar com a gestão de servidores (PaaS). Eles também usam 
intensivamente o BigQuery para analisar o comportamento dos usuários e 
o Cloud Storage para armazenar a quantidade massiva de mídia gerada. 
Com isso, eles conseguem focar em criar novos filtros e funções, 
deixando a "infra" pesada nas mãos do Google.

2. THE HOME DEPOT
A gigante do varejo de construção Civil utiliza o Google Cloud para 
modernizar sua experiência de compra, tanto física quanto online. 

Como o provedor foi utilizado:
Eles migraram seus sistemas legados para uma arquitetura de microsserviços 
rodando no Google Kubernetes Engine (GKE). Isso foi crucial para aguentar 
os picos de acesso durante o "Spring Black Friday" (o período de maior 
venda deles). Além disso, eles usam ferramentas de Machine Learning da 
IA do Google para otimizar o estoque e a logística, garantindo que o 
produto certo esteja na loja certa no momento em que o cliente precisa.

---------------------------------------------------------------------------
Fontes: 
https://cloud.google.com/customers/snap-inc
https://cloud.google.com/customers/the-home-depot
---------------------------------------------------------------------------