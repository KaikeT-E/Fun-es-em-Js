# Funções em JS

# O que são as funções em JavaScript?

As funções são uma série/bloco de instruções que executam uma determinada tarefa ou mostram um determinado valor, elas severm para organizar e estruturar o código, evitando repetições, além de poderem receber e retornar dados.

# - Expression.

O expression é uma função que gera valor. Pode realizar ações(como atribuições) ou retornar resultados.

Exemplos:

```js
     let resultado = 10 * 2;
     let ativo = true;
     let string = "ola" + "mundo";
```
Também temos outros tipos como o const.

Vantagens: 

- simples de usar
- alta compatibilidade com navegadores
- interações com o usuário

Desvantagens:

- compreensão de escopo
- depuração
- segurança

# - Declaration.

O declaration é uma instrução que cria e nomeia uma função, variável ou classe, tornando-se disponível no escopo onde foi declarada.

Exemplos:

```js
    var linguagem = "JavaScript";
    let versao = 2025;
    const autor = "Brendan Eich";

    funcion cumprimentar () {
      console.log("bem-vindo")
    }
    cumprimentar(); // saída: bem-vindo
```
Vantagens:

- flexibilidade na criação e inicialização de variaveis e funções
- controle de escopo
- menor risco de declarações acidentais

Desvantagens:

- o var pode causa confusão devido ao hoisting
- é preiso escolhe corretamente entre var, let e const de acordo com a utilização
- exige atenção ao escopo de cada tipo de declaração

# - Arrow.

O arrow é uma forma mais curta de declarar as funções. Elas não criam seu proprio this(heram do escopo onde foram criados), o que a torna ideal para callbacks e funções simples.

Exemplos:
```js
    const dobro = n => n * 2;
    console.log(dobro(8)); // saída: 16
    const boasvindas = nome => 'seja bem-vindo', ${nome}!;
    console.log(boasvindas("maria")); // saída: seja bem-vindo, maria!
    const calcularArea = (largura, altura) => largura * altura;
    console.log(calcularArea(5,3)); // saída: 15
```
Vantagens:

- sintaxe curta e direta
- possibilidade de retorno implícito
- código limpo e fácil de ler

Desvantagens:

- não podem ser usadas como construtoras
- por não possuirem seu próprios this, o uso acaba sendo limitade em alguns aspectos
