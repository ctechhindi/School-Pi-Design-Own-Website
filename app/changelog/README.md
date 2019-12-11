---
sidebar: auto
title: Change Log
lang: en-US
---

# Change Log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).


## V.0.0.4 (2019-12-11)

### Features

* `NEW:` New Global Variable for Theme Template
    ```json
    { $_PROJECT }
    { $_PROJECT_MENU }
    { $_PROJECT_CAROUSEL }
    { $_PROJECT_FACILITIES }
    { $_PROJECT_COURSES }
    { $_PROJECT_PEOPLE_MESSAGES }
    { $_PROJECT_EVENTS }
    { $_PROJECT_KEYS }
    { $_PROJECT_ALBUMS }
    { $_PROJECT_STAFF }
    { $_FLASH_MESSAGE }
    { $_FORM_ERRORS }
    <!-- Global -->
    { $FCPATH }
    { $APPPATH }
    { $BASEPATH }
    { $CURRENT_URL }
    { $CURRENT_CLASS }
    { $CURRENT_METHOD }
    { $THEMEPATH }
    ```
* `NEW:` Create a new field `Google Map Verified Address` for Google Map URL. Like this.
    ```url
    https://maps.google.com/maps?width=100%&amp;height=600&amp;hl=en&amp;
    q={{Google Map Verified Address}}
    &amp;ie=UTF8&amp;t=&amp;z=14&amp;iwloc=B&amp;output=embed
    ```
    - New Field **(`google_address`)** in JSON Data `Project Information` File
    ```json
    "building": {
        "google_address": "SND Children Academy, Moradabad",
    },
    ```
* `NEW:` Connect the contact message for send the message directly to the email address.
* `NEW:` Mail Template File for send contact message to mail, `[application\views\Layout\Mail\contact_mail.php]`
* `NEW:` Create two new theme component file for show flash and form message.
    1. `_project_data/themes/{theme_name}/components/master/flash_messages.tpl`
    2. `_project_data/themes/{theme_name}/components/master/form_messages.tpl`
    > Global Variable for Theme Template 
    ```js
    { $_FORM_ERRORS }
    { $_FLASH_MESSAGE }   
    ```
    > Data Structure of this Variables
    ```js
    [
        'type' => 'message_type', // error, success, info, warning
        'error'  => 'message_array()',
        'message' => 'message',
    ]
    ```
* `NEW:` Create new route for project subscription in the `Project Module`
    * Route
    ```php
    $route['subscribe'] = 'home/subscribe_email';
    ```
    * HTML
    ```html
    <form action="subscribe" method="post">
        <input type="email" placeholder="Enter email address">
        <input type="hidden" name="redirect_url" value="{$CURRENT_URL}">
        <input type="submit" value="Subscribe">
    </form>
    ```

### Changed

* According to Current URL Active Menu Bar Item in the Theme Template `\nav.tpl`
* Change Project Home Page Route `'/' and 'index'`
* Updated Site `Home` Controller

### Fixed

* Fix Error: `album/create` Page `'length' of undefined (create_album.js:28)` Line

## V.0.0.3 (2019-12-08)

### Added

* `NEW:` Create File Manager Module `\application\modules\file_manager\`
* `NEW:` Create Theme Module `\application\modules\themes\`
* `NEW:` Apply New Theme
* `NEW:` Upload New Theme `/project/themes/upload`
* `NEW:` Insert New Library `/zip/Zip.php`

### Changed

* Updated `\libraries\Upload_documents.php` Library Version `0.0.4`
* Change Themes Path `\application\views\themes\` to `\_project_data\themes\`

## V.0.0.2 (2019-07-12)

### Added

* Use Google reCAPTCHA V3 in `User Module - V.0.1`
* Project Force Publish : Update All JSON Files
* Use Library [Date Range Picker](http://www.daterangepicker.com)
* Create a new Vue Component `/application/components/date_time_picker.php`
* Grouping in Gallery Module for albums
* Add Group name in create new album

### Changed

* `Facilities Module - V.0.1`, Update `config_key` name to `group` name
* Event_edit.js and Notice_edit.js
* Staff Module - V.0.1
* Gallery Module - V.0.1
* Admin Panel Dashboard
* Upload Project to Online Server
  1. Edit config and database file
  2. File name change `Publish_Project.php` to `Publish_project.php`
  3. Fix path `require_once '/application/modules/file_name';`
* Minify Slider Javascript files
* Album Image Order not working in mobile version
* If we delete the album, then delete it from the album group table as well.

### Fixed

* Admin Panel Menu
* In the create a new album page
* Fix bug in create a key page
* Fix bug album grouping page

### Deprecation

* Left this library - [vue-ctk-date-time-picker](https://github.com/chronotruck/vue-ctk-date-time-picker?ref=madewithvuejs.com)

## V.0.0.1 (2019-05-20)

### Added

* `Module:` Project *Information*
* `Module:` Menu
* `Module:` Slider/Carousel
* `Module:` Facilities
* `Module:` Events
* `Module:` Notices
* `Module:` Staff
* `Module:` Keys
* `Module:` Gallery
* Add New Fields `Working time` and `Default Icon Package` and more fields in Project Information Page
* Project Icons Pack `Bootstrap3, Font Awesome, Material Design`

```
"fa" => Font Awesome Icon
"b3" => Bootstrap 3 Icon
"mdi" => Material Design Icon
```
* Upload Image for Gallery and Create Albums 
* Add Project Social Media Links
* Add Small Message links `Director's Message`