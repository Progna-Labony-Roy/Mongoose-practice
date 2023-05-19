## Task 1: Find all users who are located in New York.

## Task 2: Find the user(s) with the email "johndoe@example.com" and retrieve their favorite movie.
```
db.practice.find({ $and :[
    {  "email": { $eq: "johndoe@example.com"}},
   {"favorites.movie" : { $exists: true}}
    ]})
    .project({ "email" :1 , "favorites.movie":1})

```
## Task 3: Find all users with "pizza" as their favorite food and sort them according to age.

## Task 4: Find all users over 30 whose favorite color is "green".

## Task 5: Count the number of users whose favorite movie is "The Shawshank Redemption."

## Task 6: Update the zipcode of the user with the email "johndoe@example.com" to "10002".

## Task 7: Delete the user with the email "alicewilliams@example.com" from the user data.

## Task 8: Group users by their favorite movie and retrieve the average age in each movie group.

## Task 9: Calculate the average age of users with a favorite " pizza " food.
