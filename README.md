Integrantes:

Wendel Silva

Gustavo Pereira

Matheus Tinel

AJAX

AJAX / Asynchronous JavaScript and XML, é um conjunto de técnicas de desenvolvimento web que permite que aplicações enviem e recebam dados do servidor de forma assíncrona, sem precisar recarregar a página inteira. Isso proporciona uma experiência de usuário mais fluida e interativa.

Operação Assíncronada

Uma operação assíncrona é um modelo de execução onde uma tarefa pode ser iniciada e o controle é retornado ao chamador antes que a tarefa seja concluída. Isso permite que outras operações sejam executadas enquanto se aguarda a conclusão da tarefa assíncrona, melhorando a eficiência e a responsividade do sistema. Uma tarefa será executado mesmo que a outra não tiver sido concluída.

XmlHttpRequest:

O XMLHttpRequest (XHR) é um objeto JavaScript que permite a comunicação entre um cliente (em um navegador) com um servidor. Ele é fundamental para a construção de aplicações web modernas, pois possibilita o envio e recebimento de dados sem a necessidade de recarregar a página inteira

Velocidade levemente mais rápido em algumas situações devido à sua implementação mais antiga e otimizada, não suporta ReadableStream, tem o suporte nativo com .abort(), e a compatibilidade alta, sendo possível em navegadores mais antigos.

Sintaxe complexa de se entender (devido ao boilerplate necessário),controle de erros requer múltiplos eventos (onload, onerror) e verificações manuais de estado (readyState, status).

Fetch:

O Fetch é uma API moderna do JavaScript que permite fazer requisições HTTP/HTTPS de forma assíncrona. Ele oferece uma maneira mais intuitiva e fácil de realizar chamadas de rede, substituindo o uso do XMLHttpRequest.

Velocidade semelhante ao XmlHttpRequest, porém, mais eficiente em operações de streaming devido ao suporte a ReadableStream, suporta ReadableStream, permitindo melhor desempenho em leitura de dados em fluxo, tem suporte com AbortController e a compatibilidade boa, exceto para navegadores antigos.

Sintaxe Moderna e mais legível, simplifica requisições HTTP, leitura de código mais limpa e direta e o controle de erros simples com .catch().

Promises:

Promises (ou Promessas) são uma abstração utilizada para representar fluxos de ações em código assíncrono. Em JavaScript, uma Promise é um objeto que representa o resultado de uma operação assíncrona, podendo este resultado ser bem-sucedido ou falhar.

Velocidade igual ao fetch, pois Promises são usadas por trás (no backEnd), o streaming Depende da API utilizada e o cancelamento é feito de forma manual.

async/await:

sync/await é uma sintaxe introduzida no JavaScript para simplificar o trabalho com operações assíncronas, tornando o código mais legível e fácil de entender. Ele foi introduzido na versão ES2017 (ES8) do JavaScript.

A velocidade é Igual ao fetch, pois usa Promises por trás, suporta ReadableStream, tem o cancelamento com AbortController e a facilidade de uso.

A sintaxe requer conhecimento de Promises, usa métodos .then() e .catch() para encadear ações, leitura de código pode ficar confuso com muitos encadeamentos e tem o controle de erros com .then() e .catch().

Fontes:

https://stackoverflow.com/questions/70882625/fetch-vs-ajax-vs-xmlhttprequest-why-is-fetch-so-much-more-incredibly-fast

https://dev.to/krushna_sananse/understanding-ajax-xmlhttprequest-and-fetch-api-in-javascript-ijf

https://www.geeksforgeeks.org/difference-between-ajax-and-fetch-api/

https://www.w3schools.com/js/js_api_fetch.asp

https://www.w3schools.com/xml/xml_http.asp

https://www.w3schools.com/Js/js_promise.asp

Site utilizado para o fetch na web:

https://jsonplaceholder.typicode.com/
