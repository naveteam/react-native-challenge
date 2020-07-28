# Desafio de React Native

## Navedex

O desafio é criar um aplicativo para visualização e criação dos navers, possuindo informações como: nome, idade, cargo, tempo de empresa e projetos que participou.

O uso de [react native](https://reactnative.dev/) é essencial para o teste, pois, é a ferramenta que usamos para o desenvolvimento de apps na empresa. O uso de [expo](https://docs.expo.io/) ou da CLI do react native para inicializar o projeto, vai da preferência de quem está realizando o teste.

## Figma

Use as telas do [figma](https://www.figma.com/file/MIh7DeADz8M3mmcQwpcFdD/Teste-Mobile?node-id=1253%3A0) para se guiar no desenvolvimento. O código de estilização não será tão importante quanto o javascript, mas esperamos que o layout fique de acordo com as telas. Uma dica nossa é usar [styled-components](https://styled-components.com/) para a estilização, mas sinta-se a vontade para usar qualquer solução para estilos no react native.

## API

Para as funcionalidades da aplicação, faça integração com a api. Recomendamos o uso do [axios](https://github.com/axios/axios) para realizar as chamadas http. URL da api: https://navedex-api.herokuapp.com/v1/

A documentação da API oficial do teste pode ser utilizada com o [postman](https://www.postman.com/) importando [esse](https://www.getpostman.com/collections/e6afe4028c2a1e56e577) link. Todos os parâmetros para cada rota estão documentados nessa URL, então a utilize como base para montar o app.

Após importar o link no postman, você deve criar um cadastro utilizando a request de `user/signup`. 

## Funcionalidades

### Login

O app deverá possuir um fluxo de autenticação, onde o usuário só pode acessar as telas internas (listagem, formulários) passando pela tela de login com as credenciais criadas previamente via Postman.

Para realizar o login, você deve usar a request de `user/login` disponível no postman. Essa request retornará um token do tipo `Bearer` que deverá ser utilizado no header das próximas requisições.

### Listagem

A página inicial do app terá uma lista dos `navers`.

Para listar os `navers`, você deve usar a request de `navers/index` disponível no postman.

### Visualização

Ao clicar em algum `naver` da listagem, o usuário terá uma visualização completa das informações do mesmo.

Para apresentar um único `naver`, você deve usar a request de `navers/show` disponível no postman.
Para excluir um `naver`, você deve usar a request de `navers/delete` disponível no postman.

### Criação/edição

O usuário precisa ter a possibilidade de criar um novo `naver` ou editar um já existente.

Para criar um `naver`, você deve usar a request de `navers/create` disponível no postman.
Para editar um `naver`, você deve usar a request de `navers/update` disponível no postman.

### Utilidades

Para fazer a navegação entre rotas, utilize o [react-navigation](https://reactnavigation.org/docs/getting-started). Ele também fornece um componente de [drawer](https://reactnavigation.org/docs/drawer-based-navigation), que faz parte do layout que está no figma.

Para fazer os alertas de sucesso/confirmação/erro, pode utilizar o componente de [modal do react native](https://reactnative.dev/docs/modal).

## Observações



Ao finalizar o teste, envie o link do seu repositório por e-mail para [vagas@nave.rs](mailto:vagas@nave.rs).

Se durante o processo de desenvolvimento não conseguiu fazer algo, explique qual o impedimento que encontrou e como tentou resolver em uma seção `Dificuldades` do seu README e nos envie até onde chegou. 😄
