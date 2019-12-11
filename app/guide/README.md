# Introduction

My Application is best and perfect for school website design. To login into the application, we need to open this route.

`BASE_URL`/user/login

## Setup Application

First of all, we have to set up our project.

## Project Information

Project Information Module Database Fields. [JSON Format](/json-data/#project-information-module)

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
* Google Map Verified Address <Badge text="New"/>
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
   |  ├─ nav.tpl
   |  └─ footer.tpl
   |
   ├─ pages
   |  ├─ home.tpl
   |  ├─ gallery.tpl
   |  └─ about.tpl
   |
   |
   └─ manifest.json
```

The [manifest.json](/theme/#manifest-file-for-theme) file is most important part of theme. :tada:

## Contact Message

Contact message for send the message directly to the email address.

> Template HTML for Contact Message

```html
<form action="" method="POST">
      <input type="text" name="name" placeholder="Your Name">
      <input type="email" name="email" placeholder="Your Email">
      <input type="text" name="subject" placeholder="Subject">
      <textarea name="message" cols="30" rows="7" placeholder="Message"></textarea>
      <input type="submit" value="Send Message">
</form>
```

Mail Template file for send contact message to email address `views\Layout\Mail\contact_mail.php`

## Project Subscription

> Template HTML for User Subscription

```html
<form action="subscribe" method="post">
    <input type="email" placeholder="Enter email address">
    <input type="hidden" name="redirect_url" value="{$CURRENT_URL}">
    <input type="submit" value="Subscribe">
</form>
```

