# SISB
O Sistema de Informação em Saúde Bucal, ou simplesmente SISB, é um sistema de informação em saúde voltado para atender necessidades de informação no escopo da saúde bucal. 

### Objetivos
Os principais objetivos dos interessados (_stakeholders_) incluem:
- Fortalecer a reputação do Estado de Goiás na produção de solução de qualidade para a área da saúde.
- Posicionar a UFG como parceira relevante para ações na saúde.
- Atender os padrões de interoperabilidade adotados pelo Brasil. 
- Atender necessidades de informações em saúde bucal no escopo da atenção primária.

O [Termo de Abertura](https://docs.google.com/document/d/1-7-s9yEcUR5eE9cigPSo0GyrEhAQpxWoK1soz_29M84/edit?usp=sharing) inclui várias outras informações relevantes para o contexto do SISB.

***

### Contexto de operação (ConOps)
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

***

### Requisitos
- Suporte para múltiplos idiomas.
- Possibilidade de uso local (_on-premise_) ou "nas nuvens".
- Deve ser executado em hardware "convencional" (_commodity hardware_), que pode ser facilmente adquirido e geralmente de baixo desempenho. Noutras palavras, não exige fornecedor específico de hardware.
- Um novo dispositivo (computador) para acesso de usuários do SISB pode ser acrescentado sem necessidade de interromper o sistema. 
- O SISB deve estar em conformidade com o Manual de Certificação da SBIS. Não conformidades deverão ser aprovadas pelo patrocinador.
- O SISB deve estar em conformidade com os padrões adotado pelo Brasil para interoperabilidade semântica. 

### Entregáveis
- Definição e documentação da arquitetura de software do SISB.
- Prova de conceito da arquitetura. Deverá haver um "equilíbrio" entre a prova de conceito e a documentação da arquitetura de software. A tendência é que uma documentação extensiva diminua ou até elimine a existência (necessidade) da prova de conceito e vice-versa. 

### Links relevantes

- Extensiva lista de métodos para UX ([aqui](https://uxdesign.cc/ux-design-methods-deliverables-657f54ce3c7d#.k5lcj41zn)).
- Interação com o usuário: (a) papel e caneta; (b) possivelmente acompanhado de template [t1](http://www.uxforthemasses.com/wordpress/wp-content/uploads/2010/07/AP_Template_6_Up11.pdf) ou [t2](http://www.uxforthemasses.com/wordpress/wp-content/uploads/2010/07/AP_Template_1_Up1.pdf); (c) prototyping tool ([cara](https://www.axure.com/)); (d) [Mockups](https://www.mockplus.com), [Balsamiq](https://balsamiq.com/) e [InVisionApp](https://www.invisionapp.com) são as "mais fáceis e de grande qualidade"; (f) outras incluem JustInMind, Sketch, Adobe Experience Design, além de (g) free like [pencil](http://pencil.evolus.vn/).
- [Sumário de alta](http://www.abntcatalogo.com.br/norma.aspx?ID=353212) se aplica?
- [openeyes](http://www.openeyes.org.uk/) Código fonte: [aqui](https://github.com/openeyes).
- [Prescrição](https://github.com/kyriosdata/db/wiki/Prescri%C3%A7%C3%A3o) é um outro estudo de caso do HealthDB que ilustra cliente típico a ser disponibilizado em farmácia ou ponto de dispensação que exige acesso à prescrição para um dado paciente. 
- [Arden](https://github.com/kyriosdata/db/wiki/Arden) é uma proposta de sistema (software) que interage com o HealthDB para desempenhar ação típico de um sistema de apoio à decisão em saúde. 
- Como definir arquétipos com qualidade? ([aqui](https://ai2-s2-pdfs.s3.amazonaws.com/cc3c/ffdc896822989113155eb85f43658c7d88ad.pdf))
- National eHealth Strategy Toolkit ([aqui](http://www.who.int/ehealth/publications/overview.pdf))
- EHRs standards for India ([aqui](http://snomedctnrc.in/downloads/EHR-Standards-for-India%20-August2013-32630521.pdf))
- A review of interoperability standards ([aqui](https://www.google.com.br/url?sa=t&rct=j&q=&esrc=s&source=web&cd=10&cad=rja&uact=8&ved=0ahUKEwjsm_um_bTPAhXGj5AKHcL5DGgQFghhMAk&url=http%3A%2F%2Fsacj.cs.uct.ac.za%2Findex.php%2Fsacj%2Farticle%2Fdownload%2F176%2F73&usg=AFQjCNEAeFlOF0WQTIARIdqgFT1INBhOpA))
