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
* nodemailer: Envio de email.
* Handlebars: Template de email
  * yarn add express-handlebars nodemailer-express-handlebars
* express-async-errors: Captura os erros em funções async. Necessario para utilizar o Sentry
* Youch: Ajuda na visualização de erros
* dotenv: Ler arquivo .env


### [Exemplos](https://github.com/ArturMassaro/GoStack08/tree/master/Exemplos)






# Docker
* Postgres
* Mongodb
  * docker run --name mongobarber -p 27017:27017 -d -t mongo
* Redis
  * docker run --name redisbarber -p 6379:6379 -d -t redis:alpine


# Serviços

### Email
* Amazon SES
* Mailgun
* Mandril(Exlusivo para mailchimp)
* Mailtrap(Somente Dev)

## Sistema de fila
* Bee Queue(Mais performatico)
* kue(Menos performatico, porem tem mais funcionalidades)

## Gerenciamento de erros
* Sentry
  * yarn add @sentry/node@5.6.2 


# React

## Instalações iniciais
* yarn add @babel/core @babel/preset-env @babel/preset-react webpack webpack-cli -D
* yarn add react react-dom
* yarn add @babel/plugin-proposal-class-properties -D

  
## Loader 
* yarn add babel-loader -D
* yarn add webpack-dev-server -D Live Reload
* yarn add style-loader css-loader -D css
* yarn add file-loader -D imagem
* 
## Bibliotecas

* yarn add prop-types: Verifica o tipo de parametro passado
* yarn add styled-components
* yarn add react-icons
* yarn add axios
* yarn add polished: Modificação de cores css
* yarn add json-server
* yarn add reactotron-react-js reactotron-redux
* yarn add react-toastify: Avisos
* yarn add history
* yarn add customize-cra react-app-rewired -D
* yarn add @rocketseat/unform: Facilita a utilização de formularios
* yarn add react-perfect-scrollbars
* yarn add date-fns@next: distancia relativa em datas
* yarn add date-fns-tz: Timezone

### Redux
* yarn add redux redux-saga react-redux reactotron-react-js reactotron-redux reactotron-redux-saga immer 
* yarn add redux-persist: persistencia de dados

## Nova Projeto já com configs.
* yarn create react-app <NAME>

### Prettier & eslint
* yarn add prettier eslint-config-prettier eslint-plugin-prettier babel-eslint eslint-plugin-react-hooks -D
* yarn add eslint-import-resolver-babel-plugin-root-import -D
* yarn add babel-plugin-root-import

# React Native

## Bibliotecas
* yarn add reactotron-react-native: Log
* yarn add react-navigation react-native-gesture-handler react-native-reanimated: Navegação
* yarn add jetifier -D: Fix React Native X
* yarn add react-native-vector-icons: Icons
  * react-native link react-native-vector-icons: link necessario.
* yarn add @react-native-community/async-storage: Local Storage
* yarn add react-native-linear-gradient

## Reactotron/redux

yarn add reactotron-react-native reactotron-redux  reactotron-redux-saga redux redux-saga react-redux


# Exercícios

## Módulos
* [Módulo 01](https://github.com/ArturMassaro/GoStack08-Modulo-01)
* [Módulo 02(GoBarber - Backend)](https://github.com/ArturMassaro/GoStack08-Modulo-02)
* [Módulo 04](https://github.com/ArturMassaro/GoStack08-Modulo-04)
* [Módulo 05](https://github.com/ArturMassaro/GoStack08-Modulo-05)
* [Módulo 06](https://github.com/ArturMassaro/GoStack08-Modulo-06)
* [Módulo 07](https://github.com/ArturMassaro/GoStack08-Modulo-07)
* [Módulo 08](https://github.com/ArturMassaro/GoStack08-Modulo-08)
* [Módulo 09](https://github.com/ArturMassaro/GoStack08-Modulo-09)

## Desafios
* [Desafio 01](https://github.com/ArturMassaro/GoStack08-Desafio-01)
* [Desafio Meetapp](https://github.com/ArturMassaro/GoStack08-Meetapp)
* [Desafio Meetapp - Web](https://github.com/ArturMassaro/GoStack08-Meetapp-Web)