# Ionic Auth Firebase


## Autenticação com Facebook usando Google Firebase e Framework Ionic v1
Um simples exemplo de como autenticar o usuário atraves do facebook com o framework ionic usando o firebase da google.

## Introdução ao Google Firebase

O Firebase da Google requer uma conta para autenticação dos seus usuários, 
você pode obter uma conta gratis [clicando aqui](https://console.firebase.google.com/).

## Documentação e API

Você pode ler [a documentação completa] (https://firebase.google.com/docs/)
Bem como [a referência completa da API] (https://firebase.google.com/docs/auth/web/facebook-login)
Na documentação do desenvolvedor Firebase.


## Configuração

Antes de começar a usar este exemplo, você precisa informar as configurações de sua conta do 
Google Firebase dentro do arquivo `www\js\app.js`

```javascript
.factory('Auth', function($firebaseAuth){
    // Initialize Firebase colocar suas configurações aqui
    var config = {
      apiKey: "",
      authDomain: "",
      databaseURL: "",
      storageBucket: "",
      messagingSenderId: ""
    };
    return firebase.initializeApp(config);
})
```

Mais informações de como obter estes dados no [site da documentação](https://firebase.google.com/docs/web/setup)


## Inicializando

Depois de salvo o projeto dentro de um folder, basta ir no prompt de comando e dentro do 
diretório do projeto aplicar o seguinte comando:

```bash
$ ionic serve localhost:8100
```
