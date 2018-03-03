Collaborative filtering
=======================

Uses easily captured user behaviour data

For every User-Product combination you need metrics such as:
 * Purchases
 * Page views
 * Clicks
 * Catings
These is considered the user's affinity for X product

The algorithm will use the above to return affinity for unseen products; 
then you sort and return it.

for every User and Product we need a rating. Pick one or use multiple

Explicit rating: User provided rating; Review written
Implicit rating: Derived rating; Place chosen to eat

Represented as a matrix
```
  P1 P1 P2 P3 P4 P5
U1 3  4  -  -  -  -
U2 3  2  -  -  -  5
U3 -  2  -  5  -  -
U4 -  -  1  -  -  -
U5 -  -  -  -  4  -
U6 -  -  -  -  -  -
```

The objective of the algorithm is to fill the empty cells (-) by 
extrapolating with the valeus already filled. Ex. Nearest neighbor algorithm
