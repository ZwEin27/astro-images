# astro-images
an ui design prototype for showing astro-images


# Description

Amateur astronomers spends hours on taking and processing images from stellar objects. These images are called astro-images. Each image has many attributes including object name (e.g. Jupiter), object category (e.g. Solar System), description, photographer, location, date, Equipment and perhaps some tags. Images may have any size.

An astronomy club would like to have a website to show off their members’ astro-images to public. Users should be able to filter images based on category, object name, photographer and perhaps search for images. Photographers, may login to the site, and upload new images or delete one or more of their existing images. Photographers might have multiple images with the same set of attributes and wishes to upload them all at once. Uploaded images will be reviewed by a reviewer before becoming available to public. Reviewer is allowed to delete images on the site at any time.

# UI Design

## Provisioning Personas

•   User
•   Photographer
•   Reviewer

## Needs for each Persona

### User

1.  Be able to filter images based on category, object name, photographer.
2.  Search for images

### Photographer

1.  Need login to the site (not required to design this page)
2.  Upload new images
3.  Delete one or more of their existing images
4.  Have multiple images with the same set of attributes
5.  Can upload all images that have same set of attributes at once

### Reviewer

1.  Review images
2.  Delete images on the site at any time

## Html Pages

### user.html

•   presents astro-images for users to view.
•   provide filters show images with specific category, object name, and photographer
•   provide search function

### photographer.html

•   upload images
•   delete one or more images
•   manage image attributes

### reviewer.html

•   search all images on the site
•   check images that are not reviewed yet
•   make images public
•   delete images


