
![Cover image for Vila oculta do Polimorfismo](https://res.cloudinary.com/practicaldev/image/fetch/s--nUgrAQ_---/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://thepracticaldev.s3.amazonaws.com/i/13sih6qwxi0qeaaoar6t.png)
# Vila oculta do Polimorfismo

Override, Naruto e Duck Typing

Continuando a série sobre **Programação Orientada a Objetos** hoje o assunto será **Polimorfismo**.


Quando eu conheci Naruto pela primeira vez foi um amigo meu da sétima série eu acho. Ele usava aquele tipo de aparelho móvel, então quando ele falava era meio litro de baba e nem sempre dava pra entender o que ele falava.  
  
“Ou, você já viu Naruto?”  
  
“Que? Maroto?”  
  
“Não, Narutoooo”  
  
Que diabos esse doido ta querendo me dizer?

Na época eu tinha um computador bem ruim e uma internet pior ainda. Então eu fui até a casa dele pra ver o tal do Naruto. Ele me mostrou uma luta do [Rock Lee VS Gaara](https://www.youtube.com/watch?v=VgDgWzBL7s4) do Naruto clássico. Eu assisti, não entendi muita coisa, mas a animação da luta era algo bem diferente eu já gostei muito de Dragon Ball, mas aquele migué de que não mostra os personagens lutando porque eles estão na velocidade da luz…ai não né kkk, essa foi mesmo uma das lutas mais incríveis de todo o anime.

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--j5CXxems--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/696/1%2AAsscsA08YNe6qTppq7dNbA.jpeg)](https://res.cloudinary.com/practicaldev/image/fetch/s--j5CXxems--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/696/1%2AAsscsA08YNe6qTppq7dNbA.jpeg)

A partir daí eu comecei a absorver Naruto de diversas fontes, filmes, anime, games, mangá. E para quem conhecia um pouco de cultura japonesa através de outras histórias era algo bem interessante ver isso impregnado no anime.

O primeiro nome que me chamou atenção foi o vilão Orochimaru eu já havia escutado esse nome algumas vezes como Orochi. Quem jogava The King of Fighters 97 sabe que esse é o nome do chefe final, em Shin Megami Tensei tem abordagem a Orochi também. Então resolvi dar uma pesquisada a respeito e vi que a referência era a Yamata no Orochi.

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--9oxvHdMJ--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/600/1%2A6CB2xIi8LYJ9dwlB7Et8xw.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--9oxvHdMJ--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/600/1%2A6CB2xIi8LYJ9dwlB7Et8xw.png)

[Yamata no Orochi](https://pt.wikipedia.org/wiki/Yamata_no_Orochi) é uma criatura da [mitologia japonesa](https://pt.wikipedia.org/wiki/Mitologia_japonesa). Possuía oito cabeças, oito caudas e olhos vermelhos. Tinha musgo e árvores em suas costas. Era tão grande que ocupava oito vales e oito picos. Anualmente, Orochi exigia o sacrifício de oito virgens. Um dia, uma das oito virgens exigidas era a amada de [Susanoo](https://pt.wikipedia.org/wiki/Susanoo). Susanoo ficou revoltado com isso e foi matar o temível dragão.

Então surge o nome [Susanoo](https://pt.wikipedia.org/wiki/Susanoo) que também não é desconhecido aos fãs de Naruto. A forma como Naruto faz referência às mitologias japonesas é bastante interessante pois usa não somente nomes de personagens como técnicas. Eu mesmo não conhecia nada sobre até então, e não havia visto nada assim em nenhum anime.

Susano no anime é o nome de uma das técnicas do Clã Uchiha na mitologia Susano é o deus dos mares e das tormentas e responsável por matar Orochi.

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--4YbNdE0g--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/807/1%2A5lc039y2LmSKia90SiVkkQ.jpeg)](https://res.cloudinary.com/practicaldev/image/fetch/s--4YbNdE0g--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/807/1%2A5lc039y2LmSKia90SiVkkQ.jpeg)

Na imagem Susano usando a Espada de Kusanagi que também é referencia no anime (espada do Sasuke) e ela existe de verdade! É um dos três tesouros do império japonês ([Espada de Kusanagi](https://pt.wikipedia.org/wiki/Kusanagi_(espada)), [Yata no Kagami](https://pt.wikipedia.org/wiki/Yata_no_Kagami) e [Yasakani no magatama](https://pt.wikipedia.org/wiki/Magatama)) que se encontram em diferentes templos xintoístas do Japão.

Susano é Irmão de [Amaterasu](https://pt.wikipedia.org/wiki/Amaterasu)(Deusa do Sol) e [Tsukuyomi](https://pt.wikipedia.org/wiki/Tsukuyomi)(Deus da lua) outras duas referências encontradas em Naruto.

O início da mitologia japonesa que começa com os pais de Susanoo, [Izanagi](https://pt.wikipedia.org/wiki/Izanagi) e [Izanami](https://pt.wikipedia.org/wiki/Izanami).

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--zIvg7EQq--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/650/1%2A39d4relDMC-jBvh_s9JSCA.jpeg)](https://res.cloudinary.com/practicaldev/image/fetch/s--zIvg7EQq--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/650/1%2A39d4relDMC-jBvh_s9JSCA.jpeg)

Izanagi e Izanami foram criação dos ‘Deuses Superiores’ e se casaram em [Onogoro](https://en.wikipedia.org/wiki/Onogoro_Island) _a_ primeira terra firme. Os filhos de Izanagi e Izanami geraram os deuses do vento, árvores, montanhas entre outras divindades, além do arquipélago japonês.

Quando Izanami deu à luz ao Deus do Fogo [Kagutsuchi](https://en.wikipedia.org/wiki/Kagu-tsuchi) ela morreu queimada. Izanagi decide ir ao submundo mas quando chega Izanami a essa altura é um cadáver putrefato repleto de vermes, perseguido por Izanami e outros demônios Izanagi consegue fugir do submundo. Quando decide se lavar para se livrar das impurezas do submundo é quando são gerados Amaterasu, Tsukuyomi e Susanoo.

Além da história que a maioria já conhece sobre um garoto órfão e menosprezado Naruto carrega a cultura japonesa para as próximas gerações.

Agora falando mais de código.

O polimorfismo é simplesmente você usar métodos de modos diferentes, assim você pode criar especializações para as suas subclasses quando o método original não se encaixa tão bem assim. No Ruby é mais fácil ainda, porque você pode sobrescrever o método original criando um segundo método com o mesmo nome do original essa prática é chamada de **Override**.

```
class  Genin
    #sabe nada
end

```

Agora eu vou criar uma classe chamada **SanninLendario** ela vai ter dois métodos aninhados.  
  
1 — Método **ensina** e ele usa como parâmetro uma variável chamada **jutsu**.  
  
2 — Dentro do método eu crio outro método **rasengan** que recebe o parâmetro **Jutsu** do método anterior.

```
class  SanninLendario
    def  ensina(jutsu)
        def  jutsu.rasengan
            'Raseeeengan!'
        end
    end
end

```

Agora eu vou instanciar **Genin** na variável **naruto.  
  
SanninLendario** na variável **jirayasensei.**

Chamo o método **ensina** da classe do **SanninLendario** e o objeto que eu quero que aprenda (**naruto**)  
  
Agora eu mando o objeto da classe **Genin(naruto)** que não tinha nenhum método para usar o método*_rasengan._*

```
naruto = Genin.new
jirayasensei = SanninLendario.new
jirayasensei.ensina naruto
p naruto.rasengan

```

Resultado no console:

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--Tv-Kh8qW--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/543/1%2Anoof6WHSxMfxNc6fz9BmXA.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--Tv-Kh8qW--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/543/1%2Anoof6WHSxMfxNc6fz9BmXA.png)

OBS. O nome do arquivo aparece Speelcards porque eu usei o mesmo arquivo do artigo anterior, eu sei sou muito preguiçoso.

Isso que usei foi uma prática de **Metaprogramação** onde podemos deixar o nosso código muito mais dinâmico. Com **Metaprogramação** podemos modificar muita coisa inclusive em tempo de execução.  
  
A técnica de **Override** vem agora, queria só brincar um pouco antes, desculpa kkkkk.

No mesmo arquivo eu vou criar uma classe chamada **Sennin** e vou dar pra ela um método com o mesmo nome de um dos métodos do **SanninLendário** o **rasengan** mas o conteúdo dela não é exatamente igual ao método do **SanninLendario**.

```
class Sennin
    def rasengan
        'Oodama Raseeeengan!'
    end
end

```

Isso é o **Override** ou sobrescrever no bom português. Em seguida eu vou criar uma nova instância de **Sennin** com o nome de **narutoshippuden** e vou pedir pro **narutoshippuden** usar o método **rasengan.**

```
narutoshippuden = Sennin.new
p narutoshippuden.rasengan

```

Resultado:

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--vGMrfk2W--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/552/1%2ATjyZuqtLxPNOn5byzuws6A.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--vGMrfk2W--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/552/1%2ATjyZuqtLxPNOn5byzuws6A.png)

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--2JpH-G6H--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/428/1%2A6fB1onLq93Cml3BETnOk9g.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--2JpH-G6H--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/428/1%2A6fB1onLq93Cml3BETnOk9g.png)

Esta é apenas uma das forma de **Polimorfismo** no **Ruby**. Uma outra bastante conhecida em **Ruby** é o **Duck Typing**.

Vou criar uma classe chamada **Zabuza** com o método **jutsu.**

```
class Zabuza
    def jutsu
        'Estilo Água: Jutsu Dragão de água'
    end
end

```

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--bkppwiYM--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/486/1%2AaNGOGp9dPVxFNi31mlPh6g.jpeg)](https://res.cloudinary.com/practicaldev/image/fetch/s--bkppwiYM--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/486/1%2AaNGOGp9dPVxFNi31mlPh6g.jpeg)

Vou criar mais uma classe **Haku** com um método chamado **jutsu** também.

```
class Haku
    def jutsu
        'Jutsu Secreto: Espelhos de Cristais de Gelo'
    end
end

```

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--XxdGLBmq--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/710/1%2ANzOsn0gnYdIJB32WBnCnTA.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--XxdGLBmq--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/710/1%2ANzOsn0gnYdIJB32WBnCnTA.png)

Agora vou criar uma terceira classe chamada **Kakashi** com um método chamado **sharingan** que recebe um parâmetro chamado **copia, copia** chama **jutsu**(o mesmo método das outras duas classes, Zabuza e Haku).

```
class Kakashi
    def sharingan(copia)
        copia.jutsu
    end
end

```

Instancio as três classes e agora vou chamar o método **jutsu** no objeto **kakashi** e passo como parâmetro qual **objeto** eu quero “copiar” o método.

```
zabuza = Zabuza.new
haku = Haku.new
kakashi = Kakashi.new

p kakashi.sharingan(zabuza)
p kakashi.sharingan(haku)

```

Resultado:

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--h0soerat--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/540/1%2A7tr21Vqh82_umGI2Hyol-Q.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--h0soerat--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://miro.medium.com/max/540/1%2A7tr21Vqh82_umGI2Hyol-Q.png)

Vou deixar um adendo aqui, o jutsu espelhos de cristal é um jutsu kekkei genkai (em naruto jutsus kekkei genkai são genéticos então não podem ser copiados pelo Sharingan), mas a fim do meu próprio entretenimento caguei pra isso.

O próximo artigo será sobre Encapsulamento! Muito Obrigado a você que chegou até aqui.
