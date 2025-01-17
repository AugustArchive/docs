---
title: API Endpoints
---

Unlike the rest of the API endpoints, the Marketplace runs on its own instance at https://marketplace.muetab.com with source code available at https://github.com/mue/marketplace.

#### /
```https://marketplace.muetab.com```

Returns hello world message.
#### Response
```json
{
    "message":"Hello World"
}
```

### Get All Items
```https://marketplace.muetab.com/all```

This endpoint returns all marketplace items with description etc removed. The information is used by the marketplace homepage so there is only data it requires in this endpoint.
#### Response
```json
{
    "data": {
        "settings": [],
        "photo_packs": [
        {
            "name": "crunchyroll_hime",
            "display_name": "Crunchyroll Hime",
            "icon_url": "https://upload.wikimedia.org/wikipedia/en/thumb/f/f6/Crunchyroll_Logo.svg/1200px-Crunchyroll_Logo.svg.png",
            "author": "davidjcralph"
        },
        {
            "name": "halloween",
            "display_name": "Halloween",
            "icon_url": "https://publicdomainvectors.org/photos/hattedpumpkin-tkuczamix.png",
            "author": "davidjcralph"
        },
        {
            "name": "low_poly",
            "display_name": "Low Poly Pack",
            "icon_url": "https://i.ibb.co/4J3zrnd/polypacklogo.png",
            "author": "Jack Shanks"
        },
        {
            "name": "winter",
            "display_name": "Winter",
            "icon_url": "https://i.imgur.com/wDMOsaP.png",
            "author": "eartharoid"
        }],
        "quote_packs": []
    }
}
```

### Get Featured
```https://marketplace.muetab.com/featured```

This endpoint returns the featured information for the section on the marketplace screen.
#### Response
```json
{
    "data": {
        "title": "FEATURE CHANGELOG",
        "name": "MUE MARKETPLACE",
        "buttonText": "READ BLOG",
        "buttonLink": "",
        "colour": "#ff7f50"
    }
}
```

#### Get Item
```https://marketplace.muetab.com/item```

This endpoint allows you to get an image. If ID or category aren't specified it will return a random image from all categories.
#### Request
Parameter | Type | Info
--- | --- | ---
name | string | Name of item to search for
category | string | Category to search in
#### Response
```json
{
    "updated": "12th Dec 2020",
    "data": {
        "name": "Crunchyroll Hime",
        "description": "removed\ntest https://google.com",
        "icon_url": "https://upload.wikimedia.org/wikipedia/en/thumb/f/f6/Crunchyroll_Logo.svg/1200px-Crunchyroll_Logo.svg.png",
        "screenshot_url": "https://u.derpyenterprises.org/CcNj",
        "type": "photos", 
        "verified": false,
        "version": "1.0.0",
        "author": "davidjcralph",
        "photos": [{}]
    }
}
```
