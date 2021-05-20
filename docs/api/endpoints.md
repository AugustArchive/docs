---
title: Endpoints
---

There are endpoints for images, quotes and update information.

* [Images](#images)
* [Quotes](#quotes)
* [Other](#other)

## Images

#### Get Random Image

```https://api.muetab.com/images/random```

This endpoint allows you to get a random image. If category isn't specified it will get a random image from all categories.

<!-- tabs:start -->
#### ** Request **
Parameter | Type | Info
--- | --- | ---
category (optional) | string | Returns random image from specific category

#### ** Response **
Type | Code | Response
--- | --- | ---
OK | 200 | ```{"id":186,"category":"Outdoors","file":"https://img.muetab.com/mue/78ff331a7aa4bda3.jpg","photographer":"David Ralph","location":"Cotswold Wildlife Park", "camera": "Samsung Galaxy S8", "resolution": null}```
Not Found | 404 | ```Vercel 404 error```
<!-- tabs:end -->

#### Get Image by ID

```https://api.muetab.com/images/:id```

This endpoint allows you to get an image by ID.

<!-- tabs:start -->
#### ** Request **
Parameter | Type | Info
--- | --- | ---
id | number | Returns information for specific image ID

#### ** Response **
Type | Code | Response
--- | --- | ---
OK | 200 | ```{"id":186,"category":"Outdoors","file":"https://img.muetab.com/mue/78ff331a7aa4bda3.jpg","photographer":"David Ralph","location":"Cotswold Wildlife Park", "camera": "Samsung Galaxy S8", "resolution": null}```
Not Found | 404 | ```Vercel 404 error```
<!-- tabs:end -->

### Get Categories

```https://api.muetab.com/images/categories```

This endpoint returns all categories in an array.

<!-- tabs:start -->
#### ** Response **
Type | Code | Response
--- | --- | ---
OK | 200 | ```["Outdoors"]```
<!-- tabs:end -->

### Get Photographers

```https://api.muetab.com/images/photographers```

This endpoint returns all photographers in an array.

<!-- tabs:start -->
#### ** Response **
Type | Code | Response
--- | --- | ---
OK | 200 | ```["photographer1", "photographer2"]```
<!-- tabs:end -->

## Quotes

#### Get Random Quote

```https://api.muetab.com/quotes/random```

This endpoint allows you to get a random quote. If language isn't specified it will return a random quote in any language.

<!-- tabs:start -->
#### ** Request **
Parameter | Type | Info
--- | --- | ---
language (optional) | string | Get a random quote in a specific language

#### ** Response **
Type | Code | Response
--- | --- | ---
OK | 200 | ```{"id":4,"author":"E.E Cummings","quote":"It takes courage to grow up and become who you really are.","language":"English"}```
Not Found | 404 | ```Vercel 404 error```
<!-- tabs:end -->

#### Get Quote by ID

```https://api.muetab.com/quotes/:id```

This endpoint allows you to get a quote random. If language isn't specified it will return a random quote in any language.

<!-- tabs:start -->
#### ** Request **
Parameter | Type | Info
--- | --- | ---
id | number | Returns information for specific quote ID

#### ** Response **
Type | Code | Response
--- | --- | ---
OK | 200 | ```{"id":4,"author":"E.E Cummings","quote":"It takes courage to grow up and become who you really are.","language":"English"}```
Not Found | 404 | ```Vercel 404 error```
<!-- tabs:end -->

### Get Quote Languages

```https://api.muetab.com/quotes/languages```

This endpoint returns all quote languages in an array.

<!-- tabs:start -->
#### ** Response **
Type | Code | Response
--- | --- | ---
OK | 200 | ```["English", "French"]```
<!-- tabs:end -->

## Other

#### /

```https://api.muetab.com```

Returns hello world message.

<!-- tabs:start -->
#### ** Response **
Type | Code | Response
--- | --- | ---
OK | 200 | ```Hello world! Documentation can be found at https://docs.muetab.com```
<!-- tabs:end -->