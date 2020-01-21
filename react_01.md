# React 01

- Executar aplicação SpringBoot (que possui 2 Endpoints):
```
java -jar jar-cdc-react.jar
```
- Baixar Node.js e depois verificar a versão e o npm
```> npm install -g create-react-app```
```> npm init react-app cdc-admin```
```> create-react-app cdc-admin
```
- Caminho de execução: ```C:\Program Files\nodejs```
- Ponto de entrada na aplicação: ```index.html```, que é o padrão
- Benefício do React é a construção de *Single Page Applications*
 - a sua aplicação vai ser acessada por diferentes tipos de clientes, como: android, iOS, navegador ou uma aplicação terceira, você ficou obrigado a disponibilizar os dados em um formato diferente de respostas HTML. O formato mais usado hoje em dia é o JSON e nesse caso frameworks Javascript se integram muito bem.
 - terceiro ponto é quando você possui telas que, em função de um evento, precisam ter alguns pontos atualizados. Quanto mais complexa é a tela, mais complicado isso fica. O React deixa esse tarefa consideravelmente mais simples. Você vai atualizar uma informação e vai avisar a ele que agora uma atualização é necessária.
- Com ```create react-app``` ele iniciou um pequeno servidor que sobe com as partes do projeto pra poder acessar pelo navegador através de uma porta
- ```package.json``` é criado com init e vem com detalhes do projeto, dependências, etc
- Usa JSX, que permite usar marcação xml dentro do JavaScript
- Babel é um *transpiler*, pega o fonte JSX e converte pro React e pra versões mais antigas do JS, além de converter pro ```Node.js```
- Webpack é ferramenta de build, pega o que escreve e converte pro js que roda no navegador (converte e manda pro ```bundle.js```)
