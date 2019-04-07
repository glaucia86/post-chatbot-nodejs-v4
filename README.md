# Post Técnico: Criando ChatBot em menos de 5 minutos?! Sim. É possível!

Repositório responsável pela demo do **echoBot**. Mostrando que é possível desenvolver um ChatBot em menos de 5 minutos.

## Recursos Utilizados no Desenvolvimento: :rocket:

- **[Visual Studio Code](https://code.visualstudio.com/?wt.mc_id=post-chatbot-nodejs-v4-github-gllemos)**
- **[Node.js](https://nodejs.org/en/)**
- **[Yeoman](https://yeoman.io/)**
- **[Microsoft Bot Framework Emulator v.4](https://github.com/Microsoft/BotFramework-Emulator/releases/tag/v4.3.3)**
- **[Instalar a versão Python 2.x](https://www.python.org/downloads/)**
- **[Instalar globalmente o node-gyp](https://github.com/nodejs/node-gyp)**

## Instalação do node-gyp (para Usuários Windows) 💥

OBS.: Quando seguir o passo da instalação do **node-gyp** é de suma importância que façam o seguinte:

**Passo 1:** criar manualmente o arquivo **binding.gyp** dentro do diretório do node_modules do appData, conforme o exemplo abaixo:

```

> C:\users\UserName\appdata\roaming\npm\node_modules\node-gyp

```

**Passo 2:** incluir no arquivo **binding.gyp** o seguinte bloco de código e salve:

```

{
    "targets": [{
    "target_name": "binding",
    "sources": [ "build/Release/binding.node" ]
    }]
}

```

**Passo 3:** feito isso, agore execute os seguintes comandos abaixo, dentro do mesmo diretório do appData:

```

> node-gyp configure

```

```

> node-gyp configure --msvs_version=2015

```

```

> node-gyp build

```

Seguindo todos esses passos, vocês estará para pronta para instalar as depedências do projeto na pasta do projeto! ;)

## Atualização da Instalação (node-gyp) 11/2018 ❗️

Devido a nova versão do Node.js, houve mudanças significativas inerente aos passos acima para a instalação do pacote **node-gyp**. 
Após a versão 10.x do Node.js bastam seguir os seguintes passos:

1º - Desinstale da sua máquina o Node.js

2º - Exclua a pasta **npm** localizada no AppData: (remove manualmente):

```
C:\Users\<folder-name>\AppData\Roaming\npm directory was not deleted.
```

3º - Reinstale a última versão do Node.js 10.x: [https://nodejs.org/en/](https://nodejs.org/en)

4º - Abre agora o prompt de comando como administrador e execute o comando abaixo:

```
> npm install npm@latest -g
```

5º - E finalmente, instale globalmente o pacote **node-gyp** no prompt de comando como adminstrador:

```
> npm install -g node-gyp
```

Depois de seguir esses passos, vá até o local onde está o projeto e digite o comando:

```
> npm install
```

O problema será resolvido! :)

## Como executar a aplicação localmente? 🌀

Bastam seguir os passos abaixo:

1) Entre na pasta `echoBot` e execute o seguinte comando abaixo:

```
> nodemon
```

2) Feito isso, basta abrir o Bot Framework Emulator e testar a aplicação. Caso tenham dúvidas como proceder, bastam seguir o gif abaixo:

[![bot-builder-2.gif](https://s2.gifyu.com/images/bot-builder-2.gif)](https://gifyu.com/image/3Yqs)

## Links e Recursos Adicionais: 🔥

* **[Entenda Mais Sobre Azure Bot Service](http://bit.ly/2UpDaa3)**

* **[Depurar Aplicação ChatBot com Emulador](http://bit.ly/2U22gXz)**

* **[Documentação LUIS](http://bit.ly/2IoBIxJ)**

* **[Crie um ChatBot com LUIS](http://bit.ly/2WUa3Zn)**

* **[Experimente Grátis os Serviços Cognitivos](http://bit.ly/2WMAGPG)**


## Dúvidas?! ❓
Se tiverem alguma dúvida referente ao código feito ou para configurar o ambiente bastam criar uma **[ISSUE AQUI](https://github.com/glaucia86/post-chatbot-nodejs-v4/issues)** no GitHub que estarei respondendo a vocês!! ❤️ ❤️ ❤️ 😊
