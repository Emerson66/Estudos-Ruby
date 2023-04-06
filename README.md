# Estudos-Ruby

## Instalação

##Introdução

### Variaveis

Em Ruby, para declarar uma variavel basta definirmos
o nome da variável e atribuir um valor usando o sinal ``` = ``` :

``` idade = 2 ```

Com o Ruby instalado e configurado, para executar o codigo acima basta executa-lo dentro do irb usando este mesmo comando dentro do terminal

![IRB - terminal](https://user-images.githuburuby teste.rbsercontent.com/70235882/230253041-9cf9e17e-801e-4a71-b298-f3ca94fddbb6.png)

Outra forma de criar e executar código Ruby é criando um arquivo .rb e
executá-lo utilizando o comando ruby. Se o código acima fosse digitado dentro
de um arquivo minhaIdade.rb para executá-lo faríamos:

```ruby teste.rb```

Quando foi declarado a variavel idade, não foi informado o tipo dela, pois diferente de outras linguagens no Ruby o interpretador infere o tipo da variavel automaticamente durante a execução do código. Chamamos isso de Inferência de tipos.

Para verificar o tipo da variavel utilize o comando ```puts idade.class```:

![puts variavel class](https://user-images.githubusercontent.com/70235882/230254394-87ea3745-079e-4af2-bcf6-f9ee450cffcd.png)

Quando invocamos .class em qualquer variável, o interpretador Ruby retorna
o tipo da variável, que será impressa no IRB pelo método puts.
