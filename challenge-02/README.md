# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function soma(a,b){
    return(a+b);
}
var somaV = function(a,b){ return(a+b);}

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.

var sum = somaV(2,4);
sum = soma(2,3);

// Qual o valor atualizado dessa variável?


// Declare uma nova variável, sem valor.
var variavel;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function nomeVar(a){
    variavel = a;
    return('o Valor da variável, é: '+variavel);
}

// Invoque a função criada acima.
nomeVar(5);

// Qual o retorno da função? (Use comentários de bloco).
// --> "o Valor da variável, é : 5"

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function tresValores(a,b,c){
    if(a === undefined) {
        return('nenhum valor preenchido');

    }else if(b === undefined) {
        return ('um valor preenchidos');

    }else if(c === undefined){
        return('dois valores preenchidos');
    
    }else {
        return('todos os valor preenchido');
    }
}

// Invoque a função criada acima, passando só dois números como argumento.
tresValores(2,3);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
tresValores(2,3);

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
tresValores(2,3,5);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).


/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function tresValores(a,b,c){
        if(a === undefined) {
            return(false);

        }else if(b === undefined) {
            return (a);

        }else if(c === undefined){
            return(a+b);
        
        }else if((a,b,c) != undefined) {
            return((a+b) /c);
        }else{retorn('null');}
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
tresValores();
tresValores(1);
tresValores(1,2);
tresValores(1,2,3);
tresValores(null);