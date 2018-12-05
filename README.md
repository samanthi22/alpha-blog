# README

alpha-blog with root_path and /about path

> rm -rf config

to undo with git

> git status

> git checkout -f

config directory is back, change undone

> git remote -v

(to check if git remote add origin which)

> git add -A

---

(deploy using heroku - isntall heroku toolbelt cli) 

update npm

> nvm i v8

install heroku cli

> npm install -g heroku


---

(setup for deployment to heroku) 

move the sqlite3 gem to :development, :test

add the following lines:

```ruby 
group :production do
   gem 'pg'
   gem 'rails_12factor' # not necessary for rails 5
end
```

then do:

> bundle install --without production

---

login into heroku

> heroku login --interactive

---

> heroku create

--- 

> heroku keys:add

---

> git push heroku master

--- 

(rename app to alpha-blog)

> heroku rename alpha-blog-samanthi22

---

[deployed to heroku link](https://hidden-castle-54450.herokuapp.com/)


