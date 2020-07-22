###### rails apps deploying heroku
---



```
git clone git@gitub.com:takagotch/apptky4.1.2.git
cd apptky4.git
heroku create apptky4.1.2










```


```
// git&heroku 
heroku create apptky4
git init
git add .
//
vi Gemfile
gem 'sqlite3', group: [:deployment, :test]
gem 'pg', group: :production
//
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

---
###### 


```
```

```
```



