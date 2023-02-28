# Análise Do Brasileirão - Série A
 
Este projeto visa analisar os dados de 3.039 partidas do campeonado brasileiro de futebol masculino (serie A) referentes aos anos de 2015 até 2022, para responder a 5 perguntas de negócio.

**1 - Quais clubes venceram mais partidas?**

**2 - Quais clubes colecionam o maior número de cartões amarelos e vermelhos?**

**3 - Quais clubes marcaram mais gols?**

**4 - Quem são os maiores artilheiros do campeonato?**

**5 - Qual período do jogo costuma sair o maior número de gols?**

Estes dados serão posteriormente apresentados em um modelo de visualização utilizando o Power BI.

As perguntas 1 e 2 poderão ser respondidas de forma segmentada por ano, rodada e estádio. Já as perguntas 3, 4 e 5 poderão ser respondidas de forma segmentada por clube. 

Você poderá acessar o Dashboard clicando em:
<a href="https://app.powerbi.com/view?r=eyJrIjoiNjI2YjkxMjktZDEzOS00NTIyLWFiOWMtMjFiNjA4MzE0Njc5IiwidCI6IjUzYmMxZDQ4LTgxMWEtNGI0Ny1hYzFkLWRhYzQ2NmQwMjZjYSJ9">Dashboard Analítico do Brasileirão Série A</a>. 

## Fonte Dos Dados
Os dados originais foram extraídos da fonte: https://github.com/adaoduque/Brasileirao_Dataset. 

Você também pode encontra-los na pasta *dados_originais* ou no data.world através do link: https://data.world/raulrosa/brasileirao

## Tecnologias Utilizadas
* SQL (data.world)
* Python (Google Colab)
* Power BI

## Como Reproduzir Os Resultados

**1** - Os arquivos .csv presentes na pasta dados_originais foram carregados em um dataset do data.world: <a href="https://data.world/raulrosa/brasileirao"> brasileirao0322</a>.

**2** - Utilizando consultas em SQL no data.world, foi criado um novo dataset: <a href="https://data.world/raulrosa/brasileirao1522">brasileirao1522</a>, com algumas transformações iniciais no intuito de:
* Selecionar apenas a colunas consideradas relevantes para análise;
* Renomear colunas com o objetivo de manter o padrão de nomenclatura, principalmente da chave primária;
* Filtrar os dados referentes as partidas ocorridas a partir de 2015.
* Os arquivos .csv gerados e a sintaxe SQL utilizada para as transformações iniciais também podem ser acessadas na pasta *dados_tranformados_sql*.

**3** - Por meio da instalação da <a href="https://pypi.org/project/datadotworld/">Biblioteca Datadotworld</a> em um notebook do Google Colab foi possível:
* Carregar os arquivos .csv presentes no data.world em diferentes dataframes da biblioteca pandas;
* Tratar de dados e valores ausentes utilizando linguagem Python;
* Gravar os arquivos com as transformações no data.world.

**4** - Todo a passo a passo em python pode ser acessado em: <a href="https://colab.research.google.com/drive/1fJ0LC2SXrRXolNPIRyBDqaZUSkQTXWhL?usp=sharing">AnaliseBrasileirao</a>.

**5** - Todo o projeto utilizando o data.world pode ser acessado em: https://data.world/raulrosa/brasileirao1522.

**6** - Para facilitar a visualização dos dados e responder as 5 perguntas de negócio, foi utilizado o Power BI. Essa ferramenta permite que os dados sejam importados diretamente da sua conta no data.world.

O arquivos .csv contendo os dados finais e utilizados como fonte para criação do Dashboard no Power BI, também podem ser encontrados nas pasta *dados_transformados_python*. 

Muitas das variáveis tratadas utilizando linguagem python e disponíveis nas colunas dos arquivos .csv finais, não foram utilizadas para criação do dashboard proposto, porém foram mantidas com o objetivo de serem necessárias para futuras análises.

## Resultados 

![image](https://user-images.githubusercontent.com/75815212/221917008-5c8f0380-4b44-4291-a6c3-c49cf297d8c0.png)

Analisando o print do dashboard acima para todas as 3.039 partidas, é possível responder as 5 perguntas de negócio:

**1 - Quais clubes venceram mais partidas?**

**2 - Quais clubes colecionam o maior número de cartões amarelos e vermelhos?**

**3 - Quais clubes marcaram mais gols?**

**4 - Quem são os maiores artilheiros do campeonato?**

**5 - Qual período do jogo costuma sair o maior número de gols?**

Você também pode acessar o Dashboard de forma interativa clicando em:
<a href="https://app.powerbi.com/view?r=eyJrIjoiNjI2YjkxMjktZDEzOS00NTIyLWFiOWMtMjFiNjA4MzE0Njc5IiwidCI6IjUzYmMxZDQ4LTgxMWEtNGI0Ny1hYzFkLWRhYzQ2NmQwMjZjYSJ9">Dashboard Analítico do Brasileirão Série A</a>. 

## Sugestões Para Projetos Futuros

1 - Quais clubes com o maior número de faltas?

2 - Em qual período do jogo costuma ter o maior número de faltas e cartões?

3 - Quais clubes possuem o maior percentual de posse de bola?

4 - Qual o número medio de faltas, cartões, escanteios, chutes e gols por jogo?

## Contato
Para possíveis dúvidas, críticas ou sugestões sobre o presente projeto.

E-mail: raulrosa.dev@gmail.com

LinkedIn: linkedin.com/in/raul-rosa/
