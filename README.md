`PROJETO USANDO LESS:`

*PROJETO DESENVOLVIDO PELA EBAC*

# O que é o LESS?

Como o SASS o LESS é um **pré-processador CSS**, então ele transforma o arquivo escrito em LESS para CSS
Ambos são muito semelhantes na sua sintaxe, então se torna algo muito fácil de se aprender


# Instalando e compilando com LESS:



Para utilizarmos o LESS, primeiro vamos instalar ele de forma global em nossa -- - [máquina](*[npm install -global less]*)
*
Depois vamos iniciar nosso projeto com npm init -y e instala-lo como dependência de desenvolvedor 
*[npm install --save-dev less]*

- **[O LESS ]** por padrão não possui a função ‘watch’, mas não se preocupe vamos instalar o pacote less-watch-compiler para resolver esse nosso problema 
*npm install --save-dev less-watch-compiler*
Então agora podemos configurar nosso LESS dentro do package.json, então na parte de scripts vamos adicionar o LESS da seguinte forma:

*************************************************************************
"scripts": {
    "less": "less-watch-compiler ./src/styles ./build/styles/ main.less",
    "test": "echo \"Error: no test specified\" && exit 1"
  },
*************************************************************************


Depois de less-watch-compiler (que é o que fará a compilação) passamos onde está o arquivo fonte e onde será o arquivo final
Então executando *npm run less ***
"'ele estará pronto, compilando e mostrando em tempo real as alterações feitas. Podemos utiliza-lo a vontade a partir de agora.'"