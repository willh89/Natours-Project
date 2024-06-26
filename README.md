<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="img/favicon.png" alt="Project logo"></a>
</p>

<h1 align="center">Natours Project</h1>

<div align="center">

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)

</div>
  
---

<p align="center"> Exciting tours for adventurous people

      
#### [Click here for live site](https://wills-natours-project.netlify.app/)

</p>


![](img/Natours-collage.png)

## 📝 Table of Contents

- [About](#about)
- [Requirements](#Requirements)
- [Installation](#Installation)
- [Usage](#usage)
- [Built Using](#built_using)
- [Authors](#authors)
- [Acknowledgments](#acknowledgement)

## 🧐 About <a name = "about"></a>

The purpose of this project was to become familiar and comfortable using SASS to compile and organise CSS.

It also helped me understand more advanced CSS techniques such as animation, how to scale or rotate images using the transform property, as well as the pre-requisites needed to ensure websites are responsive, browser compatible, and accessible.

### Requirements

You will need to install [Node.js](https://nodejs.org/en/) to run this.

Check the documentation to install it on your system.


### Installation

Once Node.js is installed, you will need several extensions to run this project.

Open the terminal/command-line in your code editor, then install the following:

```
npm install node-sass ---save-dev
```

```
npm install postcss --save-dev
```

```
npm install npm-run-all --save-dev
```

```
npm install live-server --save-dev -w
```

Once the above are installed run the following commands:

```
npm run build:css
```

```
npm run start
```

```
npm watch:sass
```
Once installed, all following commands in the **package.json** file should function correctly.  
```

"scripts": {
    "watch:sass": "node-sass sass/main.scss css/style.css -w",
    "devserver": "live-server",
    "start": "npm-run-all --parallel devserver watch:sass",
    "compile:sass": "node-sass sass/main.scss css/style.comp.css",
    "concat:css": "concat -o css/style.concat.css css/icon-font.css css/style.comp.css",
    "prefix:css": "postcss --use autoprefixer -b 'last 10 versions' css/style.concat.css -o css/style.prefix.css",
    "compress:css": "node-sass css/style.prefix.css css/style.css --output-style compressed",
    "build:css": "npm-run-all compile:sass concat:css prefix:css compress:css"
  },

package.json

```

### Usage 

Changes can be made in the components SASS folder.
Run **npm watch:sass** to see in the browser all changes made in real time. 


## ⛏️ Built Using <a name = "built_using"></a>

- HTML - Markup Language
- CSS - Stylesheets
- [SASS](https://sass-lang.com/) - CSS Preprocessor
- [Node.js](https://sass-lang.com/) - CSS Preprocessor

## ✍️ Authors <a name = "authors"></a>

- [@willh89](https://github.com/willh89) - Built by
- [@jonasschmedtmann](https://github.com/jonasschmedtmann) - Idea & Initial Work

## 🎉 Acknowledgements <a name = "acknowledgement"></a>

 [Advanced CSS Course](https://github.com/jonasschmedtmann)
