# jenkins-test

## Criar um repositorio no GitHub
```
git clone *<repository_url>*
```

## Configuração inicial na pasta do GitHub
Criar o arquivo package.json
```
npm init 
```
Depois de configurar o package.json, editar e colocar no "scripts"
```
"start": "node index.js",
"test": "jest"
```
# Index.js
```
const express = require("express");

const app = express();

app.get("/", (req, res) => {
  res.status(200).json("Hello world");
});

module.exports = app.listen(process.env.PORT || 4000, () =>
  console.log(`Running on http://localhost:4000`)
);

```
## Teste com Jest

```
npm install --save-dev jest supertest
```
Criar a pasta __test__ e o arquivo index.test.js 





