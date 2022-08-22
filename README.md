# Javascript

__________

### **JavaScript** (frequentemente abreviado como **JS**) é uma linguagem de programação interpretada estruturada, de script em alto nível com tipagem dinâmica e multi-paradigma (protótipos, orientado a objeto, imperativo e funcional). Juntamente com HTML e CSS, o JavaScript é uma das três principais tecnologias da World Wide Web.

_________________

## **Estrutura de Controle**

Os tipos de estruturas de controle disponíveis diferem de linguagem para linguagem, mas podem ser cruamente caracterizados por seus efeitos. O primeiro é a continuação da execução em uma outra instrução, como na estrutura sequencial ou em uma instrução jump. O segundo é a execução de um bloco de código somente se uma condição é verdadeira, uma estrutura de seleção. O terceiro é a execução de um bloco de código enquanto uma condição é verdadeira, ou de forma a iterar uma coleção de dados, uma estrutura de repetição. O quarto é a execução de instruções distantes entre si, em que o controle de fluxo possivelmente volte para a posição original posteriormente, como chamadas de sub-rotinas e co-rotinas. O quinto é a parada do programa de computador.

---------------------

**Estrutura sequencial**

Uma estrutura sequencial realiza um conjunto predeterminado de comandos de forma sequencial, na ordem em que foram declarados no código fonte. A cada instrução, o contador de programa é incrementado.

________________

**Estrutura de seleção**

Também chamada de expressão condicional ou ainda construção condicional, a estrutura de seleção realiza diferentes computações ou ações dependendo se a seleção (ou condição) é verdadeira ou falsa. A condição é uma expressão processada e transformada em um valor booleano.

_______________

**Estrutura de repetição**

Uma estrutura de repetição realiza e repete diferentes computações ou ações dependendo se uma condição é verdadeira ou falsa, condição essa que é um expressão processada e transformada em um valor booleano. Está associado a ela além da condição (também chamada "expressão de controle" ou "condição de parada") o bloco de código: verifica-se a condição, e caso seja verdadeira, o bloco é executado. Após o final da execução do bloco, a condição é verificada novamente, e caso ela ainda seja verdadeira, o código é executado novamente.

______________

**Tomadas de Decisão**

(**IF/ELSE)** Frequentemente, queremos ser capazes de "condicionalmente" fazer algo em nossos programas - queremos ser capazes de dizer "se isto for verdadeiro, então faça X, mas se este outro for verdadeiro, então faça Y." É como quando acordamos de manhã - "se estiver chovendo, então levarei um guarda-chuva, mas se estiver fazendo sol, eu usarei óculos escuros." Podemos fazer algo condicionalmente em nossos programas usando estruturas condicionais if e estruturas condicionais if/else combinadas com expressões condicionais.

___________________

**(IF/ELSE)**

```
Se(condição)
Fazer alguma coisa
Senão
Fazer outra coisa
```

_____________

**Operadores**

Operador lógico é um elemento de ligação das palavras que compõem um comando. É o operador lógico que indica a maneira como se quer que uma palavra esteja em relação à outra.

![img](https://lh3.googleusercontent.com/he36dVX-xXsSz5w9Ylj7KI_nf3pZPAVHfs5Du3NIRWOJD7Gvde1cg9shb2T05kMW1SuQkaLMx5VGiuMQv0WCIcXf4e6S8cAZ5dmX1016egE0djAg9QRd8Mqs0v1b4tahLgBawfAmJi7hzmc)

**Vamos tentar explicar com um exemplo:**

Imagine que você quer um algoritmo (ou seja, uma sequência de comandos) para atravessar a rua com segurança. Como podemos escrevê-lo?

```
Se o semáforo estiver fechado:
Atravessar a rua.

Se não:
Aguardar.
```

- [ ] Conseguem encontrar um possível erro aqui?

________________________________________________________________

Imagine que o semáforo está fechado, mas um carro está se aproximando do semáforo em uma velocidade que claramente não conseguirá parar até chegar no mesmo. Com este algoritmo acima você seria atropelado.

Como podemos resolver isso? 



Com o operador lógico "E", poderíamos resolver nosso problema assim:

```
Se o semáforo estiver fechado E nenhum carro vindo em alta velocidade:
Atravessar a rua.
Se não:
Aguardar.
```



Além do "E", temos dois outros principais operadores lógicos para usarmos em nossos algoritmos (e futuramente no nosso código):

1.  OU
2.  NÃO

Usando o operador "**OU**":

```
Se o semáforo estiver fechado OU algum carro vindo em alta velocidade:
Atravessar a rua.
Se não:
Aguardar.
```

Usando o operador "**NÃO**":

```
Se o semáforo estiver fechado E NÃO tiver algum carro vindo em alta velocidade:
Atravessar a rua.
Se não:
Aguardar.
```

_____________

____________

**Operadores de comparação**

Neste fluxograma, como seria feita a decisão de se "**possui saldo suficiente**"?

![img](https://lh4.googleusercontent.com/wOfzUKImZ2d2qmD9mQhHTcrjuGdkBNLARkNElNMQTFGGS_-zA8UZit6V3XX9MHN-Pj48Zvw1ZSlttwMJEwC4HqLW-gRX4aBVLVIThTRcC9pThNvDpD4oKw3vVCuWbNPKsKrvGnXkKZwPGiE)

Podemos tomar esta decisão usando um operador **IGUAL**. Se a quantia solicitada for **IGUAL** ao saldo, realizar o saque. Se não, ler mensagem de saldo insuficiente.

Porém, com esta regra que criamos, nosso algoritmo ainda não funcionará adequadamente. Você consegue encontrar o problema?

Se você conseguiu encontrar o problema, resolveu o seu primeiro bug.

![img](https://lh4.googleusercontent.com/uUoMzOYtp8fvD8pc-TbsHyopx87oc8f8IIx7wRq2uqgmUd9hccgLt52U6pXDy72D2RrRbaN1x5Rnmm_CozktYAs4WglF_Odz2ZXHkWoD_h7H-_L3-k4GQgmazuzPUDQu1_tzuZA9XYp7qCQ)



Se o saldo do usuário fosse **100** reais e a pessoa tentasse sacar **20**, deveria funcionar. Mas o algoritmo que criamos anterior não deixaria o usuário sacar acusando falta de saldo.

_________

**Para resolvermos este bug temos alguns outros operadores de comparação:**

**●** MAIOR QUE **>**

● MENOR QUE **<**

● MAIOR OU IGUAL A **>=**

● MENOR OU IGUAL A **<=**

● DIFERENTE **!=**

**Para o nosso algoritmo podemos usar o operador de MENOR OU IGUAL A da seguinte maneira:**
**Se a quantidade solicitada pelo usuário for** **MENOR OU IGUAL A** **o saldo do usuário, o usuário possui saldo suficiente e o saque é permitido.**

**Se não, o usuário não possui saldo suficiente e o saque não é permitido.**

________

**Operadores aritméticos**

Já os operadores aritméticos são aqueles que estudamos na escola, aquelas funções básicas de somar, subtrair, multiplicar, dividir, etc.

E quais são eles?
 **+** **SOMAR**

 **-** **SUBTRAIR** 

**/** **DIVIDIR** 

***** **MULTIPLICAR**



Atividade em grupo 20 minutos:

Criar um algoritmo de um robô de auto-atendimento no WhatsApp.
**Importante: Aqui não vamos usar nenhuma linha de código, vamos apenas escrever um algoritmo que descreve o funcionamento do nosso robô.**
Mas o que o meu robô deve fazer?

![img](https://lh4.googleusercontent.com/BnnsEgs_aQEvSCt7O3BeASeyxpLUgxNtlGFGawfzeXonnWxpW9TWunrAxeKkFDCt9bZBUy0MtEkwqt0shTHILXdZVJnVnPxOj03-8RbRofh435w6Ry19ZSqZoU0YNzgS75yfuGaafyVEW_BrV_7rbw)



Com o algoritmo criado, agora vamos criar esse robô em javascript, podem utilizar o alert.
