# Fundamentos básicos da programação

## Variavéis:
As variáveis são usadas com nomes simbólicos para valores em sua aplicação.
São chamados de identificadores as variaveis.
O identificador Js deve começar com uma letra, underline ou cifrão.

## Var:

Declara uma variável, pode se utilizar um valor para iniciar.

## Let:

Declara uma variável local de escopo de bloco, pode se adicionar um valor para iniciar.

## Const:

Declara uma constante de escopo de bloco (apenas leitura).

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

Devemos utilizar quando queremos comparar a mesma variável ou expressão com várias opções:

A instrução switch é similar a uma série de instruções IF sobre a mesma expressão. Em muitas ocasiões, você pode querer comparar a mesma variável (ou expressão) com muitos valores diferentes, executando uma peça diferente do código dependendo de qual valor ele se encaixar. Este é exatamente o que a instrução switch faz.

switch($a) {
    case 1: {
        echo 'Variável A é igual a 1';
        break;
    }
    case 2: {
        echo 'Variável A é igual a 2';
        break;
    }
    default: {
        echo 'A Variável A não é igual a 1 nem igual a 2';
    }
}

## If

Devemos utilizar quando queremos realizar uma série de verificações distintas.

A construção if é uma das características mais importantes de muitas línguas, PHP incluir. Ela permite a execução condicional de fragmentos de código.

Exemplo no Ideone.

if ($a > $b) {
    echo "A é maior que B";
}
else if ($a < $b) {
    echo "A é menor que B";
}
else if ($a == $b) {
    echo "A é igual a B";
}
else {
    echo "A é alguma coisa não comparável com B";
}

## For

Executa o loop enquanto a condição for verdadeira, porém você pode instanciar as variaveis contadoras dentro da estrutura do loop.

for($contar = 1; $contar <= 10; $contar++){
    echo "$contar";
}

## While

Executa o loop enquanto a condição for verdadeira.

// Contar de 1 até 10
$contar = 1;
while($contar <= 10){
   echo "$contar";
   $contar++;
}

## Do While

Executa o loop primeiro e depois verifica a condição.

// Contar de 1 até 10
$contar = 0;
do{
    $contar++;
    echo "$contar";
}while($contar <= 10)
