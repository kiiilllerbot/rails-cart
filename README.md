# README
A simple Rails Ecommerce App Integrated with Paypal & Stripe Payment.

# Basic Interface (Stripe Payment)
![alt text](https://i.imgur.com/0RyrUuH.png)

# Basic Interface (PayPal Payment)
![alt text](https://i.imgur.com/OFoWSTv.png)


* Ruby version: 2.7.5

* Rails version: 5.2.3

* Node version: 16.3.1

* Development Database: SQLite


# Instructions to run in your Local Machine:
*(1) Clone the Repo.

*(2) Install all the dependencies. Run
```
bundle install
```
*(3) Create and Migrate Database. Run
```
rails db:create
rails db:migrate
```
*(3) Add Paypal & Stripe Credentials on config/application.yml file:
```
test: &default
  PAYPAL_ENV: sandbox
  PAYPAL_CLIENT_ID: 	 	YOUR_CREDENTIAL_HERE
  PAYPAL_CLIENT_SECRET: 	YOUR_CREDENTIAL_HERE
  STRIPE_PUBLISHABLE_KEY:	YOUR_CREDENTIAL_HERE
  STRIPE_SECRET_KEY: 	YOUR_CREDENTIAL_HERE
development:
  <<: *default
```
*(4) Spin up your local development server. Run
```
rails s
```