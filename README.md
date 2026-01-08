# ParaBank QA Project 
## Portfólio de Testes Manuais | QA Júnior

Este projeto simula a atuação de um **QA em um time ágil**, cobrindo desde o entendimento dos requisitos até a entrega de relatórios de qualidade.  
O sistema testado foi o **ParaBank**, uma aplicação bancária fictícia, com foco nos fluxos de **cadastro, login e segurança de acesso**.

O objetivo principal foi validar o **MVP de Acesso**, identificando falhas funcionais e pontos críticos de segurança antes da evolução do produto.

---

## 🛠️ Ferramentas e Técnicas Utilizadas

* **Jira Software**  
  Organização do backlog, planejamento de Sprint e acompanhamento das tarefas (Scrum).

* **Zephyr Scale**  
  Criação, organização e execução dos casos de teste, além da geração de relatórios.

* **BDD (Gherkin)**  
  Escrita de cenários no formato *Dado / Quando / Então*, facilitando a comunicação entre QA, desenvolvimento e negócio.

* **ScreenPal & Evidências Visuais**  
  Gravação de vídeos e captura de prints para documentar execuções e defeitos.

---
##  O Ciclo da Sprint 1: MVP de Acesso

A missão dessa Sprint foi garantir que novos usuários conseguissem se cadastrar e entrar no banco com segurança. Abaixo, mostro passo a passo como conduzi o processo.

### 1. Organizando a Casa (Backlog e Jira)
Primeiro quebrei os requisitos em **User Stories** pequenas e testáveis (usando a técnica INVEST). Organizei tudo no quadro Kanban para o time saber o que estava acontecendo.

![Quadro Kanban](assets/01_jira_sprint_board.jpg)
*(Visão geral do Board com as tarefas organizadas)*

---

### 2. Criando os Testes
Criei roteiros de teste (step by step).

![Detalhe do Caso de Teste](assets/02_test_case_steps.jpg)
*(Exemplo de um teste escrito passo a passo)*

---

### 3. Execução
Rodei os testes no ambiente de Staging. O resultado foi positivo na maioria, mas encontrei problemas.

* **Resultado:** 4 Passaram (✅) / 1 Falhou (❌)

![Ciclo de Teste Zephyr](assets/03_zephyr_execution_cycle.jpg)
*(Lista dos testes rodados e seus status)*

---

### 4. Caçando Bugs (Defeitos)
Durante os testes de segurança, encontrei uma falha crítica no Logout. Documentei tudo para o desenvolvedor não ter dúvida de como arrumar.

* **O Bug:** O botão "Voltar" do navegador mostrava a conta logada mesmo depois de sair.
* **Evidência:** Anexei vídeo e prints no ticket.

![Bug Report](assets/07_Bug report.png)
*(O ticket do bug aberto no Jira, com prioridade alta)*

---

### 5. Métricas e Relatórios Finais
Para fechar a Sprint, gerei os relatórios que mostram a saúde do projeto.

####  Resumo Visual (Donut Chart)
A maioria das funções está estável, com exceção do ponto de segurança.
![Gráfico Donut](assets/04_report_execution_summary.jpg)

####  Rastreabilidade (Traceability)
Aqui eu provo que não testei coisas aleatórias. Cada teste está ligado a um requisito de negócio.
![Matriz de Rastreabilidade](assets/05_report_traceability_matrix.jpg)

####  Lista Detalhada
Os detalhes de cada execução:
![Lista Detalhada](assets/06_report_execution_details.jpg)

---

##  Próximos Passos (Sprint 2)
Agora que o acesso básico está testado, o plano é:
1. Validar Transferências e Pagamentos.
2. Retestar o bug de Logout assim que corrigirem.

---
*Autor: Felipe Castro | [Meu LinkedIn](felipetster)*
