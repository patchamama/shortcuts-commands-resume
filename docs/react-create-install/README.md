# React installation with basic configuration using vite

### Install React

```
npx create-react-app .
npm install
```

#### The application is started as follows

```
npm start
```

Runs the app in the development mode.\
Open [http://localhost:5173](http://localhost:5173) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

_If there is errors with modules, maybe reinstall all the modules for scratch: `rm -rf node_modules/ && npm i`_

### Install extra libraries

#### Install json-server

```
npm install json-server --save-dev
```

#### To fetch data can be used axios [See more details](https://fullstackopen.com/en/part2/getting_data_from_server#axios-and-promises)

```
npm install axios
```

#### To validate type of data in JS [See more details](https://fullstackopen.com/en/part5/props_children_and_proptypes#prop-types)

```
npm install prop-types
```

#### To ESlint [See more details](https://fullstackopen.com/en/part5/props_children_and_proptypes#e-slint)

```
npm install --save-dev eslint-plugin-jest
```

_The configuration file to ESLint is [.eslintrc.cjs](.eslintrc.cjs)_

#### To Testing [See more details](https://fullstackopen.com/en/part5/testing_react_apps#rendering-the-component-for-tests)

```
npm install --save-dev @testing-library/react @testing-library/jest-dom jest-environment-jsdom @babel/preset-env @babel/preset-react  @testing-library/user-event
```

#### End to end testing with Cypress [See more details](https://fullstackopen.com/en/part5/end_to_end_testing#cypress)

```
npm install --save-dev cypress
npm install eslint-plugin-cypress --save-dev
```

_Execute the test with: `npm run cypress:open`_

#### Available Scripts

In the project directory, you can run:

- start: `react-scripts start`
- build: `react-scripts build`
- test: `react-scripts test`
- eject: `react-scripts eject`
- lint: `npm run lint`
- preview: `npm run preview`
- json-server: `npm run server`
- cypress test: `npm run cypress:open`
- cypress e2e test: `npm run test:e2e`

## Deployment

```
npm run build
```

### Install and run deployment server (to serve it with a static server)

```
npm install -g serve
serve -s build
```

# Credits

- Relative path in index.html after build: https://stackoverflow.com/questions/46235798/relative-path-in-index-html-after-build
