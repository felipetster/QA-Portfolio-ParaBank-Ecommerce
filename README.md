# 🏦 ParaBank QA Project | Portfólio de Testes Manuais

Bem-vindo(a) ao meu portfólio! Este projeto simula o dia a dia de um QA num ambiente ágil. 
O objetivo foi testar o **ParaBank** (um sistema bancário fictício), cobrindo fluxos essenciais como criar conta, login e segurança.

---

## 🛠️ O que usei nesse projeto?
* **Jira Software:** Para organizar as Sprints e tarefas (Scrum).
* **Zephyr Scale:** Para criar, organizar e rodar os testes.
* **BDD (Gherkin):** Para escrever requisitos que todo mundo entende (Dado/Quando/Então).
* **ScreenPal & Prints:** Para provar o que encontrei.

---

##  O Ciclo da Sprint 1: MVP de Acesso

A missão dessa Sprint foi garantir que novos usuários conseguissem se cadastrar e entrar no banco com segurança. Abaixo, mostro passo a passo como conduzi o processo.

### 1. Organizando a Casa (Backlog e Jira)
Primeiro, quebrei os requisitos em **User Stories** pequenas e testáveis (usando a técnica INVEST). Organizei tudo no quadro Kanban para o time saber o que estava acontecendo.

![Quadro Kanban](assets/01_jira_sprint_board.png)
*(Visão geral do Board com as tarefas organizadas)*

---

### 2. Criando os Testes (Design)
Não adianta sair clicando. Criei roteiros de teste detalhados, pensando no "Caminho Feliz" (tudo dá certo) e no "Caminho Triste" (tentar quebrar o sistema).

![Detalhe do Caso de Teste](assets/02_test_case_steps.png)
*(Exemplo de um teste escrito passo a passo)*

---

### 3. Hora da Verdade (Execução)
Rodei os testes no ambiente de Staging. O resultado foi positivo na maioria, mas encontrei problemas.

* **Resultado:** 4 Passaram (✅) / 1 Falhou (❌)

![Ciclo de Teste Zephyr](assets/03_zephyr_execution_cycle.png)
*(Lista dos testes rodados e seus status)*

---

### 4. Caçando Bugs (Defeitos)
Durante os testes de segurança, encontrei uma falha crítica no Logout. Documentei tudo bonitinho para o desenvolvedor não ter dúvida de como arrumar.

* **O Bug:** O botão "Voltar" do navegador mostrava a conta logada mesmo depois de sair.
* **Evidência:** Anexei vídeo e prints no ticket.

![Bug Report](assets/07_Bug report.png)
*(O ticket do bug aberto no Jira, com prioridade alta)*

---

### 5. Métricas e Relatórios Finais
Para fechar a Sprint, gerei os relatórios que mostram a saúde do projeto.

####  Resumo Visual (Donut Chart)
A maioria das funções está estável, com exceção do ponto de segurança.
![Gráfico Donut](assets/04_report_execution_summary.png)

####  Rastreabilidade (Traceability)
Aqui eu provo que não testei coisas aleatórias. Cada teste está ligado a um requisito de negócio.
![Matriz de Rastreabilidade](assets/05_report_traceability_matrix.png)

####  Lista Detalhada
Para quem gosta de ver o detalhe de cada execução.
![Lista Detalhada](assets/06_report_execution_details.png)

---

##  Próximos Passos (Sprint 2)
Agora que o acesso básico está testado, o plano é:
1. Validar Transferências e Pagamentos.
2. Retestar o bug de Logout assim que corrigirem.

---
*Autor: Felipe Castro | [Meu LinkedIn](felipetster)*
