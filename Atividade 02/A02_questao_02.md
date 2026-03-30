Minhas respostas foram baseadas nos conceitos fundamentais apresentados no Módulo I da AWS Academy.

**a. Quais são as seis principais vantagens da computação em nuvem?**

1. **Trocar despesas de capital por despesas variáveis:** Em vez de investir pesado em data centers antes de usá-los (CapEx), você paga apenas pelo que consome (OpEx).
2. **Beneficiar-se de economias de escala massivas:** O custo unitário cai à medida que o provedor cresce, repassando a economia para o cliente.
3. **Parar de adivinhar a capacidade:** Elimina a necessidade de prever demanda, permitindo escalar recursos para cima ou para baixo conforme necessário.
4. **Aumentar a velocidade e a agilidade:** Recursos de TI ficam disponíveis em minutos, reduzindo o tempo de experimentação e entrega.
5. **Parar de gastar dinheiro com manutenção de data centers:** Foco no negócio, deixando o gerenciamento de infraestrutura física, energia e resfriamento para o provedor.
6. **Tornar-se global em minutos:** Facilidade de implantar aplicações em várias regiões geográficas ao redor do mundo com poucos cliques.

**b. Quais são os três modelos de serviços de computação em nuvem? Defina-os brevemente e cite um exemplo.**

* **IaaS (Infraestrutura como Serviço):** Oferece o maior nível de controle sobre os recursos de TI (rede, computadores e armazenamento). Você gerencia o SO e as aplicações. 
    * *Exemplo:* **Amazon EC2**.
* **PaaS (Plataforma como Serviço):** Remove a necessidade de gerenciar a infraestrutura subjacente (hardware e SO), permitindo focar apenas na implantação e gerenciamento das aplicações. 
    * *Exemplo:* **AWS Elastic Beanstalk**.
* **SaaS (Software como Serviço):** Produto completo, gerenciado e executado inteiramente pelo provedor. O usuário final apenas utiliza a interface do software. 
    * *Exemplo:* **Google Drive / Microsoft 365**.

**c. Cite três serviços da AWS para cada categoria a seguir:**

| Categoria | Serviço 1 | Serviço 2 | Serviço 3 |
| :--- | :--- | :--- | :--- |
| **Computação** | Amazon EC2 | AWS Lambda | Amazon ECS |
| **Armazenamento** | Amazon S3 | Amazon EBS | Amazon EFS |
| **Banco de Dados** | Amazon RDS | Amazon DynamoDB | Amazon Aurora |

**d. Quais as três principais maneiras de interagir com a AWS?**

1. **AWS Management Console:** Interface gráfica via navegador web.
2. **AWS Command Line Interface (CLI):** Ferramenta de linha de comando para automação e scripts.
3. **Software Development Kits (SDKs):** Bibliotecas para integrar serviços AWS diretamente no código (ex: Python, Java, JS).

**e. Quais são as seis perspectivas do AWS Cloud Adoption Framework (AWS CAF)? Cite um stakeholder para cada.**

1. **Perspectiva de Negócios:** Garante que a nuvem gere valor ao negócio. *Stakeholder:* Gerente de Negócios / Financeiro.
2. **Perspectiva de Pessoas:** Foca na cultura, treinamento e gestão de mudanças. *Stakeholder:* RH / Gerente de Treinamento.
3. **Perspectiva de Governança:** Foca no alinhamento estratégico e controle de riscos. *Stakeholder:* CIO / Gerente de Projetos.
4. **Perspectiva de Plataforma:** Define a arquitetura e padrões de infraestrutura. *Stakeholder:* CTO / Arquitetos de Soluções.
5. **Perspectiva de Segurança:** Garante a conformidade e proteção dos dados. *Stakeholder:* CISO / Analista de Segurança.
6. **Perspectiva de Operações:** Garante a saúde e o monitoramento dos sistemas em produção. *Stakeholder:* Gerente de Operações de TI / SRE.