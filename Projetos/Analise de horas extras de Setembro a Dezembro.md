
## Sobre

O projeto consiste em montar um dashboard com os dados de horas extras de Setembro a Dezembro que permita a visualização da Redução ou aumento do overtime a cada mês.

A ideia principal é mostrar que do mês de Setembro até o mês atual tivemos um cenário de redução do Overtime da base.



## Organização dos dados
Para ficar melhor essa analise, a vizualização dos dados foi separada por semanas.

## Graficos

O projeto exige os dados em alguns gráficos, que permite uma analise e interpretação precisa do cenário do overtime da base, esses gráficos são:
* Grafico de linhas (Quantidade de horas extras x )

## Prompt para analise de overtime
Claude, tenho diversas planilhas de pendências do ponto, cada uma representando um mês ( setembro a Dezembro) e me foi pedida uma analise de horas extras deste periodo para saber se houve redução das horas extras ou aumento.

A analise já foi feita, nos formatos word, excel e ipynb,mas gostaria de adicionar mais 2 meses ao periodo ( Julho e Agosto ), porém eles estão em um formato diferente dos arquivos padrões.

Preciso que você imagine que é um especialista em criar analises de horas extras e adicione esses dois meses a analise, mantendo já a estrutura atual criada ( gráficos, textos explicativos).

### Pontos importantes para a analise
* Você deve considerar apenas ocorrências contenha as palavras ( horas extras )
* Precisa desconsiderar ocorrências duplicadas também (crie um id com matricula-marcação entrada- marcação saida ( se tiver outra ocorrência de horas extras com o mesmo id, desconsiderar))
* Coluna considerada para total de horas extras : total de horas


Também quero que remova a area de recomendações, pois não necessidade dessa area em nenhum dos documentos


## Prompt para analise de absenteismo

Preciso que você imagine que é um especialista em analise de absenteismo

Claude, tenho diversas planilhas de pendências do ponto, cada uma representa um mês e preciso montar uma analise de absenteismo em cima desses dados para saber se tivemos um aumento ou diminuição no absteismo no o periodo analisado

Para isso, devemos considerar as seguintes regras:

* As planilhas de pendência de Julho e Agosto estão em um formato diferente das demais e para a analise devemos considerar somente registros onde o campo "DESCR JUSTIFICATIVA" contenha a palavra "Falta" ou "Atestado, já nas demais planilhas os registros que devem ser considerados são os registros onde o campo "SITUAÇÃO" contenha a palavra "Falta" ou "Atestado"
* Deve ser verificado se não há registros duplicados, usando como id para essa analise de duplicadas os campos ( matricula - data - "situação ou DESCR JUSTIFICATIVA" )
* Para o mês de Dezembro deve ser considerado na conta dos absenteismo + 751 ocorrências de faltas, que constam nesse relatório, pois permaneceram como débito no ponto
* Você não deve informar que a analise foi informada automaticamente ou fazer menção a si mesmo
* Analise com taxa de absenteismo e quantidade ( separando em cada grafico os absenteismo por tipo)

### Tipo de analises
Preciso que você aja com um especialista em analise de absenteismo e mostre graficamente se tivemos aumento ou diminuição no absenteismo no periodo.

### Formatos
A analise deve ser feita em excel ( com graficos incluso) e word ( esse será o arquivo enviado para a diretoria)

### Periodo da analise
Julho a Dezembro



### Diretório da analise
Pasta analise de absenteismo


## Prompt para obter atestados no mês de Julho e Agosto


Chat, tenho uma planilha de afastamentos que contém registros de afastamentos e o periodo de afastamentos ( inicio e termino )

Preciso obter a quantidade de atestados dia no mês de Julho e Agosto e para isso precisamos contabilizar os atestados que contemplam esses periodos.


Ex: atestado 1 ( inicio 31/06/2025  e termino 03/07/2025) 3 atestados dia no mês 7



Preciso que você monte um script em html,css e javascript que recebe essa planilha nesse formato e retorna uma planilha nesse formato
colaborador : inicio do atestado e termino do atestado - total de atestado dias

essa interface deve permitir eu escolher o mês que quero analisar


## Prompt para obter analise final que justifica o aumento da extra devido o aumento do absenteismo na base
Chat, precisamos agora justificar esse aumento de horas extras no mês de Dezembro e também justificar o motivo de não ter uma redução maior no periodo analisado.

Para isso preciso que analise um documento que criei que demonstra o cenário de absteismo no periodo de setembro a Dezembro, acredito que o aumento do absenteismo sirva para justificar esse aumento nas horas extras e a não redução ainda maior das horas nos meses que apresentaram redução

NOME DO DOCUMENTO : relatorio_absenteismo.docx