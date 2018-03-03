Concerns
========

Content based filtering:
 **What attributes should I use?**
 Has an emphasis on using the right product attributes.
 Only use those attributes that influence user prefference.

 Once you choose them; meassure them

**How to meassure similarity of products?**
 1. Setup a rating/weight db add entries for each product.
    These ratings should be fixed scale (1..10) or (1..5)
    These ratings are Points in N-Dimensional Space
```
      |  * "Lord of The Rings" 
      |    \  -> distance == how similar they are
      |      * "The hobit"
      |_ _ _ _ _
     /
   /
```

 **Algorithm implementation:**

  User > Box > Recommended products

 1. Given an user input; get rating for each product from db they've liked/purchased
 2. Rate the user on the importance factor; ex. Average of ratings of products that they like
 3. Calculate distance using known math equation

```
     | * ---> ProductA    Then product A should be recommended  
    *|   * User 
     |*      *
     |_ _ _ _ _ _ 
    /
  /
```
