- MODELS
  - items
    1. belongs_to: user
    2. belongs_to: category
    2. has_and_belongs_to_many: buyers
    - price
    - location
    - pics(must have)
    - title
    - post_time
    - description
      - original_price(optional)
      - how_long_has_been_used(optional)
      - how many time it has been used(optional)
      - damage(optional)
      - smoke free, pet free(optional)
    - deadline(optional)
    - everything must go in 60 days
    - views count
    - favorite count

  - users
    1. has_many: items
    2. has_and_belongs_to_many: items
    - email
    - name
    - wechat/weibo/qq
    - password
    - profile pics(has default)
    - gender(optional)
    - notification settings
    - message account


  - categories
    1. has_many: items
    1. has_many: sub_categories
    - many to many with item(at most 2)
    - preset


  reviews
  1. belongs_to: user


1. FIRST ITERATION
  - item CRUD
  - user CRUD
  - category CRUD
  - sessions
  - list items

2. SECOND ITERATION
  - search by attributes
  - list user.item
  - sort by categories, attributes
  - search filter

3. THIRD ITERATION
  - see all post from one users
  - see where each item located
  - list search result in a map
  - favorite

4. FORTH ITERATION
  - sign up & login via social networks
  - message the seller via in-app messaging system, and details of the item should be shown in message page

5. FIFTH ITERATION
  - email confirmation
  - email settings
  - retrieve password

6. SIXTH ITERATION
  - deadline
  - auto-expire
