Aula rocketSeat API em NODE.js

{"items":[],"payments":[]}

"https://api.meuapp.com/user/32?posts=true"

https:// => PROTOCOLO
api => Subdomínio
meuapp.com => Domínio
user => recurso
32 => parâmetro 
?post=true => parâmetro de busca (search/query param)

GET => Buscar informações 			GET localhost:3333/user/1/posts
POST => TODO O RESTO


TIPO DE DADOS
GET localhost:3333/users/1/posts?search=node
Route Param => Identificação de RECURSOS(OBRIGATÓRIO)
Search/Query Param => modificar/filtrar resultados (busca/paginação/ordenação) (NÃO SÃO OBRIGATÓRIOS)
POST localhost:3333/users
Request Body => Dados para criação / atualização de um recurso (obrigatórios ou opcionais)
POST/PUT/PATCH 

Headers (Cabeçalhos)
metadados => informações adicionais que não alteram o resultado/funcionamento

POST localhost:3333/users
{ email: "dasd@das.com", password: 123456 }
{id: 43 }

Header => Accept-Language: en
{ message: "Um usuário com esse email já existe" }

HTTP status codes
2xx SUCESSO 
{
201 = recurso criado (post)
202 = Aceito
204 = sem retorno 
}
3xx REDIRECIONAMENTO
4xx ERRO DO CLIENT
{ 418 = I'm a teapot ()
5xx ERRO DO SERVIDOR (API)


=================================================================