## Notificações de Login do Usuário Root

Primeiro uma ressalva, a AWS recomenda fortemente não utilizar o usuário Root da conta para tarefas do dia a dia, pois este possui acesso quase ilimitado a todos os recursos.

No entanto, algumas tarefas específicas, como o gerenciamento de certificados, configurações de recursos de segurança e administração da conta, ainda exigem o uso do usuário Root.

Para esses casos isolados, pode ser útil configurar notificações de login do usuário Root para reforçar a segurança.

Nesta arquitetura proposta, o evento de login no Console da AWS, registrado pelo CloudTrail, é capturado por uma regra do EventBridge, que encaminha o evento para uma função Lambda. Essa função realiza a integração com o canal de comunicação desejado.hello
