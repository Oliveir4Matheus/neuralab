
Chat, tenho uma aplicação web que realiza requisições a uma determinada api e para determinadas requisições utiliza um tunnel ssh entre a VPS e uma maquina local como proxy para a requisição.

Configurei esse tunnel ssh entre os dois sistemas, porém quando tento enviar requisições de login, estou recebendo timeout e ao acessar a rota da aplicação /api/senior/diagnostico, obtenho o seguinte cenário:
|||
|---|---|
|success|true|
|message|"Diagnostico de conectividade com Senior"|
|data||
|timestamp|"2026-01-07T14:53:58.122Z"|
|tests||
|publicIP||
|success|true|
|ip|"194.35.120.137"|
|seniorLoginPage||
|success|true|
|status|200|
|statusText|"OK"|
|contentLength|10603|
|headers||
|server|"volt-adc"|
|content-type|"text/html"|
|seniorLoginEndpoint||
|success|true|
|status|500|
|statusText|"Internal Server Error"|
|loginErrorStatus|"401"|
|location|"nao presente"|
|hasCookies|true|
|gestaoPontoAPI||
|success|false|
|error|"timeout of 15000ms exceeded"|
|code|"ECONNABORTED"|
|proxyConfig||
|enabled|true|
|configured|true|
|url|"[https://127.0.0.1:8888](https://127.0.0.1:8888 "https://127.0.0.1:8888")"|
|gestaoPontoAPIviaProxy||
|success|false|
|error|"connect ECONNREFUSED 127.0.0.1:8888"|
|code|"ECONNREFUSED"|
|ipViaProxy||
|success|false|
|error|"connect ECONNREFUSED 127.0.0.1:8888"|
|code|"ECONNREFUSED"|

Preciso que idêntifique o problema