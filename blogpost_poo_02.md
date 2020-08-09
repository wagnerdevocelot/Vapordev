
![Cover image for Ru-By-Oh!](https://res.cloudinary.com/practicaldev/image/fetch/s--n2otYWmN--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://thepracticaldev.s3.amazonaws.com/i/s2uqgh82bb8yoic6meb5.png)
# Ru-By-Oh!

Continuando o assunto sobre **Programação Orientada a Objetos** hoje o assunto será sobre **Herança**. Que já adianto, não tem nada a ver com patrimônio monetário.

Caso não esteja familiarizado com os conceitos recomendo ler o artigo anterior onde falo sobre [**_Abstração_**](https://dev.to/wagnerdevocelot/shin-programming-tensei-32d).

Quando **Alan Kay** ajudou a criar o paradigma de Orientação a Objetos ele usou parte da sua experiência nos estudos de Biologia para criar a linguagem Smalltalk juntamente com **Adele Goldberg** e **Daniel Henry Holmes Ingalls**. Apesar da [**_Smalltalk_**](http://smalltalk.gnu.org/documentation) ser puramente Orientada a Objetos, outras linguagens já utilizavam características da **POO** como a [**_Simula 67_**](http://web.eah-jena.de/~kleine/history/languages/Simula-CommonBaseLanguage.pdf).

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--3kJX3t7h--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/577/1%2Atg6rFyeOQULEPzaIZimAow.jpeg)](https://res.cloudinary.com/practicaldev/image/fetch/s--3kJX3t7h--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/577/1%2Atg6rFyeOQULEPzaIZimAow.jpeg)

Alan Kay e seu bigode de dar inveja

A **Herança** que estimulou a criação dessa característica foi a **Herança Genética**, onde um organismo torna-se predisposto a adquirir características semelhantes à do organismo ou célula que o criou. O paradigma desde os anos 90 domina o mercado de software por isso hoje é tão importante conhecê-lo.

Perto de 2003 eu acho, estava na sétima série e tinha começado uma loucura que era o Anime de **Yu-Gi-Oh: Duel Monsters** na **TV Globinho** todo mundo comentava na escola no dia seguinte sobre os episódios, “nossa o Yugi derrotou o Kaiba com um Kuriboh, que humilhação”. Claro que na época a gente nem conhecia as regras verdadeiras. Onde já se viu colocar **Dragão Branco de Olhos Azuis** no campo a vontade sem fazer nenhum sacrifício?

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--Ufg-pZNH--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/1200/1%2AQJBbNujJX8BUSTkhWXKVwQ.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--Ufg-pZNH--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/1200/1%2AQJBbNujJX8BUSTkhWXKVwQ.png)

Yugi Moto e o cabelo mais difícil de fazer coslay

Na época do anime a gente não tinha as cartas então era bem triste, como sabia desenhar prometi na sala que ia fazer as cartas pra gente jogar no recreio. O design que usei para desenhar eram iguais aos do desenho pois não imaginava que eram de outro modo. Então tinha só a imagem e os pontos de ataque e defesa. Lembro que usei o papelão de uma caixa de chocolate para desenhar e uma caixa de Faber Castell. No final ficou muito legal só que duas semanas depois lançaram as cartas para comprar em bancas de jornal.

Por dois reais, você comprava um pacote que vinha com umas 3 ou 4 miniaturas dos Cards Reais. Era um negócio incrível, todo mundo tinha um card diferente que você não tinha e você queria tirar ele dessa pessoa hahaha. O jeito mais fácil era apostar batendo card até o cara ficar sem nada. Eu era bom demais nisso, cheguei a juntar umas 600 cartas.

O anime não foi muito longe na TV aberta, devido a uma histeria da família tradicional brasileira, que considerava o anime impróprio. Tudo em nome da audiência onde **Gilberto Barros** se dedicou 4/7 para convencer pais e mães desinformados de que **Yu-Gi-Oh** era “o baralho do diabo”, chegaram a falar que **Yu-Gi-Oh** tinha influência na **Yakuza**, não to brincando. Sobrou pra tudo que é anime, até mesmo **Dragon Ball** que passava na própria **Band**, emissora do **Gilberto Barros**.

Aqui temos uma demo do tipo de entretenimento que a TV Band nos proporcionava

O órgão que define a indicativa de idade para os desenhos classificou **Yu-Gi-Oh** inapropriado para menores de 12 anos e só poderia ser apresentado depois das 20H, o que fez com que a **Globo** obviamente parasse de transmitir o anime.

**Gilberto Barros** tinha um programa certamente apropriado para a família brasileira, com muita piada de duplo sentido, seminudez e tudo que dá pra colocar numa caixa escrita “sacanagem”. Essa é uma das provas de que o Brasil nunca foi para amadores e de que não era a primeira vez e nem a ultima em que a midia usava noções conservadoras para distorcer a realidade com termos como “Baralho do Diabo”.

Anos depois pude jogar **Yu-Gi-Oh Forbidden Memories** no falecido mas não esquecido **PSone**, que maravilha de jogo. Não atendia todas as regras oficiais mas era divertido mesmo assim. Quem define as regras oficiais do jogo, quais cartas são banidas e etc é a **Konami**, conhecida por publicar obras primas como **Silent Hill** e **Metal Gear Solid** e depois jogar eles na privada e dar descarga.

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--V0BlCRUz--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/468/1%2AdZghueQk3tOb8yAqRmcVhQ.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--V0BlCRUz--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/468/1%2AdZghueQk3tOb8yAqRmcVhQ.png)

Nada a ser dito aqui

Eu não vou abordar os detalhes das regras de **Yu-Gi-Oh** aqui porque é senso comum, até o padeiro sabe que carta na horizontal tá em modo de defesa e vertical é modo de ataque. Mas caso queira se aprofundar entra [aqui](https://img.yugioh-card.com/ygo_cms/ygo/all/uploads/Rulebook_v9_pt.pdf).

Geralmente na **POO** é comum ver exemplos de **Herança** como o exemplo de classe mãe e filha, onde uma herda características da outra ou com animais, é justamente dessa relação com a Biologia que cria-se uma facilidade de compreensão com os conceitos na programação.

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--8-qvnm98--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/860/1%2ANb6fKMhe5ZtBh9bBLmcVjw.jpeg)](https://res.cloudinary.com/practicaldev/image/fetch/s--8-qvnm98--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/860/1%2ANb6fKMhe5ZtBh9bBLmcVjw.jpeg)

Luke I’am your superclass

Se você leu o [**_artigo_**](https://dev.to/wagnerdevocelot/shin-programming-tensei-32d) anterior já está familiarizado com isso:

```
class  MonsterCard
    attr_accessor  :name, :attribute, :race, :level, :attack, :defense

    def  initialize
        @name  = name
        @attribute  = attribute
        @race  = race
        @level  = level
        @attack  = attack
        @defense  = defense
    end

    def  attack_defense_mode
    end

    def  attack_attack_mode
    end

    def  attack_lp_directly
    end

    def  change_position
    end

end

```

Essa seria a abstração utilizada para criar um objeto de uma carta como essa:

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--JVsEG_-I--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/326/1%2A7dRGoAeQlsJiTOzRxKFRGg.jpeg)](https://res.cloudinary.com/practicaldev/image/fetch/s--JVsEG_-I--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/326/1%2A7dRGoAeQlsJiTOzRxKFRGg.jpeg)

Link? Is that you?

Isso é a utilização da [**_Abstração_**](https://medium.com/vapordev/shin-programming-tensei-e822b28a47d5) para criar uma carta de **Yu-Gi-Oh**. Nesse caso uma carta de monstro comum. Existem monstros com efeito, monstros de fusão e vários outros. Se você pensar nisso como na herança genética, eu tenho uma carta(célula) que tem diversos atributos(genes) e eu quero criar uma nova carta, só que essa nova carta tem algo de diferente, mas em parte ela é muito parecida com a anterior.

Então eu devo dar ctrl C na anterior e dar ctrl V depois e modificar?  
  
Não. A **herança** é uma das forma de você **reutilizar** código na **POO**, não tem necessidade de você ficar re-escrevendo várias coisas iguais o tempo todo.

Então em uma relação hereditária teríamos algo assim:

```
class  MonsterEffect  < MonsterCard
    attr_accessor  :effect

    def  initialize(name, attribute, race, level, attack, defense, effect)
        super(name, attribute, race, level, attack, defense)
        @effect  = effect
    end
end

```

A carta de monstro normal tem seus atributos como nível, ataque, defesa e etc e a carta de monstro com efeito tem essas mesmas características com uma leve mudança pois ele tem uma nova característica que é um **Effect**. Além de poder usar todos os métodos da **superclasse**, como: atacar um monstro em modo de defesa, atacar diretamente e mudar de posição entre ataque e defesa.

Esse efeito pode ser ativado devido a uma circunstância, como no caso do **Man-Eater Bug**, que após ser virado para cima dá ao jogador a possibilidade de destruir um monstro do oponente.

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--niMrO9kW--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/400/1%2AQqINzgbi5tDrVWjHUM7H3g.jpeg)](https://res.cloudinary.com/practicaldev/image/fetch/s--niMrO9kW--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/400/1%2AQqINzgbi5tDrVWjHUM7H3g.jpeg)

Então temos uma relação entre **Superclasse** e **Subclasse**. Onde a classe **_MonsterEffect_** < **_MonsterCard_** (O sinal de “menor que”, simboliza essa herança de uma classe para a outra).

Uma **subclasse** pode ter outra **subclasse** também, criando uma **árvore** de classes, mas nunca uma **Superclasse** vai herdar genes de suas próprias **Subclasses**. No **_attr_accessor_** temos uma nova propriedade que é a de **_Effect_**, temos um método **_initialize_** que recebe os mesmos argumentos vistos na **Superclasse** com a adição de um novo.

O [**_super_**](https://pt.stackoverflow.com/questions/44345/qual-a-aplicabilidade-pr%C3%A1tica-da-palavra-super-em-ruby) funciona dentro do método inicializador justamente referenciando a **Superclasse**, caso contrário teríamos que escrever tudo igual da mesma forma usando todas as **variáveis de instância** e a **Herança** não faria mais nenhum sentido. Então temos um **initialize** muito menor onde só precisamos referenciar a **superclasse** + um novo atributo **Effect**. Justamente o que precisamos para criar uma carta de monstro com efeito.

Sabendo disso você tem o que precisa para criar as suas árvores de classes e isso é o básico. Mas e se um dia você precisar que a sua classe **EffectMonster** tenha duas **SuperClasses**?

Existe no **Yu-Gi-Oh** um tipo de monstro que tem características de carta mágica. Cartas mágicas em **Yu-Gi-Oh** são usadas devido a seus efeitos que podem atribuir um número maior de ataque ou defesa a um monstro, destruir outras cartas enfim, é uma infinidade de opções.  
  
E nas versões recentes temos a adição de Monstros do tipo **Pendulum**, que podem ser invocados tanto como carta mágica como monstro, o que deixa o jogo mais versátil e com certeza mais complexo.

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--tjgfizen--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/343/1%2AafnziIDomP8bUNGKbdeLig.jpeg)](https://res.cloudinary.com/practicaldev/image/fetch/s--tjgfizen--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/343/1%2AafnziIDomP8bUNGKbdeLig.jpeg)

O Monstro Pendulum além de ter os atrinutos comuns a todos os outros tem dois efeitos, um caso ele seja usado como monstro de efeito e outro logo acima caso ele seja usado como carta mágica.

No **Ruby** não podemos ter **Herança Múltipla** que é dar a uma **Subclasse** **herança** de duas **Superclasses**. Mas se você precisa “tunar” a sua classe com um método diferente, podemos usar **Mixins**.

A partir de um [**_módulo_**](https://ruby-doc.org/core-2.6.3/Module.html), podemos incluir os métodos de dentro desse **módulo** na nossa **Classe**. Geralmente criamos em um arquivo separado, aqui eu tenho um exemplo muito simples.

```
module  Spellcard
    class  Speeleffect
        attr_accessor  :name, :type, :effect

        def  initialize(name, type, effect)
            @name  = name
            @type  = type
            @effect  = effect
        end

        def  effect_spell
            'Target 1 spell/trap card on the field, send to the Graveyard'
        end
    end
end

```

Esse módulo contem uma classe de carta mágica e um metodo de efeito mágico.

No arquivo onde está a nossa classe usamos **require_relative** no topo com o nome do arquivo onde se encontra o **módulo**. O **require_relative** deve ser usado para arquivos que se encontram dentro da mesma **pasta** caso o arquivo esteja em outra pasta você precisará referenciar o arquivo usando **require** apenas e com o caminho específico.

```
require_relative 'Spellcards'

```

Para incluir o método dentro da nossa classe usamos o **include**, que fácil não?

```
class  MonsterPendulum < MonsterEffect
    include SpellCard
    attr_accessor :pendulum

    def  initialize(name, attribute, race, level, attack, defense, effect, pendulum)
        super(name, attribute, race, level, attack, defense, effect)
        @pendulum  = pendulum
    end
end

```

Agora a classe **MonsterPendulum** recebe os atributos de **Effect** da Classe **MonsterEffect** e recebe o metodo **spelleffect** do módulo **SpellCard**.

Agora eu posso criar um **objeto**, de qualquer uma das três classes que criei. Desde a **MonsterCard**, **MonsterEffect** até a **MonsterPendullum**, assim como utilizar todos seus métodos.

```
maneaterbug  =  MonsterPendulum.new('Man-Eater-Bug', 'Earth', 'Insect', 2, 450, 600, 'FLIP', 'Pendulum'
puts  maneaterbug.effect_spell

```

Instancia do Objeto usando metodo de carda mágica

Sei que o **Man-Eater Bug** não é um monstro pendulum, mas **Yu-Gi-Oh** para mim é que nem **Pokémon**, só presta as primeiras gerações hahaha.

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--DrwmbYSR--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/586/1%2AcP38GBBQ8NGB0lqbu3sK3Q.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--DrwmbYSR--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/586/1%2AcP38GBBQ8NGB0lqbu3sK3Q.png)

resultado no console

Fico por aqui, e que o coração das cartas esteja com você.
