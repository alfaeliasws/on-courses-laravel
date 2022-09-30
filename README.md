# MY PERSONAL PROJECT AS A TEST FROM ONE OF THE COMPANY THAT CONTACTED ME
![2022-09-30 21 14 50 127 0 0 1 001dfde4a5f1](https://user-images.githubusercontent.com/105652124/193289464-473296a2-a039-4699-b2bd-ec38ebd1d6a0.png)
![2022-09-30 21 15 34 127 0 0 1 81104fefa1be](https://user-images.githubusercontent.com/105652124/193289573-af8e280d-36a3-4f74-90f9-f34fcc5ee55d.png)
![2022-09-30 21 16 08 127 0 0 1 bfb28e8c7a27](https://user-images.githubusercontent.com/105652124/193289708-9e392924-9a52-4218-8a12-ab4e23ceeb43.png)

## Stack
* Laravel / PHP
* PHP
* TailwindCSS

## Back-End Features Progress: 90%
* Login/Logout
* Admin (assignment via mySQL Query, can't be via website/api)
* User
* Web Routes/Controller (For Front End Development)
    * Guest / User
    * Admin
        * Dashboard
            * See simple stats
            * See all user
            * Delete Non Admin User
        * CRUD the Listings
            * CRUD operations (delete, update, store)
            * view roles/controllers (dashboard, create form, update from)

* Api Routes/Controller
    * Guest
        * see all listings : GET /api/listing
        * see a listing detail (show) : GET /api/listing/{listing}
    * User
        * All Category : GET /api/getallcategories
        * Popular Category : GET /api/getPopularCategories
        * Filter Courses By Category : GET /api/getcategories/{category}
        * Search : GET /api/s?search={params}
        * Sort by Lowest Price : GET /api/sort/lowestprice
        * Sort by Highest Price : GET /api/sort/highestprice
        * Price equals to zero (Free) : GET /api/free
    * Admin
        * store: POST /api/listings (use body with this parameter: name, picture, tags, price, description)
        * update: PUT /api/listings/{listing} (use body with this parameter: name, picture, tags, price, description)
        * delete: DELETE (or POST with _method: DELETE in the body) /api/listings/{listing}
        * delete user (soft delete): DELETE (or POST with _method: DELETE in the body) /api/userdelete/{user}
        * simple statistic: GET /api/getsimplestats

## Back-End Development Homework
* Still in the middle to upload pictures with Cloudinary, facing some bugs so I draw back to using store in storage/image (storage/link public)

## Front-End Development (70% progress)
* 12 views 
* components
    * layout
    * card
    * categories
    * search bar
    * nav bar
    * flash message
* TailwindCSS full design with flexbox approach and many custom configs
* fade animation with JS interaction.observer

## Front-End Development Homework
* Applying part of APIs to the features like sort, and displaying all categories/popular categories

## Challanges of this projects
* Facing many bugs and debugging it
* Authorization with api, end up using web middleware in api so I can acccess the user then I can authenticate it based on their stored information
* Learning so much about middleware and route
* Deeper with php artisan to know that route actions doesn't properly refreshed with reload
* Wrestling with API doesn't returning JSON because of authentication problems

Link: Still can be run locally with php artisan serve after migration, still debugging in deployment to heroku especially with Procfile (web: vendor/bin/heroku-php-apache2 public/ not found in heroku log --tail) 
