# Mecanismo de Staking
O Mecanismo de Staking é um investimento de renda passiva de criptomoedas. Ao escolher esta funcionalidade, as empresas podem criar um contrato com o cliente, que investirá seus tokens por um período de tempo. Este mecanismo beneficia a empresa, pois a validação da blockchain será feita com os usuários que utilizarão o mecanismo de staking, e não por computadores da rede. O cliente será beneficiado recebendo rendimentos, contanto que cumpra o mínimo de dias estabelecido no contrato.

## Formato do Mecanismo de Staking
Os formatos do mecanismo irão variar de acordo com o que cada empresa escolher.
* **Período de tempo**: indica quanto tempo os tokens precisam ficar aplicados em staking para receber a recompensa. Pode ser estabelecido por quantidade de dias ou mês.

* **Quantidade mínima de participação**: indica a quantidade minima de tokens que precisa ficar aplicado em staking para ser elegível a receber a recompensa. A quantidade mínima pode ser de 1 ou mais tokens.
* **Rentabilidade**: é o valor que será aplicado como recompensa do staking. A quantidade mínima pode ser de 1% ou mais, ou qualquer valor absoluto acima de 1 token.
* **Método**: valor porcentual ou absoluto aplicado à recompensa do staking.
* **Permissão para saque adiantado**: 
  - Sim, o cliente recebe o valor calculado proporcionalmente para a quantidade de dias que participou.
  - Não, o cliente pode sacar o valor, mas não recebe nenhum valor extra, além do que ja possuía.

💡 O valor de cashback, ficará disponível somente após o vencimento do prazo configurado inicialmente, mesmo que o saque adiantado esteja permitido. 

## Exemplo

**Tabela de configuração de staking**

| ID | Período | Staking Mínimo | Valor | Permissão para saque adiantado |
| -- | --| -- | -- | -- |
| 1 | 30 dias | 0 | 10% | Não |
| 3 | 30 dias | 0 | 20 absoluto | Sim |
| 4 | 10 dias | 100 | 10% | Sim |

**Tabela de aplicação do staking**

| Usuário | Config ID | Data de início | Data de término | Quantidade de tokens para staking| Valor de cashback | Saque adiantado | Data de saque |
| -- | -- | -- | --| --| -- | -- | -- |
| U1 | 1 | 01/01 | 30/01 | 150 | 15 | Não | 31/01 |
| U2 | 1 | 01/01 | 30/01 | 150 | 0  | Sim | 29/01 |
| U3 | 3 | 10/11 | 09/12 | 100 | <s>20</s> → 10 | Sim | 25/11 |
| U4 | 4 | 01/01 | 10/01 | 50  | Isto não seria possível, pois a quantidade é menor que o Staking Mínimo| - | - |
| U4 | 4 | 01/01 | 10/01 | 200 | <s>20</s> → 12 | Sim | 06/01 |

### Legenda
* **ID**: identificação do formato do mecanismo de staking.

* **Período**: período de tempo em que os tokens devem permanecer na carteira.
* **Staking mínimo**: valor mínimo de tokens permitido pela empresa para fazer parte do mecanismo de staking.
* **Valor**: valor percentual ou absoluto que será calculado o benefício de cashback.
* **Permissão para saque adiantado**: se o formato do mecanismo de staking permite o saque adiantado com cashback.
* **Data de início**: data em que o mecanismo de staking se inicia.
* **Data de término**: data em que o mecanismo de staking termina.
* **Data de saque**: data em que o cliente retira o valor depositado.
* **Quantidade de tokens para staking**: quantidade de tokens que o cliente depositou para o mecanismo de staking.
* **Valor de cashback**: quantidade de tokens ganhados ao final do staking.
* **Saque adiantado**: se o cliente fez o saque antes da data de término.