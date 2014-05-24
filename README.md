Golp

---

#Tagline
Search, Find and Share your favorite things by location!


#Technical Summary
* Uses ruby 2.1.1
* Uses gem 'rails', '4.1.1'
* Uses Postgres database
* Uses Locu API [https://dev.locu.com/](https://dev.locu.com/)
* Uses devise gem for authentication
* Uses Google Maps v3 for mapping
* Uses geocoder gem for geocoding
* Uses sidekiq gem / Redis for Email and Dashboard
* Uses bootstrap-sass gem for bootstrap version 3
* Uses jQuery
* Is deployed to Heroku with unicorn in a single dyno

---

Personas and their User Stories

---

#Persona USV : Unknown Site Visitor

---

##Story : USV Registration

__branch_name__: ```authentication```

* As an Unknown Site Visitor
* I want to be able to register with the website
* So that I can create my list of favorited items

### Feature Spec
1. Visits the home page ```/```
2. Clicks a link labeled ```Sign Up```
3. URL is ```/register```
4. Enters a valid unregistered email in the ```email``` field
5. Enters valid password in the ```password field```
6. Enters same valid password in the ```password_confirmation``` field
7. Clicks the button labeled ```Sign Up```
8. Redirect to the home page ```/```
9. Flash Message 'Thanks for signing up!' is displayed


### Technical Spec
1. Uses devise gem
2. Copy the devise views into the app before customizing them

### Resources
* [http://devise.plataformatec.com.br/](http://devise.plataformatec.com.br/)


---

##Story : USV Login

__branch_name__: ```authentication```

* As an Unknown Site Visitor
* I want to be able to login to the website
* So that I can access my list of favorited items

### Feature Spec
1. Visits the home page ```/```
2. Clicks a link labeled ```Sign In```
3. URL is ```/login```
4. Enters a valid registered email in the ```email``` field
5. Enters the valid password in the ```password field```
7. Clicks the button labeled ```Sign In```
8. Redirect to the home page ```/```
9. Flash Message 'Welcome Back!' is displayed


### Technical Spec
1. Uses devise gem

### Resources
* [http://devise.plataformatec.com.br/](http://devise.plataformatec.com.br/)


---

##Story : USV Keyword Search

__branch_name__: ```keyword_search```

* As an Unknown Site Visitor
* I want to be able to search for Spas
* So that I can add them to my list of favorited items

### Feature Spec
1. Visits the search page ```/search```
2. Enters Search Term 'Spa'
3. USV sees a list of 5 'Restaurants' sourced from Locu (name=Spa)

### Technical Spec
1. The LOCU API key must not be in the git repo
2. Use a new Form Object class called LocuSearchForm
3. Map the user's search term to the ```name``` parameter on locu

### Resources
* [https://dev.locu.com/](https://dev.locu.com/)
* [http://robots.thoughtbot.com/activemodel-form-objects](http://robots.thoughtbot.com/activemodel-form-objects)

---







