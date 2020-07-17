# HEROKU

- Heroku lets you deploy, run and manage applications written in Ruby, Node.js, Java, Python, Clojure, Scala, Go and PHP.

![](https://miro.medium.com/max/880/1*BkLhZ0WrXPhYEqX-nmMZcg.png)

- An application is a collection of source code written in one of these languages, perhaps a framework, and some dependency description that instructs a build system as to which additional dependencies are needed in order to build and run the application.

- Dependency mechanisms vary across languages: in Ruby you use a Gemfile, in Python a `requirements.txt`, in `Node.js` a `package.json`, in Java a pom.xml and so on.

- The source code for your application, together with the dependency file, should provide enough information for the Heroku platform to build your application, to produce something that can be executed.

- When you create an application on Heroku, it associates a new Git remote, typically named heroku, with the local Git repository for your application.

As a result, deploying code is just the familiar git push, but to the heroku remote instead:

`git push heroku master`