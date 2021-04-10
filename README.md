Original App Design Project - README Template
===

# Price Compare

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Description
Since the start of COVID a lot of shoppers have turned online and many have spent a good amount of money on online shopping. Because the way that online shopping is structured an item could be found on multiple different stores/websites. This app would gather the data of the prices from across multiple platforms, compare and present them to the buyer so that the buyer can spend less money.

### App Evaluation
[Evaluation of your app across the following attributes]
- **Category:** Shopping
- **Mobile:** This app would be primarily developed for mobile but would perhaps be just as viable on a computer. Functionality wouldn't be limited to mobile devices, however mobile version could potentially have more features.
- **Story:** Searches multiple websites for different price ranges of the product the customer wants to buy.
- **Market:** Any individual who is part of the online shopping community could choose to use this app.
- **Habit:** This app could be used as often or unoften as the user wanted depending on how often they online shop
- **Scope:** First we would start off with commonly used shopping websites like Amazon and then we can grow to include the multiple different websites and applications.

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**

* User logs in to access previous purchases and the browse page
* User picks what item they are planning to buy
* User has the option to go and buy off of the cheaper seller or to stick with the current seller
* Profile pages for each user
* Settings (Accesibility, Notification, General, etc.)

**Optional Nice-to-have Stories**

* A shopping cart where the user can have items they are interested in but they don't want to buy it immediately
* Browse page where the most rellevant items based off of past purchases are displayed with different prices


### 2. Screen Archetypes

* Login 
* Register - User signs up or logs into their account
   * Upon Download/Reopening of the application, the user is prompted to log in to gain access to their profile information to be properly matched with another person. 
   * ...
* Search Page - Where to input the item the user wants to buy
   * Upon input there will be options with different prices(cheapest first)
* Profile Screen 
   * Allows user to view the previously bought items
* Settings Screen
   * Lets people change language, and app notification settings.


### 3. Navigation

**Tab Navigation** (Tab to Screen)

* Browse Page
* Profile
* Settings

Optional:
* Shopping Cart

**Flow Navigation** (Screen to Screen)

* Forced Log-in -> Account creation if no log in is available
* Search bar -> Jumps to Browse Page
* Profile -> Text field to be modified. 
* Settings -> Toggle settings

## Wireframes
[Add picture of your hand sketched wireframes in this section]
<img src="YOUR_WIREFRAME_IMAGE_URL" width=600>

### [BONUS] Digital Wireframes & Mockups

### [BONUS] Interactive Prototype

## Schema 

### Models

| Property    | Type            | Description      |
| --------    | --------        | --------         |
| objectId    | String          | Unique Id for the item to sell   |
| author      | Pointer to User | Post author     |
| image       | File            | Image associated with the item to sell     |
| price       | Number          | Price of the item     |
| priceList   | Array           | List of the different prices     |
| priceCount  | Number          | Number of the different prices for the same item     |
| createdAt   | DateTime        | Date when the post is created    |



### Networking
- [Add list of network requests by screen ]

* Home Feed Screen
    * (Read/GET) Query all posts where user is author
    * (Create/POST) Create a new post
    * (Delete) Delete existing post
* Create Post Screen
    * (Create/POST) Create a new post object
* Profile Screen
    * (Read/GET) Query logged in user object
    * (Update/PUT) Update user profile image

- [Create basic snippets for each Parse network request]

![](https://i.imgur.com/skCmazd.png)

