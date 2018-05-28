# React Forms
This is a lesson about ReactJS Forms. Please follow the steps below to get started.

## Get Started
### 1. Create React App
```
create-react-app react-forms
```
### 2. cd into app directory
```
cd react-forms
```
### 3. Open In Visual Studio Code
```
code .
```
### 4. Install Dependencies
- StyleGuidist
```
npm install --save-dev react-styleguidist
```
- Semantic-UI-React
```
npm install semantic-ui-react
```
- Semantic-UI-CSS
```
npm install semantic-ui-css
```
- WebPack: See next step

### 5. Add WebPack to your package.json
After installing dependencies, place the following line of code under devDependencies in your package.json
```
"webpack": "^3.8.1" 
```
### 6. npm install
```
npm i
```
### 7. Add the following to index.js
```
import 'semantic-ui-css/semantic.min.css';
```
### 8. Create directories and files
```
mkdir src/components
mkdir src/styles
touch src/styles/styleguidist.css
touch styleguide.config.js
```
#### 9. Copy code below to styleguide.config.js 
```js
module.exports = {
    components: 'src/components/**/*.js',
    // ignore: ['**/components/views/*.js'],
    ribbon: {
      url: 'http://github.com/drteresavasquez',
      text: 'See App In Action'
    },
    template: {
      favicon: './public/favicon.ico',
      head: {
        links: [
          {
            rel: 'stylesheet',
            href: './node_modules/semantic-ui-css/semantic.min.css'
          },
          {
            rel: 'stylesheet',
            href: './src/styles/styleguidist.css'
          }
        //   {
        //     rel: 'stylesheet',
        //     href: './node_modules/font-awesome/css/font-awesome.min.css'
        //   }
        ]
      }
    },
    theme: {
        color: {
          link: 'white',
          linkHover: 'salmon',
          sidebarBackground: '#000000',
        },
        fontFamily: {
          base: '"Droid Sans"',
        }, 
        fontSize:{
          small: 13,
        }
      }
};
```# react-forms