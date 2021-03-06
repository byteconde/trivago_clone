# Rails Trivago Clon

## Documentation:

### 1) Installation

- Create an empty directory (it's up to you)
- To clone, type in your terminal: 
```
git clone git@github.com:codeableorg/rails-trivago-clon.git
```
- Delete Gemfile.lock (Just to avoid some errors, it will be autogenerated again when you run 'bundle install')
- Run: 
```
bundle install
```
- Then Run: 
```
bin/rails db:drop
```
- Then Run:
```
bin/rails db:setup
```
- Yayyy! It's done, it's ready to be used

### 2) Usage

- To fully enjoy Trivago Clone, add a .env file

  * Create .env file
  * Copy our .env_example template that we did for you
  * You will need some credentials, if you have it, past it.


- You need to have a key generated by Facebook, follow these instructions

  * Go to https://developers.facebook.com/
  * Click on My Apps and create an app
  * Go to your recent and click in Settings > Basic
  * Copy your APP ID and APP SECRET
  * You will need both credentials for get authenticated
  * Copy both credentials in .env file
  
- You need also a key generated by Github, follow this instructions

  * Log in Github
  * Go to Settings > Developer Settings > OAuth Apps > New OAuth App
  * Set up your App Name and more details
  * When you finish, Github will provide you an APP ID and APP SECRET
  * You will need both credentials for get authenticated
  * Copy both credentials in .env file
- Generate your email credentials. Again, we prepared this awesome tutorial for you. Follow these steps

  * Go to [https://myaccount.google.com/security](https://myaccount.google.com/security) and select `App passwords` option.

  * Note: You should activate two-factor authentication in your Gmail account.

  * In `Select App`, select `Other(Custom name)`. Write a custom name like `Local web app`
  * Click on `Generate`. Copy the generated password, and click on `Done`
  * Copy your app password in your .env file

- Finally, run: 
```
rails server
```
or 
```
rails s
``` 

### 3) Recommendations

- Don't forget to run: db:drop, db:setup and bundle install before start using Trivago Clone
- Don't forget to install imagemagick
```
brew install imagemagick
```

- If you want to have more admins o users, feel free to modify seeds.rb
- If you modify seed.rb, execute again the commands from installation (drop,setup) and then run this command:
```
bin/rails db:seed
```


### 4) Contributing

- Feel free to send your PR 👮🏻‍
