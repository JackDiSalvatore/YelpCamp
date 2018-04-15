# YelpCamp App

From the web developer bootcamp
View at : https://yelpcamp-jd.herokuapp.com/


## DESIGN

RESTFUL ROUTES: a mapping between HTTP routes and CRUD

CREATE
READ
UPDATE
DESTROY
```
name       url                  method     desc.                                  Mongoose Method
--------------------------------------------------------------------------------------------------------------
INDEX     /campgrounds           GET      Display all campgrounds               campground.find()
NEW       /campgrounds/new       GET      Display form to make new campground   N/A
CREATE    /campgrounds           POST     Add new campground to DB              campground.create()
SHOW      /campgrounds/:id       GET      Shows info about one campground       campground.findById()
EDIT      /campgrounds/:id/edit  GET      Edit form for one campground          campground.findById()
UPDATE    /campgrounds/:id       PUT      Update an individual campground       campground.findByIdAndUpdate()
DESTROY   /campgrounds/:id       DELETE   Delete an individual campground       campground.findByIdAndRemove()
```

## HOW TO RUN

* Set your database with the environment variable DATABASEURL
  example on linux:
   $ export DATABASEURL=mongodb://localhost/yelp_camp

  with heroku:
   $ heroku config:set DATABASEURL=mongodb://<username>:<password>@ds261828.mlab.com:61828/yelpcamp
