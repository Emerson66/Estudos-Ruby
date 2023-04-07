# Estudos-Ruby

## Instalação

## Introdução

### Variaveis

  Em Ruby, para declarar uma variavel basta definirmos
o nome da variável e atribuir um valor usando o sinal ``` = ``` :

``` idade = 2 ```

  Com o Ruby instalado e configurado, para executar o codigo acima basta executa-lo dentro do ```irb``` usando este mesmo comando dentro do terminal

![IRB - terminal](https://user-images.githubusercontent.com/70235882/230254732-cda6360b-b508-4110-8a22-c8596ff95b42.png)


  Outra forma de criar e executar código Ruby é criando um arquivo .rb e
executá-lo utilizando o comando ruby. Se o código acima fosse digitado dentro
de um arquivo minhaIdade.rb para executá-lo faríamos:

```ruby teste.rb```

  Quando foi declarado a variavel idade, não foi informado o tipo dela, pois diferente de outras linguagens no Ruby o interpretador infere o tipo da variavel automaticamente durante a execução do código. Chamamos isso de Inferência de tipos.

Para verificar o tipo da variavel utilize o comando ```puts idade.class```:

![puts variavel class](https://user-images.githubusercontent.com/70235882/230254394-87ea3745-079e-4af2-bcf6-f9ee450cffcd.png)

  Quando invocamos .class em qualquer variável, o interpretador Ruby retorna o tipo da variável, que será impressa no IRB pelo método ```puts```.


### Qual a tipagem de Ruby?

  Se eu não declaro qual o tipo da minha variável, quer dizer que o tipo dela não im-
porta para meu interpretador?
  Em Ruby, a resposta é não.
  
  Apesar de ser uma linguagem com inferencia de tipos, o tipo importa para o interpretador. Na pratica isso quer dizer que se tentarmos fazer uma operação matematica entre uma variavel do tipo **integer** e uma do tipo "string" os valores não serão convertidos para outro tipo automaticamente, afim de possibilitar a operação.

```
idade = 23
multiplicador = "2"
idade * multiplicador
```

  O codigo acima não funciona ele retorna a seguinte mensagem de erro:
![Erro de inferencia](https://user-images.githubusercontent.com/70235882/230523285-1961ec9a-5242-47fb-95c1-a7ffdeef2650.png)
  
  Nesse caso o Ruby ta dizendo que é impossivel multiplicar um numero com um texto. Essa característica da linguagem de realizar operações em variáveis de tipos diferentes é chamada de tipagem fraca ou forte.
  
  No caso do Ruby, onde o tipo é determinante para o sucesso da operação, dizemos que a linguagem tem tipagem forte. Tendo a tipagem forte em mente, vamos ir mais além. Execute o seguinte código:
```
idade = 23
idade = "23"
```

  Esse condigo funciona normalmente, pois não estamos fazendo nenhuma operação que misture os tipos. Ele apenas atribui um **integer** à idade e depois atribui uma **string** a mesma variavel. Linguagens que permitem que o tipo da variável possa ser alterado durante a execução do programa são linguagens com a tipagem dinâmica.
  O contrario de tipagem dinamica é a tipagem estática. Um exemplo de linguagem com tipagem estática é o ***Java*** , uma vez que uma varíavel que nasceu ```int``` não poderá mudar o tipo como ocorre no Ruby.
