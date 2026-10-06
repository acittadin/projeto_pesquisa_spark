# Apache Iceberg

O **Apache Iceberg** é um formato de tabela aberto e de alto desempenho projetado especificamente para grandes cargas de trabalho analíticas em Data Lakes.

## Características Principais
* **Viagem no Tempo (Time Travel) e Rollback:** Permite consultar o estado exato dos dados em um ponto específico no tempo ou reverter alterações indesejadas com facilidade.
* **Evolução de Esquema Segura:** Suporta alterações estruturais em tabelas (como adicionar, renomear ou reordenar colunas) sem reescrever arquivos de dados inteiros.
* **Planejamento de Consultas Otimizado:** Utiliza metadados baseados em árvore e estatísticas avançadas de partições para ignorar arquivos irrelevantes durante as consultas SQL.

## Importância para o Projeto
O Iceberg garante a independência de ferramentas, permitindo que diferentes motores de consulta leiam os mesmos dados de forma consistente, confiável e com isolamento de transações.# Apache Iceberg

O Apache Iceberg é um formato de tabela aberto e de alto desempenho projetado para tabelas analíticas gigantes em Data Lakes. 

Ele é fundamental para o projeto pois permite:
* **Viagem no Tempo (Time Travel):** Mantém um histórico de alterações na tabela, permitindo consultar dados do passado.
* **Transações ACID:** Garante que operações como INSERT, UPDATE e DELETE ocorram de forma totalmente segura.
