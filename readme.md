<h1 align="center">
   <img src='.github/assets/feracode.png' style="border-radius:50%"  alt="Feracode"/>
</h1>

<h1 align="center">Feracode Challenge</h1>
<p align="center">
  <img alt="challenge" src="https://badgen.net/badge/feracode/Challenge/b">

  <a href="https://github.com/Zagetsus">
    <img alt="Made by Luan Verdelho" src="https://badgen.net/badge/made by/Luan Verdelho/b">
  </a>

<a href="https://github.com/Zagetsus/feracode-challenge/blob/main/LICENSE">
  <img alt="License" src="https://badgen.net/badge/license/MIT/b">
</a>
</p>

---

Este projeto está arquitetado na biblioteca `React Native`, [leia a documentação](https://reactnative.dev/) para mais
detalhes ou veja o resumo existente na sessão `Configurações > React Native`.

- Conteúdo
    - [Sobre o projeto](#about)
        - [Requisitos](#requirements)
        - [Instalação](#install)
        - [Rodando o Projeto](#run)
    - [Configurações](#configs)
        - Scripts
        - Typescript
        - React Native
    - [Padrões de commits](#commit-patterns)
    - [Licença](#license)

## Sobre o projeto <a name="about"></a>
Aplicativo para o torcedor ficar antenado sobre tudo que está acontecendo nas ligas de futebol do mundo todo. Nele é possível checar como seu time do coração está performando!

### *Requisitos:* <a name="requirements"></a>

- [NodeJs `>16.0.0`](https://nodejs.org/en/)

- [Yarn](https://classic.yarnpkg.com/en/docs/install/#mac-stable)

### Instalação: <a name="install"></a>

Após clonar o projeto, no terminal faça:

```bash 
cd feracode_challenge 
yarn # or yarn install
```

*Note:* Após a instalação deve-se rodar o lint no projeto para fazer uma varredura dos padrões:

```bash
# Para realizar o lint em todo o projeto.

yarn lint
```

### Rodando o Projeto: <a name="run"></a>

Na linha de comando faça:

```bash 
yarn android
```


## Configurações <a name="configs"></a>

<details>
  <summary><b>Scripts</b> (click to show)</summary>

O projeto conta com diversos scripts de linha de comando para uso via terminal, i.e., `yarn <SCRIPT>`
ou `npm run <SCRIPT>`

*DETALHAMENTO*

| Script      | Descrição                                                                                          |
|-------------|----------------------------------------------------------------------------------------------------|
| android     | Builda e inicia o servidor de desenvolvimento com hot auto-reload no ambiente Android              |
| ios         | Builda e inicia o servidor de desenvolvimento com hot auto-reload no ambiente IOS                  |
| test        | Roda os testes do projeto                                                                          |
| lint        | Roda o ESLINT para conferir o styleguide do código, corrigindo automaticamente erros simples       |

</details>

<details>
  <summary><b>Typescript</b> (click to show)</summary>

Esta arquitetura utiliza [*Typescript*](https://www.typescriptlang.org/) como linguagem de codificação. Todas as
features disponíveis pelo framework estão em Typescript e são altamente extensiveis, o que torna todo o código produzido
super flexível para o desenvolvimento de softwares.

Apesar de adicionar uma estrutura diferente há sintaxe do javascript e que muitos programadores poderão não estar
habitualidos a usar, TS trás vários benefícios a codificação:

- Suporte [intellisense](https://code.visualstudio.com/docs/editor/intellisense) para prover auto-completo, informações
  de parametros, informações rápidas, lista de membros, etc., tudo a nível de IDEs de código-fonte.
- Melhor tooling para debug do desenvolvedor, fazendo verificações de erros e garantias de tipagens ao codificar.
- Adição de suporte para design patterns como Abstract, Factories, Decorators, Singles, etc., para facilitar a gerência
  das dependências de forma padronizada e reutilizável.
- Fornece um código mais confiável e explícito, menos sucetível a erros durante a programação.
- Entre outros.

O projeto já possui um linter e o prettier configurados para garantir boa parte da formatação desejada no padrão de
código definido. Arquivos de configuração `.prettierrc` e `.eslintrc.js` explicitam as configurações que dentre as
poucas decisões definem: *utilização obrigatória de aspas SIMPLES* e a *não-utilização de ponto e vírgula*.

Um arquivo `.editorconfig` também dita as configurações acerca da formatação de arquivos: *identação com 2 espaços*,
com *codificação em UTF-8* e com *linha em branco ao final dos arquivos*.

</details>

<details>
<summary><b>React Native</b> (click to show)</summary>

O React Native funciona como uma biblioteca e facilitador de recursos de JavaScript que possibilita o desenvolvimento de
aplicações mobile, tanto para Android como para iOS.

Antes do React Native já existiam algumas soluções híbridas tais como o Apache Cordova (open source), o Adobe PhoneGap (
que utiliza o Cordova também) e o MobileFirst Platform Foundation da IBM.

Para soluções nativas, o profissional de desenvolvimento que precisava rodar uma aplicação para os dois sistemas
operacionais tinha em mãos um projeto muito mais complexo, já que utilizava as linguagens específicas (Java para Android
e Objective-C para iOS), além de não conseguir aproveitar quase nada entre os dois códigos.

Essa sempre foi uma questão na hora de empresas aplicarem projetos de apps mobile, já que aumentavam o número de
profissionais envolvidos e também os custos dos projetos. Também, muitas vezes, era preciso de uma equipe especializada
em JavaScript e outra em Objective-C, fazendo com que aplicações fossem criadas em paralelo, já que os códigos não
tinham correspondência. Nesse aspecto, o React Native veio para facilitar (e muito!) o desenvolvimento de aplicativos
que devem rodar nos dois sistemas operacionais.

*Links úteis*

- [Documentação](https://reactnative.dev/)
- [Atomic Design](https://bradfrost.com/blog/post/atomic-web-design/)
- [Componentização](https://inside.contabilizei.com.br/componentização-no-front-end-f40b0b85143f)

</details>


## Padrões de commit <a name="commit-patterns"></a>

Quando falamos de padrões de commit não podemos esquecer
o [conventional commit](https://www.conventionalcommits.org/en/v1.0.0/), ele já é utilizando como padrão universal de
commits e a sua documentação já exemplifica bem como é trabalhado as confirmações das tarefas no projeto.

Fora o formato padronizado que do convetional, o projeto possui algumas outras peculariedades.

**exemplo:**

- **Liguagem do commit**: `Somente nomenclatura em inglês`
- **Comprimento**: `Mínimo de 10 e no máximo 100 caracteres `
- **Formato**: `[COMMIT_TYPE]: update README to add developer tips`

Agora, segue a tabela com a descrição de cada tipo de commit:

| **COMMIT_TYPE** | DESCRIPTION |
|-----------------|---------------------------------------------------------------------------------------------------------------------|
| **feat**        | uma nova feature. | 
| **fix**         | Ajuste de bugs. | 
| **docs**        | Ajustes na documentação. | 
| **style**       | Ajustes que não alteram a funcionalidade do código, por exemplo (espaços, lint, add vírgulas, etc). | 
| **refactor**    | Ajustes que não são features ou bugs. | 
| **test**        | Ajustes ou implementação de testes. | 
| **chore**       | Ajustes no processo de build, ferramentas auxiliares e outras coisas relacionadas ao ambiente de desenvolvimento. | 
| **perf**        | Ajustes de performance do projeto. | 
| **ci**          | Ajustes em scripts ou processos de CI. | 
| **build**       | Ajustes que afetam diretamente o*build* ou dependencies do projeto (example scopes: gulp, broccoli, npm). | 
| **temp**        | Commits temporários que não serão mergiados e/ou não serão incluidos no CHANGELOG. |


## Licença <a href='license'></a>

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para mais detalhes.
