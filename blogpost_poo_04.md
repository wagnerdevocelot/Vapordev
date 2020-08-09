![](https://res.cloudinary.com/practicaldev/image/fetch/s--aYuB-ad5--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/560/1%2AmkaVgFHEwnGtWURrW2-VkQ.png)
# Code Club

A primeira regra do “code club” é usar encapsulamento

Esse é o último capítulo sobre **POO** e eu deixei o pior para o final, é comum ver que a maioria dos iniciantes em programação assim como eu tem dificuldades em entender o **encapsulamento**.

Mas antes de falar de código, como de costume vou falar sobre alguma **random-shit** que talvez você não tenha interesse.

> “_A história de dois amigos que iniciam um clube amador de boxe para jovens desfavorecidos e a mulher que aparece entre eles._”

Segundo **Brad Pitt** essa é a melhor definição sobre o “Clube da Luta”

Segundo [**Friedrich Nietzsche**](https://pt.wikipedia.org/wiki/Friedrich_Nietzsche) talvez o Clube da Luta seria uma tentativa fracassada de superar o **Niilismo**.

O [Niilismo](https://pt.wikipedia.org/wiki/Niilismo) é ponto de vista que considera que as crenças e os valores tradicionais são infundados e que não há qualquer sentido ou utilidade na existência. A partir de certo ponto e da discussão do assunto novos significados e derivações foram abordados como o **Niilismo-Existencial** e o **Niilismo-Absurdista**.

Na história de Clube da Luta o personagem principal interpretado por **Edward** **Norton** encontra valor em uma vida consumista, que tem propósito nas coisas que compra como, móveis, apartamento e roupas.

O personagem principal segue as regras e valores pelos quais todos nós estamos inseridos, assim como as **leis**, **honra** e a **democracia**, assumindo um papel totalmente reativo durante sua existência, valores que nos tornam cada vez mais dóceis e domesticáveis. Dentro dele, assim como dentro de todos nós, existe uma parte que anseia se livrar dessas amarras, uma parte que deseja nos mostrar que nada disso tem sentido inerente.

Essa parte se chama **Tyler** **Durden** interpretado por **Brad** **Pitt**.

**Tyler** **Durden** é a total antítese do protagonista, potente, másculo, faz o que der na telha sem nenhum medo das consequências que suas ações possam ter. O que o protagonista sente em relação a **Tyler** é puramente amor platônico. Juntos eles formam um clube de homens que através de lutas de boxe clandestinas ditam as próprias regras de como devem agir no clube e perante a sociedade.

**Regras**:

**A primeira regra do Clube da Luta é:** _você não fala sobre o Clube da Luta._

**A segunda regra do Clube da Luta é:** _você não fala sobre o Clube da Luta._

**Terceira regra do Clube da Luta:** _se alguém gritar “Pára!”, fraquejar, sinalizar, a luta está terminada._

**Quarta regra:** _apenas dois caras numa luta._

**Quinta regra:** _uma luta de cada vez, pessoal._

**Sexta regra:** _sem camisas, sem sapatos._

**Sétima regra:** _as lutas duram o tempo que for necessário._

**E a oitava e última regra:** _se esta for a sua primeira noite no Clube da Luta, você tem de lutar._

O protagonista que de pessoa fraca, sem atividade e com valores apenas consumistas, passa por um período niilista onde todos os seus valores anteriores são quebrados por **Tyler Durden**, que em uma metáfora a filosofia de **Nietzsche** seria o martelo. **Martelo** responsável por quebrar todas as amarras metafísicas do ser humano como **religião**, **ciência** e o **comunismo**, onde o ser somente alcança a sua plenitude através de uma vivência que tem apenas a sua própria vida como valor.

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--w67ka0xA--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/1280/1%2A6RIJNo2vezY-2L_p2bwVmg.jpeg)](https://res.cloudinary.com/practicaldev/image/fetch/s--w67ka0xA--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/1280/1%2A6RIJNo2vezY-2L_p2bwVmg.jpeg)

Mas essa era a primeira fase da desconstrução de valores do personagem, em seguida é colocado em prática o projeto **Mayhem**, que tem como objetivo promover ataques contra o consumismo.

E assim como o amor descrito por Platão, onde amamos o que desejamos e desejamos aquilo que não temos, a partir do momento que o protagonista descobre que **Tyler Durden** é parte de sua própria psique o amor por Tyler Durden acaba, pois a partir do momento em que o protagonista descobre que tem dentro de si mesmo aquilo que desejava, isso se torna um fardo.

> _“Em uma dinâmica doentia em que se sente angústia de não ter a disposição o objeto do amor e aborrecido quando o possuímos.”_

É nesse ponto então em que o protagonista atira em sua pŕopria cabeça, fazendo com que a personalidade de **Tyler Durden** se apague. Voltando ao status anterior. Aqui acredito que seria a missão de vencer o niilismo fracassado, pois para **Nietzsche** a ideia de **Niilismo** é trabalhada a partir de que o sujeito niilista é aquele que possui valores construídos pela massa reativa, justamente o inverso do conceito de niilismo discutido anteriormente.

Falando sobre encapsulamento, acredito que a maioria das pessoas devem ter dificuldade assim como eu tenho, porque elas não sabem a princípio, o que deve ser encapsulado, quais atributos devem ser **privados**, **protegidos** ou **públicos**.

E a resposta para essa pergunta é; Depende!

E justamente por isso que é difícil de cravar, isso é protegido, isso é público e etc. E justamente pela resposta ser depende, é difícil de explicar e também difícil de entender. Qualquer um que vai te dar um exemplo vai falar sobre um atributo cartão de crédito, e aí tem que ser protegido obviamente e etc.

Da mesma forma como nem todo mundo vai trabalhar com **POO** criando abstração de classe chamada “Cachorro” ou “Gato” nem todos vão trabalhar com cartão de crédito ou **dados sensíveis**.

Então a minha resposta seria, aprenda a fazer, mas neste momento não precisa entender todas as aplicações. Quando você estiver em um projeto onde seja necessário você vai ter essa experiência e isso vai te ajudar a seguir com o restante. Então, se você souber como, já é suficiente.

Anteriormente já falei sobre o [**_attr_accessor_**](https://dev.to/vapordev/shin-programming-tensei-32d)

Ele é um atalho para os métodos de leitura e de escrita de um atributo.  
  
Com o **Ruby** os métodos são sempre públicos, então se você colocar qualquer coisa privada dentro de um método ele será acessível. Assim como o Java tem os métodos **getters** e **setters** para que possamos acessar essas propriedades. No **Ruby** além do **attr_accessor** podemos usar:

[**_attr_reader_**](https://www.rubyguides.com/2018/11/attr_accessor/)[**_attr_writer_**](https://www.rubyguides.com/2018/11/attr_accessor/)

```
class Protagonista
    attr_writer :primeira_personalidade
    attr_reader :segunda_personalide

    def initialize(primeira_personalidade,segunda_personalide)
        @primeira_personalidade =primeira_personalidade
        @segunda_personalide =segunda_personalide
    end
end

```

Aqui temos uma classe chamada protagonista que tem dois atributos **primeira_personalidade** e **segunda_personalidade** que são atributos de **escrita** e um de **leitura**. Como eu defini isso? Arbitrariamente, porque eu quis.

A primeira personalidade assim como o Protagonista de clube da luta eu vou descrevê-la como sendo frágil e fácil de influenciar. Sendo assim, eu posso instanciar a classe **Protagonista** e redefinir o atributo **primeira_personalidade** como **Tyler Durden**, assim.

```
consumistorcompulsivo  =  Protagonista.new('Consumista', 'Anarquista')

p  consumistorcompulsivo.primeira_personalidade=  'Tyler Durden'

```

E no terminal o resultado:

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--aSbWnFyB--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/570/1%2A7Ei5I4iL1f0X3kPCekczlw.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--aSbWnFyB--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/570/1%2A7Ei5I4iL1f0X3kPCekczlw.png)

Então por ser um atributos de escrita ele pode ser modificado sem menores problemas, agora quando falamos da **segunda_personalidade** que no caso vamos defini-la como a mais forte, ou seja “**Tyler Durden**” acontece isso.

```
consumistorcompulsivo  =  Protagonista.new('Consumista', 'Anarquista')
p  consumistorcompulsivo.segunda_personalide=  'Retomar o Controle'

```

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--nBtZBCBS--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/811/1%2AJF4DDkfeTDive_bPLJpLYA.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--nBtZBCBS--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/811/1%2AJF4DDkfeTDive_bPLJpLYA.png)

O terminal retorna um erro perguntando se você queria chamar **segunda_personalidade**, que foi o que eu fiz, porém eu tentei chamá-la redefinindo seu atributo a algo diferente, o que ela não permite, pois é um atributo de **leitura** apenas.

Como no **Ruby** é possível fazer muita coisa em tempo de execução, podemos redefinir a **segunda_personalidade** inserindo ela dentro de um **método**, assim.

```
def consumistorcompulsivo.segunda_personalide(controle)
    segunda_personalide = controle
end

p consumistorcompulsivo.segunda_personalide'Acorda'

```

Resultado no terminal:

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--EiLn5air--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/587/1%2AQ5RsSIgPujoS0G3ihhsPfw.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--EiLn5air--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/587/1%2AQ5RsSIgPujoS0G3ihhsPfw.png)

Quando você insere um atributo ou método que é **protegido** dentro de outro **método** ele se torna **público**, porque nomes de métodos sempre são públicos por padrão. A mesma coisa com um método seria assim.

```
class Protagonista
    attr_writer :primeira_personalidade
    attr_reader :segunda_personalide

    def initialize(primeira_personalidade,segunda_personalide)
        @primeira_personalidade =primeira_personalidade
        @segunda_personalide =segunda_personalide
    end

    private
    def sono
        'Dormir'
    end
end

```

Temos o método **sono** do qual o protagonista do filme é privado. E aqui nós privamos ele apenas escrevendo **private**, ele só irá funcionar dentro da **Classe**. Para acessá-lo como fizemos com o atributo a lógica é a mesma.

```
consumistorcompulsivo = Protagonista.new('Consumista', 'Anarquista')

def consumistorcompulsivo.niilismo
    sono
end

p consumistorcompulsivo.niilismo

```

Como a galera gosta de inventar história em programação como aquela do **Duck Typing**, vou inventar a minha aqui a respeito de métodos no Ruby. Que é “Diga-me com quem andas, e lhe direi quem és” — Wagner Abrantes.

Resultado no terminal:

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--jtH1mTH9--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/566/1%2A5vBd1Y5nvM8WeJOV4-436A.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--jtH1mTH9--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/566/1%2A5vBd1Y5nvM8WeJOV4-436A.png)

Por último, a **visibilidade** para métodos e atributos, além de **private**, e **public** podem também ser **protected**.

**Public** — Todo mundo pode usar  
  
**Private** — Somente a Classe pode usar  
  
**Protected** — Apenas a Superclasse e suas Subclasses podem usar

O assunto sobre os Pilares da **Programação Orientadas a Objetos** termina aqui. Porém o assunto é muito mais amplo e pretendo abordá-los futuramente. Como **Solid**, **Patterns** e etc.

Finalizando o assunto sobre o Clube da Luta, que hoje já é um subproduto da própria crítica, existe mais nesse filme além do **suicídio**, **consumismo**, **niilismo** e também o **machismo**.

Depois do anos 2000 onde os Homens já não tem mais uma guerra para lutar e já não conseguem encontrar mais utilidade preenchendo a vida com bugigangas qualquer pessoa carismática o suficiente como **Tyler Durden** (e nem precisa ser muito inteligente) são capazes de manipular uma massa de homens buscando um pŕoximo objetivo de vida antes de morrer. Desde a antiguidade os homens foram levados a acreditar que tinham um propósito maior, até hoje miltares na américa são reverenciados por matar mulheres e crianças no **Vietnã**.

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--vSgi1LM_--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/1500/1%2AQF3j6xsSTeJ6NhAJkwdm7A.jpeg)](https://res.cloudinary.com/practicaldev/image/fetch/s--vSgi1LM_--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/1500/1%2AQF3j6xsSTeJ6NhAJkwdm7A.jpeg)

Ataque químico ao vilarejo de Trang Bang, no Vietnã-1972

Parte da critica do filme que é soterrada pelo consumismo é sobre a masculinidade tóxica que leva uma massa a acreditar em valores criados por poderes reativos e suas regras. E esse link com a **Guerra do Vietnã** acredito ser justificado quando muito cedo no filme **Tyler Durden** ensina o Protagonista a fazer **Napalm** caseiro.

Todos já conhecem o Clube da Luta, já falaram sobre e eu ainda to aqui falando de Clube da Luta. Porque **quebrar** a primeira **regra** do Clube da Luta ainda vale a pena.

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--5xfJ-oUd--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/800/1%2A3yep-GGjQgBgMpH2Bi5ptw.jpeg)](https://res.cloudinary.com/practicaldev/image/fetch/s--5xfJ-oUd--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/800/1%2A3yep-GGjQgBgMpH2Bi5ptw.jpeg)

Full Metal Jacket — Filme de 1987
