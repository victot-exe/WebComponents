## Webcomponent
É um conjunto de elementos pré definido parecido com uma -funcion- onde vc economiza linhas de escrita.  
[cssGenerator](https://www.cssmatic.com/box-shadow)

`Parsed`-> processo de conversão do html para o D.O.M. assim o browser exibe  
`D.O.M.` -> Document Object Model modelo de arvore que divide as divs e tags em ramos e galhos (como numa árvore).  
`Shadow D.O.M.` -> shadow dom (estrutura de arvore dentro da estrutura de arvorea - ramos de arvore), feita para ter mais liberdade. _encapsulamento_  
`custom element` -> criar a sua própria \<div>  
[CAN I USE](https://caniuse.com/) -> mostra o que é compativel com os navegadores.
* Todo o componente é uma function que retorna mais JS, HTML e CSS.  

## Criando a Shadow D.O.M.
* definida em uma classe de JS que extends HTMLElement
* `.attachShadow({mode:""})` -> Cria a shadow D.O.M.  
        * `mode:"closed"`-> O exterior(outro JS) não consegue interferir na shadow D.O.M.  
        * `mode:"open"`-> O exterior consegue interferir na shadow D.O.M.  
* `customElements.define("nome-da-tag", nomeDaClasseJS)`-> Assim vc vai criar um element customizado  
## Definindo as propriedades da tag
*  `componentRoot.textContent = this.getAttribbute("nome-da-propriedade")`  

