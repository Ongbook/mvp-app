# MVP Ongbook App

Catálogo de Entidades com as causas mais nobres do planeta.

**Tabela de Conteúdo**  

- [Principais Tecnologias Utilizadas](#principais-tecnologias-utilizadas)
	- [Typescript](#typescript)
	- [Angular](#angular)
	- [Ionic](#ionic)
	- [Ionic App Scripts](#ionic-app-scripts)
  - [Sass](#sass)
- [Visão Geral](#visão-geral)
	- [Build System](#build-system)
	- [Dependências](#dependências)
	- [Instalando](#instalando)
	- [Executando](#executando)
	- [Executando no dispovitivo móvel para teste](#Executando-no-dispovitivo-móvel-para-teste)

# Principais Tecnologias Utilizadas
Essas são as principais ferramentas, *frameworks* e *libraries* que dão suporte ao projeto:

## [Typescript](https://www.typescriptlang.org/)
TypeScript é uma linguagem para desenvolvimento JavaScript em larga escala. 
Com TypeScript podemos escrever código utilizando uma estrutura fortemente tipada e ter este código compilado para JavaScript puro. Nem todas as features do ES2105 já são suportados pelos browsers. TypeScript permite desfrutar de todas as novas características da linguagem hoje, 
covertendo código ES2015 em código equivalente em ES5. Qualquer navegador. Qualquer host.

## [Angular](https://angular.io)
Angular é um framework estrutural para aplicações web dinâmicas.

## [Ionic](http://ionicframework.com/)
Ionic é um framework que visa a criação de aplicações híbridas para dispositivos móveis. 

## [Ionic-App-Scripts](https://github.com/ionic-team/ionic-app-scripts)
Scripts de build para projetos ionic usando o webpack como tecnologia subjacente.

## [Sass](http://sass-lang.com/)

SASS é uma poderosa extensão da linguagem CSS que permite uma escrita profissional e completa das folhas de estilo de forma muito mais dinâmica e produtiva. 

## Dependências
Ferramentas necessárias para rodar a aplicação:
* `node + npm` versão LTS: [https://nodejs.org/en/download/](https://nodejs.org/en/download/)
* ionic: `npm i -g ionic`
* cordova: `npm i -g cordova`

obs: o ionic e o cordova são instalados no escopo global (-g).

## Instalando
1. `fork` este repositório pelo GitHub
2. clone o seu fork: `git clone <url-github-fork>`
3. acesse o diretorio criado: `cd mvp-app`
4. instale as dependências da aplicação: `npm install`

## Executando
O **MVP Ongbook App** usa `ionic-app-scripts` para compilar a aplicação e executar o ambiente de desenvolvimento. Depois de instaladas todas as dependências, você deve *rodar* a aplicação. O comando `ionic serve`. Isso irá iniciar o build utilizando o ionic, vai gerar um *bundle* da aplicação, *subir* um servidor de desenvolvimento e *escutar* por alterações em todos os arquivos. 

Por padrão a aplicação será servida em http://localhost:3000.

## Executando no dispovitivo móvel para teste

Com o celular plugado no PC e reconhecido pelo sistema.

1. `npm run build:android`
2. `cordova platform add android`
3. `cordova prepare android -f`
4. `cordova run android`
