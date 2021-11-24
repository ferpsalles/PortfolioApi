# PortfolioApi
Portfólio e contribuições individuais de cada projeto.


## 1º Semestre - Projeto webbot - Hey Series

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

## Contribuições individuias

Desenvolvimento front-end: primeiro contato com html, css e  javascript.

```

<html>

<head>
  <meta charset="UTF-8">
  <link rel="stylesheet" type="text/css" href="../static/css/main.css">
  <title>Hey Series</title>
  <link rel="icon" type="image/png" sizes="96x96" href="../static/img/favicon-96x96.png">
  <link href="https://fonts.googleapis.com/css?family=Neuton:800&display=swap" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css?family=Alata&display=swap" rel="stylesheet">
  <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
  <script src="/static/js/jquery.js"></script>
  <script src="/static/js/index.js"></script>
</head>

<body>
  <header class="menu-principal">

    <div class="redes-sociais">
      <a href="https://gitlab.com/Jeferson.Constantino/projeto-webbot" target="_blank">
        <img src="../static/img/Git-Logo-White.png" />
      </a>
      <div class="dropdown">
        <p>ABOUT</p>
        <div class="dropdown-content">
          <p> Trabalho realizado pelos alunos da FATEC/SJC do 1º Semestre/2019.
            Consiste na criação de um webbot, coletando dados de diversas plataformas
            cinematográficas e otimizar a experiência do usuário em indicação de séries.
          </p>
        </div>
      </div>

    </div>

  </header>

  <div class="logo">
    <img src="../static/img/logo.png">
  </div>


  <div class="search">
    <input placeholder="Search Something" type="search" id="text" list="historico" />
    <i id="btnSearch" class="material-icons">
      search
    </i>
    <datalist id="historico">

    </datalist>
  </div>

  <div class="options">
    <div class="field">
      <input type="radio" id="rdbGenre" name="search" value="genre">Genre</input>&nbsp;
    </div>

    <div class="field">
      <input type="radio" id="rdbTitle" name="search" value="title">Title</input>&nbsp;
    </div>

    <div class="field">
      <input type="radio" id="rdbYear" name="search" value="year">Year</input>
    </div>
  </div>


  </div>

  <div class="results-space">

    <div class="results">
      <table id="tableSeries">
        <thead>
          <tr>
            <th>
              Title
            </th>
            <th>
              Note
            </th>
            <th>
              Genre
            </th>
            <th>
              Year
            </th>
          </tr>
        </thead>
        <tbody>
          {% for serie in data %}
          <tr>
            <td>{{serie.title}}</td>
            <td>{{serie.notes}}</td>
            <td>{{serie.genre}}</td>
            <td>{{serie.year}}</td>
          </tr>
          {% endfor %}
        </tbody>
      </table>

    </div>
  </div>

</body>



</html>
```
 
## 2º Semestre - Loading


Consiste na criação de uma aplicação web utilizando o diagrama de Gantt para análise e controle de projetos.

## Problema

O cliente busca otimizar a organização dos projetos, desenhando uma visão estratégica em um software que administre projetos, tarefas e horas trabalhadas pelos desenvolvedores. O mesmo deverá ter como base o gráfico Gantt. 

![](/Imagens/MashGGantt.gif)

## Requerimentos (Tecnologias e bibliotecas utilizadas)

- Node.js
- biblioteca: dhtmlx
- banco de dados: MySQL

## Contribuiçoes individuais

Nesse projeto, foi possível entender como trabalhar com uma nova ferramenta (dhtmlx) e configurando o front end.

```
<!doctype html>
<html lang="pt-br">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css" integrity="sha384-9aIt2nRpC12Uk9gS9baDl411NQApFmC26EwAOH8WgZl5MYYxFfc+NcPb1dKGj7Sk" crossorigin="anonymous">
    <link rel="stylesheet" type="text/css" href="static/css/cadastro.css">
    <title>Cadastro</title>
</head>
<body>
	<div class="card" id="telaCadastro" style="text-align: center">
		<div class="card-body" >
                <div class="name-body">
				<label>Nome Completo</label>
				<input type="text" class="form-control" id="name_user" placeholder="Nome Completo">
                </div>
                <div class="email-body">
                <label>Email</label>
                <input type="email" class="form-control" id="email_user" aria-describedby="emailHelp" placeholder="Digite o email">
                </div>
                <div class="form-group">
                <label>Senha</label>
                <input type="password" class="form-control" id="senha_user" placeholder="Digite a senha">
                </div>
                <button type="submit" class="btn btn-outline-secondary"  id="cadastro" onclick="cadastrar()">Cadastrar</button>
                <button type="submit" class="btn btn-outline-secondary"  id="sair" onclick="sair()">Sair</button>
		</div>
	</div>

	<script type="text/javascript">
		function sair(){
			window.location.href= "login.html";
		}
	</script>
</body>
</html>
```

```
<!DOCTYPE html>
<head>
	<meta http-equiv="Content-type" content="text/html; charset=utf-8">
	<title>DARWING!</title>

	<script src="https://cdn.dhtmlx.com/gantt/edge/dhtmlxgantt.js"></script>
	<link href="https://cdn.dhtmlx.com/gantt/edge/dhtmlxgantt.css" rel="stylesheet">
	<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
	<!-- jQuery -->
	<script src="https://code.jquery.com/jquery-3.4.1.slim.min.js" integrity="sha384-J6qa4849blE2+poT4WnyKhv5vZF5SrPo0iEjwBvKU7imGFAV0wwj1yYfoRSJoZ+n" crossorigin="anonymous"></script>
	<script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script>
	<!-- Bootstrap JS -->
	<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>
	<link rel="stylesheet" href="static/css/main.css">
	<style type="text/css">
		html, body{
			height:100%;
			padding:0px;
			margin:0px;
			overflow: hidden;
		}
		.gantt_task_line.gantt_project{
				color:white;
			}

			.gantt_side_content{
				color:#333;
			}

			.summary-bar{
				font-weight: bold;
			}

			.gantt_resource_task .gantt_task_content{
				color:inherit;
			}

			.gantt_resource_task .gantt_task_progress{
				background-color:rgba(33,33,33,0.3);
			}

			.gantt_cell:nth-child(1) .gantt_tree_content{
				border-radius: 16px;
				width: 100%;
				height: 80%;
				margin: 5% 0;
				line-height: 230%;
			}
	</style>
</head>

<body>
	<header>
		<div id="container">
		  <h5 style="text-align:center;background-color:#4b4276;color: #fff;padding: 5px 5px">DARWING</h5>
		  <nav>
		  <ul>
			<li style="text-align:center;background-color:#4b4276;color: #fff"><a><input type="radio" id="scale1" class="gantt_radio" name="scale" value="hour"><label for="scale1">Hour scale</label></a></li>
			<li style="text-align:center;background-color:#4b4276;color: #fff"><a><input type="radio" id="scale3" class="gantt_radio" name="scale" value="day"><label for="scale3">Day scale</label></a></li>
			<li style="text-align:center;background-color:#4b4276;color: #fff"><a><input type="radio" id="scale2" class="gantt_radio" name="scale" value="week"><label for="scale2">Week scale</label></a></li>	
			<li style="text-align:center;background-color:#4b4276;color: #fff"><a><input type="radio" id="scale3" class="gantt_radio" name="scale" value="month"><label for="scale3">Month scale</label></a></li>
		  </ul>
		  </nav>
		</div>
	</header>

<div id="gantt_here" style='width:100%; height:100%;'></div>
<script type="text/javascript">

gantt.config.duration_unit = "hour";
var zoomConfig = {
		levels: [
			{
				name:"hour",
				scale_height: 27,
				min_column_width:80,
				scales:[
				{unit: "hour", step: 1, format: "%H:%i"}
				]
			},
			{
				name:"day",
				scale_height: 27,
				min_column_width:80,
				scales:[
					{unit: "day", step: 1, format: "%d %M"}
				]
			},
			{
				name:"week",
				scale_height: 50,
				min_column_width:50,
				scales:[
					{unit: "week", step: 1, format: function (date) {
						var dateToStr = gantt.date.date_to_str("%d %M");
						var endDate = gantt.date.add(date, -6, "day");
						var weekNum = gantt.date.date_to_str("%W")(date);
						return "#" + weekNum + ", " + dateToStr(date) + " - " + dateToStr(endDate);
					}},
					{unit: "day", step: 1, format: "%j %D"}
				]
			},
			{
				name:"month",
				scale_height: 50,
				min_column_width:120,
				scales:[
					{unit: "month", format: "%F, %Y"},
					{unit: "week", format: "Week #%W"}
				]
			}
		]
	};

	gantt.ext.zoom.init(zoomConfig);
	gantt.ext.zoom.setLevel("day");
	gantt.ext.zoom.attachEvent("onAfterZoom", function(level, config){
		document.querySelector(".gantt_radio[value='" +config.name+ "']").checked = true;
	})

	function zoomIn(){
		gantt.ext.zoom.zoomIn();
	}
	function zoomOut(){
		gantt.ext.zoom.zoomOut()
	}

	var radios = document.getElementsByName("scale");
	for (var i = 0; i < radios.length; i++) {
		radios[i].onclick = function (event) {
			gantt.ext.zoom.setLevel(event.target.value);
		};
	}
	var dev =  [
		{key: 1, label: "Vitor", backgroundColor:"#03A9F4", textColor:"#FFF"},
		{key: 2, label: "Fernanda", backgroundColor:"#f57730", textColor:"#FFF"},
		{key: 3, label: "Gabriela", backgroundColor:"#e157de", textColor:"#FFF"},
		{key: 4, label: "Cadu", backgroundColor:"#78909C", textColor:"#FFF"},
		{key: 7, label: "Adriana", backgroundColor:"#8D6E63", textColor:"#FFF"},
		{key: 8, label: "  ", backgroundColor:"#000", textColor:"#FFF"}
	]
		//lista de DEVS'
	gantt.serverList("staff", dev);
		//CONFIG DA BARRA LATERAL
	gantt.config.grid_width = 420;
	gantt.config.grid_resize = true;
	gantt.config.open_tree_initially = true;

	var labels = gantt.locale.labels;
	labels.column_owner = labels.section_owner = "Owner";

	function byId(list, id) {
		for (var i = 0; i < list.length; i++) {
			if (list[i].key == id)
				return list[i].label || "";
		}
		return "";
	}

			//CONFIGURAÇÃO DA COLUNAS DE INFO
	gantt.config.columns = [
		{name: "owner", width: 80, align: "center", template: function (item) {
				return byId(gantt.serverList('staff'), item.owner_id)}},
		{name: "text", label: "Task name", tree: true, width: '*'},
    	{name: "start_date", align: "center", width: 80, resize: true},
    	{name: "duration", width: 60, align: "center"},
		{name: "add", width: 40}
	];
			//MODAL DA ADIÇÃO DE TAREFAS
	gantt.config.lightbox.sections = [
		{name: "description", height: 38, map_to: "text", type: "textarea", focus: true},
		{name: "owner", height: 22, map_to: "owner_id", type: "select", options: gantt.serverList("staff")},
		{name: "time", type: "duration", map_to: "auto"}
	];

	gantt.templates.grid_row_class =
		gantt.templates.task_row_class =
			gantt.templates.task_class = function (start, end, task) {
		var css = [];
		if (task.$virtual || task.type == gantt.config.types.project)
			css.push("summary-bar");

		if(task.owner_id){
			css.push("gantt_resource_task gantt_resource_" + task.owner_id);
		}

		return css.join(" ");
	};

	gantt.attachEvent("onParse", function(){
		var styleId = "dynamicGanttStyles";
		var element = document.getElementById(styleId);
		if(!element){
			element = document.createElement("style");
			element.id = styleId;
			document.querySelector("head").appendChild(element);
		}
		var html = [];
		var resources = gantt.serverList("staff");

		resources.forEach(function(r){
			html.push(".gantt_task_line.gantt_resource_" + r.key + "{" +
				"background-color:"+r.backgroundColor+"; " +
				"color:"+r.textColor+";" +
			"}");
			html.push(".gantt_row.gantt_resource_" + r.key + " .gantt_cell:nth-child(1) .gantt_tree_content{" +
				"background-color:"+r.backgroundColor+"; " +
				"color:"+r.textColor+";" +
				"}");
		});
		element.innerHTML = html.join("");
	});

	gantt.config.xml_date = "%Y-%m-%d %H:%i:%s";

	gantt.config.order_branch = true;/*!*/
	gantt.config.order_branch_free = true;/*!*/

	gantt.init("gantt_here");

	gantt.load("/data");

	var dp = new gantt.dataProcessor("/data");
	dp.init(gantt);
	dp.setTransactionMode("REST");
</script>
</body>

```

```
<!doctype html>
<html lang="pt-br">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css" integrity="sha384-9aIt2nRpC12Uk9gS9baDl411NQApFmC26EwAOH8WgZl5MYYxFfc+NcPb1dKGj7Sk" crossorigin="anonymous">
    <link rel="stylesheet" href="static/css/login.css">
    <title>Login</title>
  </head>
  <body>
    <div class="card" id="telaLogin" style="text-align: center">
		<div class="card-body" >
            <div class="cardy-body">
              <label>Usuário</label>
              <input type="email" class="form-control" id="usuario" aria-describedby="emailHelp" placeholder="Digite o email">
            </div>
            <div class="form-group">
              <label>Senha</label>
              <input type="password" class="form-control" id="senha" placeholder="Digite a senha">
            </div>
            <div class="buttons">
            <button class="btn btn-outline-secondary" id="login" onclick="validar()">Entrar</button>
            <button class="btn btn-outline-secondary" id="cadastro" onclick="cadastro()">Cadastrar</button>
            </div>
        </div>
      </div>
 </body>
<script type="text/javascript" src="js/jquery-3.5.1.slim.min.js"></script>
<script type="text/javascript">
	function validar(){
		if ($("#usuario").val()!= "admin@darwing" || $("#senha").val()!= "darwing") {
			return alert("Usuário ou Senha Inválidos");
		}
		window.location.href="index.html";

	}
	$("#usuario, #senha").keypress(function(event){
		if (event.keyCode == 13) {
			validar()
		}
	})
</script>
<script type="text/javascript">
	function cadastro(){
		window.location.href="cadastro.html"
	}
</script>
</html>

```


# KIND OF - 3º Semestre de Banco de Dados FATEC/SJC 2020/2.

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

## Contribuições individuias:

1. Front End
![Screenshot](https://gitlab.com/ferpsalles/kind-of-pi/-/blob/master/bd/login.png)

![Screenshot](https://gitlab.com/ferpsalles/kind-of-pi/-/blob/master/bd/cad.png)

2. Back-end: A aplicação foi desenvolvida com spring boot. 
Desenvolvimento do model, controller e view.


# LOADING - 4º Semestre de Banco de Dados FATEC/SJC 2021/1.

## Apresentação do Projeto</br>

### Visão do Projeto</br> <a name="-visao"/></a>
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
•    flask_mysqldb</br>]
•    sqlalchemy</br>

## Contribuições individuias

### 1. Desenvolvimento front-end e modelagem do banco de dados

![Screenshot](https://github.com/Vitordan5/API-Loading/blob/main/gifs/bancodedados.jpeg)


### 2. Rotas Disponíveis 

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
