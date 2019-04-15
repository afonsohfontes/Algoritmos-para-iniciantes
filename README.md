# Algorítmos para Iniciantes

Este guia irá compor as ferramentas para ensino de Algoritmos e Programação de Computadores, onde os alunos aprendem alguma linguagem de programação sem necessidade de um conhecimento prévio.

Esta página é uma coleção de exercícios progressivamente mais difíceis que são adequados para pessoas que tem interesse em aprender Lógica de Programação. Os exercícios, em sua maioria, são algorítmicos e devem/podem ser solucionados sem o uso de bibliotecas. A dificuldade dos exercícios, claro, depende da linguagem de programação que você usa, como por exemplo C, que não têm suporte integrado à listas. Alguns exemplos serão resolvidos em javaScript.

## Começando

Aprender a programar significa aprender a resolver problemas usando código. Conceitualmente, não é muito difícil escrever um programa que resolva um problema que você possa resolver sozinho. A habilidade que você precisa adquirir é pensar precisamente sobre como você resolve o problema e o divide em etapas tão simples que um computador pode executá-las. Encorajo-vos a resolver primeiro algumas instâncias de um problema à mão e pensar sobre o que você fez para encontrar a solução. Por exemplo, se a tarefa estiver classificando listas, classifique algumas listas curtas você mesmo. Um método razoável seria encontrar o menor elemento, anotá-lo e retirá-lo da lista original e repetir esse processo até que você tenha classificado toda a lista. Então você tem que ensinar o computador 1) como encontrar o menor elemento, 2) como escrevê-lo, 3) como atravessá-lo, e envolvê-lo em um loop. Em seguida, continue com o processo de detalhamento da tarefa até ter certeza de que você sabe como escrever o programa necessário.


Este [vídeo](https://www.youtube.com/watch?v=8mei6uVttho) é um ótimo início para nossa jornada, leve o tempo que precisar, assista, pause, reveja quantas vezes achar nescessário.

[![Algoritmos: Primeiro contato](https://img.youtube.com/vi/8mei6uVttho/0.jpg)](https://www.youtube.com/watch?v=8mei6uVttho)


### Pré-requisitos

*[NotePad++](https://notepad-plus-plus.org/download/v7.6.6.html) - O editor de texto/código utilizando pelos autores. Fique a vontade de utilizar outras opções dispoíveis.
*Precisaremos também de um navegador capaz de compilar javaScript, como [Google Chrome](https://www.google.com/intl/pt-BR_ALL/chrome/) ou [Firefox](https://www.mozilla.org/pt-BR/firefox/new/).



## Input/Output

### Input
Funções de input são funções que permitem receber dados informados pelo usuário.
As principais funções de input são: prompt e confirm.

As estruturas básicas são:
`` `
var leitura = prompt("Mensagem que será mostrada ao usuário pedindo algo","Resposta padrão"(opcional));
`` `

- É importante lembrar de atribuir o retorno do prompt há alguma variável para que a informação não seja perdida.
- A mensagem que virá do prompt será tratada como uma string. Caso queira que seja tratada como um número inteiro, é necessário o uso da função parseInt().
`` `
var leitura = confirm("Mensagem para perguntar se ele deseja confirmar");

`` `
 - A função confirm atribui true caso o usuário clique em "Ok" ou atribui false caso o usuário clique em "Cancelar"

### Output
Funções de output são funções que permitem informado dados ao usuário que foram obtidos com o programa.
As principais funções de output são: document.write e alert.

As estruturas básicas são:
alert("Mensagem a ser mostrada ao usuário em uma janela pop up" + variável_a_ser_exibida_caso_necessário);
- O alert abrirá uma caixa pop up com a mensagem ou variável que será colocada entre os parênteses.

document.write("Mensagem a ser mostrada da seção document da página html" + variável_a_ser_exibida_caso_necessário);
- O document.write exibirá na parte "document" da página web a mensagem ou variável que será colocada entre os parênteses.


[Link para for](https://github.com/raulfontenele/Algoritmo-e-Programa-o-de-Computadores/blob/master/Exemplo_Quest%C3%B5es_For/Exemplo_For.html)




Write a program that prints ‘Hello World’ to the screen.
    
Write a program that asks the user for their name and greets them with their name.
    
Modify the previous program such that only the users Alice and Bob are greeted with their names.

Write a program that asks the user for a number n and prints the sum of the numbers 1 to n

Modify the previous program such that only multiples of three or five are considered in the sum, e.g. 3, 5, 6, 9, 10, 12, 15 for n=17

Write a program that asks the user for a number n and gives them the possibility to choose between computing the sum and computing the product of 1,…,n.

Write a program that prints a multiplication table for numbers up to 12.

Write a program that prints all prime numbers. (Note: if your programming language does not support arbitrary size numbers, printing all primes up to the largest number you can easily represent is fine too.)

Write a guessing game where the user has to guess a secret number. After every guess the program tells the user whether their number was too large or too small. At the end the number of tries needed should be printed. It counts only as one try if they input the same number multiple times consecutively.

Write a program that prints the next 20 leap years.
    
## Listas e Strings

Write a function that returns the largest element in a list.

Write function that reverses a list, preferably in place.

Write a function that checks whether an element occurs in a list.

Write a function that returns the elements on odd positions in a list.

Write a function that computes the running total of a list.

Write a function that tests whether a string is a palindrome.
Write three functions that compute the sum of the numbers in a list: using a for-loop, a while-loop and recursion. (Subject to availability of these constructs in your language of choice.)

Write a function on_all that applies a function to every element of a list. Use it to print the first twenty perfect squares. The perfect squares can be found by multiplying each natural number with itself. The first few perfect squares are 1*1= 1, 2*2=4, 3*3=9, 4*4=16. Twelve for example is not a perfect square because there is no natural number m so that m*m=12. (This question is tricky if your programming language makes it difficult to pass functions as arguments.)

Write a function that concatenates two lists. [a,b,c], [1,2,3] → [a,b,c,1,2,3]

Write a function that combines two lists by alternatingly taking elements, e.g. [a,b,c], [1,2,3] → [a,1,b,2,c,3].

Write a function that merges two sorted lists into a new sorted list. [1,4,6],[2,3,5] → [1,2,3,4,5,6]. You can do this quicker than concatenating them followed by a sort.

Write a function that rotates a list by k elements. For example [1,2,3,4,5,6] rotated by two becomes [3,4,5,6,1,2]. Try solving this without creating a copy of the list. How many swap or move operations do you need?

Write a function that computes the list of the first 100 Fibonacci numbers. The first two Fibonacci numbers are 1 and 1. The n+1-st Fibonacci number can be computed by adding the n-th and the n-1-th Fibonacci number. The first few are therefore 1, 1, 1+1=2, 1+2=3, 2+3=5, 3+5=8.

Write a function that takes a number and returns a list of its digits. So for 2342 it should return [2,3,4,2].

Write functions that add, subtract, and multiply two numbers in their digit-list representation (and return a new digit list). If you’re ambitious you can implement Karatsuba multiplication. Try different bases. What is the best base if you care about speed? If you couldn’t completely solve the prime number exercise above due to the lack of large numbers in your language, you can now use your own library for this task.

Write a function that takes a list of numbers, a starting base b1 and a target base b2 and interprets the list as a number in base b1 and converts it into a number in base b2 (in the form of a list-of-digits). So for example [2,1,0] in base 3 gets converted to base 10 as [2,1].

Implement the following sorting algorithms: Selection sort, Insertion sort, Merge sort, Quick sort, Stooge Sort. Check Wikipedia for descriptions.

Implement binary search.

Write a function that takes a list of strings an prints them, one per line, in a rectangular frame. For example the list ["Hello", "World", "in", "a", "frame"] gets printed as:

    *********
    * Hello *
    * World *
    * in    *
    * a     *
    * frame *
    *********

Write function that translates a text to Pig Latin and back. English is translated to Pig Latin by taking the first letter of every word, moving it to the end of the word and adding ‘ay’. “The quick brown fox” becomes “Hetay uickqay rownbay oxfay”.

## Intermediate

 
 Write a program that outputs all possibilities to put + or - or nothing between the numbers 1,2,…,9 (in this order) such that the result is 100. For example 1 + 2 + 3 - 4 + 5 + 6 + 78 + 9 = 100.

Write a program that takes the duration of a year (in fractional days) for an imaginary planet as an input and produces a leap-year rule that minimizes the difference to the planet’s solar year.
 
 Implement a data structure for graphs that allows modification (insertion, deletion). It should be possible to store values at edges and nodes. It might be easiest to use a dictionary of (node, edgelist) to do this.
 
 Write a function that generates a DOT representation of a graph.

Write a program that automatically generates essays for you.

Using a sample text, create a directed (multi-)graph where the words of a text are nodes and there is a directed edge between u and v if u is followed by v in your sample text. Multiple occurrences lead to multiple edges.

Do a random walk on this graph: Starting from an arbitrary node choose a random successor. If no successor exists, choose another random node. 

Write a program that automatically converts English text to Morse code and vice versa.

Write a program that finds the longest palindromic substring of a given string. Try to be as efficient as possible!

Think of a good interface for a list. What operations do you typically need? You might want to investigate the list interface in your language and in some other popular languages for inspiration.

Implement your list interface using a fixed chunk of memory, say an array of size 100. If the user wants to add more stuff to your list than fits in your memory you should produce some kind of error, for example you can throw an exception if your language supports that.

Improve your previous implementation such that an arbitrary number of elements can be stored in your list. You can for example allocate bigger and bigger chunks of memory as your list grows, copy the old elements over and release the old storage. You should probably also release this memory eventually if your list shrinks enough not to need it anymore. Think about how much bigger the new chunk of memory should be so that your performance won’t be killed by allocations. Increasing the size by 1 element for example is a bad idea.

If you chose your growth right in the previous problem, you typically won’t allocate very often. However, adding to a big list sometimes consumes considerable time. That might be problematic in some applications. Instead try allocating new chunks of memory for new items. So when your list is full and the user wants to add something, allocate a new chunk of 100 elements instead of copying all elements over to a new large chunk. Think about where to do the book-keeping about which chunks you have. Different book keeping strategies can quite dramatically change the performance characteristics of your list.

Implement a binary heap. Once using a list as the base data structure and once by implementing a pointer-linked binary tree. Use it for implementing heap-sort.

Implement an unbalanced binary search tree.

Implement a balanced binary search tree of your choice. I like (a,b)-trees best.

Compare the performance of insertion, deletion and search on your unbalanced search tree with your balanced search tree and a sorted list. Think about good input sequences. If you implemented an (a,b)-tree, think about good values of a and b.

## Advanced

 Given two strings, write a program that efficiently finds the longest common subsequence.

Given an array with numbers, write a program that efficiently answers queries of the form: “Which is the nearest larger value for the number at position i?”, where distance is the difference in array indices. For example in the array [1,4,3,2,5,7], the nearest larger value for 4 is 5. After linear time preprocessing you should be able to answer queries in constant time.

Given two strings, write a program that outputs the shortest sequence of character insertions and deletions that turn one string into the other.

Write a function that multiplies two matrices together. Make it as efficient as you can and compare the performance to a polished linear algebra library for your language. You might want to read about Strassen’s algorithm and the effects CPU caches have. Try out different matrix layouts and see what happens.

Implement a van Emde Boas tree. Compare it with your previous search tree implementations.

Given a set of d-dimensional rectangular boxes, write a program that computes the volume of their union. Start with 2D and work your way up.



### Instalando

Uma série passo a passo de exemplos que informam como obter um env de desenvolvimento em execução

Diga qual será o passo

`` `
Dê o exemplo
`` `

E repita

`` `
até terminar
`` `

Termine com um exemplo de obter alguns dados do sistema ou usá-los para uma pequena demonstração

## Rodando os testes

Explicar como executar os testes automatizados para este sistema

### Divida em testes de ponta a ponta

Explique o que esses testes testam e por que

```
Dê um exemplo
```

### E testes de estilo de codificação

Explique o que esses testes testam e por que

`` `
Dê um exemplo
`` `

## Desdobramento, desenvolvimento

Adicione notas adicionais sobre como implantar isso em um sistema ativo

## construído com

* [Dropwizard] (http://www.dropwizard.io/1.0.2/docs/) - O framework web usado
* [Maven] (https://maven.apache.org/) - Gerenciamento de Dependência
* [ROMA] (https://rometools.github.io/rome/) - usado para gerar feeds RSS

## Contribuindo

Leia [CONTRIBUTING.md] (https://gist.github.com/PurpleBooth/b24679402957c63ec426) para obter detalhes sobre nosso código de conduta e sobre o processo de envio de solicitações de recebimento para nós.

## Versioning

Nós usamos [SemVer] (http://semver.org/) para controle de versão. Para as versões disponíveis, veja as [tags neste repositório] (https://github.com/your/project/tags).

## Autores

*** Billie Thompson ** - * Trabalho inicial * - [PurpleBooth] (https://github.com/PurpleBooth)

Veja também a lista de [contribuidores] (https://github.com/your/project/contributors) que participaram deste projeto.

Licença ##

Este projeto está licenciado sob a licença MIT - consulte o arquivo [LICENSE.md] (LICENSE.md) para obter detalhes

## Agradecimentos

* Dica de chapéu para qualquer pessoa cujo código foi usado
* Inspiração
* etc
