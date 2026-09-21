# TebasFin — Editor de Planejamento YAML e Gantt

## Contexto do produto

O Editor de Planejamento YAML e Gantt é uma ferramenta visual para estruturar, acompanhar e ajustar o cronograma do projeto **TebasFin Gestora — Valora**. O produto combina uma visão textual estruturada com uma linha do tempo interativa, permitindo que planejamento, arquitetura, desenvolvimento, testes e homologação sejam tratados em uma única interface.

O planejamento segue uma organização inspirada em PMBOK e em estruturas analíticas de projeto, com pacotes de trabalho, tarefas, subtarefas, dependências, esforço, recursos, prioridade e situação de execução.

## Objetivo

Centralizar o cronograma do projeto e facilitar sua manutenção, oferecendo simultaneamente:

- Estrutura hierárquica dos pacotes de trabalho.
- Visualização temporal das atividades.
- Edição direta das informações do planejamento.
- Clareza sobre datas, duração, dependências e responsáveis.
- Visão macro e detalhada do projeto na mesma tela.

## Público-alvo

- Product Owner e responsáveis pelo planejamento.
- Arquitetura e liderança técnica.
- Equipes de backend, frontend, dados e DevOps.
- Qualidade, testes e homologação.
- Gestores e demais participantes do projeto.

## Estrutura do planejamento

### Projeto

Representa o planejamento principal e contém:

- Identificador do projeto.
- Nome do projeto.
- Data-base usada como referência visual no cronograma.

### Pacote de trabalho

Representa uma entrega ou agrupamento macro. Cada pacote pode conter tarefas e outros níveis de subtarefas.

Principais informações:

- ID e nome.
- Descrição.
- Frente de trabalho.
- Status.
- Prioridade.
- Data de início e fim.
- Esforço estimado.
- Recursos envolvidos.
- Dependências.

### Tarefa e subtarefa

Representam as atividades necessárias para concluir um pacote de trabalho. A estrutura permite múltiplos níveis hierárquicos para decompor entregas maiores em itens executáveis e acompanháveis.

## Funcionalidades principais

### Visão dividida

A interface apresenta o planejamento estruturado e o gráfico de Gantt lado a lado. Cada painel pode ser minimizado individualmente para ampliar a área útil do outro.

### Estrutura hierárquica

- Pacotes de trabalho funcionam como elementos de primeiro nível.
- Tarefas podem ser adicionadas abaixo de qualquer item.
- Ramos podem ser expandidos ou recolhidos individualmente.
- Um controle geral permite expandir ou recolher toda a árvore.
- A visualização inicial mantém os ramos recolhidos para reduzir excesso de informação.

### Edição das atividades

Cada atividade permite editar:

- ID.
- Nome.
- Descrição.
- Data de início.
- Data de fim.

O nome recebe maior destaque visual. Em repouso, cada atividade ocupa no máximo duas linhas. Ao entrar em edição, a linha é expandida para melhorar a leitura e o preenchimento; ao clicar fora, retorna ao formato compacto.

### Inclusão e exclusão

- Inclusão de novos pacotes de trabalho na raiz.
- Inclusão de tarefas ou subtarefas em qualquer ponto da árvore.
- Exclusão de uma atividade e de toda a sua estrutura subordinada.
- Controles de adicionar e excluir organizados verticalmente para preservar espaço horizontal.

### Gráfico de Gantt

- Exibição das atividades ao longo do tempo.
- Rolagem horizontal para cronogramas extensos.
- Cabeçalho fixo durante a rolagem vertical.
- Coluna estrutural fixa durante a rolagem horizontal.
- Barra visual para cada atividade.
- Deslocamento de atividades por arrastar e soltar, preservando sua duração.
- Destaque da data-base do projeto.

### Escala temporal

O cronograma pode ser visualizado em:

- Dias.
- Semanas.
- Meses.

A mudança de escala não altera as datas das atividades; apenas modifica a forma como o período é apresentado.

### Cabeçalho do produto

O título e o subtítulo identificam dinamicamente:

- Nome do projeto.
- Código do projeto.
- Tipo da ferramenta.
- Data-base do planejamento.

## Organização visual

- O ID permanece em uma coluna exclusiva.
- Nome, descrição e datas compartilham a área principal da atividade.
- O nome é exibido em negrito como informação prioritária.
- Descrição e datas usam hierarquia visual secundária.
- O cabeçalho da estrutura apresenta: **Estrutura · descrição · início · fim**.
- Os controles de linha são compactos para maximizar a área de conteúdo.

## Regras de interação

- Datas devem seguir o padrão `AAAA-MM-DD`.
- A data final não pode ser anterior à data inicial.
- IDs devem ser únicos em todo o planejamento.
- Toda atividade deve possuir ID, nome, início e fim.
- Ao mover uma barra no Gantt, início e fim são deslocados pela mesma quantidade de dias.
- Ao excluir um item pai, todas as tarefas abaixo dele também são removidas.

## Escopo atual

O produto cobre a criação e manutenção visual de um cronograma estruturado. Não fazem parte deste contexto:

- Gestão financeira do projeto.
- Controle de horas realizadas.
- Apontamento individual de esforço.
- Aprovação formal de mudanças.
- Gestão documental.
- Autenticação e perfis de acesso.

## Evoluções possíveis

- Marcos e entregas-chave.
- Caminho crítico.
- Relações visuais entre dependências.
- Percentual de conclusão.
- Baseline planejada versus realizado.
- Filtros por frente, status, prioridade e recurso.
- Identificação de atrasos e conflitos de dependência.
- Histórico de alterações.
- Colaboração compartilhada entre usuários.
