
#API Tests Postman 

Projeto de automação de testes de API utilizando Postman para validação dos principais endpoints da API ServeRest, com validação de cenários positivos e negativos.


#Tecnologias utilizadas
Postman
Serverest - API REST
JavaScript para scripts de teste


#Fluxos testados 
-Cadastro de usuario
-Login (autenticacao)
-Criacao de produto
-Listagem de produto
-Exclusao de produto


#Cenarios testados: 
Positivos:
Criar usuario
Login com sucesso
Criar produto com token
Deletar produto com token


Negativos: 
Criar usuário com email duplicado
Criar produto sem token
Deletar produto sem token 
Deletar produto com ID inexistente


Como executar >
1. Importar a collection no Postman
2. Importar o environment
3. Executar via Collection Runner


Execução via Newman
Para rodar os testes via terminal:
npm install -g newman
newman run collections/serverest_collection.json -e environments/serverest_environment.json
 
 
Relatório de testes
Para gerar relatório em HTML:
npm install -g newman-reporter-html
newman run collections/serverest_collection.json -e environments/serverest_environment.json -r html


Diferenciais: 
Uso de variáveis de ambiente
Encadeamento de requisições
Testes automatizados com validação de status code 
Organização por módulos
Newman para execução automatizada dos testes via terminal e geração de relatórios


Desenvolvido por Maria Eduarda Parrela 

