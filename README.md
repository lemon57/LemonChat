# README
**Chat application on RoR, JS and CSS without Asset Pipeline.**

Ruby on Rails application with minimal authentication and ActionCable. Different approach to build front-end on Ruby on Rails. 

Stack: *Rails, JavaScript and CSS.* </br>
Without Asset Pipeline, Sprockets, CoffeeScript and Sass. 

## Got followings skills:
1. initialized project with `webpacker gem` and set of modern tools:
    + node_modules,
    + package.json as well as yarn.lock,
    + .babelrc,
    + .postcssrc.yml - allow you to use all the features described in cssnext.</br>
    `rails new evil_chat --skip-coffee --skip-sprockets --skip-turbolinks --webpack --database=postgresql  -T`
2. using `hivemind` to launch the server,
3. choose `Prettier` as code formatter,
4. set up the automated linting with **ESLint**, so my code style is always kept in check
5. using `stylelint` to detect errors and convention violations in the stylesheets - use normalize.css for that, 
6. creating required Components. Each component is represented by a folder inside the `frontend` part of our application. It consists of three files: 
    + an .erb partial, 
    + a .css stylesheet and 
    + a .js script
7. using **Action Cable** - integrates WebSockets in Rails, allowing you to write server-side logic in Ruby and client-side in JavaScript,
8. deploying to **Heroku**
    + using *Heroku CLI*
    + enable *Redis* in production in order for *Action Cable* to work on *Heroku*
    + using *Heroku Redis* Addon </br>
    + deploy: </br>
      `git add . && git commit -m "prepare for deploy"`</br>
      `git push heroku master`</br>
      `heroku run rails db:migrate`</br>
      `heroku open`
