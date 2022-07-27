# Terraform_no_Azure

[Udemy Curso](https://www.udemy.com/course/terraformazure/)

## Definir

### Resource Groups

Grupos de recursos do Azure, devem compartilhar o mesmo ciclo de vida. Desta
forma, quando um **RG** é deletado, todos os seus Recursos são deletados em cascata.
Também significa que cada Recurso pode existir somente dentro(contido) de um
**RG**.

Recursos podem ser movidos de um **RG** para outro, sem problemas.

**RG** podem conter Recursos que residem em diferentes regiões. Dessa forma,
pode-se ter uma VM rodando no Brasil e outra no oeste dos EUA, e ambas estarem
contidas no mesmo **RG**.

Recursos podem interagir com outros Recursos que estejam contidos em **RGs**
diferentes.

#### Controles

##### Tags

Tem por função taguear um Recurso, de foma a definir uma descrição definindo a
qual finalidade o Recurso pertence.

##### Locks

Funciona como um bloqueio. Por exemplo, pode-se adicionar um Lock que impeça a
exclusão acidental.

##### IAM

Trata-se de um sistema de controle de acesso. Permite a definição de assinaturas
individuais para cada usuário. E protege as credenciais com controle de acesso.

##### Policies

Controla determinado tipo de comportamento ou efeito no **RG**.
