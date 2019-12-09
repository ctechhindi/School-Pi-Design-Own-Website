# Introduction

My Application is best and perfect for school website design. To login into the application, we need to open this route.

`BASE_URL`/user/login

## Setup Application

First of all, we have to set up our project.

## Project Information

Project Basic Details

* Full Name
* Short Name
* Address 1
* Address 2
* City
* Post Code
* State Name
* Country Name `(IN)`
* Mobile Number
* Phone Number
* Email Address
* Website URL
* Working Time `(Mon - Sat: 07:30 AM - 03:00 PM)`
* Our Mission
* Our Vision

**Project Social Media Links**

* Facebook
* Twitter
* Google+
* LinkedIn
* Instagram
* YouTube

**Configuration**

* Set Default Icon Package
      
      1. Font Awesome Icon
      2. Bootstrap 3 Icon
      3. Material Design Icon

**Building Information**

* Building Latitude
* Building Longitude
* Building Map URL
* Building Photo `Maximum Size 1 MB`

**Upload Project Logo**

Project Logo Maximum Size `150 KB` and Only `.jpg` and `.png` files are allowed.

**Site Meta Tags**

* Title
* Description
* Keywords
* Type
* Publisher
* Author
* Site Name
* Site URL
* Google Site Verification
* Project Icon

Project Icon Maximum Size `150 KB` and Only `.ico` files are allowed.

## Structure

::: warning COMPATIBILITY NOTE
You can not change the structure of the project.
:::


```
├─ application
└─ _project_data
   └─ themes
      ├─ default
      └─ {and other themes folder}
```

* `_project_data`

This folder contains the json data of our project that we use in our project.

* `_project_data/themes`

In this folder we keep the themes of our project. Whose structure is like this -

```{16}
└─ default # Theme Folder Name
   ├─ assets
   |  └─ thumbnail
   |
   ├─ components
   |  ├─ header.tpl
   |  └─ nav.tpl
   |  └─ footer.tpl
   |
   └─ pages
   |  ├─ home.tpl
   |  ├─ gallery.tpl
   |  └─ about.tpl
   |
   |
   └─ manifest.json
```

The`manifest.json` file is most important part of theme.

<!-- TODO: Show Line How to Make Theme -->

:tada: