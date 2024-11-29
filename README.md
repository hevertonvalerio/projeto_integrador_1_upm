## Projeto de Saúde e Nutrição com base nos dados do Sisvan

Este projeto tem intuito de contribuir para o planejamento de políticas públicas estaduais, fundamentado nos dados disponíveis na base nacional do Sistema de Vigilância Alimentar e Nutricional (Sisvan). 

## Objetivo

O objetivo do projeto é elaborar um estudo de Análise Exploratória de Dados sobre o contexto do estado nutricional da população brasileira, em específico das crianças com idades compreendidas entre 0 e 6 anos.

## Estrutura do Projeto

- Extrair Dados: Acessar os dados disponíveis sobre estado de nutrição infantil disponível no Datasus e extrair os dados necessários;

- Transformar Dados: Após a etapa de extração, seguiremos com as etapas de filtragem dos dados, processamento e apresentação das informações; 

- Análise e Visualização: Estudo de investigação um conjunto de
dados e sintetizar as suas características principais, usando técnicas e métodos
quantitativos e de visualização de dados, que ampare o planejamento de políticas públicas no combate a desnutrição infantil;

- Relatório Final: Destacaremos as principais descobertas, oferecendo algumas recomendações com base nas percepções encontradas na análise. Com isso, visamos elaborar índices que amparem o Ministério da Saúde e as Secretarias Estaduais a tomar decisões baseadas em dados.

## Recursos Utilizados

- Python

- Google Colab

- Visual Studio Code

- Github


## Bibliotecas Python

- Pandas

- PySpark


## Docentes:

- Professor Thiago Graziani Traue

- Professor Tutor Vinicius Piro Barragam 


## Discentes:

- Bruna Freitas Soares

- Heverton Valerio de Lima

- João Victor Fontebasso Alves

- Mariana Silva de Oliveira


###
---
## Variáveis do Dataset

### **Código do Acompanhamento**  
> #### CO_ACOMPANHAMENTO  
> Código único que identifica  
o acompanhamento  
realizado pelo indivíduo  
> ***

### **Código do Indivíduo**
> #### CO_PESSOA_SISVAN   
> Código de identificação do
indivíduo
> ***  

### **Status Participa ANDI**  
> #### ST_PARTICIPA_ANDI  
> Status que indica se o município  
é participante do programa Atenção Nutricional à Desnutrição Infantil (ANDI) S: sim; N:
não  
> ***

### **Código do Município**
> #### CO_MUNICIPIO_IBGE   
> Código IBGE do município.
> ***

### **Código do CNES**  
> #### CO_CNES  
> Estabelecimento de Saúde
> ***

### **Idade em Anos**
> #### NU_IDADE_ANO   
> Anos de vida do indivíduo
> ***

### **Código da Fase da Vida**  
> #### NU_FASE_VIDA  
|Código|Descrição|
|---|---|
|1|'MENOR DE 6 MESES'|
|2|'ENTRE 6 MESES A 2 ANOS'|
|3|'ENTRE 2 ANOS A 5 ANOS'|
|4|'ENTRE 5 ANOS A 7 ANOS'|
|5|'ENTRE 7 ANOS A 10 ANOS'| 
|6|'ADOLESCENTE'|
|7|'ADULTO'|
|8|'IDOSO'|

### **Fase da Vida**  
> #### DS_FASE_VIDA  
> Campo textual com a
descrição das fases da vida
> ***

### **Sexo**
> #### SG_SEXO   
|Código|Descrição|
|---|---|
|0|Masculino|
|1|Feminino|

### **Código da Raça/Cor**  
> #### CO_RACA_COR  
> Código da raça/cor declarada pelo indivíduo:  
Branca, Preta, Amarela, Parda, Indígena, ou Sem Informação  
> **Códigos:**  

|Código|Descrição|
|---|---|
|X | Invalido|
|01 | Branca  |
|02 | Preta  |
|03 | Amarela | 
|04 | Parda  |
|05 | Indígena|  
|99 | Sem Informação  |
> ***

### **Raça/Cor**  
> #### DS_RACA_COR  
> Descrição textual da raça/cor declarada pelo indivíduo  
> ***

### **Código do Povo ou Comunidade Tradicional**
> #### CO_POVO_COMUNIDADE   

|Código|Descrição|
|---|---|
|1|POVOS QUILOMBOLAS|
|2 | AGROEXTRATIVISTAS|
|3 | CAATINGUEIROS|
|4 | CAIÇARAS|
|5 | COMUNIDADES DE FUNDO E FECHO DE PASTO|
|6 | COMUNIDADES DO CERRADO|
|7 | EXTRATIVISTAS|
|8 | FAXINALENSES|
|9 | GERAIZEIROS|
|10 | MARISQUEIROS|
|11 | PANTANEIROS|
|12 | PESCADORES ARTESANAIS|
|13 | POMERANOS|
|14 | POVOS CIGANOS|
|15 | POVOS DE TERREIRO|
|16 | QUEBRADEIRAS DE COCO-DE-BABAÇU|
|17 | RETIREIROS|
|18 | RIBEIRINHOS|
|19 | SERINGUEIROS|
|20 | VAZANTEIROS|
|21 | OUTROS|

### **Descrição do Povo ou Comunidade Tradicional**  
> #### DS_POVO_COMUNIDADE  
> Descrição do povo ou comunidade  
> ***

### **Código da Escolaridade**
> #### CO_ESCOLARIDADE   

|Código|Descrição|
|---|---|
|1|Creche|
|2 | Pré-escola (exceto CA)|
|3 | Classe Alfabetizada - CA|
|4 | Ensino Fundamental 1ª a 4ª séries|
|5 | Ensino Fundamental 5ª a 8ª séries|
|6 | Ensino Fundamental Completo|
|7 | Ensino Fundamental Especial|
|8 | Ensino Fundamental EJA - séries iniciais (Supletivo 1ª a 4ª)|
|9 | Ensino Fundamental EJA - séries iniciais (Supletivo 5ª a 8ª)|
|10 | Ensino Médio, Médio 2º Ciclo (Científico, Técnico e etc)|
|11 | Ensino Médio Especial|
|12 | Ensino Médio EJA (Supletivo)|
|13 | Superior, Aperfeiçoamento, Especialização, Mestrado, Doutorado|


### **Descrição a Escolaridade**
> #### DS_ESCOLARIDADE   
> Descrição da Escolaridade  
> ***  

### **Data do Acompanhamento**
> #### DT_ACOMPANHAMENTO   
> Data do Acompanhamento nutricional do Indivíduo  
> ***  

### **Competência do Acompanhamento (ANO MÊS)**
> #### NU_COMPETENCIA   
> Competência do acompanhamento
nutricional que este registro faz referência.  
Formato do campo: YYYYMM (ANO MÊS)  
> ***  

### **Peso**
> #### NU_PESO   
> Peso do Indivíduo em Quilos  
> ***  

### **Altura**
> #### NU_ALTURA   
> Altura em Centímetros  
> ***  

### **Índice de Massa Corporal - IMC**
> #### DS_IMC   
> Índice de Massa Corporal - IMC  
> ***  

### **Índice de Massa Corporal Pré Gestacional - IMC**
> #### DS_IMC_PRE_GESTACIONAL   
> Índice de Massa Corporal Pré Gestacional - IMC  
> ***  

### **Estado Nutricional de Peso para Idade de Crianças (0 a 10 anos)**
> #### PESO X IDADE   
> Cálculo Nutricional de
crianças (0 a 10 anos) com
as seguintes informações:
'Muito baixo peso para a
idade', 'Baixo peso para a
idade', 'Peso adequado
para idade', 'Peso elevado
para a idade'
> ***

### **Estado Nutricional de Peso para Altura de Crianças (0 a 10 anos)**
> #### PESO X ALTURA   
> Cálculo Nutricional de
crianças (0 a 5 anos) com
as seguintes informações:
'Magreza acentuada',
'Magreza', 'Peso Adequado
ou Eutrófico', 'Risco de
sobrepeso', 'Sobrepeso';
crianças (5 a 10 anos) com
as seguintes informações:
'Magreza acentuada',
'Magreza', 'Peso Adequado
ou Eutrófico', 'Sobrepeso',
'Obesidade' 
   
> ***  

### **Estado Nutricional de Altura para Idade de Crianças (0 a 10 anos)**
> #### CRI. ALTURA X IDADE   
> Cálculo Nutricional de
crianças (0 a 10 anos) com
as seguintes informações:
'Muito baixa estatura para
idade', 'Baixa estatura para
idade', 'Estatura
adequada para a idade'
> ***

### **Estado Nutricional de IMC para Idade de Crianças (0 a 10 anos)**
> #### CRI. IMC X IDADE
> Cálculo Nutricional de
crianças (0 a 10 anos) com
as seguintes informações:
'Magreza acentuada’,
‘Magreza’, ‘Eutrofia', 'Risco
de sobrepeso',
'Sobrepeso', 'Obesidade'
> ***


### **Estado Nutricional de Altura para Idade de Adolescentes (10 a menos de 20 anos)**  
> #### ADO. ALTURA X IDADE  
> Cálculo Nutricional de adolescentes (10 a menos de 20 anos) com as seguintes informações:  
> 'Muito baixa estatura para idade', 'Baixa estatura para idade', 'Estatura adequada para a idade'  
> ***  

### **Estado Nutricional de IMC para Idade de Adolescentes (10 a menos de 20 anos)**  
> #### ADO. IMC X IDADE  
> Cálculo Nutricional de adolescentes (10 a menos de 20 anos) com as seguintes informações:  
> 'Magreza acentuada', 'Magreza', 'Eutrofia', 'Risco de sobrepeso', 'Sobrepeso', 'Obesidade'  

### **Estado Nutricional de Adultos**  
> #### CO_ESTADO_NUTRI_ADULTO  
> Cálculo Nutricional de adultos (20 a 60 anos) com as seguintes informações:  
> 'Baixo peso', 'Adequado ou Eutrófico', 'Sobrepeso', 'Obesidade Grau I', 'Obesidade Grau II', 'Obesidade Grau III'  
> ***  

### **Estado Nutricional de Idosos**  
> #### CO_ESTADO_NUTRI_IDOSO  
> Cálculo Nutricional de idosos (60 anos ou mais) com as seguintes informações:  
> 'Baixo peso', 'Adequado ou Eutrófico', 'Sobrepeso'  
> ***  

### **Estado Nutricional de Gestantes**  
> #### CO_ESTADO_NUTRI_IMC_SEMGEST  
> Cálculo Nutricional de Adolescentes e adultas (10 a 60 anos) com as seguintes informações:  
> 'Baixo peso', 'Adequado ou Eutrófico', 'Sobrepeso', 'Obesidade'  
> ***  

### **Código do Sistema de Origem**  
> #### CO_SISTEMA_ORIGEM_ACOMP  
> Código do sistema de origem, 1, 'SISVAN WEB', 2, 'AUXILIO BRASIL', 4, 'ESUS AB'  
> ***  

### **Sistema de Origem**  
> #### DS_SISTEMA_ORIGEM_ACOMP  
> Código do sistema de origem, 1, 'SISVAN WEB', 2, 'AUXILIO BRASIL', 4, 'ESUS AB'  
> ***  
