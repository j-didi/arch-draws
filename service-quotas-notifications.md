## Notificação Sobre Limites de Serviços na AWS

A escalabilidade dos produtos da AWS muitas vezes nos leva a acreditar que não precisamos nos preocupar com limites dos serviços. Contudo, cada serviço possui algum tipo de restrição e monitorar esses limites é essencial para garantir a continuidade e a performance das aplicações.

Um exemplo é o limite de 1.000 instâncias de Lambdas em execução simultânea por conta. Embora esse número pareça alto, ele pode ser atingido dependendo da quantidade de funções na arquitetura e da carga do sistema.

Por isso, é crucial monitorar esses limites e planejar ações preventivas. Se os valores se aproximarem do limite, você pode, por exemplo, solicitar à AWS um aumento dessa cota.

Felizmente, ferramentas como o AWS Service Quotas facilitam esse acompanhamento. Você pode criar alarmes do CloudWatch para notificações automáticas, garantindo que sua equipe seja alertada o quanto antes.