# RSS-Browser

  - Cross Device Support.
  - Easy to include.
  - Easy to use.

> 

### Dependencies

Here's what's used:

* Github - Hosting the reader.
* Heroku - Hosting the proxy.
* CORS-Anywhere - CORS Headers proxy.

### Menu Array

* Simple Array Structure in rss.js

`{ cli : "(unique)", ver : "category, desc : "description", api : "url", external : "external" },`

### Sourcing

Include an iframe in your html with the [site](https://acktic.github.io).

`<iframe class="rss" src="https://acktic.github.io"></iframe>`

Specify an Initial category

* News
* Style
* Social
* Sports
* Technology
* World


This would be for default dark with category Technology.

`<iframe class="rss" src="https://acktic.github.io?dark=1&cat=Technology"></iframe>`

### Styling
<p align="center"><img src="https://ackti.files.wordpress.com/2019/11/2586808985927.png"></p>
<p align="center"><img src="https://ackti.files.wordpress.com/2019/11/3842359093289.png"></p>

### Variables
| Name | Use |
| ------ | ------ |
| dark | Dark mode |
| rss | get != pop |
| sel | .cat Selected |
| tap | Touchstart/Click |

### Classes
| Name | Use |
| ------ | ------ |
| .con | Container |
| .tag | .cat Parent |
| .cat | Category |
| .out | Output |
| .get | get() |
| .pop | .sel Populate |
| .xml | .out Elements |
| .bar | Buffer/Toggle |
| .fav | Pop/Random |

### Functions
| Name | Use |
|------|------|
| url | window.open() |
| scr | Scroll element:last |
| pop | .out sel Append |
| xhr | .xml get() |
| app | Previously applyColors() |
| ran | Random |
| get | Ajax Request |
  

### Cloning and app()

 - Replace https://acktic.github.io/rss.js in index.html's `<script src=>` with the local rss.js for menu editing. 

 - var sel = "Category"

 - app(false) uses transparent background and black foreground.
  
` $("body").css({"background-color":"transparent","color":"#000000"})`

 - app(true) uses black background and white foreground.
 
`$("body").css({"background-color":"#000000","color":"#FFFFFF"})`
 
### CORS Proxy

- Heroku's CORS Proxy
`http://cors-anywhere.herokuapp.com/`

- Personal Heroku CORS-Anywhere Instance
`https://salty-refuge-64158.herokuapp.com/`

[cors-anywhere](https://github.com/Rob--W/cors-anywhere) is a reverse proxy which adds CORS headers to the request.

[heroku-cli](https://github.com/heroku/cli) makes it easy to create apps directly from the terminal.

[npm](https://github.com/npm/cli) the package manager for JavaScript.

```sh
git clone https://github.com/Rob--W/cors-anywhere.git
cd cors-anywhere/
npm install
heroku create
git push heroku master
```

### Development

Want to contribute? Great!
- Clone this Repo
- Submit a Feed
- File an issue

License
----

MIT
