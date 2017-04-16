
# Especificação de Requisitos do SISB
O SISB envolve várias funcionalidades conforme o [ConOps](https://github.com/kyriosdata/sisb/blob/master/ConOps.md), que inspira as características desejáveis apresentadas abaixo. Tais características, por sua vez, deverão inspirar requisitos de usuário e/ou requisitos de software. 

## Características
As características desejáveis seguem abaixo agrupadas por "tópicos" relevantes. Os itens de cada tópico seguem em ordem de prioridade.

- A1 [Agendamento](https://github.com/kyriosdata/sisb/blob/master/docs/Requisitos.md#a1-agendamento)
- F2 [Financeiro e faturamento](https://github.com/kyriosdata/sisb/blob/master/docs/Requisitos.md#f2-financeiro-e-faturamento)
- P3 [Paciente](https://github.com/kyriosdata/sisb/blob/master/docs/Requisitos.md#p3-paciente)

### A1 Agendamento
- A1.1 Agendamento de consultas
- A1.2 Agenda telefônica e de contatos. Incluir endereços de whatsapp e skype, dentre outros.
- A1.3 Alerta de retorno (via lembrete de email enviado automaticamente ou via whatsapp).
- A1.4 Controle de retornos
- A1.5 Confirmar consulta
- A1.6 Disponibilidade (para agendamento)
- A1.7 Enviar SMS, receber SMS e produzir relatório de enviados/recebidos
- A1.8 Pesquisa de satisfação
- A1.9 Exibir agendas por dia, semana ou mês.
- A1.10 Relatórios detalhados e quantitativos de agendamentos
- A1.11 Mala direta

### F2 Financeiro e faturamento
- F2.1 Receitas, despesas
- F2.2 Orçamentos
- F2.3 Emissão de NFe
- F2.4 Integração com cielo e pagseguro
- F2.5 Gerenciar convênios
- F2.6 Faturamente TISS
- F2.7 Emissão de boleto e de recibos
- F2.8 Operadora de plano
- F2.9 Controle de faturamento de múltiplos convênios
- F2.10 Dashboard
- F2.11 Contas bancárias
- F2.12 Caixa interno
- F2.13 Controle de custo
- F2.14 Auditoria
- F2.15 Comissões
- F2.16 Relatórios de contratos
- F2.17 Multas
- F2.18 Configuração de boleto bancário

### P3 Paciente
- P3.1 Cadastro de paciente com fotos
- P3.2 Atendimentos
- P3.3 Gerenciamento de espera de paciente
- P3.4 Filas de atendimento
- P3.5 Aniversariantes
- P3.6 Importação de paciente
- P3.7 Plano de indicação
- P3.8 Controle de retorno
- P3.9 Pendências
- P3.10 Botão de pânico

### S4 Atenção à saúde
- S4.1 CID-10, CID-O
- S4.2 Alertas
- S4.3 Odontograma gráfico
- S4.4 Situação bucal
- S4.5 Prescrição
- S4.6 Atestado
- S4.7 Planejamento
- S4.8 Anamnese clínica
- S4.9 Fotografias (anexo de imagens)
- S4.10 Solicitação de exames
- S4.11 Solicitação de encaminhamentos
- S4.12 Relatório de procedimentos
- S4.13 Procedimentos em aberto, realizados e cancelados
- S4.14 Medicamentos
- S4.15 Fórmulas
- S4.16 Solicitação de próteses

### E5 Estoque
- E5.1 Inventário de estoque
- E5.2 Cadastro de produtos
- E5.3 Categorias de produtos
- E5.4 Fornecedores
- E5.5 Ordem de compra
- E5.6 Controle de compras
- E5.7 Requisição de produtos

### R6 Recursos humanos
- R6.1 Cadastro de corpo clínico (inclusive por consultório)
- R6.2 Estatística de produtividade
- R6.3 Comunicação interna (chat com colaboradores da clínica)
- R6.4 Controle de ponto
- R6.5 Ranking de dentistas
- R6.6 Relatório de “todos os dentistas”
- R6.7 Relatório de remunerações

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
