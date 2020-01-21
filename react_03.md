# React 03

- Componentes possuem comportamento (```render()```):
```
constructor(){
  super();
  this.state = {lista : []};
}
```
- Guarda estado na variável state, que é um JSON representando o estado do objeto
- Código dinâmico usa {}
- Usa função dos arrays ```map``` para mapear os objetos JSON em HTML, usando ```return()```
- Sempre que trocar o estado (```this.setState({novo JSON}))```), o React invoca o método ```render()``` novamente
 - Passa pra ele a propriedade atualizada
 - React Lifecycle tem métodos e propriedades dos componentes, antes de serem renderizados e depois
 - Sua função React retorna um pedaço do Virtual DOM e avalia pra saber se tem distinção, e aí altera no navegador (no DOM real)
 - Pra auxiliar nessa alteração, usa a ```key``` do objeto
 - ```JSON.stringfy({nome: '', email: ''})``` passa um JSON para String
 - ```bind``` "conserta" o this indicando que é o elemento do React
- Os values dos inputs joga dentro do state para que sejam atualizados ```value = {this.state.atributo}```
- Componentes possuem o ```props``` além do state para ajudar a passar parâmetros para eles
