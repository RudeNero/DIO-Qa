# DIO-QA

🚀 Processo de QA
Este repositório documenta as melhores práticas de Qualidade de Software (QA) abordadas durante o curso. O conteúdo foca em estratégias de teste, gerenciamento de tarefas com Jira e o ciclo de vida de bugs.

📋 Conteúdos
User Story
Mind Map
Testes Step by Step
BDD - Behavior-Driven Development
Uso do Jira
Ciclo de Vida de Bugs
📝 User Story
Uma User Story descreve uma funcionalidade do sistema do ponto de vista do usuário. Ela é escrita no formato:

Como [persona],
Quero [ação],
Para [benefício].
Exemplo:
"Como um cliente, quero resetar minha senha para acessar o sistema caso eu esqueça."

Aceitação da User Story:
Adicione critérios de aceitação para validar se a funcionalidade foi entregue corretamente.

O usuário consegue solicitar a redefinição da senha.
O sistema envia um e-mail com link de recuperação.
A nova senha é aceita após redefinição.
🧩 Mind Map
O Mind Map é uma técnica de visualização para organizar as ideias e os testes. Ele ajuda a identificar cenários principais e alternativas.

Exemplo de Ferramentas:
XMind
Miro
Lucidchart
Estrutura:
Funcionalidade Principal (ex.: Login)
Cenários Positivos (ex.: Login válido)
Cenários Negativos (ex.: Senha incorreta, usuário inexistente)
Cenários de Erro (ex.: Falha de rede)
🔄 Testes Step by Step
Os Testes Step by Step descrevem cada etapa que deve ser realizada para validar uma funcionalidade.

Exemplo de Teste: Login
Passo Ação Resultado Esperado
1 Abrir a página de login A página é carregada
2 Inserir usuário e senha válidos Usuário logado com sucesso
3 Inserir senha inválida Mensagem de erro exibida
🧪 BDD - Behavior-Driven Development
O BDD é uma abordagem focada em comportamento, escrita no formato Given/When/Then.

Formato Geral:
gherkin

Feature: [Título da funcionalidade]
Scenario: [Título do cenário]
Given [Contexto]
When [Ação]
Then [Resultado esperado]
Exemplo: Resetar Senha
gherkin

Feature: Recuperação de senha
Scenario: Usuário solicita recuperação de senha com e-mail válido
Given que o usuário está na página de recuperação de senha
When ele insere um e-mail cadastrado e solicita recuperação
Then o sistema envia um e-mail com um link de redefinição
🛠️ Uso do Jira
O Jira é usado para gerenciar tarefas, bugs e histórias de usuário.

Como Usar:
Criação de User Stories:

Use o formato Como/Quero/Para.
Adicione critérios de aceitação.
Criação de Bugs:

Informe o Comportamento Esperado e o Comportamento Atual.
Adicione passos para reproduzir e evidências (print, vídeo).
Boards de Kanban/Scrum:

Acompanhe tarefas em To Do, In Progress e Done.
Movimente os cards conforme o progresso.
🐛 Ciclo de Vida de Bugs
O ciclo de vida de bugs define os estados pelos quais um defeito passa:

Novo: Bug reportado pela primeira vez.
Atribuído: Atribuído para um desenvolvedor.
Em Correção: Bug sendo corrigido.
Para Teste: Bug corrigido e enviado para teste.
Reaberto: Caso o problema persista.
Fechado: Bug confirmado como resolvido.
Exemplo Visual:
css

[ Novo ] -> [ Atribuído ] -> [ Em Correção ] -> [ Para Teste ] -> [ Fechado ]
↑ ↓
[ Reaberto ]  
🔗 Links Úteis
Documentação Oficial do Jira
Ferramentas para BDD
Gerador de Mind Maps Gratuito
💡 Conclusão
Este documento cobre os principais tópicos para estruturar um processo de QA eficiente, desde o planejamento com User Stories até a execução com BDD e gerenciamento de bugs.

🔍 Explore, colabore e pratique! 🚀
