
# NodeJS Setup and components

## Package.JSON 

Initiate by running 
```
npm init -y
```

Frequent installs
```
npm install dotenv express body-parser express-handlebars mongoose
npm install --save-dev @types/express @types/express-handlebars @types/mongoose @types/node nodemon ts-node typescript
```

Standard Structure
```
mkdir src&&cd src
mkdir views&&mkdir middleware&&mkdir exceptions&&mkdir interfaces
cd views&&mkdir layouts&&mkdir partials&&mkdir layouts
cd ..
touch app.ts&&touch server.ts

```


### Useful scripts

```javascript
  "main": "src/server.ts",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "dev": "ts-node ./src/server.ts",
    "start": "nodemon ."
  },
```

## Express

## Typescript

initialise by
```
tsc --init
```

### Useful scripts
`tsconfig.json`

```javascript
{
  "compilerOptions": {
    "sourceMap": true,
    "experimentalDecorators": true,
    "moduleResolution": "node",
    "target": "es2017",
    "outDir": "./dist",
    "baseUrl": "./src",
    "paths": {
      "*": ["node_modules/*"]
    }
  },
  "include": [
    "src/**/*.ts"
  ],
  "exclude": [
    "node_modules"
  ]
}
```

## Nodemon
### Useful script

`nodemon.json`

```javascript
{
    "watch": ["src"],
    "ext": "ts",
    "ignore": ["src/**/*.spec.ts"],
    "exec": "ts-node ./src/server.ts"
  }
```

## Gulp

 
