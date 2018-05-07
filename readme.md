


#RESTful Routes.................
(A TABLE OF ALL 7 RESTFUL ROUTES)

name       url              verb     disc.                               mongoose methods
======================================================================================================
INDEX     /dogs             GET        Display a list of dogs.            Dog.find()
NEW       /dogs/new         GET        Display form to add new dog.       N/A
CREATE    /dogs             POST       Add new dog to DB.                 Dog.create()
SHOW      /dogs/:id         GET        Shows information about one dog.   Dog.findById()
EDIT      /dogs/:id/edit    GET        Show edit form for one dog.        Dog.findById()
UPDATE    /dogs/:id         PUT        Update a perticular dog,
                                       then redirect somewhere.           Dog.findByIdAndUpdate()
DISTORY   /dogs/:id         DELETE     Delete a perticular dog,
                                       then redirect somewhere.           Dog.findByIdAndRemove()

==================================================================================
* NOTE: In html form somehow PUT and DELETE is not worked.
* What is the solution for this?
* Ans:  We need to install package called "method-override" and then in tamplate
        we have to specife that type in action attr.
===================================================================================



#RESTful Routing.................

##Introduction
========================================
* Define REST and explain WHY it matters
* List all 7 RESTful routes
* REST -> Representational State Transfer


REST -> A mapping between HTTP routes and CRUD

CRUD means -> CREATE
              READ
              UPDATE
              DISTORY

REST is the representation of routes, It's a way to mapping HTTP routes and CRUD

====================== or ==================================================

REST is just a convention, It's an architecture for mapping our HTTP routes to CRUD functionality.


* For eg:
        
        Blog Website
        ------------
        CREATE   /blogs/new
        READ     /allBlogs
        UPDATE   /updateBlog/:id
        DISTORY  /distoryBlog/:id