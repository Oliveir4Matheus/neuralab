

Chat, eu tenho um sistema que realiza diversas requisições para um sistema de gestão de marcações do ponto e escala e estou com um problema na funcionalidade responsável por realizar o envio de alterações de escala.

A lógica é a seguinte:
O colaborador envia uma planilha que contém nome, matrícula e horário de escala dos colaboradores e os dias de folga, dias trabalhados ou dias que ele entra outro horário ( esses são preenchidos com um código de horário entre ( * )  e o sistema, através de um arquivo de horários ( horários.csv, converte os horários de escala do colaborador em código de horário, pegando o código de horário que corresponde ao horário de escala dele e convertendo os dias de folgas e dias trabalhados do colaborador em um outro formato.

O problema é que:
Ao tentar realizar a conversão da escala dos colaboradores, diversos códigos não estão sendo convertidos, sendo que os mesmos constam na planilha de horários essa que pode ser facilmente encontrada na pasta server>horarios.csv

Preciso que você analise a lógica atual implementada e encontre onde está ocorrendo a falha.

Agora um ponto importante: Essa funcionalidade já está bem ajustada e qualquer ajuste que não tenha haver com o problema que te informei pode causar diversos problemas na escala do colaborador. 
Por isso preciso que você analise com cuidado, encontre o problema e documente o que você fez na pasta /docs, inclusve, caso tenha alguma dúvida me pergunte

Outro ponto importante, isso funciona localmenten, mas quando rodo na minha vps ( via container docker - docker compose ) o problema acontece

Eu consegui ser claro 