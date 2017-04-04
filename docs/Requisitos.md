
# Especificação de Requisitos do SISB
O SISB envolve várias funcionalidades conforme o [ConOps](https://github.com/kyriosdata/sisb/blob/master/ConOps.md).
Em consequência, acredita-se que, em uma análise preliminar, uma hierarquia iniciada por necessidades/objetivos dê origem a características ou requisitos de usuário (registrados por meio de estórias de usuários e/ou casos de uso) que, por sua vez, deem origem a requisitos de software.


## Requisitos preliminares

### Agendamento
- Agendamento de consultas
- Agendamento simplificado
- Controle de agendamentos
- Enviar SMS, receber SMS, relatório de enviados/recebidos
- Agendamento por dia
- Pesquisa de satisfação
- Lembrete via email
- Relatórios detalhados e quantitativos de agendamentos
- Disponibilidade
- Controle de retornos
- Mala direta
- Confirmar consulta
- Alerta de retorno (whatsapp)
- Três tipos diferentes de agenda
- Agenda telefônica e de contatos (whatsapp, skype, ..)

### Financeiro e faturamento
- Gerenciar convênios
- Contas bancárias
- Multas
- Orçamentos
- Configuração de boleto bancário
- Caixa interno
- Relatórios de contratos
- Emissão de boleto e de recibos
- Comissões, NFSe
- Controle de custo
- Auditoria
- Dashboard
- Receitas, despesas
- NFe
- Integração com cielo e pagseguro
- Operadora de plano
- Controle de faturamento de múltiplos convênios
- Faturamente TISS

### Fluxo de paciente
- Sala de espera
- Consultório
- Pendências
- Atendimentos
- Aniversariantes
- Botão de pânico
- Importação de paciente
- Plano de indicação
- Filas de atendimento
- Cadastro de paciente com fotos
- Cadastro de paciente
- Controle de retorno

### Atenção à saúde
- Alertas
- Odontograma gráfico
- Situação bucal
- Prescrição
- Atestado
- Planejamento
- Anamnese clínica e ATM
- Fotografias
- Solicitação de exames
- Solicitação de próteses
- Relatório de procedimentos
- Procedimentos em aberto
- Procedimentos realizados
- Procedimentos cancelados
- Ortodontia
- Anexo de imagens (fotos antes e depois)
- Ficha clínica 
- Histórico clínico
- Medicamentos
- Fórmulas
- CID-10

### Produtos
- Produtos
- Fornecedores
- Categorias
- Ordem de compra
- Controle de compras
- Requisição de produtos
- Inventário de estoques

### Pessoal
- Ranking de dentistas
- Relatório de “todos os dentistas”
- Relatório de remunerações
- Estatística de produtividade
- Comunicação interna
- Cadastro de corpo clínico
- Chat com colaboradores da clínica
- Controle de ponto

### Software e hardware
- Backup diário
- Cliente disponível para iOs, Android e desktop (browser)
- Acesso à agenda online, tanto pelo paciente quanto pelo odontólogo
- Funcionalidade pode ser executada em Windows, Linux ou MacOS.
- Pode ser implantado em "nuvem"
- Deve ser executado em hardware "convencional" (commodity hardware).
- Suporte para múltiplos idiomas.
- O SISB deve estar em conformidade com o Manual de Certificação da SBIS. Não conformidades deverão ser aprovadas pelo patrocinador.
- Qualidade interna. A interação de clientes (interface com o usuário) e os serviços oferecidos será projetado em conformidade com as diretrizes contidas no [API Design Guid](https://cloud.google.com/apis/design/). 
- O SISB deve estar em conformidade com os padrões adotado pelo Brasil para interoperabilidade semântica.
- O SISB deve interagir com os serviços do barramento do SUS: CNS, CNES, SIGTAP, e-SUS AB e Horus.
- Manutenção corretiva deve ser feita em no máximo 2 dias.
- Não poderá ficar indisponível por no máximo 2 horas por dia.
- Apresentar bom desempenho.
- O SISB deve ser capaz de se manter em operação por um peíodo ininterrupto de 30 dias. 
- O cenário típico de uso do SISB é uma instalação que atende 10 usuários. Outros cenários devem contemplar 50, 200, 1.000 e 10.000 usuários.
- O SISB deve estar apto para armazenar dados para 5000, 100.000 e 10.000.000 de pacientes.
-  O cycle time do SISB deve ser de, no máximo, 2 horas.
- A facilidade de uso do SISB deve ser uma de suas principais características. De fato, apenas com a autorização do patrocinador do projeto um aspecto de usabilidade deverá ser "prejudicado" em detrimento de outro requisito.
