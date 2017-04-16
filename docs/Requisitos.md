
# Especificação de Requisitos do SISB
O SISB envolve várias funcionalidades conforme o [ConOps](https://github.com/kyriosdata/sisb/blob/master/ConOps.md).
Em consequência, acredita-se que, em uma análise preliminar, uma hierarquia iniciada por necessidades/objetivos dê origem a características ou requisitos de usuário (registrados por meio de estórias de usuários e/ou casos de uso) que, por sua vez, deem origem a requisitos de software.

## Características
As características desejáveis seguem abaixo agrupadas por "tópicos" relevantes. Os itens de cada tópico seguem em ordem de prioridade.

### Agendamento
- Agendamento de consultas
- Agenda telefônica e de contatos (whatsapp, skype, ..)
- Alerta de retorno (whatsapp)
- Controle de retornos
- Confirmar consulta
- Disponibilidade (para agendamento)
- Enviar SMS, receber SMS e produzir relatório de enviados/recebidos
- Lembrete via email
- Pesquisa de satisfação
- Exibir agendas por dia, semana ou mês.
- Relatórios detalhados e quantitativos de agendamentos
- Mala direta

### Financeiro e faturamento
- Receitas, despesas
- Orçamentos
- NFe
- Integração com cielo, pagseguro (outro?)
- Gerenciar convênios
- Faturamente TISS
- Emissão de boleto e de recibos
- Operadora de plano
- Controle de faturamento de múltiplos convênios
- Dashboard
- Contas bancárias
- Caixa interno
- Controle de custo
- Auditoria
- Comissões
- Relatórios de contratos
- Multas
- Configuração de boleto bancário

### Fluxo de paciente
- Cadastro de paciente com fotos
- Atendimentos
- Gerenciamento de espera de paciente
- Filas de atendimento
- Aniversariantes
- Importação de paciente
- Plano de indicação
- Cadastro de paciente
- Controle de retorno
- Pendências
- Botão de pânico

### Atenção à saúde
- CID-10, CID-O
- Alertas
- Odontograma gráfico
- Situação bucal
- Prescrição
- Atestado
- Planejamento
- Anamnese clínica
- Fotografias
- Solicitação de exames
- Solicitação de encaminhamentos
- Relatório de procedimentos
- Procedimentos em aberto, realizados e cancelados
- Anexo de imagens (fotos antes e depois)
- Medicamentos
- Fórmulas
- Solicitação de próteses

### Produtos
- Inventário de estoque
- Produtos
- Categorias de produtos
- Fornecedores
- Ordem de compra
- Controle de compras
- Requisição de produtos

### Pessoal
- Cadastro de corpo clínico (inclusive por consultório)
- Estatística de produtividade
- Comunicação interna (chat com colaboradores da clínica)
- Controle de ponto
- Ranking de dentistas
- Relatório de “todos os dentistas”
- Relatório de remunerações

### Software e hardware
- Livre de royalties
- O SISB deve estar em conformidade com o Manual de Certificação da SBIS. Não conformidades deverão ser aprovadas pelo patrocinador.
- Cliente disponível para iOs, Android e desktop (browser)
- Acesso à agenda online, tanto pelo paciente quanto pelo odontólogo
- Backup diário
- Deve ser executado em hardware "convencional" (commodity hardware).
- Pode ser implantado em "nuvem"
- Execução pode ser em Windows, Linux ou MacOS.
- Suporte para múltiplos idiomas.
- A facilidade de uso do SISB deve ser uma de suas principais características. De fato, apenas com a autorização do patrocinador do projeto um aspecto de usabilidade deverá ser "prejudicado" em detrimento de outro requisito.

### Qualidade interna
- A interação de clientes (interface com o usuário) com o SISB e os serviços oferecidos serão projetados em conformidade com as diretrizes contidas no [API Design Guid](https://cloud.google.com/apis/design/). 
- O SISB deve estar em conformidade com os padrões adotado pelo Brasil para interoperabilidade semântica.
- O SISB deve interagir com os serviços do barramento do SUS: CNS, CNES, SIGTAP, e-SUS AB e Horus.
- Manutenção corretiva deve ser feita em no máximo 2 dias.
- Não poderá ficar indisponível por no máximo 2 horas por dia.
- Apresentar bom desempenho.
- O SISB deve ser capaz de se manter em operação por um peíodo ininterrupto de 30 dias. 
- A instalação padrão deve atender 10 usuários. Outros cenários: 50, 200, 1.000 e 10.000 usuários.
- O SISB deve estar apto para armazenar dados para 5000, 100.000 e 10.000.000 de pacientes.
-  O cycle time do SISB deve ser de, no máximo, 2 horas.
