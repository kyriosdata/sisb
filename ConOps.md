# Contexto de operação (ConOps)
Abaixo segue uma visão operacional do SISB na perspectiva dos seus usuários. Essa visão é útil para fornecer evidências dos serviços oferecidos pelo SISB para satisfazer os objetivos identificados acima.

#### Contexto do sistema

![sisb-context](https://cloud.githubusercontent.com/assets/1735792/23717130/617f2376-0411-11e7-95de-35b33e00bc21.png)

| Ator           |   Descrição  |
|:--------------:|----------------|
|Administrador   | Responsável pela manutenção do SISB em operação. |
|Odontólogo      | Profissional de saúde que consulta e gera informação em saúde bucal nos prontuários dos pacientes.     |
|Sistema externo | Sistema com o qual o SISB interage, tanto para enviar quanto para receber informações em conformidade com os padrões adotados pelo Brasil.|
|Barramento SUS| Conjunto de serviços oferecidos pelo Datasus (CNS, CNES, Horus, SIGTAP e eSus-AB).|


#### Casos de uso

![sisb-use-cases](https://cloud.githubusercontent.com/assets/1735792/23718572/c02b3356-0416-11e7-8617-99558f063784.png)

| Caso de Uso    |   Descrição  |
|--------------|----------------|
|Acrescentar informações| Permite acrescentar informações ao prontuário de um paciente.|
|Consultar informações|Permite consulta às informações contidas em um prontuário de um dado paciente.|
|Localizar paciente| Permite busca por paciente (apenas dados demográficos)|
|Trocar informações| Permite o envio para e o recebimento de informações em saúde contida em sistema externo ao SISB. Em ambos os casos a operação não permite ao usuário o acesso às informações propriamente ditas, mas apenas àquelas pertinentes à transação (transferência).|
|Cadastrar paciente| Dados demográficos de pacientes já cadastrados podem ser confirmados e, se necessário, atualizados, bem como um novo cadastro criado. Permite a recuperação de informações via CNS.|
|Monitorar SISB|Permite acompanhar a operação (funcionamento do SISB).|
|Gerenciar usuários|Permite a gestão do cadastro de usuários do SISB, o que inclui recursos para habilitar/desabilitar usuário, alteração de senha e outras questões pertinentes.|

#### Modelo do domínio
Os principais conceitos utilizados pelo SISB são ilustrados abaixo. De forma resumida, um Registro Eletrônico em Saúde (RES), de um dado Paciente, é formado por uma composição de dados em saúde. Cada dado é definido por um arquétipo e, naturalmente, foi produzido por um profissional de saúde (usuário), que possui a devida autorização para tal. As trocas de informação com sistemas externos ou são de importação ou de exportação de dados e, em ambos os casos, está associada a um dado específico.

![sisb-domain](https://cloud.githubusercontent.com/assets/1735792/23722478/436b2994-0424-11e7-872c-1fc261542468.png)

#### Visão operacional
Em um cenário típico, por meio da internet tem-se acesso às recursos oferecidos pelo SISB. Esse acesso é utilizado por odontólogos, pela secretária e também pelo administrador do SISB. Dada a necessidade de manutenção das informações, há previsão de montagem de cópia de segurança, conforme ilustrado abaixo.

![sisb-operacional](https://cloud.githubusercontent.com/assets/1735792/23764690/35f2216e-04dd-11e7-99e8-735665815761.png)

No cenário acima um servidor atende requisições de vários terminais simultanemente. O SISB, contudo, deve ser capaz de operar em outros cenários, por exemplo, no qual o usuário interage com um computador no qual o SISB está em execução, sem conexão com serviço remoto.

#### Restrições

- Fazer uso exclusivo de tecnologia "livre" de royalties. 
- O SISB deve apresentar "baixo" custo de implantação e também "baixo" custo de manutenção. O custo deve ser monitorado e, na presença de mudança, aprovado pela patrocinadora do projeto. Naturalmente, o custo é uma função de várias variáveis, inclusive da quantidade de acessos concorrentes por unidade de tempo para os quais o serviço deve se manter estável. 

