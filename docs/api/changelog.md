---
title: Changelog
---

The changelog dates use the DD-MM-YYY format.

### 1.5.0 - 20/05/21
#### Changed
* URLs for all endpoints have been changed
#### Removed
* Unsplash documentation as it's private
* Information about marketplace themes as they are no longer planned

### 1.4.0 - 14/01/21
#### Added
* Documentation now covers marketplace information
* /getQuoteLanguages route and allow getting quotes in other languages

#### Changed
* API optimisations
* Various fixes and changes

### 1.3.0 - 31/08/20
#### Added
* A lot more info to the /getUpdate endpoint, now using data from the blog
* /getPhotographers endpoint
* /getImages now includes camera model and resolution

### 1.2.1 - 14/12/19
#### Changed
* Make error messages like the Fastify default

### 1.2.0 - 10/12/19
#### Added
* Status codes on invalid id and invalid category (400) as well as 404
* Make [source code](https://github.com/mue/api) public

#### Changed
* Changed "Category not found" to "Invalid Category"
* Changed "404" to "404 Not Found"
* Update internal libraries (less broken now)
* Possibly improve performance (removed no longer needed module)

### 1.1.1 - 07/12/19
#### Changed
* Improve error messages
* Update internal libraries (less broken now)
* Improve security (and possibly performance)

### 1.1.0 - 03/12/2019
#### Added
* Support for getting images and quotes via specific ID

### 1.0.0 - 26/06/2019
Please note the date for this update may not be exact.
#### Added
* Initial Release