# Instructions to deploy an R app

1. Clone this repo locally:

```
git clone git@github.com:firasm/dashR_deployed.git
```

2. Change directory into the cloned repo:

```
cd dashR_deployed
```

3. Using the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli) create a Heroku App **AND** set the stack to container:

```
heroku create --stack container your-app-name
```

4. Push the app to heroku and this branch

```
git push heroku main
```

5. Navigate to your-app-name.herokuapp.com in your browser!

## Known issues

- I am trying to upgrade the version of R to 4.1 so that the native pipe can be used.
- It takes a LONG time for the app to deploy the first time (~ 20 minutes)
