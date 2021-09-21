### API, REST, e RESTFUL

---

#### API

###### Cliente (Client)

###### Garçom (pedidos, levar seu pedidos, para a cozinha) (API)

###### Cozinha (Server)

Acrônimo de **Application Programming Interface** (Interface de Programação de Aplicações) é basicamente um conjunto de rotinas e padrões estabelecidos por uma aplicação, para que outras aplicações possam utilizas as funcionalidades desta aplicação.

- Responsável por estabelecer comunicação entre diferentes serviços.
- Meio de campo entra as tecnologias.
- Intermediador para troca de informações.

---

#### REST

Acrônimo para **REpresentational State Transfer** (Transferência de Estado Repesentativo).
Será feita a transferência de dados de uma maneira simbólica, figurativa, representativa, de maneira didática.
A transferência de dados, geralmente, usando o protocolo **HTTP**.
**Resources** seria então, uma entidade, um objeto.

#### <div align="center"> 6 NECESSIDADES (constraints) para ser RESTful </div>

#### _Client-server_

**Separação** do cliente e do armazenamento de dados (**servidor**), dessa forma, poderemos ter uma portabilidade do nossso sitema, usando o React para Web e React Native para mobile, por exemplo.

#### _Stateless_

Cada requisição que o cliente faz para o servidor, **deverá conter todas as informações necessárias para o servidor** entender e responder (**RESPONSE**), a requisição (**REQUEST**).

**Exemplo**: A sessão do usuário deverá ser enviada em todas as requisições, para saber se aquele usuário está autenticadoe apto a usar os serviços

#### _Cacheable_

As repostas para uma requisição, deverão ser explicitadas ao dizer se aquela requisição, pode ou não ser cacheada pelo cliente.

#### _Layered System_

O cliente acessa um **endpoint**, sem precisar saber da complexidade, de quais passos estão sendo necessários para o servidor responder a requisição, ou quais outras camadas o servidor estará lidando, para que a requisição seja respondida.

#### _Conde on Demand (optional)_

Dá a possibilitade da nossa aplicação pegar códigos, como o javascript, para por exemplo executar no cliente.

#### _Uniform Interface_

Uniform significa "uniforme", ou seja, uma única forma, quando usamos um **endpoint** (`/client`) do nosso **resource**, devemos sempre seguir isso para todos os Resources. Então, a interface que estamos construindo para os resources está seguindo essa constraint. Foi criado uma **padronização** dos resources.

**Exemplo 01**: Sabe quando falo que usamos por padrão o .json como formato de escrita das mensagens? Então. Desde que sua API não fiquei usando uma hora json, outra hora xml, outra hora outro formato, você continua seguindo o conceito de uniformidade da interface, e maneira de se comunicar está bacana. Sua API está coerente até aqui.

**Exemplo 02**: Quando a API precisa enviar detalhes para quem está consumindo ela. Então, é necessário sempre manter o resource com informações suficientes para quem vai consumi-lo. Talvez links para outros endpoints, por exemplo.

**Exemplo 03**: Quando se deve usar certinho os verbos HTTP para comunicação clara e efetiva. O uso correto dos verbos é coerente, então, estamos sendo uniformes na nossa interface.

Até aqui, fica intuitivo e tranquilo para meu cliente entender como minha API funciona, e o que posso fazer com ela, então, a **Interface** está **Uniforme**.

---

#### RESTFUL

RESTful, é a aplicação dos padrões REST.
