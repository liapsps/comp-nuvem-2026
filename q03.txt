---------------------------------------------------------------------------
Q03: ESTUDOS DE CASOS DE SUCESSO AWS (AMAZON WEB SERVICES)
ALUNO: Ana Julia Chaves Souto da Costa
---------------------------------------------------------------------------

===========================================================================
CASO 01: NUBANK (Setor Financeiro / Fintech)
===========================================================================

EMPRESA:
O Nubank é hoje uma das maiores plataformas de serviços financeiros do 
mundo, tendo começado no Brasil em 2013. Eles ficaram famosos por oferecer 
um cartão de crédito sem anuidade controlado totalmente por aplicativo. 
Diferente dos bancos tradicionais, o Nubank já nasceu "na nuvem", o que 
permitiu que eles crescessem muito rápido, chegando a mais de 100 milhões 
de clientes no Brasil, México e Colômbia.

DESAFIO:
O grande problema do Nubank não era só começar, mas sim aguentar o 
crescimento absurdo de usuários sem que o aplicativo caísse ou ficasse 
lento. Além disso, no setor bancário, a segurança e o cumprimento de leis 
(compliance) são muito rígidos. Eles precisavam de uma infraestrutura que:
1. Conseguisse processar bilhões de transações com latência quase zero.
2. Permitisse que o time de engenharia fizesse centenas de atualizações 
   por dia sem tirar o sistema do ar.
3. Fosse barata o suficiente para manter o modelo de "tarifa zero" para 
   o cliente final.
4. Gerenciasse um volume gigante de dados (logs) para análise de fraudes.

POR QUE USAR A AMAZON?
O Nubank escolheu a AWS por ser uma plataforma madura e que permitia o 
foco total no código e no produto, em vez de gastar tempo montando 
servidores físicos. Outros motivos principais foram:
- A facilidade de escalar (aumentar ou diminuir recursos) automaticamente.
- O acesso aos processadores AWS Graviton (que são mais baratos e rápidos).
- A integração nativa com ferramentas de Big Data e segurança que já 
  atendem às normas do Banco Central.

BENEFÍCIOS:
- Economia Real: Ao migrar para os processadores Graviton, o Nubank 
  conseguiu reduzir os custos de processamento em cerca de 14%.
- Agilidade: O tempo para colocar uma funcionalidade nova no ar caiu de 
  90 minutos para apenas 15 minutos. Hoje eles fazem mais de 700 
  "deploys" por semana.
- Estabilidade: O sistema aguenta picos de acesso gigantescos (como na 
  Black Friday) sem engasgar.
- Sustentabilidade: O uso de instâncias mais modernas reduziu a pegada 
  de carbono da empresa em 21%.

ARQUITETURA:
A arquitetura deles é baseada em microsserviços (mais de 4.500 pequenos 
serviços independentes). Eles utilizam:
- Amazon EKS (Kubernetes): Para gerenciar todos esses microsserviços 
  em contêineres.
- Amazon S3 e DynamoDB: Para armazenar os dados de forma segura e rápida.
- AWS Graviton: Servidores com chips da própria Amazon que entregam 
  mais performance gastando menos energia.
- Amazon Kinesis: Usado para capturar e processar os fluxos de dados em 
  tempo real.

---------------------------------------------------------------------------

===========================================================================
CASO 02: FORMULA 1 (Setor de Esportes / Entretenimento)
===========================================================================

EMPRESA:
A Formula 1 dispensa apresentações, sendo a maior categoria do automobilismo 
mundial. Mas, por trás dos carros na pista, existe uma operação de dados 
gigante. É um esporte decidido nos milésimos de segundo, onde a tecnologia 
é tão importante quanto o piloto.

DESAFIO:
A F1 tinha dois problemas principais para resolver com tecnologia:
1. Aerodinâmica: Os carros antigos geravam muita turbulência, o que impedia 
   que um piloto andasse perto do outro para tentar uma ultrapassagem. 
   Simular isso fisicamente em túneis de vento é caro e lento.
2. Engajamento dos Fãs: As transmissões de TV eram muito "estáticas". Eles 
   precisavam de uma forma de mostrar ao público o que estava acontecendo 
   na estratégia (desgaste de pneus, chances de ultrapassagem, etc) em 
   tempo real.

POR QUE USAR A AMAZON?
A F1 escolheu a AWS principalmente pela capacidade de Computação de Alto 
Desempenho (HPC) e Machine Learning. Eles precisavam rodar simulações de 
dinâmica de fluidos (CFD) que são extremamente pesadas e exigem milhares 
de núcleos de processamento trabalhando juntos. Ter um supercomputador 
próprio seria inviável pelo custo e pela logística de levar isso para 
cada GP ao redor do mundo.

BENEFÍCIOS:
- Melhores Corridas: Com as simulações na AWS, a F1 desenhou o carro de 
  2022 que reduziu a perda de pressão aerodinâmica de 50% para apenas 15%. 
  Isso resultou em muito mais ultrapassagens nas temporadas recentes.
- Velocidade de Pesquisa: O tempo para rodar uma simulação complexa caiu 
  em 70% (de 60 horas para apenas 18 horas).
- F1 Insights: Agora, durante a corrida, a AWS processa mais de 1 milhão 
  de pontos de dados por segundo para gerar aqueles gráficos que vemos 
  na TV, como "Previsão de Parada no Box" ou "Batalha de Frenagem".
- Redução de Custo: Eles conseguiram reduzir o tamanho do data center físico 
  que levavam para as pistas, economizando em frete e energia.

ARQUITETURA:
A estrutura da F1 na nuvem é um exemplo de processamento em tempo real:
- Amazon EC2 (Instâncias C5 e C6g): Usadas para as simulações pesadas de 
  aerodinâmica (HPC).
- Amazon SageMaker: Onde eles treinam os modelos de Inteligência Artificial 
  para prever o comportamento dos pneus e as estratégias de corrida.
- Amazon Kinesis: Para receber os dados via telemetria diretamente dos 
  sensores dos carros (são mais de 300 sensores por carro) com latência 
  mínima.
- Amazon S3: Onde guardam o histórico de décadas de corridas para análise.

---------------------------------------------------------------------------
Fontes: 
https://aws.amazon.com/pt/solutions/case-studies/nubank-graviton/
https://aws.amazon.com/pt/solutions/case-studies/formula-1/
---------------------------------------------------------------------------