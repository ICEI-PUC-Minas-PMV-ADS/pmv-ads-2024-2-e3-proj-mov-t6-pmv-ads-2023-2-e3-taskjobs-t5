# Especificações do Projeto

Este projeto tem como objetivo desenvolver um aplicativo móvel para ajudar candidatos a gerenciar de forma organizada suas candidaturas a vagas de emprego e entrevistas. O aplicativo permitirá o registro e acompanhamento de informações essenciais, como empresas em que o usuário se candidatou, status das candidaturas e lembretes para entrevistas agendadas. Com uma interface intuitiva e funcionalidades práticas, o sistema visa proporcionar uma experiência mais eficiente e menos estressante para quem busca uma nova oportunidade de trabalho, ajudando a otimizar o planejamento e a organização pessoal.

# Personas
| **Persona**               | **João Silva**               | **Maria Oliveira**            | **Lucas Santos**              | **Ana Costa**                 | **Pedro Almeida**             |
|---------------------------|------------------------------|-------------------------------|-------------------------------|-------------------------------|-------------------------------|
| **Idade**                 | 23 anos                      | 35 anos                       | 42 anos                       | 20 anos                       | 30 anos                       |
| **Gênero**                | Masculino                    | Feminino                      | Masculino                     | Feminino                      | Masculino                     |
| **Profissão**             | Recém-formado em Engenharia de Software | Analista de Marketing, migrando para UX Design | Gerente de Projetos em busca de recolocação | Estudante de Administração     | Designer Gráfico Freelancer  |
| **Localização**           | São Paulo, SP                | Rio de Janeiro, RJ            | Porto Alegre, RS              | Belo Horizonte, MG            | Curitiba, PR                  |
| **Interesse no App**      | Organizar candidaturas e lembrar entrevistas marcadas | Facilitar o acompanhamento de candidaturas em nova carreira | Centralizar informações de entrevistas e manter organização | Controlar datas, horários e detalhes de entrevistas de estágio | Organizar candidaturas, visualizar status e se preparar para entrevistas |

# Histórias de Usuários
Com base na análise das personas forma identificadas as seguintes histórias de usuários:

| **Eu, como**                | **Quero/Preciso**                                                           | **Para**                                                                                              |
|-----------------------------|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------|
| João Silva                  | Uma funcionalidade que me permita registrar e organizar empresas e entrevistas. | Acompanhar eficientemente o status de cada candidatura e garantir que não perca prazos importantes. |
| Maria Oliveira              | Visualizar o progresso das minhas candidaturas e preparar-me para as entrevistas. | Facilitar minha transição de carreira para UX Design e manter uma visão clara sobre minhas oportunidades na nova área. |
| Lucas Santos                | Uma ferramenta que ajude a centralizar e acompanhar todas as informações sobre entrevistas e empresas. | Manter uma organização eficaz durante o processo de recolocação e não perder oportunidades valiosas. |
| Ana Costa                   | Controlar datas e horários das entrevistas de estágio e registrar detalhes importantes. | Assegurar que estou bem preparada e organizada durante minha busca por estágio.                    |
| Pedro Almeida              | Acompanhar o status das minhas candidaturas e visualizar o progresso das entrevistas agendadas. | Preparar-me melhor e otimizar minha busca por oportunidades de trabalho fixo, mantendo controle sobre todas as informações relevantes. |


## Sistema de Mapeamento de Inscrições

| Atores           | Casos de Uso                          |
|------------------|---------------------------------------|
| **Candidato**    | Criar perfil                           |
|                  | Pesquisar vagas                        |
|                  | Inscrever-se em vagas                  |
|                  | Gerenciar inscrições                   |
| **Empresa**      | Publicar vagas                         |
|                  | Avaliar candidatos                     |
| **Administrador**| Gerenciar usuários                     |
|                  | Gerar relatórios                       |

# Requisitos
Requisitos Funcionais
|ID    | Descrição                | Prioridade |
|-------|---------------------------------|----|
| RF-01 | Um usuário deve poder fazer login no sistema usando seu nome de usuário e senha. | Alta | 
| RF-02 | A criação do “Card” de tarefa deverá conter um título. | Alta |
| RF-03 | Usuário terá acesso a um calendário para ver e definir prazos das vagas| Alta |
| RF-04 | O usuário poderá adicionar comentários à tarefa | Alta |
| RF-05 | A aplicação permitirá ao usuário a customização dos “Cards” | Alta |
| RF-06 | A aplicação permitirá ao usuário a customização do plano de fundo | Média |
| RF-07 |  A aplicação terá a função de alertas e lembretes das vagas | Média |

# Requisitos Não Funcionais
|ID      | Descrição               |Prioridade |
|--------|-------------------------|----|
| RNF-01 | A aplicação deverá ser responsiva permitindo a visualização em dispositivos diversos de forma adequada.| Alta  | 
| RNF-02 |Usuário terá segurança em seu login, ao tentar se conectar com login ou senha errado não acessaram o site e terá retorno de erro| Média | 

# Restrições

O projeto está restrito pelos itens apresentados na tabela a seguir.

| ID     | Descrição da Restrição                                                                                      |
|--------|-------------------------------------------------------------------------------------------------------------|
| RE-01  | O projeto deve ser entregue até o final do ano, com data limite em 08/12/2024.                               |
| RE-02  | O desenvolvimento do aplicativo deve utilizar exclusivamente as tecnologias disponíveis no framework React Native. |
| RE-03  | A aplicação deve ser desenvolvida exclusivamente para dispositivos móveis (iOS e Android).                   |
| RE-04  | O código-fonte deve ser armazenado e versionado em um repositório Git, com commits regulares.                |
| RE-05  | A entrega deve incluir uma documentação completa, incluindo descrição e documentação técnica do projeto.      |

# Diagrama de casos de uso

![Diagrama de caso de uso (1)](https://github.com/user-attachments/assets/d65eb127-ac61-4670-af92-c373d17afdcd)

# Matriz de Rastreabilidade

| Atores           | Criar Perfil | Pesquisar Vagas | Inscrever-se em Vagas | Gerenciar Inscrições | Publicar Vagas | Avaliar Candidatos | Gerenciar Usuários | Gerar Relatórios |
|------------------|--------------|-----------------|-----------------------|----------------------|----------------|--------------------|-------------------|-----------------|
| **Candidato**    | X            | X               | X                     | X                    |                |                    |                   |                 |
| **Empresa**      |              |                 |                       |                      | X              | X                  |                   |                 |
| **Administrador**|              |                 |                       |                      |                |                    | X                 | X               |

# Descrição do Processo BPMN atual

### 1. Página de Login
- **Start Event:** O processo começa na página de login onde o usuário tem a opção de logar ou registrar-se na plataforma.
- **Gateway: Logar ou Registrar?** 
  - **Logar:** Se o usuário já possui uma conta, ele pode escolher logar.
  - **Registrar:** Se o usuário não possui uma conta, ele pode escolher registrar-se.

### 2. Página Inicial
- Após o login ou registro, o usuário é direcionado para a página inicial.
- **Intermediate Event: Página Inicial**

### 3. Funcionalidades Disponíveis na Página Inicial
- **Task: Adiocionar Card**
  - O usuário pode registrar suas inscrições de emprego na plataforma.
- **Task: Visualizar Perfil**
  - O usuário pode visualizar seu perfil e verificar suas informações.
- **Task: Deletar Card**
  - O usuário pode deletar o card de inscrições previamente registrado.
- **Task: Deslogar**
  - O usuário pode deslogar da plataforma.

### 4. Fim da Sessão
- **End Event: Fim da Sessão**
  - O processo termina quando o usuário escolhe deslogar da plataforma.

### Diagrama BPMN

Segue a representação visual do processo em BPMN:
![BPMN 2 0](https://github.com/user-attachments/assets/ea8b8af0-824c-4970-8792-e177242b4b78)


# Descrição do Projeto BPMN detalhado

### 1. **Página de Login**
   - **Start Event:** O processo começa na **Página de Login**, onde o usuário é convidado a fazer login no sistema.
   - **Task: Login do Usuário:** O usuário insere seu **nome de usuário** e **senha**.
   - **Gateway: Informações Corretas?**
     - **Se as informações forem corretas**, o usuário será direcionado à página inicial.
     - **Se as informações forem incorretas**, uma **mensagem de erro** será exibida e o usuário poderá tentar novamente.
   - **Task: Recuperar Senha** (Opcional): O usuário pode optar por **recuperar a senha** caso tenha esquecido, e então o fluxo retorna à verificação de informações.

### 2. **Página Inicial**
   - **Intermediate Event:** Após um login bem-sucedido, o usuário é direcionado à **Página Inicial**.

### 3. **Funcionalidades Disponíveis na Página Inicial**
   - **Task: Criar um Card de Tarefa:** O usuário pode **criar um "Card" de tarefa**, inserindo um **título** para o mesmo.
   - **Task: Acessar Calendário:** O usuário pode visualizar e definir prazos no **calendário** para as tarefas e atividades.
   - **Task: Adicionar Comentários:** O usuário pode **adicionar comentários** nas tarefas já criadas para fornecer mais informações ou feedbacks.
   - **Task: Customizar "Cards":** O usuário tem a opção de **customizar os "Cards"**, alterando informações como cor, tamanho ou estilo visual.
   - **Task: Customizar Plano de Fundo:** O usuário poderá **personalizar o plano de fundo** da interface de acordo com suas preferências.
   - **Task: Visualizar e Gerenciar Alertas e Lembretes:** O sistema permite que o usuário configure e visualize **alertas e lembretes** para suas tarefas, ajudando a manter prazos.

### 4. **Fim da Sessão**
   - **Task: Deslogar:** O usuário tem a opção de **deslogar** do sistema a qualquer momento.
   - **End Event: Fim da Sessão:** O processo se encerra quando o usuário opta por deslogar.

### **Fluxo Completo do Processo**
1. **Início:** O processo começa com o **Login do Usuário**.
2. **Página Inicial:** Se o login for bem-sucedido, o usuário é redirecionado para a **Página Inicial**, onde tem acesso a diversas funcionalidades.
3. **Funcionalidades:** O usuário pode realizar atividades como a **criação e customização de cards**, **gerenciamento de prazos**, **personalização do sistema**, e **configuração de lembretes e alertas**.
4. **Fim da Sessão:** O processo se encerra quando o usuário escolhe **deslogar** da plataforma.

### Diagrama BPMN "FAZER"

Segue a representação visual do processo em BPMN: "FAZER"

![image](https://github.com/ICEI-PUC-Minas-PMV-ADS/ads-2024-1-e3-proj-mov-t8-connectskill/assets/94996003/ab41e73b-fb14-4a13-83db-f9601e9dbe61)


# Gerenciamento de Projeto 
O gerenciamento será realizado por meio da ferramenta disponibilizada pelo Git: 
https://github.com/orgs/ICEI-PUC-Minas-PMV-ADS/projects/1268


## Gerenciamento de Tempo

![image](https://github.com/user-attachments/assets/725898ae-9159-46c3-9c80-30b8abcf206d)

## Gestão de Orçamento

| **Descrição**        | **Valor (R$)** |
|----------------------|----------------|
| **Recursos Humanos**  | 300.000        |
| **Hardware**          | 40.000         |
| **Rede**              | 10.000         |
| **Software**          | 20.000         |
| **Serviços**          | 5.000          |
| **TOTAL**             | **375.000**    |


