# Configuração

<p> Caso baixe o seu código do zero, não esuqueça de modificar o arquivo <strong> package.json </strong> e acrescente esse código </p>


## Alteração importante que deve ser feita
```
name": "app",
  "version": "0.1.0",
  "private": true,
  "scripts": {
    "start": "npm run serve",
    "serve": "vue-cli-service serve",
    "build": "vue-cli-service build",
    "lint": "vue-cli-service lint"
  },
```

<p> 
	Observe no código acima que você tem que adicionar é o <strong> "start" : "npm run serve" </strong> pois é esse comando que vai ser executado no docker-compose. Esse comando abaixo que vai ser executado no docker-compose
</p>

## Esse comando vai ser executado no docker-compose

```
  command: >
      sh -c "npm i && npm start"

```


## Observação
<p> Esse formato está funcionado apenas com Vue.js </p>


#Versão das Modificações

## 0.1 - Atual

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
