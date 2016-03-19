# near.farm

Database Design:
```
farms
  id
  name
  address1
  address2
  city
  state
  zip
  location (point, requires MySQL 5.6)
  phone
  email
  profile
  header
  thumbnail
  theme
products
  id
  name
  thumbnail
  image
  description
shoppers
  id
  name
  address1
  address2
  city
  state
  zip
  username
  password
shoppersToLocations
  shopperId
  location
  date
shoppersToProducts
  shopperId
  productId
  date
shoppersToFarms
  shopperId
  farmId
  date
farmsToProducts
  farmId
  productId
  description
  price
  unit
farmsToAbout
  farmId
  about
  updatedDate
farmsToHome
  farmId
  home
  updatedDate
farmsToContact
  farmId
  contact
  updatedDate
farmsToReviews
  shopperId
  farmId
  productId1
  productId2
  productId3
  productId4
  productId5
  rating
  content
viewsToLocations
  viewId
  shopperId
  farmId
  productId
  page
  location

```
