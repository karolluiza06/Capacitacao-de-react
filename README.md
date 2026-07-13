# React

## Pré-requisitos
Antes de começar, certifique-se de ter instalado na sua máquina:
* **Node.js** (versão LTS recomendada)
* Um gerenciador de pacotes (o **npm** já vem instalado junto com o Node)
* Um editor de código (como o **VS Code**)

## Instalação e Criação do projeto
No terminal, navegue até a pasta onde deseja salvar o projeto e execute o comando para iniciar o Vite:

```bash
npm create vite@latest
```
O terminal vai te guiar por algumas perguntas de configuração. Dê o nome que preferir ao seu projeto, escolha a opção React e, em seguida, TypeScript. Para o restante das perguntas, basta ir apertando Enter para aceitar os padrões.

Depois que terminar, entre na pasta e rode o projeto:
```c
npm run dev
```

> **Nota importante:** O Vite já baixa as dependências automaticamente durante a criação do projeto. Porém, se você clonar este repositório do GitHub novamente ou abrir o projeto em outra máquina, lembre-se de rodar `npm install` no terminal antes de iniciar com o `npm run dev`.

## Estrutura do projeto

```text
EXEMPLO/
├── .vscode/         # Configurações locais do VS Code
├── node_modules/    # Dependências e pacotes instalados do projeto
├── public/          # Arquivos estáticos acessíveis publicamente
└── src/             # Código fonte principal da aplicação
    ├── app/         # Páginas, rotas ou lógica principal do app
    ├── assets/      # Arquivos de mídia (imagens, ícones, logos)
    ├── components/  # Componentes React reutilizáveis
    └── styles/      # Arquivos de estilização e CSS global

## O que é react?
O React é uma biblioteca de código aberto utilizada para construir interfaces de usuário dinâmicas e interativas, sendo a escolha ideal para o desenvolvimento de aplicações de página única (SPAs). Sua principal função é permitir a criação de sistemas web extremamente rápidos, onde a página não precisa ser recarregada por inteiro a cada interação; em vez disso, apenas os dados modificados são atualizados na tela de forma instantânea. No nosso projeto, ele funciona em conjunto com o TypeScript, que adiciona tipagem estática ao código para torná-lo mais seguro e evitar erros antes mesmo do código ser executado.

## O que é um componente?
Um componente é o bloco de construção fundamental de uma aplicação React, funcionando como uma unidade de código isolada e independente. Ele agrupa a estrutura visual, a estilização e a lógica (escrita em TypeScript) para formar um pedaço específico da tela, como um botão, uma barra de navegação ou um card de perfil. A grande vantagem dessa arquitetura é a reutilização, pois você escreve o código desse bloco visual uma única vez e pode replicá-lo por todo o projeto, alterando apenas as informações que cada um exibe de forma tipada e segura.

## O que é props?
As **Props** (abreviação de *properties*, ou propriedades) são a forma como enviamos informações de um componente pai para um componente filho no React.

Quando criamos um componente, ele nasce com uma estrutura fixa. As props servem para passar dados dinâmicos para dentro dele, permitindo que o mesmo componente exiba informações diferentes dependendo de onde e como é utilizado. Em um projeto com TypeScript, nós definimos exatamente quais dados (e de quais tipos, como `string`, `number` ou `boolean`) esse componente aceita, garantindo que nenhum dado obrigatório seja esquecido ou enviado de forma errada.

As props são estritas e de **apenas leitura**, o que significa que o componente que as recebe não pode modificá-las diretamente; ele apenas as utiliza para renderizar a interface de forma segura e previsível.
