# Ficha4


## Como executar o projeto

1. Abre dois terminais no VS Code.
2. No primeiro terminal, entra na pasta `server` e executa `npm start`.
3. No segundo terminal, entra na pasta `client` e executa `npm run dev`.
4. Abre o endereço indicado pelo Vite no browser.

## 3. Quem bloqueou o fetch?

Quem bloqueou foi o browser, através da política CORS.
Se o servidor não tivesse recebido o pedido, não apareceria nada no seu terminal.
Como o pedido chega ao servidor, mas o browser bloqueia a resposta, sabemos que é um problema de CORS.
A solução é configurar o header `Access-Control-Allow-Origin` no servidor.

## 4. Comparação com a Ficha 3

Agora a app React faz 1 request ao abrir para ir buscar as cartas ao servidor.
Ao filtrar, não faz novos requests, porque os dados já estão carregados.
Os dados vivem no servidor e são enviados para o client através da API.
O HTML é construído no client pelo React, no browser.

