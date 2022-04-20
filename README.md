# fipeexcel
Projeto desenvolvido no SENAI BETIM, inspirado na ideia  do aluno Bruno Gomes
<h1> FIPEEXCEL</h1>

Uma concessionária de veículos realiza consultas online a tabela
FIPE(tabela de valores de automóveis) mensalmente. O tempo gasto nessas
consultas é em média <b>2 horas</b> diárias, pois são consultados cerca de
400 veículos. Visando solucionar esse problema
criamos um sistema que consulta os dados online e os armazena em uma
planilha excel. Utilizando o sistema o <b> tempos gasto na consulta cai para
em média 5 minutos</b>.

# Requisitos Funcionais do Sistema

RF-001: O sistema deve permitir a busca de informação dos veículos a partir
de um código e ano de fabricação.

RF-002: O sistema deve gravar os dados  retornados pela
consulta em um arquivo Excel, os dados que são aramazenados
são: Código do Veículo, Marca, Modelo, Ano, Preço, Tipo de
Combustível, Mês de Referência da Consulta.

# Requisitos Não Funcionais

RNF: 001 - O sistema deve salvar o arquivo  em XLSX versão 
2007 ou superior.

RNF: 002 - Sistema deve ter acesso a internet.

RNF: 003 - O usuário deve ter instalado em seu computador o
Python na versão 3.7 ou superior.

# Regra de Negócio

Regra de Negócio: 001 - Consulta a tabela FIPE. A consulta a tabela FIPE deve 
ser feita pela código oficial do véculo, todo veículo possui um código,
gerenciado pela organização que cuida da FIPE. Requisito Funcional - 001.


# Caso de Uso
![uc001](https://user-images.githubusercontent.com/103469667/164120790-fdb51af7-1b7b-4675-bb97-98bf269827de.png)

#Caso de Uso: FIPEEXCEL

Visão Geral:  Gerar Excel com fipe dos veículos: Este sistema gerar  uma tabela fipe dos veículos
que mostra uma tabela com as descrisãos dos veículos .
 
Consultar Fipe: o usuário ele vai ser deparar com uma tabela de consulta fipe  dos veículos que estão localizado na tabela.

Enviar Tabela por email: E logo em seguida o usuário vai ser deparar no sue email o código  já pronto.
https://parallelum.com.br/fipe/api/v2/cars/brands
