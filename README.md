
# Teste de Software Javascript - Jest, sucrase e integração contínua com CircleCI

[![CircleCI](https://circleci.com/gh/circleci/circleci-docs.svg?style=svg)](https://circleci.com/gh/circleci/circleci-docs)

### Criar o package.json
```
npm init -y
```

### Criar a estrutura de pastas
```
mkdir src
mkdir test
cd src
mkdir model
mkdir service
```

### Instalar o nodemon
```
npm i nodemon -D
```

### Instalar o jest
```
npm install --save-dev jest
```

### Instalar o sucrase
```
npm install --save-dev sucrase
```

### Criar um script de build no package.json
```
 "scripts": {
    "test": "jest",
    "build": "sucrase ./src -d ./dist --transforms imports",
    "dev": "nodemon src/app.js",
    "start": "node dist/app.js"
  },

Testar o script
npm run build
```

### Instalar a dependência do express
```
npm i express
```

### Instalar o plugin sucrase
```
npm i @sucrase/jest-plugin -D
```

### Rodar testes
```
npm test
```
