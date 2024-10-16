# resumo-do-lab- CLOUD AZURE
![Badge](https://img.icons8.com/?size=100&id=81727&format=png&color=000000)
### Beneficios da Nuvem 
- #### Alta disponibilidade
  se concentra em garantir a disponibilidade maxima, independemente de interrupçoes ou eventos que possam ocorrer.

- #### Escalabilidade
  refere-se a capacidade de ajustar recursos para atender a demanda, significa que você podera adicionar mais recursos para atender a demanda.

- #### Elasticidade
  seus recursos implantados poderiam ser expandidos de acordo com a demanda (automaticamente ou manualmente).



## Terror dos 9 - (Brincadeira à parte)

Os "9" são considerados o tempo de inatividade do serviço. Quanto mais "9", menos tempo o seu serviço ficará indisponível. Veja este [documento](https://www.microsoft.com/licensing/docs/view/Service-Level-Agreements-SLA-for-Online-Services?lang=1) sobre SLA.

### Entendendo os "9" no SLA
O conceito de SLA é frequentemente expresso como porcentagens de disponibilidade anual. Quanto maior a porcentagem de SLA, menos tempo de inatividade o serviço terá. Veja abaixo uma tabela que ilustra o tempo de inatividade correspondente a cada nível de SLA:

| SLA (%)    | Disponibilidade anual | Tempo de inatividade por ano | Tempo de inatividade por mês |
|------------|-----------------------|------------------------------|------------------------------|
| 99%        | Alta                  | 87,6 horas                   | 7,2 horas                    |
| 99,9%      | Muito Alta            | 8,76 horas                   | 43,8 minutos                 |
| 99,99%     | Extremamente Alta     | 52,56 minutos                | 4,38 minutos                 |
| 99,999%    | Quase perfeita        | 5,26 minutos                 | 26,3 segundos                |

### Como garantir mais "9"
Claro que esses "9" podem ser modificados de acordo com o peso e a criticidade do seu serviço. Se você criar, por exemplo, uma máquina virtual com **3 zonas de disponibilidade**, ou aumentar os recursos alocados, o tempo de inatividade diminui e, consequentemente, a disponibilidade do serviço aumenta.

- **Zonas de disponibilidade**: Implementar redundância em várias zonas de disponibilidade garante que seu serviço continue ativo mesmo que uma zona falhe.
- **Recursos adicionais**: Ao aumentar o poder de computação, armazenamento e a redundância da rede, você reduz os riscos de downtime, mas isso aumenta o custo ($$).

### Relação Custo x Disponibilidade
Quanto maior a disponibilidade (mais "9"), mais caro será o serviço. Isso acontece porque você está utilizando mais recursos e aumentando a resiliência do sistema. Por exemplo:

- Um SLA de 99,9% pode ser atingido com máquinas virtuais simples, mas adicionar zonas de disponibilidade pode levar seu SLA para 99,99%, aumentando os custos. Essa é uma escolha importante que deve ser baseada na criticidade da aplicação.

Por fim, é essencial equilibrar o nível de SLA com o custo, levando em consideração o impacto do downtime para o seu negócio. Serviços críticos que não podem ficar offline, como sistemas financeiros ou plataformas de e-commerce, podem justificar custos mais altos para garantir maior disponibilidade.


