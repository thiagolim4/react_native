# React 02

- ```import './css/caminho'``` quem faz é o Webpack
- Com o ```creat-react-app``` estamos usando o ```Node.js```
- No ```index.html``` ele vai procurar automaticamente o ```index.js``` dentro de ```src``` e depois importará itens do React (```react``` e ```react-dom```)
- Dois módulos serão usados com maior frequência: ```ReactDOM```, classe que cria os elementos em memória e simula o DOM do navegador e o ```React```, que permite criar novos componentes
- Quando usa ```export default```, na importação não precisa das chaves
 - Se não usar, precisa colocar os módulos entre chaves
- Comentário em JSX: ```{ /*comentario*/ }```
- Usamos o create-react-app para facilitar a configuração da nossa aplicação. Ele já traz junto dele o Babel que é um compilador de código ES6 para uma versão mais antiga do Javascript interpretado por uma maior quantidade de browsers, também chamado de transpiler. Por exemplo, podemos usar sintaxe suportada pelo ES6 e o JSX justamente por conta dele, que já veio configurado com os plugins necessários para essa compilação. Falando especificamente do JSX, qual o motivo da sua utilização?
- Quando usamos o React, trabalhamos com os componentes que utilizam código HTML diretamente do código Javascript. Até poderia ser usado as funções do próprio React para isso, mas, como vimos, acabaríamos com um código complicado de ler. O JSX nos ajuda justamente nisso, permitindo que escrevamos código "html" que na verdade vai ser convertido para Javascript exigido pelo React. Por sinal, essa conversão só é possível porque já está habilitado o React JSX Transform, do Babel.
- O react-create-app traz junto Babel e o webpack. Essas duas ferramentas, combinadas, possibilitam que todo o código ES6 seja transformado para um Javascript válido no navegador.
- O Babel é um famoso transpiler que tem a capacidade, utilizando plugins, de pegar o seu código fonte escrito na versão mais nova do Javascript(ES6) e transformá-lo num código da versão antiga do Javascript(ES5). Por exemplo, a versão recomendada de download do Node.js ainda não implementa todas as funcionalidades do ES6.

Só que esse código Javascript gerado ainda é um código válido para o ambiente de servidor, por exemplo se você estiver usando um Node.js. Como o objetivo é que o código rode no navegador, precisamos de alguém para fazer uma segunda transformação, e é justamente aí que entra o Webpack. Ele vai transformar, por exemplo, as linhas de import de módulo JavaScript e CSS em um código válido no navegador. Como foi explicado no vídeo, essa transformação toda é "cuspida" no arquivo bundle.js.
