###### rails apps deploying heroku
---


```
vi Gemfile
gem 'sqlite3', group: [:deployment, :test]
gem 'pg', group: :production

```


```
// git&heroku 
heroku create apptky4
git init
git add .
git comit -m "1st"
// New Repository - github
//: apptky4
// Create
// git remote
git remote add origin git@github.com:takagotch/apptky4.2.git // git remote
git push -u origin master
git push heroku master

```

https://apptky4.herokuapp.com/


```
```

```
```



