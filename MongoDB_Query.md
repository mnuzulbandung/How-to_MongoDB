
# **MongoDB Query or Filter**

## **A. Comparison Operator**
1. Filter documents where the genres field has Comedy
    ```json
    {"genres": "Comedy"}
    ```

2. Filter documents where the genres field that only has Comedy
    ```json
    {"genres": ["Comedy"]}
    ```

3. Filter documents where the age field is greater than 25:
    ```json
    { "age": { "$gt": 25 } }
    ```
* Other:
  * `$eq` : equal to
  * `$gt` : greater than
  * `$lt` : lower than
  * `$gte` : greater than or equal to
  * `$lte` : lower than or equal to
  * `$ne` : not equal to

4. Filter documents where the age field is greater than 25 and lower than 30
    ```json
    {"age": {$gt:25, $lt:30}}
    ```

## **B. Logical Operators**
1.  Filter documents where status is "active" and age is greater than 25
    ```json
    { "$and": [ { "status": "active" },
                { "age": { "$gt": 25 } } ] }
    ```
* Other:
  * `$and`: AND operator
  * `$or`: OR operator
  * `$not`: NOT operator

## **C. Inclusion and Exclusion**
1. Filter documents where category is either "electronics", "furniture", or "book"
    ```json
    { "category": { "$in": ["electronics", "furniture", "book"] } }
    ```
* Other:
  * `in`: IN operator
  * `nin`: NOT IN operator


## **D. Pattern Matching**
1. Filter documents where the name field starts with "John"
    ```json
    { "name": { "$regex": "^John", "$options": "i" } }
    ```

    * `"$regex": "^John"`: Mencari kata berawalan dengan John
    * `"$options": "i"`: Membuat pencarian kata case-insensitive

## **E. Checking Field Presence**
1. Filter documents where the email field exists. Ubah `true` menjadi `false` jika ingin mencari document tanpa field tertentu.
    ```json
    { "email": { "$exists": true } }
    ```

## **F. Multiple Conditions**
1. Filter documents where status is "active", AND age is greater than 30, AND category is "electronics"
    ```json
    { 
      "status": "active",
      "age": { "$gt": 30 },
      "category": "electronics"
    }
    ```

## **G. Nested Query**
1. Filter Documents that has nested field

    ```json
    {"imdb.rating": {$gt: 7}}
    ```

