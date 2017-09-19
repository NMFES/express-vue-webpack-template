# Simple template based on ExpressJS / VueJS / Webpack

This template consists of two other separate templates:
* [Webpack-simple](https://github.com/vuejs-templates/webpack-simple)
* Template that generates "[express-generator](http://expressjs.com/en/starter/generator.html)" with ejs

## What's included?
* Express 4
* Vue JS 2
* SocketIO
* MondoDB driver + Mongoose
* Webpack 3
* Bootstrap 4 (beta)
* FontAwesome
* Sass


## Installation

For installing you should run next commands:
* `git clone https://github.com/NMFES/express-vue-webpack-template.git`
* `cd express-vue-webpack-template`
* `npm install`
* `sudo npm install nodemon -g`

Also you need to install MongoDB

... and something else you need to do. If i forgot something :)


## Usage

You should manualy open two terminals. In the first one you run Webpack in dev-mode. In that mode Webpack will open browser with URL "http://localhost:8080" and will be waiting for changes in "/webpack" directory. All css/js files in that mode Webpack storages in memory (not on the hdd). 

In the second terminal you run Express in dev-mode Nodemon. It will be opened via Nodemon and will listen "http://localhost:3000". Express will be waiting for changes in "/express" directory. Remember, at this stage all static files (css/js) is serving by Webpack and storaging in memory. Express doesn't know about them. Do some work, write code etc. Webpack/Express will watching for changes and will reload if needed.

When you're ready to production you run Webpack in prod-mode. He will precess all static files and will save them into "/express/public" dir. You should run this command when you're ready to upload your site on remote host. Then you run Express in prod-mode (on remote server). He will serve css/js-files (not Webpack). After that all requests should coming to "http://localhost:3000".

``` bash
#dev-mode
npm run webpack-dev

#prod-mode
npm run webpack-prod

#dev-mode
npm run express-dev

#prod-mode
npm run express-prod
```
