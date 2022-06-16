## Comandos

* `yarn add @babel/core @babel/cli @babel/preset-env -D`
* `yarn add @babel/preset-react -D`
* `yarn babel src/index.jsx --out-file dist/bundle.js`
## Observações

* **Source Map:** Possibilita ver o código da aplicação mesmo no arquivo bundle gerado pelo Webpack. **Atenção para a segurança!** <https://www.capscode.in/blog/how-to-hide-reactjs-code-from-browser#env-file-in-reactjs>

* **SASS**: Pré-processador de css, muito útil para manter uma organização dos estilos, principalmente pela possibilidade de implementação de herança, tal como na Orientação a Objetos.

* **Operador '??'**: Nova funcionalidade do Javascript, tendo o seu uso mais comum quando queremos atribuir um valor padrão a algo. Se um valor 'a' é 'defined' então retorna 'a', se o valor 'a' é 'undefined' então retornamos 'b': 

>* ```result = a ?? b``` <br> 
> _**é igual a**_ <br>
>* ```result = (a !== null && a !== undefined) ? a : b``` <br>

* **Operador '&&'**: .

* **Programação Funcional - Imutabilidade**: Conceito da programação funcional na qual o React se inspirou, diz que não devemos alterar o objeto original, para trabalharmos com eles, devemos criar cópias desse objeto com as alterações que queremos.

>* ```listaDeFrutas = ['maçã', 'pêssego', 'goiaba']``` <br>
>* ```novaListaDeFrutas = [...listaDeFrutas, 'banana']``` <br>
