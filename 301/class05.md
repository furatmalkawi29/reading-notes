#  Deploy Your Blog to Heroku


## 1- Use Node.js to build your server . 

## 2- start server at your terminal

## 3- use browser to see your server response locally , using your server address .

<br><br>


![](http://i.imgur.com/idykoj7.png)


## 4- Turn your local server into a world wide server 

## 5- Deploy your server on heroku (Heroku : cloud application platform)

## A) Create an account

## B) Steps in terminal :

## 1- Heroku installation steps

## 2- Deployment steps :


### - Open your terminal within your project folder


```
cd /path/to/my/project
```

### - Empty Git repository will be initialized in .git/ folder.:

```
git init
```


### - Then this command allows Git to track your files changes:

```
git add .

```


### -  Now commit your files to the initialized Git repo:

```
git commit -m "Simple server functionality added"
```

### - We'll create our first Heroku application now:

```
heroku create
```

### -  Now we can deploy our project. Every Heroku app starts with no branches and no code. So, the first time we deploy our project, we need to specify a remote branch to push to:

```
git push heroku master
```

### -  The application is now deployed. Ensure that at least one instance of the app is running:

```
heroku ps:scale web=1
```

### -  And now, before we open it, it's time to choose a proper name for our first creation. I called it myfirstserver:

```
heroku apps:rename myfirstserver
```

### - Everything is done. You can try it now will open your Heroku project in your web browser. :

```
heroku open
```


## - In this particular case, server address is https://myfirstserver.herokuapp.com/. Now you can share your first web application with any person you want.
