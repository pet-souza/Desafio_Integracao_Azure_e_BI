# Desafio_Integra-o_Azure_e_BI
Integração de banco de dados criado na Azure com o Power BI para limpeza e tratamento de dados.

Integração, Tratamento e Transformação de Dados com Azure, MySQL e Power BI
📌 Sobre o projeto

Este projeto apresenta o processo de extração, integração, tratamento e transformação de dados realizado a partir de um banco de dados MySQL hospedado no Microsoft Azure, utilizando o Power BI e o Power Query.

O desafio teve como objetivo aplicar, na prática, conceitos relacionados ao processo de ETL (Extract, Transform and Load), preparando os dados para utilização em análises e futuras visualizações no Power BI.

Durante o desenvolvimento, foram realizadas etapas de integração com o banco de dados, limpeza, transformação, combinação de tabelas e criação de novas informações a partir dos dados existentes.

🛠️ Tecnologias e ferramentas utilizadas
Microsoft Azure — hospedagem do banco de dados;
MySQL — gerenciamento e armazenamento dos dados;
Microsoft Power BI — integração, tratamento e análise dos dados;
Power Query — limpeza e transformação dos dados;
GitHub — documentação e disponibilização do projeto.
🔄 Etapas do projeto
1. Criação do banco de dados

Inicialmente, foi criado um banco de dados MySQL no Microsoft Azure.

Após a criação do banco, foram executados os comandos SQL disponibilizados para o desafio, responsáveis pela criação das tabelas e inserção dos respectivos registros.

2. Integração do banco de dados com o Power BI

Com o banco de dados disponibilizado no Azure, foi realizada a integração com o Power BI, permitindo a importação das tabelas para o ambiente de tratamento e transformação de dados.

Após a conexão, as tabelas foram disponibilizadas no Power Query, onde foram iniciadas as etapas de preparação dos dados.

3. Limpeza e tratamento dos dados

Com as tabelas carregadas no Power Query, foi realizada uma análise inicial da estrutura dos dados.

Durante essa etapa:

Foram excluídas colunas consideradas desnecessárias para o projeto;
Foram identificados valores nulos (Null);
Os valores nulos encontrados foram tratados e preenchidos de acordo com a necessidade de cada informação;
Foram realizadas transformações necessárias para melhorar a organização e utilização dos dados.
4. Tratamento da coluna de endereço

Na tabela Employee, a coluna referente aos endereços apresentava diferentes informações separadas pelo delimitador -.

Para facilitar a utilização e análise dessas informações, a coluna foi dividida utilizando o caractere - como delimitador.

Essa transformação permitiu separar as informações originalmente armazenadas em uma única coluna, tornando os dados mais estruturados.

5. Mesclagem das tabelas Employee e Department

Foi realizada a mesclagem entre as tabelas Employee e Department utilizando o recurso de combinação de consultas do Power Query.

O objetivo foi relacionar os funcionários aos seus respectivos departamentos, acrescentando à tabela Employee a informação correspondente ao departamento.

Após a mesclagem, foram mantidas apenas as informações necessárias para o projeto, sendo excluídas as demais colunas resultantes da combinação.

6. Criação da coluna Complete_Name

Na tabela Employee, as colunas:

Fname;
Minit;
Lname;

foram combinadas em uma única coluna denominada Complete_Name.

Essa transformação permitiu centralizar o nome completo de cada funcionário em um único campo, facilitando sua utilização em análises, relacionamentos e visualizações.

7. Identificação dos gerentes diretos

Ainda na tabela Employee, foi criada uma nova coluna denominada Super_Name.

Essa coluna apresenta o nome do gerente direto de cada funcionário, utilizando como base o relacionamento existente entre os registros de funcionários e seus respectivos supervisores.

Para realizar essa transformação, foi utilizado o recurso de Mesclar Consultas (Merge Queries) do Power Query.

8. Tratamento da tabela Dept_Locations

Na tabela Dept_Locations, foi realizada uma mesclagem com a tabela correspondente aos departamentos.

O objetivo foi associar cada localização ao respectivo nome do departamento, permitindo que as informações de localização fossem apresentadas de forma mais completa e contextualizada.

📊 Resultado

Ao final do processo, os dados originalmente armazenados no banco de dados MySQL hospedado no Azure passaram por um processo de limpeza, tratamento, transformação e integração utilizando o Power Query.

As principais transformações realizadas foram:

Conexão do Power BI com banco de dados MySQL no Azure;
Limpeza de dados;
Tratamento de valores nulos;
Exclusão de colunas desnecessárias;
Divisão de colunas utilizando delimitadores;
Mesclagem de tabelas;
Criação de novas colunas derivadas;
Combinação de informações de nome e sobrenome;
Identificação dos gestores diretos;
Associação entre departamentos e respectivas localizações.

O resultado foi um conjunto de dados mais estruturado, consistente e adequado para utilização em análises e visualizações no Power BI.

📚 Conceitos aplicados

Durante a realização do desafio, foram aplicados conceitos relacionados a:

ETL (Extract, Transform and Load)
Processo de extração dos dados da fonte, transformação das informações e preparação para utilização em análises.

Data Cleaning
Identificação e tratamento de inconsistências, valores nulos e informações desnecessárias.

Data Transformation
Alteração da estrutura dos dados para adequá-los às necessidades de análise.

Data Integration
Combinação de informações provenientes de diferentes tabelas por meio de relacionamentos e mesclagens.

Power Query
Utilização dos recursos de transformação e preparação de dados disponíveis no Power BI.

🎯 Objetivo do desafio

O desenvolvimento deste projeto teve como objetivo colocar em prática conhecimentos de Business Intelligence, integração de dados, ETL e tratamento de informações, utilizando ferramentas amplamente empregadas em processos de análise e preparação de dados.

Além da execução técnica, o projeto permitiu compreender, na prática, a importância da etapa de preparação dos dados para garantir maior qualidade e confiabilidade nas análises realizadas posteriormente.
