#Golp!

---

Search, Find and Share your favorite things by location!

---

#Overview

Golp! allows the user to search for geographically close resources and Favorite them

Each favorite belongs to one user, has a location (lat,lng) and address, as well as an optional
description, an optional photograph and an optional relationship to the Locu API

Users' favorites are displayed on their profile pages along with a thumbnail of the image

Resources may optionally be related to items in the Locu API


Additional functionality may be spec'd and developed by team members!

---


#Technical Summary
* Will use ruby 2.1.1
* Will use gem 'rails', '4.1.1'
* Will use Postgres database
* Will use Locu API [https://dev.locu.com/](https://dev.locu.com/)
* Will use devise gem for authentication
* Will use Google Maps v3 for mapping
* Will use geocoder gem for geocoding
* Will use sidekiq gem / Redis for Email and Dashboard
* Will use bootstrap-sass gem for bootstrap version 3
* Will use paperclip gem to add images to favorites
* Will use jQuery for client side scripting
* Will be deployed to Heroku with unicorn in a single dyno
* Will use Rspec, Capybara and Nokogiri for Feature Tests

---

#Personas

---

* USV : Unknown Site Visitor : Named: Yusef
* RU : Registered User : Named: Regina

---

#User Stories

---

#Story : USV Keyword Search

__branch_name__: ```basic_keyword_search```

* As an Unknown Site Visitor
* I want to be able to search for Spas
* So that I can add them to my list of favorited items

## Feature Spec
1. Visits the search page ```/search```
2. Enters Search Term 'Spa'
3. USV sees a list of 5 'Restaurants' sourced from Locu (name=Spa)

## Technical Spec
1. The LOCU API key must not be in the git repo
2. Use a new Form Object class called LocuSearchForm
3. Map the user's search term to the ```name``` parameter on locu

## Resources
* [https://dev.locu.com/](https://dev.locu.com/)
* [http://robots.thoughtbot.com/activemodel-form-objects](http://robots.thoughtbot.com/activemodel-form-objects)
* [https://github.com/typhoeus/typhoeus](https://github.com/typhoeus/typhoeus)
---


#Story : USV Registration

__branch_name__: ```authentication```

* As an Unknown Site Visitor
* I want to be able to register with the website
* So that I can create my list of favorited items

## Feature Spec
1. Visits the home page ```/```
2. Clicks a link labeled ```Sign Up```
3. URL is ```/register```
4. Enters a valid unregistered email in the ```email``` field
5. Enters valid password in the ```password field```
6. Enters same valid password in the ```password_confirmation``` field
7. Clicks the button labeled ```Sign Up```
8. Redirect to the home page ```/```
9. Flash Message 'Thanks for signing up!' is displayed


## Technical Spec
1. Uses devise gem
2. Copy the devise views into the app before customizing them

## Resources
* [http://devise.plataformatec.com.br/](http://devise.plataformatec.com.br/)


---

#Story : USV Login

__branch_name__: ```authentication```

* As an Unknown Site Visitor
* I want to be able to login to the website
* So that I can access my list of favorited items

## Feature Spec
1. Visits the home page ```/```
2. Clicks a link labeled ```Sign In```
3. URL is ```/login```
4. Enters a valid registered email in the ```email``` field
5. Enters the valid password in the ```password field```
7. Clicks the button labeled ```Sign In```
8. Redirect to the home page ```/```
9. Flash Message 'Welcome Back!' is displayed


## Technical Spec
1. Uses devise gem

## Resources
* [http://devise.plataformatec.com.br/](http://devise.plataformatec.com.br/)

---








