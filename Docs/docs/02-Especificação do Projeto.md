# Especificações do Projeto

Definição do problema e ideia de solução a partir da perspectiva do usuário. É composta pela definição do diagrama de personas, histórias de usuários, requisitos funcionais e não funcionais além das restrições do projeto.

Apresente uma visão geral do que será abordado nesta parte do documento, enumerando as técnicas e/ou ferramentas utilizadas para realizar a especificações do projeto

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
<table border="1" cellpadding="10" cellspacing="0">
    <thead>
        <tr>
            <th>ID</th>
            <th>Descrição da Restrição</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>RE-01</td>
            <td>O projeto deve ser entregue até o final do ano, com data limite em 08/12/2024.</td>
        </tr>
        <tr>
            <td>RE-02</td>
            <td>O desenvolvimento do aplicativo deve utilizar exclusivamente as tecnologias disponíveis no framework React Native.</td>
        </tr>
        <tr>
        <tr>
            <td>RE-03</td>
            <td>A aplicação deve ser desenvolvida exclusivamente para dispositivos móveis (iOS e Android).</td>
        </tr>
        <tr>
        <tr>
            <td>RE-04</td>
            <td>O código-fonte deve ser armazenado e versionado em um repositório Git, com commits regulares.</td>
        </tr>
        <tr>
            <td>RE-05</td>
            <td>A entrega deve incluir uma documentação completa, incluindo descrição e documentação técnica do projeto.</td>
        </tr>
    </tbody>
</table>

# Diagrama de casos de uso

![Diagrama de caso de uso (1)](https://github.com/user-attachments/assets/d65eb127-ac61-4670-af92-c373d17afdcd)

# Matriz de Rastreabilidade

| Atores           | Criar Perfil | Pesquisar Vagas | Inscrever-se em Vagas | Gerenciar Inscrições | Publicar Vagas | Avaliar Candidatos | Gerenciar Usuários | Gerar Relatórios |
|------------------|--------------|-----------------|-----------------------|----------------------|----------------|--------------------|-------------------|-----------------|
| **Candidato**    | X            | X               | X                     | X                    |                |                    |                   |                 |
| **Empresa**      |              |                 |                       |                      | X              | X                  |                   |                 |
| **Administrador**|              |                 |                       |                      |                |                    | X                 | X               |

## Descrição do Processo BPMN atual

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

## Descrição do Processo BPMN Situação Futura - "FAZER"

### 1. Página de Login
- **Start Event:** O processo começa na página de login onde o usuário tem a opção de registrar ou logar na plataforma.
- **Gateway: Informações Corretas?**
  - **Registrar ou Logar:** O usuário pode escolher registrar ou logar.
  - **Mensagem de Erro:** Se as informações fornecidas estiverem incorretas, uma mensagem de erro é exibida.
  - **Recuperar Senha:** Se necessário, o usuário pode optar por recuperar a senha.

### 2. Página Inicial
- Após o login bem-sucedido, o usuário é direcionado para a página inicial.
- **Intermediate Event: Página Inicial**

### 3. Funcionalidades Disponíveis na Página Inicial
- **Task: Registrar Interesse**
  - O usuário pode registrar seus interesses na plataforma.
- **Task: Visualizar Perfil**
  - O usuário pode visualizar seu perfil e verificar suas informações.
- **Task: Editar Perfil**
  - O usuário pode editar as informações do seu perfil.
- **Task: Pesquisar Interesses**
  - O usuário pode pesquisar interesses de outras pessoas.
- **Task: Editar Interesse**
  - O usuário pode editar os interesses previamente registrados.
- **Task: Deletar Interesse**
  - O usuário pode deletar seus interesses previamente registrados.

### 4. Conexões com Outros Usuários
- **Task: Visualizar Pessoa com Interesse em Comum**
  - O usuário pode visualizar pessoas com interesses em comum.
- **Task: Solicitar Conexão com a Pessoa**
  - O usuário pode solicitar conexão com a pessoa.
- **Gateway: Resposta?**
  - **Compartilhar Dados de Contato:** Se a resposta for positiva, o usuário pode compartilhar dados de contato.
  - **Cancelar Conexão:** Se a resposta for negativa, a conexão é cancelada.

### 5. Fim da Sessão
- **Task: Deslogar**
  - O usuário pode deslogar da plataforma.
- **End Event: Fim da Sessão**
  - O processo termina quando o usuário escolhe deslogar da plataforma.

### Diagrama BPMN "FAZER"

Segue a representação visual do processo em BPMN: "FAZER"

![image](https://github.com/ICEI-PUC-Minas-PMV-ADS/ads-2024-1-e3-proj-mov-t8-connectskill/assets/94996003/ab41e73b-fb14-4a13-83db-f9601e9dbe61)


# Gerenciamento de Projeto "FAZER"

O projeto será desenvolvido em etapas, onde a cada entrega haverá uma prioridade em foco. Ele será administrado por meio da designação de tarefas pela plataforma Trello, e qualquer necessidade de criar prototipagem ou wireframes será atendida utilizando o Figma.

(https://trello.com/invite/b/wl1WNmiq/ATTI901c0ae89ee9162bf10fc3e337799066011507C9/etapa-2))

## Gerenciamento de Tempo

O gráfico de Gantt ou diagrama de Gantt também é uma ferramenta visual utilizada para controlar e gerenciar o cronograma de atividades de um projeto. Com ele, é possível listar tudo que precisa ser feito para colocar o projeto em prática, dividir em atividades e estimar o tempo necessário para executá-las.

![image](https://github.com/ICEI-PUC-Minas-PMV-ADS/ads-2024-1-e3-proj-mov-t8-connectskill/assets/127440373/cc649bcd-3184-4f3b-af54-8589e5d45ddd)


## Gerenciamento de Equipe

O time será gerenciado por meio da ferramenta de atribuição, Jira. 
https://connectskill.atlassian.net/jira/servicedesk/projects/SUP/boards/1


## Gestão de Orçamento

![image](https://github.com/ICEI-PUC-Minas-PMV-ADS/ads-2024-1-e3-proj-mov-t8-connectskill/assets/127440373/708f39c0-a521-45f5-a77d-0a26cac0404d)

# Gestão de Orçamento
O processo de determinar o orçamento do projeto é uma tarefa que depende, além dos produtos (saídas) dos processos anteriores do gerenciamento de custos, também de produtos oferecidos por outros processos de gerenciamento, como o escopo e o tempo.


