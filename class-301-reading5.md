# Heroku - Deploy your blog to Heroku

- brew install heroku/brew/heroku
- heroku login
* node --version
* npm --version
* git --version


* Cloning a sample applicaiton
- git clone https://github.com/heroku/node-js-getting-started.git
cd node-js-getting-started

## Deploy the site

- heroku create

- (Deploy code) git push heroku main

- (Ensure one instance of the app is running) heroku ps:scale web=1

- Open the app `heroku open`

- (View logs) heroku logs --tail

### Node.js

> We will use Node.js for our project. Node.js is an open source, cross-platform runtime environment, which allows you to build server-side and networking applications. It's written in JavaScript and can be run within the Node.js runtime on any platform. First of all, of course, you need to install it. You'd better check the download page for more details. I'll wait until you finish, so don't worry. Is it done? Great! Now you can create your first web server. And it will be one of the easiest tasks in your life.

- Create .js file
- use (node 'filename.js') to run it
- Open local host 3000 to check to see if the server works


Reference:  https://howtonode.org/deploy-blog-to-heroku