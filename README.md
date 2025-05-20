
XmlHttpRequest:

Velocidade: Levemente mais rápido em algumas situações devido à sua implementação mais antiga e otimizada.
Streaming: Limitado, não suporta ReadableStream.
Cancelamento: Suporte nativo com .abort().
Compatibilidade: Alta, incluindo navegadores antigos como o Internet Explorer.
fetch:

Velocidade: Semelhante ao XmlHttpRequest, mas pode ser mais eficiente em operações de streaming devido ao suporte a ReadableStream 1.
Streaming: Suporta ReadableStream, permitindo melhor desempenho em leitura de dados em fluxo 2.
Cancelamento: Suporte com AbortController.
Compatibilidade: Boa, exceto para navegadores muito antigos.
Promises:

Velocidade: Igual ao fetch, pois Promises são usadas por trás.
Streaming: Depende da API utilizada.
Cancelamento: Manual.
async/await:

Velocidade: Igual ao fetch, pois usa Promises por trás.
Streaming: Suporta ReadableStream.
Cancelamento: Com AbortController.
Facilidade de Uso
XmlHttpRequest:

Sintaxe: Verbosa e complexa, requer múltiplos eventos (onload, onerror) e verificações manuais de estado (readyState, status).
Leitura de código: Pouco legível devido ao boilerplate necessário.
Controle de erros: Complexo, usando eventos.
fetch:

Sintaxe: Moderna e mais legível, simplifica requisições HTTP.
Leitura de código: Mais limpa e direta.
Controle de erros: Simples com .catch()1.
Promises:

Sintaxe: Requer conhecimento de Promises, usa métodos .then() e .catch() para encadear ações.
Leitura de código: Pode ficar confuso com muitos encadeamentos.
Controle de erros: Sim, com .then() e .catch().
async/await:

Sintaxe: Extremamente legível e próximo de código síncrono.
Leitura de código: Muito legível e fácil de entender.
Controle de erros: Claro com try/catch .

Fontes:
https://stackoverflow.com/questions/70882625/fetch-vs-ajax-vs-xmlhttprequest-why-is-fetch-so-much-more-incredibly-fast
https://dev.to/krushna_sananse/understanding-ajax-xmlhttprequest-and-fetch-api-in-javascript-ijf
https://www.geeksforgeeks.org/difference-between-ajax-and-fetch-api/
https://www.w3schools.com/js/js_api_fetch.asp
https://www.w3schools.com/xml/xml_http.asp

