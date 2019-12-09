---
sidebar: auto
title: JSON Data
lang: en-US
---

# JSON Data

## Project Information Module

```json
{
    "full_name": "Project Full Name",
    "short_name": "Project Short Name",
    "address": {
        "address1": "Address 1",
        "address2": "Address 2",
        "state": "State Name",
        "city": "City Name",
        "postcode": "Post Code",
        "country": "IN",
        "mobile": "xxxxxxxxxxx",
        "phone": "xxxxxxxxxxx"
    },
    "email": "xxx@gmail.com",
    "site": "Site URL",
    "working_time": "",
    "our_mission": "",
    "our_vision": "",
    "config": {
        "icon_pack": "fa"
    },
    "building": {
        "latitude": "",
        "longitude": "",
        "map_url": "",
        "photo": {
            "org": "",
            "x128": "",
            "x192": "",
            "x256": "",
            "x512": ""
        }
    },
    "social_links": {
        "fb": "",
        "twitter": "",
        "google_plus": "",
        "linkedin": "",
        "instagram": "",
        "youtube": ""
    },
    "logo": {
        "org": "",
        "x16": "",
        "x24": "",
        "x32": "",
        "x64": "",
        "x128": "",
        "x192": "",
        "x256": "",
        "x512": "",
    },
    "meta": {
        "title": "Meta Title",
        "description": "Meta Description",
        "keywords": "Meta Keywords",
        "type": "Meta Type",
        "publisher": "Meta Publisher",
        "author": "Meta Author",
        "site_name": "Meta Site Name",
        "url": "Meta Site URL",
        "google_site_verification": "Google Site Verification",
        "icon": "xxx.ico"
    }
}
```

## Menu Module

```json
{
    "title": "OUR Menu",
    "subtitle": "",
    "description": "",
    "items": [
        {
            "id": "",
            "name": "Home",
            "url_type": "base",
            "url": "home",
            "full_url": "",
            "custom_class": "",
            "custom_style": "",
            "is_show": true
        },
        {
            "id": "",
            "name": "Home",
            "url_type": "base",
            "url": "home",
            "full_url": "",
            "custom_class": "",
            "custom_style": "",
            "is_show": true
        }
        ....
    ],
    // Other Groups
    "main_nav": {
        "title": "",
        "subtitle": "",
        "description": "",
        "items": [
            {
                "id": "",
                "name": "Home",
                "url_type": "base",
                "url": "home",
                "full_url": "",
                "custom_class": "",
                "custom_style": "",
                "is_show": true
            },
            {
                "id": "",
                "name": "Home",
                "url_type": "base",
                "url": "home",
                "full_url": "",
                "custom_class": "",
                "custom_style": "",
                "is_show": true
            }
            ...
        ]
    }
}
```

## Slider Module (Carousel)

```json
{
    "title": "OUR Slider",
    "subtitle": "",
    "description": "",
    "items": [
        {
            "id": "",
            "title": "",
            "subtitle": "",
            "description": "",
            "image": {
                "org": "",
                "x128": "",
            },
            "link": {
                "title": "",
                "url": ""
            },
            "position": "",
            "is_show": true
        },
        ...
    ],
    // Other Groups
    "home_slider": {
        "title": "",
        "subtitle": "",
        "description": "",
        "items": [
            {
                "id": "",
                "title": "",
                "subtitle": "",
                "description": "",
                "image": {
                    "org": "",
                    "x128": "",
                },
                "link": {
                    "title": "",
                    "url": ""
                },
                "position": "",
                "is_show": true
            }
            ...
        ]
    }
}
```

## Courses Module

```json
```

## Events Module

```json
{
    "title": "OUR EVENTS",
    "subtitle": "We provides the opportunity to prepare for life",
    "description": "",
    "items": [
        {
            "haxId": "",
            "name": "Event Name",
            "title": "Event Title",
            "description": "",
            "start_date": "",
            "end_date": "",
            "location": "",
            "img": "",
            "created_at": "4 hours ago",
            "modified_at": "3 hours ago",
            "is_show": true
        }
        ....
    ],
    // Other Groups
    "home_page_upcoming": {
        "title": "",
        "subtitle": "",
        "description": "",
        "items": [
            {
                "haxId": "",
                "name": "Event Name",
                "title": "Event Title",
                "description": "",
                "start_date": "",
                "end_date": "",
                "location": "",
                "img": "",
                "created_at": "4 hours ago",
                "modified_at": "3 hours ago",
                "is_show": true
            }
            ....
        ]
    }
}
```

## Facilities Module

```json
{
    "title": "OUR FACILITIES",
    "subtitle": "We provides the opportunity to prepare for life",
    "description": "",
    "items": [
        {
            "haxId": "",
            "title": "",
            "subtitle": "",
            "description": "",
            "image": {
                "org": "",
                "x150": "",
                "x256": "",
                "x512": "",
            },
            "icon": "",
            "created": "",
            "modified": "",
            "is_show": true
        }
        ....
    ],
    // Other Groups
    "main_facility": {
        "title": "",
        "subtitle": "",
        "description": "",
        "items": [
            {
                "haxId": "",
                "title": "",
                "subtitle": "",
                "description": "",
                "image": {
                    "org": "",
                    "x150": "",
                    "x256": "",
                    "x512": "",
                },
                "icon": "",
                "created": "",
                "modified": "",
                "is_show": true
            }
            ....
        ]
    }
}
```

## Keys Module

```json
{
    "{Key_Name}": {
        "haxId": "",
        "key": "",
        "short_value": "",
        "long_value": "",
        "attachment": "",
        "created_at": "",
        "modified_at": "",
        "is_show": true
    }
    ...
}
```

## Messages Module

```json
{
    "{Unique_ID}": {
        "name": "",
        "designation": "",
        "title": "",
        "subtitle": "",
        "description": ""
    }
    ....
}
```

## News Module

```json

```

## Notices Module

```json
{
    "title": "OUR NOTICES",
    "subtitle": "We provides the opportunity to prepare for life",
    "description": "",
    "items": [
        {
            "haxId": "",
            "title": "",
            "description": "",
            "attachment": "",
            "created_at": "",
            "modified_at": "",
            "is_show": true
        }
        ....
    ],
    // Other Groups
    "key2": {
        "title": "",
        "subtitle": "",
        "description": "",
        "items": [
            {
                "haxId": "",
                "title": "",
                "description": "",
                "attachment": "",
                "created_at": "",
                "modified_at": "",
                "is_show": true
            }
            ....
        ]
    }
}
```

## Staff Module

```json
{
    "title": "OUR STAFF",
    "subtitle": "We provides the opportunity to prepare for life",
    "description": "",
    "items": [
        {
            "haxId": "",
            "name": "",
            "gender": "",
            "designation": "",
            "qualification": "",
            "joining_date": "",
            "leave_date": "",
            "mobile": "",
            "email": "",
            "message": "",
            "address": "",
            "fb": "",
            "twitter": "",
            "linkedin": "",
            "instagram": "",
            "youtube": "",
            "img": "",
            "created_at": "",
            "modified_at": "",
            "is_show": true
        }
        ....
    },
    // Other Groups
    "about_page_messages": {
        "title": "",
        "subtitle": "",
        "description": "",
        "items": [
            {
                "haxId": "",
                "name": "",
                "gender": "",
                "designation": "",
                "qualification": "",
                "joining_date": "",
                "leave_date": "",
                "mobile": "",
                "email": "",
                "message": "",
                "address": "",
                "fb": "",
                "twitter": "",
                "linkedin": "",
                "instagram": "",
                "youtube": "",
                "img": "",
                "created_at": "",
                "modified_at": "",
                "is_show": true
            }
            ....
        ]
    }
}
```
