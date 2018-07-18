# 401-Front-End-Lab-Scaffolding Steps 
### Last Update: Monday July 16

## CD into your repo, then copy-paste this block of code into your terminal and the magic will happen
```
mv README.md LAB.md

mkdir src
mkdir src/components
mkdir src/style
mkdir src/lib

touch src/main.js
touch src/style/main.scss
touch src/lib/utils.js

npm init -y

curl -o README.md https://raw.githubusercontent.com/ashtonkellis/401-Lab-Scaffolding/master/readme-template.md

curl -O https://raw.githubusercontent.com/codefellows/seattle-javascript-401d25/master/00-FRONTEND-lab-scaffold-template/.babelrc
curl -O https://raw.githubusercontent.com/codefellows/seattle-javascript-401d25/master/00-FRONTEND-lab-scaffold-template/.eslintignore
curl -O https://raw.githubusercontent.com/codefellows/seattle-javascript-401d25/master/00-FRONTEND-lab-scaffold-template/.eslintrc.json
curl -O https://raw.githubusercontent.com/codefellows/seattle-javascript-401d25/master/00-FRONTEND-lab-scaffold-template/.gitignore
curl -O https://raw.githubusercontent.com/codefellows/seattle-javascript-401d25/master/00-FRONTEND-lab-scaffold-template/.travis.yml
curl -O https://raw.githubusercontent.com/codefellows/seattle-javascript-401d25/master/00-FRONTEND-lab-scaffold-template/webpack.common.js
curl -O https://raw.githubusercontent.com/codefellows/seattle-javascript-401d25/master/00-FRONTEND-lab-scaffold-template/webpack.dev.js
curl -O https://raw.githubusercontent.com/codefellows/seattle-javascript-401d25/master/00-FRONTEND-lab-scaffold-template/webpack.prod.js

code .

```

this part is not your terminal/bash. 
you have to open the package.json file and copy paste this JSON directly nested in the object
```
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "watch": "webpack-dev-server --config webpack.dev.js",
    "build": "webpack --config webpack.prod.js",
    "lint": "eslint --fix **/*.js"
  },
    "devDependencies": {
    "babel-core": "^6.26.3",
    "babel-eslint": "^8.2.5",
    "babel-loader": "^7.1.5",
    "babel-plugin-transform-object-rest-spread": "^6.26.0",
    "babel-preset-env": "^1.7.0",
    "babel-preset-react": "^6.24.1",
    "babel-preset-stage-0": "^6.24.1",
    "css-loader": "^1.0.0",
    "enzyme": "^3.3.0",
    "enzyme-adapter-react-16": "^1.1.1",
    "eslint": "^5.1.0",
    "eslint-config-airbnb-base": "^13.0.0",
    "eslint-plugin-import": "^2.13.0",
    "eslint-plugin-jest": "^21.17.0",
    "eslint-plugin-react": "^7.10.0",
    "html-webpack-plugin": "^3.2.0",
    "jest": "^23.4.0",
    "mini-css-extract-plugin": "^0.4.1",
    "node-sass": "^4.9.2",
    "prop-types": "^15.6.2",
    "react": "^16.4.1",
    "react-dom": "^16.4.1",
    "sass-loader": "^7.0.3",
    "style-loader": "^0.21.0",
    "webpack": "^4.16.0",
    "webpack-cli": "^3.0.8",
    "webpack-dev-server": "^3.1.4",
    "webpack-merge": "^4.1.3"
  },
  "dependencies": {
    "dotenv": "^6.0.0",
    "superagent": "^3.8.3"
  }
```

Then run `npm i`
