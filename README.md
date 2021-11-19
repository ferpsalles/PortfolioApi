# PortfolioApi
Portfólio e contribuições individuais de cada projeto.


1. 1º Semestre

Hey Series
Trabalho realizado pelos alunos da FATEC/SJC do 1º Semestre/2019. Consiste na criação de um webbot, coletando dados de diversas plataformas cinematográficas e otimizar a experiência do usuário em indicação de séries.

Construção

Git Bash
Visual Code ou PyCharm


Requerimentos (Instalação de bibliotecas)

Python 3
Pip3


Instalação do projeto/ Funcionalidade

Crie uma pasta no seu computador
Abra o terminal
Faça o clone do projeto com git clone https://gitlab.com/Jeferson.Constantino/projeto-webbot.git

Abrir a pasta 'projeto-webbot'
Abrir o diretório: CÓDIGO/Front End/ProjetoPI - HTML
Instalar as dependências através do pip3: pip3 install bs4, pip3 install requests, pip3 install flask

2. 2º Semestre -

## Projeto Integrador realizado pelos alunos do 2º (segundo) semestre de Banco de Dados da FATEC/SJC no ano de 2020.

Consiste na criação de uma aplicação web utilizando o diagrama de Gantt para análise e controle de projetos.

1. Disciplinas relacionadas:
- Arquitetura e Modelagem de Banco de dados - Prof Emanuel Mineda
- Engenharia de Software - Prof Giuliano Araujo Bertoti
- Linguagem de Programação I - Prof Adriana da Silva Jacinto
- Laboratório em Desenvolvimento em Banco de Dados II - Prof Adriana da Silva Jacinto

## Problema

O cliente busca otimizar a organização dos projetos, desenhando uma visão estratégica em um software que administre projetos, tarefas e horas trabalhadas pelos desenvolvedores. O mesmo deverá ter como base o gráfico Gantt. 

![](/Imagens/MashGGantt.gif)

## Requerimentos (Tecnologias e bibliotecas utilizadas)

- Node.js
- biblioteca: dhtmlx
- banco de dados: MySQL

## Levantamento de requisitos:
Criação de uma tabela dinâmica (projetos) com livre movimentação de tarefas, que será designada para cada projeto, e designar desenvolvedores para elas.

##### Requisitos Funcionais

| Requisitos funcionais             |  Código |              Descrição                                                                                                                                     |Prioridade|
| ----------------------------------|---------| -----------------------------------------------------------------------------------------------------------------------------------------------------------|----------|
|Cadastrar projetos                 |RF01     |Pessoas responsáveis para o registro no sistema serão capacitados para cadastrar os projetos, informando: data, cliente, descrição, tarefa e desenvolvedores|    1     |
|Cadastrar tarefas                  |RF02     |Cadastrar tarefas em projetos existentes (Informar: tempo de desenvolvimento, desenvolvedor e descrição)                                                    |    2     |
|Cadastrar desenvolvedores          |RF03     |Cadastrar desenvolvedores em tarefas existentes (Informar: nome, carga horária de trabalho e disponibilidade)                                               |    3     |   
|Excluir dados                      |RF04     |O usuário poderá excluir dados envolvendo os projetos, tarefas e desenvolvedores designados                                                                 |    4     |       
|Alterar dados                      |RF05     |O usuário poderá alterar dados envolvendo os projetos, tarefas e desenvolvedores designados                                                                 |    5     |
|Filtrar dados                      |RF06     |O sistema poderá filtrar os dados: projetos, tarefas e desenvolvedores                                                                                      |    6     |
|Gerar relatórios                   |RF07     |O usuário poderá imprimir relatórios: projetos, tarefas e desenvolvedores                                                                                   |    7     |                                              


##### Requisitos não funcionais


| Requisitos não funcionais         |  Código |              Descrição                                                                                                           |
| ----------------------------------|---------| ---------------------------------------------------------------------------------------------------------------------------------|
|Usabilidade                        |RNF01    |Estética e Design minimalista: A interface do usuário deve ser implementada de maneira simples (interface web)                    |
|Visibilidade do status do sistema  |RNF02    |As tarefas e projetos serão organizados em cores: verde (em andamento), amarelo (chegando perto da entrega) e vermelho (entregue) |
|Consistência e padrões             |RNF03    |Consistência e padrões: Os dados serão visualizados em tabelas (diagrama de gantt)                                                |                                                                               |             
|Portabilidade                      |RNF04    |A consulta ao acervo deve estar disponivel na internet (principais navegadores disponíveis)                                       |
|Acesso de segurança                |RNF05    |O sistema deve controlar o acesso das funcionalidades                                                                             |                                                                                     |              
|Responsividade                     |RNF06    |Velocidade de resposta e tempo de atualização de tela                                                                             |                 


## Instalação do projeto/ Funcionalidade

1) Clonar reposiório, dando o seguinte comando no terminal de sua maquina: git clone "https://gitlab.com/VitorDan/projeto-integrador-2-sem.-2020.git"
2) Abrir o terminal dentro da pasta do projeto e digitar "npm install", para instalar os módulos utilizados.
3) Com o Mysql instalado, criar um banco de dados na porta "3306" com o nome "gantt_howto_node" e implementar as tabelas que estão no aquivo schema.sql
4) Abrir o terminal no arquivo server.js e digitar "node server.js".
5) O projeto será executado na porta "1337" no "localhost".


3. 3º Sementre

## :page_with_curl: Sobre o projeto <a name="-sobre"/></a>

> É proposto o desenvolvimento de um Sistema de Recompensas dentro de uma aplicação do cliente. O cliente busca otimizar seu negócio através de uma dashbord, com as informações mais atrativas e impactantes para seus clientes. O cliente pode acompanhar seus respectivos dados de maneira segura e organizada, e caso necessário, e tomar a decisões a partir delas.

O objetivo do trabalho é reinventar a forma de aproximação do usuário da plataforma. Não consistindo na criação web de apenas consultas, mas sim em uma aplicação utilizando o sistema de recompensas, na qual o usuário poderá utiliza-los dentro da aplicação com o que o cliente poderá fornecer. As recompensas foram demostradas através de cursos que poderão auxiliar o usuário com a própria gestão financeira. 


## :memo: Referências <a name="-tecnologias"/></a> 

```
- Java, Html, Css, JavaScript
- frameworks: Spring Boot, Boostrap 
- banco de dados relacional: MySQL
```

## :memo: Levantamento de Requisitos <a name="-requisitos"/></a> 


> Criação de uma aplicação web com dashbord estatistica, com a linguagem principal utilizada sendo o Java.

> A aplicação deve conter um login. As informações apresentadas devem ser intuitivas pois trata-se de um ambiente com assuntos financeiros, ou seja, deve agregar pessoas bancarizadas e não bancarizadas. 

> A aplicação precisa agregar valor a um sistema já em andamento. A aproximação do cliente/usuário será realizada atraves da utilização de pontos e utilizar na "loja" virtual ambientalizada dentro do login de cada usuário.


4. 4º Semestre 

# Apresentação do Projeto</br>

## Visão do Projeto</br> <a name="-visao"/></a>
O projeto realizado está na área de recrutamento de candidatos, na qual consiste na criação de uma api web simples para criação de vaga e busca do candidato, com foco na otimização da seleção. A estruturação de um eficiente processo de recrutamento facilita a seleção de talentos e competências necessárias para a continuidade e o sucesso das instituições.
</br></br>

## Funcionalidade </br>

O usuário poderá selecionar candidato atráves de filtros, sendo ele: pcd, conhecimento, idioma, vale transporte (vt), nível de escolaridade. Os filtros foram alinhados juntamente com o cliente, sendo fixado o vt < 3 quilômetros da instituição como vt =0. Todos os filtros são ordenados conforme necessidade e relevancia do usuário para a busca do candidado "ideal". Ao criar uma vaga, a mesma irá trazer os candidatos, assim como, a pesquisa isolada dos candidatos também será permitido. 

## Tecnologias Utilizadas</br> <a name="-tecnologias"/></a>
•    [Python 3.9](https://www.python.org/)</br>
•    [MySQL](https://www.mysql.com/)</br>
•    [Flask 2.0](https://flask.palletsprojects.com/en/2.0.x/)</br>
•    [Postman](https://www.postman.com/)</br>


As escolhas das tecnologias foram baseadas em performance e redução de complexidade. A escolha de um banco relacional MySQL possibilitou a criação de indices que aumentaram a performance do próprio banco com um número volumoso de dados, assim como o MySQL se tornou o mais popular banco de dados Open Source do mundo.

## Bibliotecas Utilizadas</br> <a name="-bibliotecas"/></a>
•    requests </br>
•    ast</br>
•    flask_mysqldb</br>
•    sqlalchemy</br>

As bibliotecas utilizadas facilitaram na comunicação com o banco de dados, assim como cálculos de localização e aproximação dos candidatos. 


## Instruções de implementação </br> <a name="-instrucao"/></a>

 > Crie o banco de dados 
 1. Utilizar o script SQL que está na pasta "API-Loading/projetointegrador/bd/bd.sql" para ter o modelo do banco.
 
 > Como rodar a aplicação:
 1. Alterar as configurações do banco de dados nos arquivos "bd.py" e "app.py"
 2. Para [configurar e executar o ambiente virtual](https://www.youtube.com/watch?v=hA2l0TgaZhM), a pasta do ambiente virtual criado para este projeto se encontra na pasta "venv" 
 4. Com o ambiente virtual ativado execute o arquivo "app.py"
 5. Recomendamos que utilize o software [Postman](https://www.postman.com/downloads/) para testar a rotas disponiveis no projeto.

# Requisitos</br> <a name="-requisitos"/></a>
## Requisitos Funcionais</br>

· Criar interface de submissão de currículos que recebam, de forma padronizada e adequada ao processo, os candidatos; </br>
· Busca de candidatos por vagas; </br>
· Utilizar filtros configuráveis nas buscas de cada vaga; </br>


## Requisitos Não Funcionais</br>
· Arquitetura do BD;</br>
· Desempenho;</br>
· Segurança (Safety);</br>
· Documentação específica;</br>


## Rotas Disponíveis <a name="-rotas"/></a>

|  ROTAS  CRUD | METHOD | RESPOSTA |
|--------|----------|----------|
| "/insertUsuario" | "POST" | Criação de usuários que são capazes de criar vagas |
| "/insertVaga | "POST" | Inserção de vaga no banco de dados|
| "/updateVaga/informe o id" | "PUT" | Update das descrições da vaga |
| "/dropVaga/informe o id"| "DELETE" | Deletar Vaga |
| "/filterVaga/informe o id" | "GET" | Filtrar as informações da vaga |
| "/filterVaga" | "GET" | Listar todas as vagas disponíveis | 
| "/filterVagaPeso/informe o id" | "GET" | Filtro da vaga retornando os candidatos | 
| "/insertCandidato" | "POST" | Inserir candidatos |
| "/updateCandidato/informe o cpf" | "PUT" | Atualização dos dados do candidato |
| "/dropCandidato/informe o cpf"| "DELETE" | Deletar candidato |
| "/filterCandidato/cep=informe o cep" | "GET" | Filtra candidatos |
| "/filterCandidato" | "GET" | Filtrar todos os candidatos | 
   
##  Exemplos de inserção das rotas disponíveis
   
Informar os dados para inserção do Candidato:</br>
· É necessário informar todas os dados;</br>
· O nível de escolaridade é formado por um ENUM com os seguintes dados (Sem Escolaridade, Tecnico, Medio Completo, Ensino Superior, Pos Graduado);</br>
· Caso só tenha um idioma e um conhecimento é necessário manter dentro de [ ] conforme o exemplo;</br>
· Caso só tenha uma experiencia é necessário manter dentro de [ { } ] conforme o exemplo;</br>
   
```
/insertCandidato
{ 
    "nomeCandidato":"João",
    "cpfCandidato":"0000000000",
    "dataNascimentoCandidato":"01/01/1999",
    "emailCandidato":"joao@hotmail.com",
    "pcdCandidato": 2,
    "cepCandidato":"12335130",
    "telResCandidato":"988888888",
    "telCelCandidato":"988888888",
    "nivelEsc": "Medio Completo",
    "conhecimento": [1, 2, 3],
    "idioma": [1, 2, 3],
    "experiencia": [{"empresa":"EXPERIENCIA", "cargo":"DEV", "tempo": 19},
   {"empresa":"EXPERIENCIA1", "cargo":"DEV", "tempo": 10},
   {"empresa":"EXPERIENCIA2", "cargo":"DEV", "tempo": 4}]
}
```

Para realizar o Update:</br>
· Informar o CPF do candidato na rota e o JSON com as informações a serem atualizadas no exemplo serão atualizados apenas o conhecimento e o idioma.</br>

```
/updateCandidato/informar o CPF
{
    "conhecimento": [2],
    "idioma": [2],
} 
```

Para excluir um candidato informar apenas o CPF do candidato na rota:

```
/dropCandidato/informar o CPF
```

Informar o CEP da "VAGA" na rota para calcular as distancias e o JSON com os filtros caso não queira utilizar algum filtro basta remover a chave:

```
/filterCandidato/cep= informar o CEP
{
    "pcdCandidato": 2,
    "nivelEsc": "Medio Completo",
    "conhecimento": 3,
    "idioma": 2
}
```

Para listar todos os candidatos cadastrados utilize apenas a rota:

```
/filterCandidato
```

Informar os dados para inserção da Vaga:</br>
· Nome , IdUsuario e  CEP são essenciais.</br>

```
/insertVaga
{
    "nomeVaga":"Vaga",
    "idUsuario":1,
    "idConhecimento": 1,
    "pesoConhecimento": 2,
    "idIdiomaVaga": 1,
    "pesoIdioma": 1,
    "cepVaga":"12335130",
    "nivelEsc": "Medio Completo",
    "pesoEscolaridade": 4,
    "pcdVaga": 2,
    "pesoPCD": 3,
    "vt":1
}
```

Informar a ID da vaga na rota e o JSON com as informações a serem atualizadas, no exemplo serão atualizados apenas o conhecimento, idioma e o VT:

```
/updateVaga/<id>
{
    "idConhecimento": 2,
    "idIdiomaVaga": NULL,
    "vt":0
}
 ```
   
Para excluir uma vaga utilize apenas a ID da vaga na rota:   
   
   ```  
/dropVaga/<id>
  ```
 
Para filtrar as informações de uma vaga, utilize apenas a ID da vaga na rota:
  
  ``` 
/filterVaga/<id>
  ``` 
  
Para listar todas as vagas cadastradas use apenas a rota:
 
 ```
/filterVaga
```

Para exibir a vaga com os candidatos filtrados:</br>
· Informe a ID da vaga na rota e o JSON com a ordenação desejada do s candidatos;</br>
· No exemplo ele esta ondenando primeiramente  os candidatos com PCD igual a sim e posteriormente pelo idioma e assim por diante.</br>
   
   ``` 
   /filterVagaPeso/<id>
{
    "order":["pcdCandidato","idioma.idIdioma", "nivelEscolaridade", "conhecimento.idConhecimento"]
}
