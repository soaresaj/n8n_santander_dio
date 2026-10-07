Atue como um especialista em N8N.

Quero criar uma automação no N8N para:

[gerenciar leads desde o primeiro contato até o fechamento da venda, integrando formulários de captura, CRM, notificações internas e follow-up automático.]

Público ou responsável:

[Equipe de Marketing, Equipe de Atendimento/Customer Success, Equipe Financeira, Gestão/Administrativo]

Resultado esperado:

[Essa automação integrada cria um ecossistema colaborativo: vendas capturam e nutrem leads, marketing analisa conversões, atendimento garante experiência positiva, financeiro acompanha impactos e gestão tem visão estratégica. Ou seja, é uma solução transversal que conecta várias áreas da empresa em torno de um fluxo único.]

Ferramentas envolvidas:
[Webhook Node, Function Node, HTTP Request Node, Slack/Teams/Email Node, Google Sheets, Drive Node]

Fluxo desejado:

1 - [Entrada: dados chegam via Webhook.]

2 - [Validação: Function Node verifica se os campos obrigatórios estão corretos.]

3 - [Decisão: aplica regras de prioridade (ex.: APROVADO → segue para pagamento).]

4 - [Integração: HTTP Request envia dados para CRM, ERP ou API bancária.]

5 - [Notificação: Slack/Teams/Email informa a equipe responsável.]

6 - [Armazenamento: Google Sheets/Drive registra o evento para histórico.]

7 - [Monitoramento: Scheduler revisa periodicamente o status e dispara alertas se necessário.]

8 - [Saída: Output Node retorna resposta padronizada ao sistema que chamou o fluxo.]

Regras importantes:

[Regras de decisão:
START → VALIDATE
PROCESS → SAVE
ERROR → RETRY
END → FINISH
Qualquer outro valor → INVALID]

[Validações:
Campos obrigatórios devem estar presentes (ex.: clienteId, status).
Comparação exata de strings (maiúsculas/minúsculas).]

[Exceções:
Se status for inválido → retorna INVALID.
Se faltar campo essencial → envia para revisão manual.
Se API externa não responder → fluxo retorna erro e dispara alerta.]

Explique quais nós do N8N devem ser utilizados e a lógica de funcionamento do workflow.
