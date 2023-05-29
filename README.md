API para Sistema de Avaliação de Créditos
Uma empresa de empréstimo precisa criar um sistema de análise de solicitação de crédito. Sua tarefa será criar uma API REST SPRING BOOT E KOTLIN 🍃💜 para a empresa fornecer aos seus clientes as seguintes funcionalidades:

Cliente (Customer):
Cadastrar:
Request: firstName, lastName, cpf, income, email, password, zipCode e street
Response: String
Editar cadastro:
Request: id, firstName, lastName, income, zipCode, street
Response: firstName, lastName, income, cpf, email, income, zipCode, street
Visualizar perfil:
Request: id
Response: firstName, lastName, income, cpf, email, income, zipCode, street
Deletar cadastro:
Request: id
Response: sem retorno
Solicitação de Empréstimo (Credit):
Cadastrar:
Request: creditValue, dayFirstOfInstallment, numberOfInstallments e customerId
Response: String
Listar todas as solicitações de emprestimo de um cliente:
Request: customerId
Response: creditCode, creditValue, numberOfInstallment
Visualizar um emprestimo:
Request: customerId e creditCode
Response: creditCode, creditValue, numberOfInstallment, status, emailCustomer e incomeCustomer
API para Sistema de Avaliação de Créditos
Diagrama UML Simplificado de uma API para Sistema de Avaliação de Crédito

Arquitetura em 3 camadas Projeto Spring Boot
Arquitetura em 3 camadas Projeto Spring Boot

DESAFIO
Implemente as regras de negócio a seguir para a solicitação de empréstimo:

o máximo de parcelas permitido será 48
data da primeira parcela deverá ser no máximo 3 meses após o dia atual
