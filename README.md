# Bootcamp GoStack 8

Este repositório tem como objetivo server de índice e histórico dos projetos desenvolvidos durante o Bootcamp, mas também deve servir para anotações de ferramentas e bibliotecas importantes ou úteis para o desenvolvimento na Stack abordada.

## Sobre o Bootcamp GoStack 

Segundo a definição da RocketSeat o GoStack é um treinamento online, intensivo com foco na prática e produtividade. O GoStack aborda a fundo as tecnologias Node.js, React e React Native bem como as ferramentas necessárias para que seja possa ser feito desde o desenvolvimento até o deploy. Incluindo teste, integração contínua, publicação na lojas e as mais utilizadas bibliotecas e frameworks para ser capaz de enfrentar os desafios reais.

# Node.js

## Packages
* Express - Criação do servidor
* Nodemon: Reinicia o servidor toda vez que é alterado um arquivo -- deve ser instalado com a flag '-D' indicando que é apenas para desenvolvimento
  
     * Adicionar "scripts" como o comando "dev" para executar o arquivo de index
* Sucrase: possibilita usar novo padrão de importação.
* Sequelize: Realiza a conexão com o banco e cria abstração do SQL.
  * Nova migrate :sequelize migration:create --name=
* Eslint: Padroniza o codigo

     * Padrão Airbnb
     * yarn eslint --init
* Prettier: complemento para o eslint.
  * instalação: yarn add prettier eslint-config-prettier eslint-plugin-prettier -D
* EditorConfig: Mantém a configuração entre os editores de texto.
* Bcryptjs: Cria Hash
* jsonwebtoken: Autenticação
* Promisify
  * Transforma função de callback em uma função que aceita async/await
  * import { promissify } from 'util';
  * await promissify({ Função de callback })({ Parametros });
* yup: Cria validação dos atributos do model.
* Multer: Possibilita a uttilização de upload de arquivo em multi part form data
* crypto: Gera caracteres aleatorios, entre outras coisas.
* resolve: navega entre paths.
* date-fns: Manipulação de datas.
  *  yarn add date-fns@next - instala a versão mais recente 
* mongoose: Realiza a conexão com o banco e cria abstração do banco nao relacional mongoDB.


### [Exemplos](https://github.com/ArturMassaro/GoStack08/tree/master/Exemplos)

# Exercícios

## Módulos
* [Módulo 01](https://github.com/ArturMassaro/GoStack08-Modulo-01)
* [Módulo 02(GoBarber - Backend)](https://github.com/ArturMassaro/GoStack08-Modulo-02)

## Desafios
* [Desafio 01](https://github.com/ArturMassaro/GoStack08-Desafio-01)
* [Desafio Meetapp](https://github.com/ArturMassaro/GoStack08-Meetapp)
