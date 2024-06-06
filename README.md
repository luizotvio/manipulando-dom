# Projeto: Manipulando o DOM

## Descrição

Este projeto tem como objetivo demonstrar a manipulação de elementos HTML usando JavaScript. A estrutura do projeto é composta por dois arquivos principais:

- `index.html`: Contém a estrutura padrão de um documento HTML, e 4 tags vazias para serem preenchidas através do script.js.
- `script.js`: Contém o código JavaScript que altera o conteúdo de diversos elementos HTML utilizando diferentes métodos de seleção e manipulação do DOM.

### index.html

```
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="./script.js" defer></script>
    <title>Manipulando o DOM</title>
</head>
<body>
    <h1 id="titulo"></h1>
    <ul></ul>
    <a href="https://prozeducacao.com.br"></a>
    <ol id="lista-ordenada"></ol>
</body>
</html>
````

### script.js

```
let titulo = document.getElementById('titulo').innerText = 'Colocando o título com JavaScript';


let listaNaoOrdenada = document.querySelector('ul').innerHTML = `
    <li>usando ID</li>
    <li>querySelector</li>
    <li>innerHTML e innerText</li>
`;

let link = document.querySelector('a').innerText = 'Site - Proz Educação'

let listaOrdenada = document.getElementById('lista-ordenada').innerHTML = `
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
`
```

## Funcionalidade do script.js

O arquivo `script.js` manipula diversos elementos HTML da seguinte forma:

1. **Adicionando um Título:**

    ```
    let titulo = document.getElementById('titulo').innerText = 'Colocando o título com JavaScript';
    ```

    - O elemento `<h1>` com o `ID` titulo tem seu texto alterado para "Colocando o título com JavaScript".

2. **Atualização da Lista Não Ordenada:**

    ```
    let listaNaoOrdenada = document.querySelector('ul').innerHTML = `
    <li>usando ID</li>
    <li>querySelector</li>
    <li>innerHTML e innerText</li>
    `;
    ```

    - A lista `<ul>` é selecionada usando querySelector e seu conteúdo HTML é atualizado para conter três novos itens de lista.

3. **Alteração do Texto do Link:**

    ```
    let link = document.querySelector('a').innerText = 'Site - Proz Educação';
    ```

    - O primeiro link `<a>` na página tem seu texto alterado para "Site - Proz Educação".

4. **Atualização da Lista Ordenada:**

    ```
    let listaOrdenada = document.getElementById('lista-ordenada').innerHTML = `
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
    `;
    ```
    
    - A lista `<ol>` com o ID lista-ordenada tem seu conteúdo HTML atualizado para conter três novos itens de lista.

## Instruções para Rodar o Projeto

Siga as instruções abaixo para rodar o projeto e verificar as manipulações do DOM:

1. Clone o repositório ou faça o download dos arquivos do projeto.

2. Abra o arquivo index.html em um navegador web.

    - Você pode fazer isso de duas formas:
        - Clique duas vezes no arquivo index.html para abri-lo diretamente no navegador padrão.

        - Abra o navegador de sua preferência e arraste o arquivo index.html para a janela do navegador.

3. Verifique as alterações na página.

    - O título da página deverá estar como "Colocando o título com JavaScript".

    - A lista não ordenada deverá conter os itens: "usando ID", "querySelector" e "innerHTML e innerText".

    - O texto do link deverá ser "Site Proz Educação".

    - A lista ordenada deverá conter os itens: "HTML", "CSS" e "JavaScript".