# Api REST e RESTFul
Uma API REST é um tipo de API que segue os princípios da arquitetura Representational State Transfer (REST). Ela fornece uma maneira padrão para aplicativos da Web se comunicarem entre si pela Internet, usando o protocolo HTTP e formatos de dados como JSON, XML ou YAML1. Uma API RESTful é uma implementação mais completa e estrita dos princípios REST, que adere a critérios adicionais, como a interface uniforme, clientes sem estado e operações baseadas em recursos2.

# Diferenças entre REST e RESTFul
Enquanto as APIs REST seguem os princípios básicos do REST, as APIs RESTful são uma implementação mais completa e estrita desses princípios. APIs RESTful aderem a critérios adicionais, como2:

* Interface uniforme: as APIs RESTful devem usar os mesmos verbos HTTP, códigos de status e formatos de dados para todas as requisições e respostas, de forma a garantir a consistência e a simplicidade da comunicação.
* Clientes sem estado: as APIs RESTful devem tratar cada requisição de forma independente, sem armazenar informações sobre o estado do cliente no servidor. Isso aumenta a escalabilidade e a performance da API, pois reduz a carga no servidor.
* Operações baseadas em recursos: as APIs RESTful devem identificar os recursos (entidades, objetos, dados) que são manipulados pela API por meio de URIs (identificadores uniformes de recursos) e usar os verbos HTTP para indicar as operações que são realizadas sobre esses recursos (GET, POST, PUT, DELETE, etc.).

# HTTP verbs
Os verbos HTTP são métodos que indicam a ação que o cliente deseja realizar sobre um recurso no servidor. Os verbos HTTP mais comuns usados pelas APIs REST e RESTful são1:

* GET: usado para solicitar a representação de um recurso, sem alterá-lo. É considerado um método seguro e idempotente, ou seja, não causa efeitos colaterais no servidor e pode ser repetido sem problemas.
* POST: usado para enviar dados ao servidor para criar ou atualizar um recurso. É considerado um método não seguro e não idempotente, ou seja, pode causar efeitos colaterais no servidor e não pode ser repetido sem problemas.
* PUT: usado para enviar dados ao servidor para substituir um recurso existente ou criar um novo recurso, se ele não existir. É considerado um método não seguro, mas idempotente, ou seja, pode causar efeitos colaterais no servidor, mas pode ser repetido sem problemas.
* DELETE: usado para solicitar a remoção de um recurso do servidor. É considerado um método não seguro, mas idempotente, ou seja, pode causar efeitos colaterais no servidor, mas pode ser repetido sem problemas.

#HTTP Status Code
Os códigos de status HTTP são números de três dígitos que indicam o resultado de uma requisição HTTP. Eles são divididos em cinco classes, de acordo com o primeiro dígito1:

* 1xx: códigos de informação, que indicam que a requisição foi recebida e está sendo processada pelo servidor.
* 2xx: códigos de sucesso, que indicam que a requisição foi completada com êxito pelo servidor.
* 3xx: códigos de redirecionamento, que indicam que o cliente deve fazer uma nova requisição para outro endereço para completar a operação.
* 4xx: códigos de erro do cliente, que indicam que a requisição foi malformada, não autorizada ou não encontrada pelo servidor.
* 5xx: códigos de erro do servidor, que indicam que o servidor encontrou um problema interno ao processar a requisição.
  
Alguns exemplos de códigos de status HTTP são1:

* 200 OK: indica que a requisição foi bem sucedida e o recurso solicitado foi retornado ao cliente.
* 201 Created: indica que a requisição foi bem sucedida e um novo recurso foi criado no servidor.
* 301 Moved Permanently: indica que o recurso solicitado foi movido permanentemente para outro endereço e o cliente deve usar esse novo endereço nas próximas requisições.
* 400 Bad Request: indica que a requisição foi malformada e o servidor não pôde entendê-la.
* 401 Unauthorized: indica que a requisição requer autenticação e o cliente não forneceu as credenciais necessárias.
* 404 Not Found: indica que o recurso solicitado não foi encontrado no servidor.
* 500 Internal Server Error: indica que o servidor encontrou um erro interno ao processar a requisição e não pôde completá-la.
