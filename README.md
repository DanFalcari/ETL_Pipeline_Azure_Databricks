# Análise da base de dados de diabetes 

O diabetes é uma condição crônica grave que compromete a capacidade do organismo de regular os níveis de glicose no sangue de forma eficaz, o que pode resultar em uma diminuição da qualidade de vida e da expectativa de vida.

O Sistema de Vigilância de Fatores de Risco Comportamentais (BRFSS) é uma pesquisa de saúde conduzida anualmente por telefone pelo Centro de Controle e Prevenção de Doenças dos Estados Unidos (CDC). Esse levantamento coleta informações de milhares de americanos sobre comportamentos de risco à saúde, condições crônicas e o uso de serviços preventivos.

Neste projeto, foi utilizado o conjunto de dados do BRFSS referente ao ano de 2015, disponível no

Kaggle: https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset

![imagem](imagens/capa_diabetes.jpg)


## Um pouco mais sobre a base de dados 

[Clique aqui](referencias/01_dicionario_de_dados.md) para ver o dicionário de dados da base utlilizada


## Resumo resultados obtidos

### **Conclusões da análise dos dados**  

**Fatores de Maior Risco para Diabetes:**  
1. **Hipertensão (75.27%)** e **colesterol alto (67.01%)** → Reforçam a relação do diabetes com doenças cardiovasculares.  
2. **Idade avançada** → Maior incidência a partir dos 50 anos.  
3. **Sedentarismo** → Percentual menor de atividade física entre diabéticos (63.05%).  
4. **Baixa escolaridade e renda** → Pode indicar falta de acesso a informação e cuidados médicos.  
5. **Saúde Geral Ruim** → Quase 13% dos diabéticos avaliam sua saúde como "ruim".

### **Correlações Importantes** 

1. **A correlação entre doenças crônicas e saúde geral reforça a necessidade de prevenção.**
2. **Baixa renda está associada a pior saúde e menos acesso a saúde, consultas médicas e alimentação de qualidade.**
3. **Atividade física pode atuar como um fator de proteção para várias condições.**
4. **Fumantes apresentam mais problemas cardíacos e metabólicos, o que confirma os riscos conhecidos.**

## Organização do projeto

```

├── .gitignore         <- Arquivos e diretórios a serem ignorados pelo Git
├── ambiente.yml       <- O arquivo de requisitos para reproduzir o ambiente de análise
├── LICENSE            <- Licença de código aberto (MIT)
├── README.md          <- README principal para desenvolvedores que usam este projeto.
|
├── dados              <- Arquivos de dados para o projeto.
|
|
├── notebooks          <- Jupyter Notebooks com tratamento e análise dos dados.
│
|   └──src             <- Código-fonte para uso neste projeto.
|      │
|      ├── __init__.py  <- Torna um módulo Python
|      └──config.py    <- Configurações básicas do projeto
|    
|
├── referencias        <- Dicionários de dados
|
├── relatorios         <- Análises geradas em HTML, PDF, LaTeX, etc.
│   └── imagens        <- Imagens usadas no projeto
```

## Configuração do ambiente

1. Faça o clone do repositório.

    ```bash
    git clone git@github.com:DanFalcari/Projeto_diabetes.git
    ```

2. Crie um ambiente virtual para o seu projeto utilizando o conda.

      ```bash
      conda env create -f ambiente.yml --name diabetes 
      ```