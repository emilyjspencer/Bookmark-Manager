# Bookmark Manager

### Week 4 Project at Makers Academy.

We were tasked with building a bookmark manager that stores a collection of bookmarks as
URLs.


 
## User Stories

 ```
 As a user,
 So I can view my most-used websites,
 I want to view a list of bookmarks

 As a user,
 So I can retrieve my most-used websites at a later date,
 I want to to be able to store these websites 
 ```



 ## Databases Setup

 * **Connect to psql:**

 ```
 brew install postgresql

 brew services start postgresql

 psql postgres
 ```

 * **Create the database and test database:**

development database:

```html
CREATE DATABASE bookmark_manager;
```

test database:

```html
CREATE DATABASE bookmark_manager;
```

Connect to the database

```html
\c bookmark_manager;
```

Run the following migrations. which can be found in the db/migrations subfolder: 

```html
 CREATE TABLE bookmarks(id SERIAL PRIMARY KEY, url VARCHAR(60));
```

Repeat for the test database

### How to use:

**Clone this repository:**

```html
git clone https://github.com/emilyjspencer/Bookmark-Manager.git
```

**cd into the repo**

**Run**

```html
bundle install
```

**Start the server:**

```html
rackup
```

**Go to localhost:9292**

### How to run the tests:

```html
rspec
```

### Built with:

* Ruby
* Sinatra
* HTML/CSS
* SQL

### Tested with:

* RSpec
* Capybara

### What it looks like:


