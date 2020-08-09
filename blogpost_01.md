# **Refactoring: improving the mind of legacy Developers**

Complete o meme: O dev precisa…

![Image for post](https://miro.medium.com/max/1080/1*clINqpH7dRYWojyUyGkb1g.png)

Tenho visto uma galera da comunidade querendo ditar como e porque tal pessoa tem que fazer conteúdo, em alguns casos desqualificando a pessoa que faz um conteúdo considerado avançado porque supostamente essa pessoa não domina isso.

> “Bro, seu código não é escalável! “ — disse, Engenheiro formado, melhor do que você

Então quer dizer que se eu não sou o mestre de todas as “melhores práticas” qualquer conteúdo que eu replique durante meu estudo sobre boas práticas é invalidado?



![Image for post](https://miro.medium.com/max/900/1*V4ufV_5vxpsTgbsVWqwBtg.png)

Qualquer pessoa iniciante deve contribuir com a comunidade com o conteúdo que ela achar melhor e você ajuda muito mais a comunidade apontando para ela detalhes de melhoria no conteúdo do que invalidá-las publicamente.

> “Você precisa escrever código em inglês, esse código misturado parece uma favela “ — disse, Purista idiomático

Então de iniciante para iniciante eu vou tocar em alguns pontos aqui sobre programação, esse não será um tutorial, mas vai ter código, porém você não precisa se preocupar com ele.


![Image for post](https://miro.medium.com/max/1300/1*5By1KxTszKqi-MWRNYCKBQ.png)

> “O cara deixou um código legado macarrônico lá onde trabalho, agora tá aí palestrando sobre boas práticas” — disse, O cara que estuda as boas práticas mas não compartilha com ninguém

O interessante sobre a programação é que com o básico você já consegue exercitar o suficiente para construir **algoritmos**. Talvez você não precise ver isso agora, caso você seja muito iniciante, mas em um caminho comum estudando programação você irá passar mais cedo ou mais tarde por **algoritmos** e estruturas de dados.

Um exemplo é o _Bublesort_, esse está em _Python_

~~~python
# Python program for implementation of Bubble Sort 

def bubbleSort(arr): 
	n = len(arr) 
	for i in range(n): 
	
		for j in range(0, n-i-1): 
		
			if arr[j] > arr[j+1] : 
				arr[j], arr[j+1] = arr[j+1], arr[j] 
				
arr = [64, 34, 25, 12, 22, 11, 90] 

bubbleSort(arr) 

~~~

Na construção desse **algoritmo** e na maioria dos demais você vai precisar de conhecimentos introdutórios como:

_- tipos de dados_

_- dados compostos_

_- operadores relacionais_

_- operadores lógicos_

_- funções_

Talvez a única coisa que pra um iniciante não seja tão óbvio são as funções len e range, mas com uma busca simples no Google você descobre o que elas fazem e não é nada complicado.

Isso é pra se ter uma ideia de que mesmo nas partes mais importantes da programação o que vai te levar longe é o conhecimento aprofundado em fundamentos. Então talvez seja o momento de deixar aquela biblioteca complicada de lado e focar no arroz com feijão.

Como você pode exercitar com os fundamentos? Eu estava com um pouco de dificuldade um tempo atrás em resolver problemas com **algoritmos** e claro que era falta de prática, mas não escrevendo código mas sim pensando sobre. Hoje em dia com muito pouco uso da lógica você consegue fazer um **CRUD** básico, graças ao nível de abstração que os frameworks conseguiram chegar.

É muito possível que você escreva **CRUD**’s e **API**’s o dia todo e não precise usar lógica pra isso. Você escreveu dezenas de linhas e mesmo assim não precisou pensar logicamente na construção de um **algoritmo** porque no final o seu **Model** não faz nenhuma operação com os dados.

Mas nem só de **CRUD** vive o desenvolvedor, e possivelmente quando você for fazer uma entrevista pedirão para que você faça operações lógicas com o seu modelo de **CRUD** e as vezes é algo bem simples, mas que talvez por não estar com a lógica em dia você tenha certa dificuldade. E como eu deveria resolver esse problema?

Acho que podemos evoluir em níveis de abstração lógica a partir de um problema, e podemos resolvê-lo de diferentes maneiras, e também com níveis de diferentes de complexidade.

Então eu pensei em um problema simples e tentei resolvê-lo da maneira que viesse na cabeça. Você pode começar até mais simples que isso.

// Um algoritmo que faz a contagem de quantas vezes um cliente alugou _carros_ na sua locadora

// Que aplica um _desconto_ de 30% no valor do aluguel a cada 10 locações

Da primeira vez que tentei resolver cheguei a algo como isso:
~~~Go
for i := 0; i <= 10; i++ {
	if i == 10 {
	desconto := (carro * 35) / 100
	valor := carro - desconto
	fmt.Println(valor)
	}
}
~~~

Dessa vez o código é em _Golang_, aqui eu uso um _for_ com um _if_ aninhado, esse combo resolve uma porrada de problemas, mas não esse.

Aqui o _for_ faz um _loop_ em dez itens

_for i := 0; i <= 10; i++_

e quando o item for 10 ele aplica um _desconto_ de 35% ao item.

_if i == 10 {_

_desconto := (carro * 35) / 100_

_valor := carro — desconto_

Fique sabendo que até mesmo pra saber como fazer calculo de _desconto_ eu tive que buscar no Google eu deveria me envergonhar de não ter esse conhecimento matemático fundamental? Talvez, mas eu não ligo e você também não deveria, não tenha medo de buscar no Google.

Aliás o cálculo é o valor que você quer como porcentagem vezes o valor da compra dividido por 100

_P X V / 100_

Fica ai de sugestão pro próximo filho da Grimes com o Elon Musk

O Problema desse código é que ele só aplica o _desconto_ uma vez, e se eu fizer um _loop_ com 20 itens ele não vai aplicar um segundo _desconto_ o que me deixa longe do objetivo inicial.

_for i := 0; i <= 20; i++ = FAIL_

Se você reparar uma parte do problema foi resolvida, que é a de aplicar _descontos_, ele não resolve o problema como um todo, mas já possui uma parte bem encaminhada. Às vezes problemas mesmo que pareçam ser pequenos ainda podem ser divididos em partes menores.

// um programa que faz a contagem de quantas vezes um cliente alugou _carros_ na sua locadora

// e aplica um _desconto_ de 30% no valor do aluguel a cada 10 locações

O meu problema era encontrar as dezenas de um número para que eu pudesse passar valores maiores que 10 e ter os _descontos_ de acordo com as dezenas desse número.
~~~go
func aluguelv2(carro int, numero int) {
	unidade := numero % 10
	numero = (numero - unidade) / 10
	dezena := numero % 10

	for i := 0; i < dezena; i++ {
	desconto := (carro * 35) / 100
	valor := carro - desconto
	fmt.Println(valor)
	}
}
~~~

Aqui apesar de ter mais código o **algoritmo** não ficou tão complexo, coloquei essa lógica dentro de uma função, do jeito que o diabo gosta.

E essa recebe dois parâmetros que são _carro_ e _número_, sendo _carro_ o valor do aluguel em si e _número_ a quantidade de vezes alugadas. Os nomes dos parâmetros não estão tão bons assim, mas esse é o jeito das ruas, nome de variável a gente muda depois.

Agora temos duas lógicas dentro da mesma função a dos números decimais e a do _desconto_, estamos aplicando o _desconto_ no _número_ de dezenas encontradas na lógica anterior ao invés de escrever o _número_ direto no _loop_ for.

Esse **algoritmo** funciona, ele recebe o _número_ de vezes alugadas e aplica um desconto a cada dez vezes no valor do aluguel do _carro_. Problema resolvido!

Como existem mais formas ainda de melhorar um **algoritmo** chegamos a uma terceira forma.
~~~go
func  aluguelv3(meses []int, carro int)  {

	for  i  :=  0; i <  len(meses); i++  {
	unidade  := meses[i]  %  10
	meses[i]  =  (meses[i]  - unidade)  /  10
	dezena  := meses[i]  %  10
	fmt.Println(dezena)

		for  i  :=  0; i < dezena; i++  {
		desconto  :=  (carro *  35)  /  100
		valor  := carro - desconto
		fmt.Println(valor)
		}
	}
}

~~~

No exemplo anterior eu só poderia aplicar o _desconto_ a um valor mas não faria sentido eu dizer que um cliente alugou um _carro_ 90 dias de uma vez só, então resolvi transformar os dados de entrada de aluguel em meses que é um slice(estrutura de dados composta) de números _inteiros_, onde cada índice representa um mẽs e o valor do índice o número de vezes que o cliente alugou o _carro_.

_meses := []int{20,30,20,12}_

Isso seriam quatro meses onde o cliente alugou o mesmo carro 20 vezes no primeiro mẽs, 30 no segundo e assim por diante. Então de acordo com as dezenas deve-se aplicar _desconto_ 8 vezes no período de 4 meses de um total de 82 locações.

Eu poderia ter abordado de um forma diferente, mas queria usar uma estrutura de dados composta nesse caso. Repare também que existe um padrão onde eu poderia dividir o total de locações 82 por 10(dezena) para chegar ao mesmo resultado mas a ideia é que o **algoritmo** agisse como o próprio cliente e que o _desconto_ fosse aplicado na exata décima locação seguida.

O Parâmetro de _carro_ continua sendo um inteiro.

A lógica de encontrar os decimais de um _número_ agora está dentro de um range em que essa lógica é repetida para cada índice do slice.
~~~go
package main

import  "fmt"

type  carro  struct  {
	nome string
	preço int
}

func  main()  {

carro1  := carro{
nome:  "Golf",
preço:  500,
}

meses  :=  []int{10,  30,  32,  20}

aluguelv3(meses, carro1.preço)
}
~~~

Esses são os dados de entrada e a chamada da função, no caso do _carro_ usei um struct e passei o atributo preço como argumento na função.

Esse código poderia ser melhorado, mostrando o valor total de todos os aluguéis, o valor total com os descontos aplicados, uma variação de preços com novos _carros_ sendo utilizados.

Mas o objetivo principal definido foi cumprido, muitas vezes a gente pensa em começar projetos extremamente ambiciosos e se assusta com o quanto eles podem ser difíceis, mas grandes projetos são feitos de pequenas incrementações.

Nossos programas dificilmente serão performáticos, escaláveis logo de cara. Código foi feito pra ser modificado, ninguém vai escrever a solução final logo de cara, códigos começam pequenos e sim cheios de más práticas e é por isso que existe refatoração, para melhorar o design do código legado, quem diria?

Acho que o exercício aqui é que você comece a pensar em problemas e solucionar os próprios problemas, começa pequeno e vai pensando em coisas mais complexas tente se manter nos fundamentos até que se sinta confortável em ler o **algoritmo** e entender a lógica por trás dele. Mesmo que não tenha entendido o código que você viu aqui o importante é entender que o verdadeiro exercício não tá no código e sim na sua cabeça.

Tente resolver um problema sem escrever nada, só imaginando e você vai perceber que programação não tem a ver apenas com a linguagem.

Inclusive o código que você viu aqui é bem feio e pode ser melhorado de muitas formas, fique a vontade para fazer a sua própria versão. Cada desenvolvedor está no seu próprio tempo desenvolvendo com as práticas que ele aprendeu e um dia quem sabe ele fará um código “elegante” ou escalável do qual ele mesmo se propôs a fazer sem copiar de um tutorial de boas práticas, quem sabe ele mesmo desenvolva novas boas práticas.

Por enquanto é isso, caso alguém encontre algo de errado e queira melhorar a qualidade de conteúdos feitos pela comunidade para a comunidade é só chamar. Caso contrário é melhor ficarem calados, **devs** iniciantes já tem muitos problemas com síndrome do impostor e todas as outras dificuldades que iniciantes da área tem carregado, não estamos interessados no seu ego.
