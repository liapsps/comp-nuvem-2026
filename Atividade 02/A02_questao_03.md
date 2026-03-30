Pesquisa sobre modelos de serviço alternativos (XaaS).

**a. Descreva o modelo: FaaS (Function as a Service)**
O FaaS, conhecido popularmente como computação "Serverless", permite que os desenvolvedores implantem fragmentos de código (funções) que são executados em resposta a eventos específicos. A principal característica é que o usuário não precisa gerenciar servidores, sistemas operacionais ou instâncias; o provedor de nuvem cuida de todo o provisionamento e escalonamento automático. A cobrança é feita apenas pelo tempo de execução exato da função, e não por recursos ociosos.

**b. Desenhe uma figura que represente o modelo (Diagrama)**

Preferi fazer em mermaid, está aqui um diagrama simples:

```mermaid
graph LR
    A[Gatilho/Evento] -- Dispara --> B{Função FaaS}
    B -- Executa Lógica --> C[Banco de Dados]
    B -- Processa --> D[Armazenamento/S3]
    B -- Retorna --> E[Resposta ao Usuário]