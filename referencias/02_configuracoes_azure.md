#Recursos Utilizados
O projeto faz uso dos seguintes recursos no Microsoft Azure:

##Resource Group:

`Nome`: falcari-grupo-recursao.

`Descrição`: Grupo de recursos onde todos os serviços estão alocados.

##Azure Storage Account:

`Nome`: falcaristorage.

`Tipo`: Blob Storage.

`Descrição`: Armazena os arquivos de dados brutos (camada Bronze) e transformados (Silver, Gold). Containers Criados (dentro do Storage Account)

##Azure Databricks:

`Nome`: falcari-azure-databricks.

`Configuração`: Cluster baseado em Spark. Utilizado para processamento e transformação de dados.

##Azure SQL Database:

`Nome`: falcari-database.

`Tipo`: SQL Server.

`Descrição`: Banco de dados onde os dados processados são armazenados e consultados.

`bronze`: Armazena os dados brutos.

`silver`: Armazena dados limpos e transformados.

`gold`: Contém os dados preparados para análise e consumo.
