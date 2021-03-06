# Analyzing and planning a new Rails app

Today we will be looking at how to go about planning and thinking through a Rails application. We will be talking about some of the things that need to be done before you start coding.

## Agenda
After this lesson, you will know:

  * User Stories
  * Planning
  * Mockups
  * Modelling


## User Stories

As a ...
I want ...
So that...

- Who are the users?
- What do they need to do?
- Why do they need it? What is the goal they're trying to accomplish?







### EXAMPLES







## Prioritize
1. NEED TO HAVE
- As a user, I want to be able to post an item, add pics
- As a user, I want to be able to see all the item I posted
- As a user, I want to be able to see all the item posted to the website
- As a user, I want to be able to sign up & login
- As a user, I want to be able to see the contact information of the seller
- As a user, I want to be able to delete and update my posts
- As a user, I want to be able to update my user profile
- As a user, I want to be able to search through items


2. WANT TO HAVE
- As a user, I want to be able to sign up & login via social networks
- As a user, I want to be able to see where each item located
- As a user, I want to be able to list search result in a map
- As a user, I want to be able to filter items by attribution, to refine search
- As a user, I want to be able to sort the item by categories and attributions, and each category should have a seperate page
- As a user, I want to be able to set favorate items for later access
- As a user, I want to be able to message the seller via in-app messaging system, and details of the item should be shown in message page
- As a user, I want to be able to see all post from one users
- As a user, I want retrieve my password if I forget
- As a user, I want to set a deadline for my post
- As a user, I want to automatically remove my post after a certain time


3. NICE TO HAVE

- As a user, I want to be able to send reminder via email
- As a user, I want to set my email and other notification settings
- As a user, I want to be able to see my browsing history
- As a user, I want to be able to add friends
- As a user, I want to be able to follow anther user
- As a user, I want to be able to leave a review for other users
- As a user, I want to be able to see the reviews about a user, and his/her profile
- As a user, I want to be able to see analytics about my posts


4. MAY OR MAY NOT HAVE
- As a user, I want to be able to invite friend to the platform
- As a user, I want to be able to discuss about a particular item posted to the platform
- As a user, I want to be able to add hash-tag to my posts
- As a user, I want to be able to view by hash-tags or themes
- As a user, I want to be able to have auto-filled or preset descriptions
- As a user, I want to be able to combine my posted items into bundles
- As a user, I want to be able to view individual item in a bundle, and I can see what bundles an item is in
- As a user, I want to be able to view the pages in different languages
- As a user, I want to automatically push my post into the front page


## Define our key words
items
- price
- location
- seller_id
- pics(must have)
- title
- category_id
- post_time
- description
  - original_price(optional)
  - how_long_has_been_used(optional)
  - how many time it has been used(optional)
  - damage(optional)
  - smoke free, pet free(optional)
- deadline(optional)
- everything must go in 60 days
- views
- favorite

users
- email
- name
- wechat/weibo/qq
- password
- profile pics(has default)
- gender(optional)
- notification settings
- message account


categories
- many to many with item(at most 2)
- preset


reviews
- belongs_to: user


hash-tags/styles
- to be determined



## Tough decisions about making a reservation
- Diners and owners need to remember the reservation details
- Length of stay (Duration)
- No shows or showing up with a different party size
- Table sizes and layouts
- Difficult or impossible to contact diners
- Walk-ins, phone bookings, etc.
- Overlapping bookings




## Planning
- Make assumptions


- Make mockups
  - views
    - index

    - category.items

    - item-show
    - item-new
    - item-update
    - item-delete

    - user-show
    - user-new
    - user-update
    - user.items
    - user.favorite
    - user.browsing_history*
    - user.reviews

    - review-new
    - review-update
    - review-delete

    - login

    - search_result
    - search_result_map

    - messaging











## Modelling
- Pen and paper / Whiteboard
- Create models
- Draw relationships
- Authorization
