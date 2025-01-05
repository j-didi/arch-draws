## Gerando Relatórios de Login de Clientes via AWS Cognito

O Cognito é a ferramenta de autenticação como serviço da AWS. Com o Cognito User Pools, você pode adicionar autenticação nas suas aplicações e usufruir de recursos como: grupos de permissões, login social, autenticação de multiplos fatores, entre outros.

Muitas empresas já utilizam o Cognito para prover autenticação para seus microsserviços, principalmente pela integração simples com o AWS API Gateway, garantindo que toda requisição que passe pelo API Gateway possua um token válido.

Porém o Cognito não entrega relatórios sobre logins, e algumas empresas precisam desses dados para análises de segurança ou até mesmo para monitorar o uso da plataforma. Então, como entregar essa funcionalidade de forma simple e sem impactar a performance do login na sua aplicação?

Uma opção simples é direcionar os logs do Cognito, que incluem eventos de login, para o CloudWatch Logs. A partir daí, você pode utilizar o CloudWatch Log Insights, por exemplo via Lambda, para executar queries nos logs e processar os resultados.