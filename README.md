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

### index.html

•   home page for the website
•   user click search button on this page can go to the user.html to see the astro-images
•   if a user, named ZwEin, has log in and he is also a photographer, click “Hi, ZwEin” (profile button), he can go to “photographer.html” to manage his images.
•   the link for reviewer is not provided in this page, since we can if a logged member is reviewer or photographer in the server side, and provide diffenret action in profile button. Besides, reviewer also can login through login page, but this page is not required to design.

### user.html

•   default page for user, which can be accessed from index.html
•   presents astro-images for users to view.
•   provide filters show images with specific category, object name, and tags
•   provide search on the top bar.
•   mouse action on image can be monitored, and user can choose see detail, download or favorite this page. (download and favorite feature is not required, but it’s nice in real design)
•   click image can jump to user_image_detail.html.

### user_image_detail.html

•   presents how many users download this image and its category.
•   users can choose to favorite this image by clicking favorite button.
•   provide different size of image for user to download
•   provide basic information like photographer’s name, image location, date and tags
•   related image set is shown on the bottom, user can find the images at the same images set. Image set contain images that have similar attributes. 

### photographer.html

•   default page for photographer.
•   can be accessed from “manage image set” option on the menu.
•   provide menu for basic actions, only use “images” actions in this design.
•   provide image set list with set’s name, account, last update date and delete action.
•   click the name of image set, can see the detail of image set, by which photographer can go to photographer_images.html.

### photographer_images.html

•   can be accessed from photographer.html
•   provide basic information for images
•   provide delete action for each image
•   this page sample can be used for both image set management or new uploaded image set.
•   click “continue” button to photographer.html

### photographer_upload.html

•   can be accessed from all photographer pages by clicking “Upload” button on the menu
•   upload images by clicking the “upload icon”.
•   click “continue” button to photographer_imageset_info.html

### photographer_imageset_infro.html

•   can be accessed from photographer_upload.html
•   photographer can add basic information like image set name, description and tags.
•   image location and photographer’s name are not required in this page, because these attributes information can be processed from image by server side function.
•   click “continue” button to photographer_images.html.

### reviewer.html

•   default reviewer page
•   can be accessed by login profile from index.html. The login action is not required in this design, and thus this page only can be access by itself.
•   provide search action on the top bar
•   provide image set list for reviewers
•   provide pass and delete actions
•   can see which image set is reviewed or not
•   image set is reviewed only because all images in the image set are reviewed
•   click image set names in the list can see the detail, reviewr_images.html
•   can filter reviewed and images need to review (named unreviewed)

### reviewer_images.html

•   can be accessed from reviewer.html
•   “need review” tag will be shown for the image set that needs review.
•   provide action button for directly pass or delete whole image set.
•   present image grid for reviewers
•   mouse actions on image are monitored.
•   reviewers can choose pass or delete single images

