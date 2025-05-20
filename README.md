Integrantes:

Wendel Silva

Gustavo Pereira

Matheus Tinel

XmlHttpRequest:

Velocidade levemente mais rápido em algumas situações devido à sua implementação mais antiga e otimizada, não suporta ReadableStream, tem o suporte nativo com .abort(), e a compatibilidade alta, sendo possível em navegadores mais antigos.

Fetch:

Velocidade semelhante ao XmlHttpRequest, porém, mais eficiente em operações de streaming devido ao suporte a ReadableStream, suporta ReadableStream, permitindo melhor desempenho em leitura de dados em fluxo, tem suporte com AbortController e a compatibilidade boa, exceto para navegadores antigos.

Promises:

Velocidade igual ao fetch, pois Promises são usadas por trás (no backEnd), o streaming Depende da API utilizada e o cancelamento é feito de forma manual.

async/await:

A velocidade é Igual ao fetch, pois usa Promises por trás, suporta ReadableStream, tem o cancelamento Com AbortController e a facilidade de Uso

XmlHttpRequest:

Sintaxe: Verbosa e complexa, requer múltiplos eventos (onload, onerror) e verificações manuais de estado (readyState, status).
Leitura de código: Pouco legível devido ao boilerplate necessário.
Controle de erros: Complexo, usando eventos.

fetch:

Sintaxe: Moderna e mais legível, simplifica requisições HTTP.
Leitura de código: Mais limpa e direta.
Controle de erros: Simples com .catch().
Promises:

Sintaxe: Requer conhecimento de Promises, usa métodos .then() e .catch() para encadear ações.
Leitura de código: Pode ficar confuso com muitos encadeamentos.
Controle de erros: Sim, com .then() e .catch().
async/await:

A sintaxe é de fácil entendimento e próximo de código síncrono, sendo mais "simples" na leitura do código e o controle de erros simples com : try/catch .

Fontes:

https://stackoverflow.com/questions/70882625/fetch-vs-ajax-vs-xmlhttprequest-why-is-fetch-so-much-more-incredibly-fast

https://dev.to/krushna_sananse/understanding-ajax-xmlhttprequest-and-fetch-api-in-javascript-ijf

https://www.geeksforgeeks.org/difference-between-ajax-and-fetch-api/

https://www.w3schools.com/js/js_api_fetch.asp

https://www.w3schools.com/xml/xml_http.asp
