# Bem vindos ao PHP Poket
A intenção é fazer um resumo do que ando aprendendo na linguagem PHP, não é de intuito deixar uma referência completa sobre a linguagem mas sim algo que sejá o básico para construção de algum sistema ou website simples.
___
## Bibliografia
Todo contéudo abordado aqui é o meu entendimento baseado nos cursos da Alura, Cod3r, livro Desenvolvimento web com PHP e Mysql - Casa do Código - Evaldo Junior Bento e entre outras. Estou pegando o conteúdo e tentando deixar o mais simples possível para futuras consultas e para consultas de outras pessoas também.  

## Instalação

Existe algumas maneiras de fazer a instalação do PHP no Windows:

1- **XAMPP ou WAMPP**  
    Básicamente esses programas tem o ambiente de desenvolvimento para o PHP, eles possui em suas instalação o servidor do apache, mysql e a versão 7 do PHP.

2- **Instalação manual**  
        1. A instalação manual consistem em baixar o PHP no site  (https://www.php.net/downloads), você baixa a versão mais estável.       
        2. Descompacta o arquivo, renomeia o arquivo **php.ini-development** para **php.ini**.  
        3. Pega o caminho da pasta junto com o nome do executável **C:\php-7.4.3-Win32-vc15-x64\php.exe** e abre as variavéis de ambiente do windows. Adiciona o caminho acima no **PATH**.  
        4. Abra o prompt de comando e digite php -v o prompt deve lhe retornar a versão do php
___

## Editores de código e IDE 

Existem vários editores de código, como sublime, notepad ++, bloco de notas e etc.

Recomendo usarem IDEs como PHPStorm, Vscode, Eclipse, NetBeans e etc. As IDEs facilitam muito o trabalho na hora de programar, recomendo tentar testar cada uma citada.

___

## Primeiro Programa em PHP

Abra seu editor de código ou IDE, crie um novo arquivo e coloque o nome de ola-mundo.php ( Todo arquivo em php, terminará com essa extensão. )

Com o arquivo aberto digite os comandos abaixo:

``` PHP
    <?php
        echo "Olá Mundo!"
```

Salve e abra o terminal, vá com o terminal até a pasta que o arquivo se encontra.

Exemplo: c:\estudo-php\ e digite no terminal php ola-mundo.php

O terminal vai retornar:

``` PHP
    Ola mundo!
``` 
Com isso acabamos de criar nosso primeiro programa em PHP.
___

## Introdução

O PHP é uma linguagem de programação interpretada e bastante usada e de curva de aprendizado pequena.

Eu como você sou iniciante mas como tenho um pouco mais de conhecimento e pretendo adquirir mais conhecimento de acordo com que vou escrevendo aqui. Eu vou compartilhando o mesmo. 

Aqui  constará minhas observações e anotações para tentar deixar o conteúdo mais simples e intendivél.

Então vamos começar!

**Tag:** O PHP é uma linguagem que pode ser colocada ou não dentro de um código HTML, por isso usamos dois tipos de tags em php.

##### Tradicional:
```PHP
<?php
    Bloco de código;

?>
```
Ou
```PHP
<?php
    Bloco de código;
```

No primeiro abrimos a tag com **<?php** e fechamos com **?>** só é necessário fechar a tag se acaso os próximos códigos não sejam mais em php, essa tag é bastante utilizada quando misturamos o código php com html

No segundo caso apenas abrimos a tag **<?php** e não fechamos pois estamos supondo que após abertura da tag, todo código que for digitado será apenas em php.

##### Simplificada:

```PHP
    <?=
        Bloco de código;
    ?>
```

Essa tag simplificada não há necessidade de usar o comando "echo" para poder imprimir algo em tela, basta apenas fazer como exemplo abaixo:

```PHP
     <?=
        "Olá Mundo!"
     ?>
```
___
**Váriavéis:** Como o próprio nome já diz, é algo que muda, utilizamos variavéis para armazenar determinado valor na memória e depos acessar o mesmo.
```PHP
<?php
    /*
        Para declar uma váriavel em php é necessário colobar  
        o simbolo $ e logo em seguida o nome da variavel.
    */
    $nome = "Mario";

    /* acima declaramos uma variavel que recebe como valor   
    o nome Mario. */
```

**Comentários:** São usados para "desativar um trecho de código", comentar para que server aquele bloco de código e etc..  

```PHP
<?php
    /*Comentário de várias linhas
     como podemos ver*/

     //comentário de uma única linha
     
    //$nome = "Mario";  ** NOTE QUE COMENTAMOS UMA LINHA DE CÓDIGO **
    
    echo 'Meu nome é: '.$nome;

    saida sera "Meu nome é: "

    /* acima declaramos uma variavel que recebe como valor   
    o nome Mario. */
```
**Tipos:** Acima vimos como declarar váriavéis, diferente de outras linguagens de programação como JAVA o PHP não precisa declarar o tipo da variavel. Abaixo iremos ver os tipos primitivos em PHP:

-Inteiro -> Números inteiros ex: {..., -2, -1, 0, 1, 2, ...}.  
-String -> Texto.  
-Boleando-> Verdadeiro ou Falso.  
-Fload-> Números de ponto flutuantes ex: 9.5 .  

Para saber mais https://www.php.net/manual/pt_BR/language.types.php