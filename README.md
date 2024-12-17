# 🚀 **Processo de QA**

Este repositório documenta as melhores práticas de **Qualidade de Software (QA)** abordadas durante o curso. O conteúdo foca em estratégias de teste, gerenciamento de tarefas com Jira e o ciclo de vida de bugs.

---

## 📋 **Conteúdos**

1. [User Story](#user-story)  
2. [Mind Map](#mind-map)  
3. [Testes Step by Step](#testes-step-by-step)  
4. [BDD - Behavior-Driven Development](#bdd---behavior-driven-development)  
5. [Uso do Jira](#uso-do-jira)  
6. [Ciclo de Vida de Bugs](#ciclo-de-vida-de-bugs)  

---

## 📝 **User Story**

Uma **User Story** descreve uma funcionalidade do sistema do ponto de vista do usuário. Ela é escrita no formato:

- **Como [persona]**,  
- **Quero [ação]**,  
- **Para [benefício]**.  

### **Exemplo:**
> *"Como um cliente, quero resetar minha senha para acessar o sistema caso eu esqueça."*

### **Aceitação da User Story:**
Adicione critérios de aceitação para validar se a funcionalidade foi entregue corretamente.  
- O usuário consegue solicitar a redefinição da senha.  
- O sistema envia um e-mail com link de recuperação.  
- A nova senha é aceita após redefinição.  

---

## 🧩 **Mind Map**

O **Mind Map** é uma técnica de visualização para organizar as ideias e os testes. Ele ajuda a identificar cenários principais e alternativas.

### **Exemplo de Ferramentas:**
- XMind  
- Miro  
- Lucidchart  

### **Estrutura:**
- **Funcionalidade Principal** (ex.: Login)  
  - Cenários Positivos (ex.: Login válido)  
  - Cenários Negativos (ex.: Senha incorreta, usuário inexistente)  
  - Cenários de Erro (ex.: Falha de rede)  

---

## 🔄 **Testes Step by Step**

Os **Testes Step by Step** descrevem cada etapa que deve ser realizada para validar uma funcionalidade.

### **Exemplo de Teste: Login**

| Passo | Ação                           | Resultado Esperado            |
|-------|--------------------------------|--------------------------------|
| 1     | Abrir a página de login        | A página é carregada           |
| 2     | Inserir usuário e senha válidos | Usuário logado com sucesso     |
| 3     | Inserir senha inválida         | Mensagem de erro exibida       |

---

## 🧪 **BDD - Behavior-Driven Development**

O **BDD** é uma abordagem focada em comportamento, escrita no formato **Given/When/Then**.

### **Formato Geral:**
```gherkin
Feature: [Título da funcionalidade]
  Scenario: [Título do cenário]
    Given [Contexto]
    When [Ação]
    Then [Resultado esperado]
```
Exemplo: Resetar Senha
```gherkin
Feature: Recuperação de senha
  Scenario: Usuário solicita recuperação de senha com e-mail válido
    Given que o usuário está na página de recuperação de senha
    When ele insere um e-mail cadastrado e solicita recuperação
    Then o sistema envia um e-mail com um link de redefinição
```

---


# 🛠️ **Uso do Jira**

O **Jira** é uma ferramenta essencial para gerenciar tarefas, bugs e histórias de usuário no processo de QA. Aqui estão algumas orientações de como usar o Jira de forma eficiente:

---

## 📋 **Como Usar**

### **Criação de User Stories:**
- Utilize o formato **Como/Quero/Para**:
  - **Como [persona]**,  
  - **Quero [ação]**,  
  - **Para [benefício]**.  
- **Adicione critérios de aceitação** para garantir que a funcionalidade seja validada corretamente.

---

### **Criação de Bugs:**
Ao criar um bug no Jira, é importante incluir as seguintes informações:

1. **Comportamento Esperado**: O que deveria ocorrer.
2. **Comportamento Atual**: O que está acontecendo de forma inesperada.
3. **Passos para Reproduzir**: Como replicar o erro.
4. **Evidências**: Como prints de tela, vídeos ou logs.
5. **Prioridade**: Qual a urgência de resolver o problema.
6. **Versão do Sistema**: Em qual versão o bug foi encontrado.

---

## 📊 **Boards de Kanban/Scrum**

No Jira, você pode organizar suas tarefas utilizando Boards de **Kanban** ou **Scrum**. Esses Boards ajudam a visualizar o progresso das tarefas de maneira eficiente.

### **Colunas do Board:**

1. **To Do (A Fazer)**: Tarefas a serem realizadas.
2. **In Progress (Em Andamento)**: Tarefas que estão em andamento.
3. **Done (Concluído)**: Tarefas finalizadas.

Mova os cards entre essas colunas conforme o progresso da tarefa, mantendo o fluxo de trabalho claro e organizado.

---


# 🐛 **Ciclo de Vida de Bugs**

O **ciclo de vida de bugs** define os estados pelos quais um defeito passa desde o seu primeiro relatório até a sua resolução final. Cada estado é importante para o acompanhamento adequado da correção do bug.

---

## 📅 **Estados do Ciclo de Vida do Bug**

1. **Novo**: Bug reportado pela primeira vez.
2. **Atribuído**: O bug foi atribuído a um desenvolvedor para correção.
3. **Em Correção**: O bug está sendo corrigido pelo desenvolvedor.
4. **Para Teste**: O bug foi corrigido e está aguardando a validação/teste da equipe de QA.
5. **Reaberto**: Caso o problema persista ou ocorra novamente após a correção, o bug é reaberto.
6. **Fechado**: O bug foi confirmado como resolvido, seja por correção bem-sucedida ou por não ser mais relevante.

---

## 📊 **Exemplo Visual do Ciclo de Vida do Bug**

```css
[ Novo ] -> [ Atribuído ] -> [ Em Correção ] -> [ Para Teste ] -> [ Fechado ]
                             ↑                              ↓
                          [ Reaberto ]
```
---


## 🤝 **Conclusão**

Entender o ciclo de vida de um bug é essencial para garantir que todos os envolvidos no processo de QA — desde desenvolvedores até testers — saibam exatamente onde o problema está e como ele será tratado. O fluxo bem definido, desde o momento em que um bug é reportado até sua correção e fechamento, facilita a comunicação e melhora a eficiência da equipe.

Com uma gestão organizada no Jira, cada tarefa recebe a atenção necessária e é tratada da forma mais eficaz, garantindo que o produto final seja cada vez mais robusto e sem falhas. Lembre-se, o processo de correção de bugs não é apenas sobre encontrar e corrigir erros, mas sobre aprender com eles para melhorar continuamente.

Ao seguir esses passos e manter uma boa comunicação dentro da equipe, você contribui diretamente para a entrega de um software de qualidade, mais confiável e melhor para os usuários.
