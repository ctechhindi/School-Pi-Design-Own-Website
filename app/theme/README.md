---
sidebar: auto
title: Theme
lang: en-US
---

# Theme

## Introduction

Your are using multi-theme template. Create a own theme with dynamic data.

## Manifest File for Theme

The most important part of theme is `manifest.json` file.

```json
{
    "version": "0.0.1",
    "name": "default 2",
    "title": "Default 2 Theme",
    "description": "Default 2 Theme Description",
    "thumbnail": {
        "mobile": "mobile.png",
        "tablet": "tablet.jpg",
        "desktop": "desktop.jpg"
    },
    "manifest_version": "1"
}
```

## Structure

```
└─ default # Theme Folder Name
   ├─ assets
   |  ├─ thumbnail
   |  ├─ js
   |  ├─ images
   |  ├─ fonts
   |  └─ css
   |
   ├─ components
   |  ├─ master
   |  |  ├─ flash_messages.tpl
   |  |  └─ form_messages.tpl
   |  |
   |  ├─ header.tpl
   |  ├─ nav.tpl
   |  └─ footer.tpl
   |
   ├─ pages
   |  ├─ home.tpl
   |  ├─ gallery.tpl
   |  ├─ album.tpl
   |  ├─ about.tpl
   |  ├─ contact.tpl
   |  └─ staff.tpl
   |
   |
   └─ manifest.json
```

## Theme Global Variables

These variable to render data in theme template.

```tpl
$_PROJECT
$_PROJECT_MENU
$_PROJECT_CAROUSEL
$_PROJECT_FACILITIES
$_PROJECT_COURSES
$_PROJECT_PEOPLE_MESSAGES
$_PROJECT_EVENTS
$_PROJECT_KEYS
$_PROJECT_ALBUMS
$_PROJECT_STAFF
$_FLASH_MESSAGE
$_FORM_ERRORS

// Global Variables
$FCPATH
$APPPATH
$BASEPATH
$CURRENT_URL
$CURRENT_CLASS
$CURRENT_METHOD
$THEMEPATH
```

## Flash/Form Messages

Create two new theme component file for show flash and form message.

* `{theme_name}/components/master/flash_messages.tpl`
* `{theme_name}/components/master/form_messages.tpl`

Global Variable for Theme Template.

```tpl
{$_FORM_ERRORS}
{$_FLASH_MESSAGE}
```

Data Structure of this Variables.

```php
[
    'type' => 'message_type', // error, success, info, warning
    'error'  => 'message_array()',
    'message' => 'message',
]
```