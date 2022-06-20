## Comandos

* `yarn add @babel/core @babel/cli @babel/preset-env -D`
* `yarn add @babel/preset-react -D`
* `yarn babel src/index.jsx --out-file dist/bundle.js`
## Observações

* **Source Map:** Possibilita ver o código da aplicação mesmo no arquivo bundle gerado pelo Webpack. **Atenção para a segurança!** <https://www.capscode.in/blog/how-to-hide-reactjs-code-from-browser#env-file-in-reactjs>

* **SASS**: Pré-processador de css, muito útil para manter uma organização dos estilos, principalmente pela possibilidade de implementação de herança, tal como na Orientação a Objetos.

* **Operador '??'**: Nova funcionalidade do Javascript, tendo o seu uso mais comum quando queremos atribuir um valor padrão a algo. Se um valor 'a' é 'defined' então retorna 'a', se o valor 'a' é 'undefined' então retornamos 'b': 

```js
result = a ?? b 

// é igual a

result = (a !== null && a !== undefined) ? a : b
```

* **Operador '&&'**: Executa um código dada uma determinada condição somente se esta for verdadeira. É como uma validação ternária que só retorna verdadeiro.

```js
isDevelopment && console.log("Ambiente de Desenvolvimento")
```

* **Programação Funcional - Imutabilidade**: Conceito da programação funcional na qual o React se inspirou, diz que não devemos alterar o objeto original, para trabalharmos com eles, devemos criar cópias desse objeto com as alterações que queremos.

```js
const listaDeFrutas = ['maçã', 'pêssego', 'goiaba']

const novaListaDeFrutas = [...listaDeFrutas, 'banana']
```

* **Refresh Webpack Plugin**: Mantém alterações no state para fins específicos.

* **Filter(Boolean)**: Retorna somente se a condição for verdadeira, ignorando os valores "falsy" como null e undefined.

```js
isDevelopment && new ReactRefreshWebpackPlugin(), 
new HtmlWebpackPlugin({
    template: path.resolve(__dirname, 'public', 'index.html')
})
].filter(Boolean),
```

