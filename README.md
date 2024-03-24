## Visão Geral

O nosso  sistema é uma aplicação web desenvolvida para facilitar a gestão de solicitações de suporte técnico . Com uma interface intuitiva e recursos poderosos, permite que os usuários submetam tickets de suporte, acompanhem o status de suas solicitações.

## Funcionalidades Principais

-   **Envio de Tickets:** Usuários podem submeter pedidos de suporte técnico, detalhando o problema encontrado.
-   **Acompanhamento de Tickets:** Os usuários podem acompanhar o status de seus tickets e receber notificações sobre atualizações.
-   **Priorização de Tickets:** Os tickets são classificados com base na gravidade do problema relatado, permitindo uma resposta rápida para questões críticas.
-   **Gerenciamento de Tarefas:** Os agentes de suporte podem atribuir tarefas uns aos outros, colaborando para resolver problemas complexos.
-   **Base de Conhecimento:** Uma extensa base de conhecimento está disponível para os usuários, fornecendo soluções para problemas comuns e permitindo autoatendimento.
-   **Relatórios e Métricas:** Administradores podem gerar relatórios detalhados sobre o desempenho do help desk, identificando áreas para melhoria contínua.

## Tecnologias Utilizadas

-   **Frontend:** HTML, CSS, JavaScript,
-   **Backend:** Node.js, Express.js
-   **Banco de Dados:** MySQL

## Backlog

| Rank | Prioridade | User Story | Estimativa | Sprint | Requisito Parceiro |
| --- | --- | --- | --- | --- | --- |
| 1 | Alta | Eu, como usuário, quero poder criar uma conta que guarda meu nome, meus tickets e meu CPF. | 8 | 2 | 1 |
| 2 | Média | Eu, como admin, quero poder criar contas para o time de Suporte e revogar o acesso dessas contas. | 3 | 2 | 1 |
| 2 | Baixa | Eu, como usuário, quero poder acessar informações básicas da minha conta e poder mudar minha senha. | 4 | 3 | 1 |
| 4 | Baixa | Eu, como admin, quero uma página dedicada a mostrar métricas dedicadas a estatísticas sobre a minha gestão de chamadas de serviços. | 5 | 4 | 2 |
| 5 | Baixa | Eu, como cliente, quero poder marcar um ticket como concluído se o meu problema for resolvido. | 3 | 3 | 2 |
| 6 | Média | Eu, como técnico, quero que fique claro na página se um ticket já ultrapassou seu tempo de resposta estipulado. | 3 | 3 | 3 |
| 7 | Alta | Eu, como usuário, quero poder criar tickets descrevendo um problema que estou tendo com a empresa. | 8 | 2 | 3 |
| 8 | Alta | Eu, como técnico, quero poder responder tickets dos clientes. | 7 | 2 | 3 |
| 9 | Baixa | Eu, como técnico, quero poder mudar o status de um ticket. | 2 | 2 | 4 |
| 10 | Média | Eu, como admin, quero que cada tipo de problema tenha um tempo de resposta diferente para que meus suportes possam ver quais tickets priorizar. | 3 | 3 | 6 |
| 11 | Baixa | Eu, como admin, quero um FAQ na minha página que mostre soluções para problemas frequentes. | 1 | 4 | 7 |
| 12 | Baixa | Eu, como admin, quero que meu FAQ encoraje meu cliente a criar uma conta caso o problema dele não esteja listado acima. | 1 | 4 | 7 |

# Tasks

**User Story 1:**
Eu, como usuário, quero poder criar uma conta que guarda meu nome, meus tickets e meu CPF.

- **Task 1.1: Configuração da Página de Registro**
    - Critérios de Aceitação:
        - Implementar uma página de registro onde o usuário pode inserir seu nome, CPF e criar uma senha.
        - Todos os campos devem ser obrigatórios.
        - A senha deve atender aos requisitos de segurança definidos.
- **Task 1.2: Armazenamento de Dados da Conta**
    - Critérios de Aceitação:
        - Implementar a lógica para armazenar os dados da conta (nome, CPF, senha) no banco de dados.
        - Criptografar a senha
- **Task 1.3: Interface do Usuário para Visualizar e Editar Dados da Conta**
    - Critérios de Aceitação:
        - Desenvolver uma interface onde o usuário possa visualizar e editar seus dados de conta (nome, CPF).
        - Permitir que o usuário altere sua senha, se necessário.
        - Garantir que apenas o usuário autenticado possa acessar e modificar seus próprios dados.

**User Story 2:**
Eu, como admin, quero poder criar contas para o time de Suporte e revogar o acesso dessas contas.

- **Task 2.1: Interface de Administração de Contas de Suporte**
    - Critérios de Aceitação:
        - Desenvolver uma interface para administradores onde possam criar novas contas de suporte.
        - Permitir que os administradores insiram o nome, e-mail e senha para as novas contas.
        - Garantir que as novas contas sejam automaticamente atribuídas ao grupo de "Suporte".
- **Task 2.2: Funcionalidade de Revogação de Acesso**
    - Critérios de Aceitação:
        - Implementar a capacidade de revogar o acesso de uma conta de suporte.
        - Ao revogar o acesso, a conta não deve mais ter permissão para acessar o sistema.
        - Garantir que todos os dados relacionados à conta revogada sejam arquivados adequadamente.
        

**User Story 3:**
Eu, como usuário, quero poder acessar informações básicas da minha conta e poder mudar minha senha.

- **Task 3.1: Interface para Visualização de Informações da Conta**
    - Critérios de Aceitação:
        - Desenvolver uma página onde o usuário possa visualizar informações básicas da sua conta, como nome e CPF.
        - Garantir que apenas o próprio usuário possa acessar essas informações.

- **Task 3.2: Funcionalidade de Alteração de Senha**
    - Critérios de Aceitação:
        - Implementar a capacidade de o usuário alterar sua senha.
        - Solicitar a senha antiga como medida de segurança.
        - Garantir que a nova senha atenda aos requisitos de segurança definidos.
        

**User Story 4:**
Eu, como admin, quero uma página dedicada a mostrar métricas dedicadas a estatísticas sobre a minha gestão de chamadas de serviços.

- **Task 4.1: Desenvolvimento da Página de Métricas**
    - Critérios de Aceitação:
        - Criar uma página dedicada para exibir métricas e estatísticas relacionadas à gestão de chamadas de serviço.
        - Incluir gráficos e tabelas que mostrem dados relevantes, como tempo médio de resolução, número de chamadas atendidas, etc.
        - Garantir que apenas administradores tenham acesso a essa página.

**User Story 5:**
Eu, como cliente, quero poder marcar um ticket como concluído se o meu problema for resolvido.

- **Task 5.1: Adicionar Funcionalidade de Marcação de Ticket Concluído**
    - Critérios de Aceitação:
        - Implementar um botão ou opção para que os clientes possam marcar um ticket como concluído.
        - Ao marcar como concluído, o ticket deve ser movido para uma seção ou estado indicando que está resolvido.
        - Notificar o técnico responsável e o cliente sobre a conclusão do ticket.

**User Story 6:**
Eu, como técnico, quero que fique claro na página se um ticket já ultrapassou seu tempo de resposta estipulado.

- **Task 6.1: Indicação de Tempo de Resposta Excedido**
    - Critérios de Aceitação:
        - Implementar um indicador visual na página de tickets para mostrar se o tempo de resposta estipulado para um ticket foi excedido.
        - Utilizar cores ou ícones para destacar os tickets com tempo de resposta excedido.
        - Garantir que os técnicos possam facilmente identificar e priorizar esses tickets.
        

**User Story 7:**
Eu, como usuário, quero poder criar tickets descrevendo um problema que estou tendo com a empresa.

- **Task 7.1: Formulário de Criação de Tickets**
    - Critérios de Aceitação:
        - Desenvolver um formulário onde os usuários possam descrever o problema que estão enfrentando com a empresa.
        - Incluir campos para título do problema, descrição detalhada e categorias.
        - Garantir que os usuários possam enviar o ticket após preencher o formulário.

**User Story 8:**
Eu, como técnico, quero poder responder tickets dos clientes.

- **Task 8.1: Funcionalidade de Resposta a Tickets**
    - Critérios de Aceitação:
        - Implementar um sistema de resposta onde os técnicos possam escrever e enviar respostas para os tickets dos clientes.
        - Garantir que as respostas sejam registradas e exibidas no histórico do ticket para referência futura.

**User Story 9:**
Eu, como técnico, quero poder mudar o status de um ticket.

- **Task 9.1: Funcionalidade de Mudança de Status de Ticket**
    - Critérios de Aceitação:
        - Adicionar opções para os técnicos alterarem o status dos tickets, como "aberto", "em andamento" e "concluído".
        - Garantir que apenas técnicos autorizados possam modificar o status dos tickets.
        - Registrar a data e hora da última alteração de status.

**User Story 10:**
Eu, como admin, quero que cada tipo de problema tenha um tempo de resposta diferente para que meus suportes possam ver quais tickets priorizar.

- **Task 10.1: Configuração de Tempos de Resposta por Tipo de Problema**
    - Critérios de Aceitação:
        - Desenvolver uma interface de administração onde os administradores possam definir tempos de resposta diferentes para cada tipo de problema (SLA).
        - Garantir que os tempos de resposta sejam aplicados corretamente aos tickets.

**User Story 11:**
Eu, como admin, quero um FAQ na minha página que mostre soluções para problemas frequentes.

- **Task 11.1: Desenvolvimento da Página de FAQ**
    - Critérios de Aceitação:
        - Criar uma página dedicada de FAQ onde os clientes possam encontrar soluções para problemas comuns.
        - Organizar as perguntas frequentes em categorias ou seções para facilitar a navegação.


## DoR

- **Sprint 1**

- Product Backlog
- Spring backlog
- Modelagem de dados
- Protótipo 



# We Are TEAM H.I.V.E.
🌠 Highly Imaginative Valiant Entrepeneurs 🌠 <br>
Nós somos um time de estudantes da FATEC São José dos Campos - Prof. Jessen Vidal e estamos cursando o 2° semestre de Desenvolvimento de Software Multiplataforma.
## 👷🏻 Time de Desenvolvimento

| Foto | Nome | Função | Github | Linkedin |
| :---------: | :---------: | :---------------------: | :-----------------: | :-------: |
| <img src="https://github.com/maarantes.png?size=50" width=50px> | Marco Antonio Arantes | Product Owner | <a href="https://github.com/maarantes"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/marco-antonio-arantes/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
| <img src="https://github.com/yokotaerik.png?size=50" width=50px> | Erik Camara Yokota | Scrum Master | <a href="https://github.com/yokotaerik"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/erik-camara-yokota-685439233/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
| <img src="https://github.com/Karnas01.png?size=50" width=50px> | Arthur Karnas da Rocha | Desenvolvedor | <a href="https://github.com/Karnas01"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/arthur-karnas-da-rocha-b90433271/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
| <img src="https://github.com/eberssj.png?size=50" width=50px> | Eber de Souza Silva Junior | Desenvolvedor | <a href="https://github.com/eberssj"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/eber-junior-b2a4a3211/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
| <img src="https://github.com/elisarachel.png?size=50" width=50px> | Elisa Rachel Beninca Martins | Desenvolvedor | <a href="https://github.com/elisarachel"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/elisa-beninca-704566292/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
| <img src="https://github.com/GuilhermeLGuimaraes.png?size=50" width=50px> | Guilherme Luz Guimarães | Desenvolvedor | <a href="https://github.com/GuilhermeLGuimaraes"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/guilherme-guimar%C3%A3es-0166a3294/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
| <img src="https://github.com/juliamariahr.png?size=50" width=50px> | Julia Maria Helbusto Rosado | Scrum Master | <a href="https://github.com/yokotaerik"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/j%C3%BAlia-rosado/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
| <img src="https://github.com/Kaue-Francisco.png?size=50" width=50px> | Kauê dos Santos Francisco | Desenvolvedor | <a href="https://github.com/Kaue-Francisco"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a> | <a href="https://www.linkedin.com/in/kau%C3%AA-francisco-3b13aa255/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> |
