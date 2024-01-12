# Fundamentos básicos da programação

## Variavéis:

As variáveis são usadas com nomes simbólicos para valores em sua aplicação.
São chamados de identificadores as variaveis.
O identificador Js deve começar com uma letra, underline ou cifrão.

O uso de "var" é menos comum atualmente, uma vez que apresenta escopo global ou de função, podendo resultar em problemas de redeclaração inadvertida. Por exemplo, se tivermos duas funções distintas que declaram variáveis com o mesmo nome, ocorrerá uma redefinição global, potencialmente gerando bugs difíceis de diagnosticar. Portanto, é aconselhável evitar "var" em favor de declarações mais modernas.

A declaração "let" é preferível quando se deseja evitar problemas de redeclaração e limitar o escopo da variável ao bloco em que ela é definida. Isso traz maior segurança e clareza ao código. Por exemplo, se tivermos um loop for e declararmos uma variável com "let" dentro desse loop, ela estará acessível apenas dentro desse bloco específico, prevenindo interferências externas e facilitando a manutenção do código.

"const" é ideal para variáveis que não devem ser reatribuídas. Se tivermos uma constante como o valor de PI em uma aplicação, declará-la como "const" garante que seu valor não seja alterado inadvertidamente em outros pontos do código. No caso de objetos, podemos utilizar "const" para garantir que a referência ao objeto permaneça constante, embora suas propriedades possam ser modificadas. Isso é útil em situações em que a estrutura do objeto deve permanecer imutável, mas seus valores podem ser atualizados conforme necessário. Em resumo, escolher entre "let", "const" e "var" depende das necessidades específicas de escopo, reatribuição e imutabilidade em um determinado trecho de código.

## Tipos de dados em programação

Integer (Inteiros)
Integers são números inteiros positivos ou negativos, eles podem ser especificados em diferentes tamanhos, dependendo da quantidade de memória necessária para armazená-los. São usados para contar quantidades, como o número de itens em um estoque, quantidade de votos em uma eleição, número de alunos em uma classe etc.

Float (Ponto Flutuante)
Floats são números com casas decimais e são usados para representar números reais, como preços de produtos, orçamentos, altura, temperatura etc.

Character (Caracteres)
Characters são usados para representar caracteres alfabéticos ou símbolos especiais, ou seja, qualquer coisa que você consegue digitar em um teclado. Eles podem ser usados para armazenar nomes de usuário, endereços de e-mail, senhas, sinais de pontuação etc.

String (Cadeia de caracteres)
Strings são usadas para armazenar textos mais longos, e cada caractere dentro de uma string é armazenado como um character separado na memória. Alguns exemplos de strings são mensagens de texto em aplicativos de bate-papo, posts em redes sociais, títulos de artigos etc.

Boolean (Booleanos)
Booleans podem ter apenas um de dois valores: true (verdadeiro) ou false (falso). Eles são usados para representar condições como se um usuário está conectado ou não, se um valor é maior ou menor que outro valor etc.

Arrays (Séries)
Arrays são usados para armazenar uma coleção de valores do mesmo tipo. Eles podem ser unidimensionais (uma única linha de valores) ou multidimensionais (matrizes de valores organizados em várias dimensões). São úteis, por exemplo, para armazenar uma lista de produtos em um carrinho de compras, uma lista de alunos em uma turma ou uma matriz de notas de um aluno em várias matérias.

O tipo de dado "number" em JavaScript é utilizado para representar valores numéricos, incluindo inteiros e números de ponto flutuante. Esses números são utilizados em cálculos matemáticos, atribuição de valores, e diversas operações aritméticas.

O tipo "undefined" é atribuído a variáveis que foram declaradas, mas não receberam nenhum valor. É comumente utilizado para indicar a ausência de valor em uma variável ou para representar o resultado de uma expressão que não retorna nenhum valor.

O valor "null" é utilizado para indicar a ausência intencional de um valor em uma variável ou objeto. É frequentemente utilizado para reiniciar o valor de uma variável ou indicar que uma propriedade de um objeto não possui valor.

O tipo "object" é utilizado para representar estruturas de dados complexas e é a base para a construção de objetos em JavaScript. Objetos podem conter propriedades e métodos, proporcionando uma forma flexível de organizar e manipular dados.

"Symbol" é um tipo de dado introduzido no ECMAScript 6, usado para criar identificadores únicos e evitar colisões de nome em propriedades de objetos. Cada símbolo é único, tornando-os úteis em cenários nos quais a identificação exclusiva é crucial.

O tipo "bigint" foi introduzido no ECMAScript 2020 e é utilizado para representar números inteiros de tamanho arbitrariamente grande. Ele é útil quando se lida com números que ultrapassam o limite do tipo "number" em JavaScript, oferecendo uma precisão maior em cálculos envolvendo inteiros extensos.

## Operadores

Operadores Aritméticos ( +, -, *, /, **, % )
Os operadores aritméticos executam operações matemáticas, como adição e subtração com operandos. Há dois tipos de operadores matemáticos: unário e binário. Os operadores unários executam uma ação com um único operando. Operadores binários executam ações com dois operandos.

Operadores Aritméticos Unários
Operadores unários são operadores aritméticos que desempenham uma ação em um único operando. A linguagem de script reconhece o negativo do operador unário (-).
O operador unário negativo inverte o sinal de uma expressão de positivo para negativo ou vice-versa. O efeito geral é de multiplicar o número por -1. 

Exemplo:

a = -10;

Os operadores Prefix incrementam ou decrementam a variável antes de remover a referência ao objeto, enquanto que os operadores Postfix incrementam ou decrementam a variável após fazer referência a ela. Exemplo:

A=1; 
B = a++; // b será igual a 1, a será igual a 2; 
A = 1; 
B = ++a; // b será igual a 2, a será igual a 2; 
A= 1; 
B = a--; // b será igual a 1, a será igual a 0;

Operador de Designação (=)
Utilize o operador de designação (=) para copiar uma constante, um literal, um resultado de expressão de variável ou um resultado de função para uma variável. A linguagem de script não suporta várias designações em uma única instrução (como a=b=c=0). Os comprimentos das cadeias são definidos com base no tamanho da cadeia designada para a variável e pode mudar dinamicamente no tempo de execução.

Operadores Lógicos (E, OU)
Os operadores lógicos permitem a combinação de mais de um teste relacional em uma comparação. Os operadores lógicos retornam um valor TRUE (1) ou FALSE (0). Os operadores lógicos têm precedência inferior aos operadores aritméticos.
Relacionais

Operadores Significados:

==	Igualdade
!=	Desigualdade
< <=  Menor / Menor ou igual
> >=  Maior / Maior ou igual

Lógicos

Operadores	Significado
!	Negação (NOT)
&&	E (AND)
||	OU (OR)

Uma string é uma seqüência de caracteres delimitada por aspas (“) ou plics(‘). Para juntar duas strings numa única, existe o operador de concatenação representado pelo símbolo +.

Por exemplo:

nome = "Ricardo"; sobrenome = "Silva";
nomeCompleto= nome + " " + sobrenome; // nomeCompleto recebe "Ricardo Silva"

Operadores podem ser utilizados em conjunto com variáveis e valores constantes no que chamamos de expressões. Da mesma forma que com expressões matemáticas, podemos usar perentesis para definir a ordem de precedência em que as operações devem ser realizadas.

Por exemplo:

var radianos = graus * 3.1416 / 180.0;

var media = (a + b + c + d) / 4;

## Switch

Switch:
O bloco "switch" em JavaScript é utilizado para realizar múltiplas verificações em uma expressão. Ele permite comparar o valor de uma variável com vários casos possíveis e executar o código associado ao caso correspondente. Isso é especialmente útil quando há várias condições a serem verificadas.

Exemplo em JavaScript:

```javascript
let day = 3;
let dayName;

switch (day) {
  case 1:
    dayName = "Sunday";
    break;
  case 2:
    dayName = "Monday";
    break;
  case 3:
    dayName = "Tuesday";
    break;
  // ... outros casos ...
  default:
    dayName = "Unknown day";
}
console.log(dayName);
```

If:
A estrutura "if" é fundamental para controlar o fluxo do programa com base em condições. Se a condição especificada for verdadeira, o bloco de código dentro do "if" é executado. Pode ser acompanhado por "else" para tratar o caso em que a condição é falsa.

Exemplo em JavaScript:

```javascript
let temperature = 25;
if (temperature > 30) {
  console.log("It's a hot day!");
} else if (temperature > 20) {
  console.log("It's a warm day.");
} else {
  console.log("It's a cold day.");
}
```
For:
O loop "for" é utilizado para iterar sobre uma sequência de valores ou realizar um número específico de iterações. É composto por uma inicialização, condição de continuação e expressões de atualização.

Exemplo em JavaScript:

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

While:
O loop "while" executa um bloco de código enquanto uma condição específica é verdadeira. É útil quando o número de iterações não é conhecido antecipadamente.

Exemplo em JavaScript:

```javascript
Copy code
let count = 0;

while (count < 5) {
  console.log(count);
  count++;
}
Do While:
O loop "do-while" é semelhante ao "while", mas garante que o bloco de código seja executado pelo menos uma vez, mesmo que a condição seja falsa.
```

Exemplo em JavaScript:

```javascript
Copy code
let x = 1;

do {
  console.log(x);
  x++;
} while (x < 5);
Cada estrutura desempenha um papel crucial no controle do fluxo de um programa JavaScript, permitindo que os desenvolvedores criem lógica condicional e iterações eficientes.
```

## Parâmetros de função

Em JavaScript, parâmetros padrões de funções são undefined. No entanto, em algumas situações pode ser útil definir um valor padrão diferente. Isto é onde os parâmetros padrão podem ajudar.

Padrão

Com parâmetros padrão, a verificação no corpo da função não é mais necessária. Agora você pode simplesmente colocar 1 como valor padrão para b no campo de declaração de parâmetros:

```javascript
function multiplicar(a, b = 1) {
return a * b;
}

multiplicar(5); // 5
```

## Argumento

Um argumento é um valor (primitivo ou um objeto) passado como um input (entrada) para uma função.

## Diferença entre parâmetro e argumento 

Parâmetro é a variável que irá receber um valor em uma função (ou método) enquanto que um argumento é o valor (que pode originar de uma variável ou expressão) que você passa para a função (ou método).

Você não passa parâmetros, você passa argumentos. Você recebe argumentos também, mas recebe em parâmetros. Você parametriza sua função com informações que virão posteriormente. Você argumenta com o que deseja executar uma função devidamente parametrizada.

Pode haver menos os mais argumentos para cada parâmetro já que existem parâmetros que são opcionais e outros que podem ser listas variáveis de dados. Portanto não há uma relação de um para um e a distinção entre eles é importante.

![Alt text](image.png)

## Retorno de função

Valores de retorno são exatamente como soam — valores retornados pela função quando são concluídos.

## Usando valores de retorno em suas próprias funções

Para retornar um valor de uma função personalizada, você precisa usar ... aguarde por isso ... a palavra-chave return. 

## Invocando funções

Provavelmente você já tem conhecimento sobre iso agora, mas... para realmente usar uma função depois dela ter sido definida, você tem que rodá-la — ou invocá-la. Isso é feito ao se incluir o nome da função em algum lugar do código, seguido por parênteses.

```javascript
function myFunction() {
  alert("hello");
}

myFunction();
// Chama a função um vez
```

## Funções anônimas

Você viu funções definidas e invocadas de maneiras ligeiramente diferentes. Até agora nós só criamos funções como esta:

```javascript
function myFunction() {
  alert("hello");
}
```

Mas você também pode criar funções que não tem nome:

```javascript
function() {
  alert('hello');
}
```
## Arrow functions 

São uma forma concisa de escrever funções em JavaScript introduzidas no ECMAScript 6 (ES6). Elas oferecem uma sintaxe mais curta e uma vinculação léxica do this, o que significa que o valor de this é capturado do contexto circundante no momento em que a função é definida, não no momento em que é executada.

Exemplo de arrow function:

```javascript
Copy code
// Sintaxe tradicional de função
function soma(a, b) {
  return a + b;
}

// Arrow function equivalente
const somaArrow = (a, b) => a + b;
```

Neste exemplo, somaArrow é uma arrow function que realiza a mesma operação de adição que a função soma, mas de forma mais concisa. Arrow functions são frequentemente utilizadas em situações onde a brevidade e a captura do contexto this são vantagens desejáveis.

## Objetos e Arrays

O array é um objeto no JavaScript, ele nos auxilia pois podemos utilizar uma única variável para armazenar uma lista de diferentes elementos.

## O que são arrays em JavaScript?

O array é um objeto no JavaScript, ele nos auxilia pois podemos utilizar uma única variável para armazenar uma lista de diferentes elementos.

Por exemplo, imagine que seja necessário armazenar os nomes de todos os alunos de uma sala de aula, criar uma variável para cada aluno seria, no mínimo, trabalhoso, dependendo do tamanho dos dados eu diria inviável.

Nesta ideia podemos então criar a variável alunos e com isso armazenar o nome de todos os alunos.

Como declarar um array no JavaScript?
Para utilizar os Arrays precisamos declarar uma variável (você pode acessar o nosso artigo conhecendo variáveis e constantes no JavaScript para saber como declarar variáveis).

E ao atribuir um valor, vamos colocar entre [] e separar cada um por ,. Por exemplo:

```javascript
let alunos = ['Wesley', 'Marina', 'Bruno', 'Paula'];
var series = ['Game of Thrones', 'Friends', 'Vikings'];
```

## Como utilizar objetos no JavaScript

Nós utilizamos objetos para agrupar valores que possuem propriedades e funções, podemos por exemplo fazer uma analogia aos objetos do mundo real. Um carro que possui cor e marca, ele também realiza ações como acelerar e frear.

Para declarar um objeto a sintaxe é bem parecida a que utilizamos para declarar arrays, porém trocamos os [] por {}. Onda as chaves, valores e funções são declaradas entre {}, conforme abaixo:

```javascript
let carro = {
		modelo: 'gol',
		cor: 'vermelho',
		acelerar(){
			console.log('Acelerando...');
		},
		frear(){
			console.log('Freando');
		},
};
```

Neste caso declaramos o objeto literal carro, que possui duas propriedades, modelo e cor, que podem ser chamadas de chaves. Declaramos também duas funções, acelerar e frear, que podem ser chamadas de métodos. Vale ressaltar que nós podemos declarar de outras formas as funções: acelerar: function () {}ou utilizando uma arrow function, acelerar: () => {}.

Após declarar nosso objeto, podemos executar um cosole.log(carro); para visualizar como é apresentado:

![Alt text](image-1.png)

## Como acessar as propriedades ou funções de um Objeto?

Para acessar uma propriedade ou uma função basta utilizarmos o nome do objeto seguido da propriedade/função separada por ponto. Por exemplo:
```javascript
console.log(carro.modelo);
console.log(carro.acelerar);
carro.acelerar();
```

Utilizamos a função console.log, para exibir os dados acessados no console, importante lembrar que para executar a função acelerar não podemos esquecer dos ().

## O que são Métodos em JavaScript?

Os métodos são blocos de código em JavaScript que executam ações e funções específicas de um objeto. Para essa aula, é importante revisar os conceitos aprendidos sobre objetos e funções.

```javascript
const zeus = {
    nome: 'Zeus',
    raca: 'Vira-Lata',
    idade: 7,
}
```
Quando criamos um objeto, como o nosso “cachorro” neste caso, definimos não apenas suas características, mas também suas capacidades e as ações que ele pode executar.

```javascript
const zeus = {
    nome: 'Zeus',
    raca: 'Vira-Lata',
    idade: 7,
    latir: function (){
        console.log('Au au au au!');
    },
}
```

Podemos criar uma função anônima dentro do nosso objeto porque ela está associada a um campo específico dentro dele. No nosso exemplo, a função está associada ao campo latir do objeto zeus.

Isso significa que se executarmos o código:

```javascript
const zeus = {
    nome: 'Zeus',
    raca: 'Vira-Lata',
    idade: 7,
    latir: function (){
        console.log('Au au au au!');
    },
}
zeus.latir();
```

 ![Alt text](image-2.png)

Nesse caso, nossa função foi executada a partir do objeto zeus. Quando uma função está contida dentro de um objeto, associada a um campo dele, chamamos de método. Ou seja, latir() será um método do objeto zeus.

Portanto, a sintaxe seria: declaramos primeiro o objeto, seguido de ponto (.) e então o nome do método.

## map() - Executa uma função em todos os itens de um array

O método map() retorna um novo array após a manipulação, ou seja, não sobrescreve o array original. Na realidade, todos os métodos que iremos aprender neste artigo retornam um novo array como resposta.

Além disso, o método map() tem uma melhor performance do que o forEach(). Vamos ver um exemplo em que usar o map() nos permite realizar uma alteração nos dados de maneira bem simples.

## filter() - Filtra um array

O próximo método que iremos falar é o filter(). Como o próprio nome diz, ele tem o objetivo de filtrar as informações de um array. Sua funcionalidade consiste em informarmos para ele uma condição. Ele irá aplicar essa condição em todos os itens de nosso array e aqueles que se enquadrarem na condição serão retornados e adicionados ao novo array de saída. Dessa forma, diferente do que ocorre no map() e no reduce(), o filter() irá retornar sempre true ou false.

## reduce() - Reduz um array em um único resultado

O método reduce() é muito interessante e pode ser usado quando desejamos realizar alguma somatória ou então quando desejamos mesclar vários arrays em um único. Ele reduz todos os valores de um array em um único resultado, baseando-se na função que informamos para ele.

Os dois primeiros parâmetros desse método são muito importantes. O primeiro representa o resultado final da redução do array. Esse valor é incrementado ao longo do processo do reduce(), a cada volta desse laço de repetição.

## Promise

O objeto Promise representa a eventual conclusão (ou falha) de uma operação assíncrona e seu valor resultante.
Uma Promise é um proxy para um valor não necessariamente conhecido quando a promise é criada. Ele permite que você associe manipuladores ao valor de sucesso ou motivo de falha de uma ação assíncrona. Isso permite que métodos assíncronos retornem valores como métodos síncronos: em vez de retornar imediatamente o valor final, o método assíncrono retorna uma promise para fornecer o valor em algum momento no futuro.

Uma Promise está em um destes estados:

pending: estado inicial, nem cumprido nem rejeitado.
fulfilled: significa que a operação foi concluída com sucesso.
rejected: significa que a operação falhou.

Promises têm um método chamado .then(), que recebe uma função callback e retorna um "objeto-promessa". Não é um retorno dos dados, é a promessa do retorno destes dados.

Resolvendo várias promessas
No caso de várias promessas que devem ser resolvidas pelo programa (por exemplo, alguns dados em endpoints REST diferentes), pode-se utilizar Promise.all:

const endpoints = [
 "https://api.com/api/user/1",
 "https://api.com/api/user/2",
 "https://api.com/api/user/3",
 "https://api.com/api/user/4"
]

const promises = endpoints.map(url => fetch(url).then(res => res.json()))

Promise.all(promises)
 .then(body => console.log(body.name))

 Existem algumas formas de se trabalhar com processamento assíncrono (ou seja, Promises) em JavaScript: utilizando o método .then(), as palavras-chave async e await ou o objeto Promise e seus métodos. Aqui, vamos focar no uso de .then(), async/await e no uso do método Promise.all.

## Async/await

As palavras-chave async e await, implementadas a partir do ES2017, são uma sintaxe que simplifica a programação assíncrona, facilitando o fluxo de escrita e leitura do código; assim é possível escrever código que funciona de forma assíncrona, porém é lido e estruturado de forma síncrona. O async/await também trabalha com o código assíncrono baseado em Promises, porém esconde as promessas para que a leitura e a escrita seja mais fluídas.

Definindo uma função como async, podemos utilizar a palavra-chave await antes de qualquer expressão que retorne uma promessa. Dessa forma, a execução da função externa (a função async) será pausada até que a Promise seja resolvida.

A palavra-chave await recebe uma Promise e a transforma em um valor de retorno (ou lança uma exceção em caso de erro). Quando utilizamos await, o JavaScript vai aguardar até que a Promise finalize. Se for finalizada com sucesso (o termo utilizado é fulfilled), o valor obtido é retornado. Se a Promise for rejeitada (o termo utilizado é rejected), é retornado o erro lançado pela exceção.

Um exemplo:

```javascript
let response = await fetch(`https://api.com/api/user/${userId}`);
let userData = await response.json();
```

Só é possível usar await em funções declaradas com a palavra-chave async, então vamos adicioná-la:

```javascript
async function getUser(userId) {
 let response = await fetch(`https://api.com/api/user/${userId}`);
 let userData = await response.json();
 return userData.name; // nas linhas de return não é necessário usar await
}
```

Uma função declarada como async significa que o valor de retorno da função será, "por baixo dos panos", uma Promise. Se a Promise se resolver normalmente, o objeto-Promise retornará o valor. Caso lance uma exceção, podemos usar o try/catch como estamos acostumados em programas síncronos.

Para executar a função getUser(), já que ela retorna uma Promise, pode-se usar await:

exibeDadosUser(await getUser(1))
Lembrando que await só funciona se estiver dentro de outra função async. Caso não esteja, você ainda pode usar .then() normalmente:

getUser(1).then(exibeDadosUser).catch(reject)

## O que é o DOM?

O Document Object Model (DOM) é uma interface de programação para os documentos HTML e XML. Representa a página de forma que os programas possam alterar a estrutura do documento, alterar o estilo e conteúdo. O DOM representa o documento com nós e objetos, dessa forma, as linguagens de programação podem se conectar à página.

Uma página da Web é um documento. Este documento pode ser exibido na janela do navegador ou como a fonte HTML. Mas é o mesmo documento nos dois casos. O DOM (Document Object Model) representa o mesmo documento para que possa ser manipulado. O DOM é uma representação orientada a objetos da página da web, que pode ser modificada com uma linguagem de script como JavaScript.

## O que são eventos?

Os eventos são basicamente um conjunto de ações que são realizadas em um determinado elemento da página web, seja ele um texto, uma imagem, ou uma div, por exemplo. Muitas das interações do usuário que está visitando sua página com o conteúdo do seu site podem ser consideradas eventos.

Existe uma infinidade de eventos definidos para uso em JavaScript, abaixo podemos ver alguns dos principais e mais utilizados:

onBlur	remove o foco do elemento
onChange	muda o valor do elemento
onClick	o elemento é clicado pelo usuário
onFocus	o elemento é focado
onKeyPress	o usuário pressiona uma tecla sobre o elemento
onLoad	carrega o elemento por completo
onMouseOver	define ação quando o usuário passa o mouse sobre o elemento
onMouseOut	define ação quando o usuário retira o mouse sobre o elemento
onSubmit	define ação ao enviar um formulário

## Como adicionar e remover classes de elementos HTML com Vanilla JS

Usando a API classList
Além de ser compatível com muitos browsers, ela é muito fácil de aplicar. É só declarar o elemento e chamar a lista de classes:

HTML-----
<p id="elemento" class="essas sao varias classes"></p>
JS-------
document.getElementById('id').classList;

Esse código retornará o seguinte objeto:

{
  1: "essas",
  2: "sao",
  3: "varias",
  4: "classes",
}
E você pode, então, trabalhar esse objeto utilizando os métodos da API:

add() — Adiciona uma classe
remove() — Remove uma classe
contains() — Retorna um booleano indicando se o elemento contém ou não a classe indicada.
toggle() — Adiciona ou remove a classe indicada, dependendo se ela existe ou não no elemento.
Existem outros métodos, mas vamos focar apenas nos que fazem sentido para adicionar ou remover classes de elementos HTML.

Utilizando os métodos da API
Só o que você precisa fazer é selecionar o elemento e usar o método, como no exemplo:

document.getElementById('elemento'); // Retorna o elemento
---> <p id="elemento"></p>
document.getElementById('elemento').classList.add('classe'); // Adiciona classe
---> <p id="elemento" class="classe"></p>
document.getElementById('elemento').classList.remove('classe'); // Remove classe
---> <p id="elemento"></p>
document.getElementById('elemento').classList.toggle('classe'); // Faz toggle na classe
---> <p id="elemento" class="classe"></p>

## Armazenamento 

LocalStorage é também chamado de Web Storage ou Armazenamento local. localStorage é um objeto JavaScript que usamos para armazenar dados no navegador. Ele fornece métodos para armazenar e recuperar a informação. O uso da API é bem simples, é baseada em chave-valor.

```javascript
// Utilizando let ou const para definir o nome e a idade
const nome = 'Marta Silva Rocha';
const idade = 28;

// Armazenando os valores no localStorage
localStorage.setItem('nome', nome);
localStorage.setItem('idade', idade);

// Recuperando os valores usando getItem
const nomeArmazenado = localStorage.getItem('nome');
const idadeArmazenada = localStorage.getItem('idade');

console.log(nomeArmazenado); // Marta Silva Rocha
console.log(idadeArmazenada); // 28

// Utilizando JSON para armazenar um objeto no localStorage
const usuario = { nome: "John Smith da Silva", idade: 29 };
localStorage.setItem('usuario', JSON.stringify(usuario));

// Recuperando o objeto usando JSON.parse
const usuarioArmazenado = JSON.parse(localStorage.getItem('usuario'));

console.log(usuarioArmazenado.nome); // John Smith da Silva
console.log(usuarioArmazenado.idade); // 29

// Propriedade length para mostrar a quantidade de dados armazenados
const quantidadeDeDados = localStorage.length;

// Método key para obter a chave armazenada em uma determinada posição
const primeiraChave = localStorage.key(0);

// Obtendo o valor armazenado na primeira chave
const valorPrimeiraChave = localStorage.getItem(primeiraChave);

// Exibindo informações
console.log(quantidadeDeDados);
console.log(primeiraChave);
console.log(valorPrimeiraChave);
```

## Elementos do DOM

Para selecionar elementos no DOM, o Vanilla JS utiliza os métodos querySelector e querySelectorAll. O querySelector retorna o primeiro elemento que corresponde a um seletor CSS especificado, enquanto o querySelectorAll retorna uma NodeList contendo todos os elementos correspondentes ao seletor.

Aqui está um exemplo de como usar querySelector para selecionar um elemento pelo seu ID e adicionar uma classe a ele:

```javascript
Copy code
// Seleciona o elemento pelo ID
let meuElemento = document.querySelector('#id-do-elemento');

// Adiciona uma classe ao elemento
meuElemento.classList.add('minha-classe');
```
No exemplo acima, substitua 'id-do-elemento' pelo ID real do seu elemento HTML e 'minha-classe' pela classe que você deseja adicionar.

Além disso, para remover uma classe, você pode usar o método classList.remove:

```javascript
Copy code
// Remove uma classe do elemento
meuElemento.classList.remove('minha-classe');
```

Caso você queira alternar a presença de uma classe, ou seja, adicioná-la se ela não estiver presente e removê-la se já estiver, use o método classList.toggle:

```javascript
Copy code
// Alterna a presença da classe no elemento
meuElemento.classList.toggle('minha-classe');
```

Para selecionar vários elementos e realizar operações em todos eles, você pode usar querySelectorAll. Por exemplo, para adicionar uma classe a todos os elementos de uma determinada classe:

```javascript
Copy code
// Seleciona todos os elementos pela classe
var todosElementos = document.querySelectorAll('.minha-classe');

// Adiciona uma classe a todos os elementos
todosElementos.forEach(function(elemento) {
    elemento.classList.add('outra-classe');
});
```

Estes são apenas alguns exemplos básicos de como adicionar e remover classes usando Vanilla JS. Essas operações são fundamentais para a criação de interatividade dinâmica em páginas web.