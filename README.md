# Desafio-dio-power-bi-transformacao-dados

  Para completar esse desafio era necessário criar um banco de dados, fazer a limpeza e transformação e criar um relatório a partir destes dados.
  A primeira etapa foi criar o banco de dados na azure e fazer a integração com o Power BI.
  Após os dados estarem no Power BI foi necessário fazer a limpeza e transformação dos dados, que seguiu os passos abaixo:
    
    	- Verificação dos cabeçalhos e tipos de dados;
  		- Os valores monetários foram modificados para o tipo double preciso;
  		- Verificada a existência dos nulos e os únicos encontrados foram os gerentes, que por padrão
    	não tem Super_ssn;
  		- Verificado os colaboradores e não há colaborador sem gerente;
  		- Verificado os departamentos e não há departamento sem gerente;
   		- Verificado o número de horas dos projetos;
    	- A coluna adress da tabela employee foi dividida em 4 novas colunas: Street, Number, City and State. 
     	Para isso foi necessário modificar um dos valores da coluna, o "Fire-Oak" foi trocado para 
       	"FireOak", depois foi utilizado o delimitador "-" para concluir a divisão;
    	- Mesclagem das consultas employee e departament para criar uma tabela employees com o nome dos 
     	departamentos associados aos colaboradores. A mescla teve como base a tabela employee;
    	- Foram eliminadas as colunas desnecessárias da tabela employees;
    	- Mesclada as colunas de Nome e Sobrenome da tabela employees para ter apenas uma coluna definindo os
     	nomes dos colaboradores; 
    	- Realizada a junção dos colaboradores e respectivos nomes dos gerentes utilizando a mescla;
    	- Mescla dos nomes de departamentos e localização;
    	- No caso acima foi utilzado o mesclar, já que era necessário juntar informações de duas colunas
     	diferentes. Já o atribuir é usado quando é necessário adicionar uma nova coluna com valores 
       	calculados ou derivados, ou seja, iria modificar os dados existentes;
    	- Agrupamento dos dados a fim de saber quantos colaboradores existem por gerente;
    	- Eliminação das colunas desnecessárias, que não serão usadas no relatório, de cada tabela;
    	- Mesclado horas trabalhadas por colaboradores;
    	- Mesclado número de dependentes por colaborador.
  Por fim foi criado um relatório utilizando estes dados.

