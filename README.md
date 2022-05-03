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

Caso de Uso : Enviar tabela por Email
#
O usuário deve acessar a opção de envio da planilha gerada por e-mail. O usuário insere o email desejado e
clica no botão selecionar para  buscar o relatório em excel. Ele então seleciona o relátorio e clica na opção
enviar.
O sistema emite um alerta dizendo que o email com o relatório foi enviado com sucesso.

<h3>Caso de Uso: Gerar planilha excel baseado na tabela FIPE</h3>
#
O usuário acessa o sistema e seleciona em caixa de seleção o tipo de
veículo que ele está buscando(caminhão, carro ou moto),
deve informar também o ano inicial da busca e o ano final da busca.
Após o usuário clica no botão gerra planilha e o sistema começa a busca baseado nos 
parametros informados(Caso de Uso: Consulta FIPE).Após gerar o relatório o sistema deve emitir um alerta
dizendo que a atividade foi concluída com suscesso. No arquivo Excel devem ser exibidos os 
seguintes dados: Código Fipe do veículo, nome do veículo, valor, ano e tipo de combustível.

<h3>Caso de Uso : Consuta FIPE,<h3>
#
O sistema deve realizar uma busca através uma API Web que traz dados oficais da FIPE quais são os veículos
de acordo com os paramentros selecinados. Esses dados irão compor a planilha do Excel.



<h3>Diagrama  de Classe<h3>

  
![Untitled](https://user-images.githubusercontent.com/103469667/165191013-6dae9e47-a696-4936-b8d6-552a9ffd99f6.png)
  
  
  # Diagram de Atividade FIPEEXCEL

![diagrama de Atividade FIPEXCEL](https://user-images.githubusercontent.com/103469667/166343179-bccc16ae-e94c-4c2a-939e-83d8d84dfb64.png)
