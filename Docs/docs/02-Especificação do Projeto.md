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


# Modelagem do Processo de Negócio
Análise da Situação Atual
Apresente aqui os problemas existentes que viabilizam sua proposta. Apresente o modelo do sistema como ele funciona hoje. Caso sua proposta seja inovadora e não existam processos claramente definidos, apresente como as tarefas que o seu sistema pretende implementar são executadas atualmente, mesmo que não se utilize tecnologia computacional.

Descrição Geral da Proposta
Apresente aqui uma descrição da sua proposta abordando seus limites e suas ligações com as estratégias e objetivos do negócio. Apresente aqui as oportunidades de melhorias.

Processo 1 – NOME DO PROCESSO
Apresente aqui o nome e as oportunidades de melhorias para o processo 1. Em seguida, apresente o modelo do processo 1, descrito no padrão BPMN.

Processo 1

Processo 2 – NOME DO PROCESSO
Apresente aqui o nome e as oportunidades de melhorias para o processo 2. Em seguida, apresente o modelo do processo 2, descrito no padrão BPMN.

Processo 2

# Indicadores de Desempenho
Apresente aqui os principais indicadores de desempenho e algumas metas para o processo. Atenção: as informações necessárias para gerar os indicadores devem estar contempladas no diagrama de classe. Colocar no mínimo 5 indicadores.

Usar o seguinte modelo:

Indicadores de Desempenho Obs.: todas as informações para gerar os indicadores devem estar no diagrama de classe a ser apresentado a posteriori.

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

O diagrama de casos de uso é o próximo passo após a elicitação de requisitos, que utiliza um modelo gráfico e uma tabela com as descrições sucintas dos casos de uso e dos atores. Ele contempla a fronteira do sistema e o detalhamento dos requisitos funcionais com a indicação dos atores, casos de uso e seus relacionamentos.

As referências abaixo irão auxiliá-lo na geração do artefato “Diagrama de Casos de Uso”.


# Matriz de Rastreabilidade
A matriz de rastreabilidade é uma ferramenta usada para facilitar a visualização dos relacionamento entre requisitos e outros artefatos ou objetos, permitindo a rastreabilidade entre os requisitos e os objetivos de negócio.

A matriz deve contemplar todos os elementos relevantes que fazem parte do sistema, conforme a figura meramente ilustrativa apresentada a seguir.

Exemplo de matriz de rastreabilidade


# Gerenciamento de Tempo
Com diagramas bem organizados que permitem gerenciar o tempo nos projetos, o gerente de projetos agenda e coordena tarefas dentro de um projeto para estimar o tempo necessário de conclusão.

Diagrama de rede simplificado notação francesa (método francês)

O gráfico de Gantt ou diagrama de Gantt também é uma ferramenta visual utilizada para controlar e gerenciar o cronograma de atividades de um projeto. Com ele, é possível listar tudo que precisa ser feito para colocar o projeto em prática, dividir em atividades e estimar o tempo necessário para executá-las.

Gráfico de Gantt

# Gerenciamento de Equipe
O gerenciamento adequado de tarefas contribuirá para que o projeto alcance altos níveis de produtividade. Por isso, é fundamental que ocorra a gestão de tarefas e de pessoas, de modo que os times envolvidos no projeto possam ser facilmente gerenciados.

Simple Project Timeline

# Gestão de Orçamento
O processo de determinar o orçamento do projeto é uma tarefa que depende, além dos produtos (saídas) dos processos anteriores do gerenciamento de custos, também de produtos oferecidos por outros processos de gerenciamento, como o escopo e o tempo.


# Orçamento
