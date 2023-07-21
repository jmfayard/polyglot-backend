# URL shorter service


## Specs

3 URLS :
1. POST to `/shorten`
2. GET to `/index`
3. POST to `/admin/index`
4. GET to `/oops`

### Shorten a given URL

> POST to `/shorten`

+ This URL should be called with some **json**
+ This URL should return
  + a 201 in case of success
    + the create alias should be returned
  + a 422 otherwise
    + error should be explicit

## Get the form to create URL

>  GET to `/index`

+ This URL should return **html**
+ The **HTML** should expose a form
+ This form should should call the previous URL on submission

## List all URL and their shorten version

> GET to `/admin/index`

+ This URL should authenticable
+ This URL should return **json**

## Redirect to base form

> GET to `/oops`

+ This URL should redirect to `/index`