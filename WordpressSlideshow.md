# Introduction #

The purpose of this guide is to demonstrate how to create and manage photos and slideshows using WordPress and the slideshow plugin.

It is recommended that you use Mozilla Firefox to upload photos using WPSS; Safari and Internet Explorer should work as well, but they have not been completely tested.

## Uploading and labeling photos ##

Once you have opened Firefox, log into the Wordpress wp-admin area and enter your username and password.  When you view a list of posts from wp-admin, you will be able to see whether a post already has a photo associated by observing the far-right column. If there is already a title in bold, this post already has a photo associated.

![http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot1.png](http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot1.png)

To upload a photo, click on the post title to edit, and then scroll down until you see a box called Slideshow.  Most articles will only need a single photo, so click on the Single Photo button, then the Add photo button.

![http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot2.png](http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot2.png)

This will bring up the WPSS photo selection screen.  Usually, you will want to upload a new photo for an article.  If you want to choose a photo that's already in the photo library, however, you may click on the See all button, or use the search field if you know the name of the image.

![http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot3.png](http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot3.png)

Once you have selected a file, click Upload.  Depending on the size of the file you are uploading and the speed of your network connection, it may take a moment for the image to finish uploading and appear below.  Once it is done, you will see a thumbnail preview of the image and other information.

You must fill in the Photo credit, Title, and Caption fields in order to finish.  If you do not fill in these fields, you will not be able to proceed.  There are also optional fields:

Original URL: Use this if you have obtained the photo from somewhere else online, such as a Flickr page.  You should always use the URL of the page on which the image appears, not a direct link to the file itself.

`Good: http://www.flickr.com/photos/dramaqueennorma/303819485/`

`Bad: http://farm1.static.flickr.com/121/303819485_7449a0be30.jpg`

Geo location: If you know exactly where the photo was taken, you should geo-tag it.  Enter a street address, and click Show in map to confirm your input was understood.

`Good: 1800 E 10th St Bloomington IN`

`Bad: Ashton Hall`

Alt Text: Enter a short, literal description of the image for vision-impaired readers and search engines.

![http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot4.png](http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot4.png)

Finally, hit Insert photo.  Do not press 'Insert into Post' or 'Save all changes.'
The photo will then appear in the slideshow box, with all the fields still available to edit.

![http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot5.png](http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot5.png)

Finally, remember to hit Save, and to preview the post on the site to make sure everything looks correct.

## Uploading and labeling slideshows ##

It is recommended that you read sections I and II before beginning this section.

To create a slideshow in WPSS, begin by editing a post, and then scroll down until you see a box called Slideshow.  To add a slideshow, click on the Slideshow button.

![http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot2.png](http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot2.png)

At minimum, you will need to enter a slideshow title and description.  If all the photos in the slideshow can be credited to a single photographer or organization, the slideshow credit field provides an opportunity to credit them.  If all the photos were taken in approximately the same location, the geo location field allows for geotagging the whole slideshow.

Note that despite filling in any of these fields, you must still continue to enter all this same information for each photo in the slideshow as well.

Once the relevant information is entered, click Add photo to begin adding photos to the slideshow.  Refer to section II, Uploading and Labelling a Photo, for instructions on how to upload and label photos properly.

![http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot6.png](http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot6.png)

Once all of your photos have been added to the slideshow successfully, you will need to choose which photo to use as the title slide and post thumbnail.  You can do this by simply clicking the button underneath your selected photo that says Slideshow Thumbnail.  This tells WPSS to use that photo as the title slide and thumbnail.  When the article appears elsewhere on the site, this will be the image that appears next to the title and link to the article.

![http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot7.png](http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot7.png)

## Using machine tags to control the appearance of photos within posts ##

A new feature of WPSS is the ability to place images and slideshows anywhere in the body of a post, replacing Wordpress's native method of inserting inline images.

First, make sure that all the photos or slideshows you would like to appear inline in your post are uploaded and created.  Then, in brackets, [ ] , put the word slideshow or photo (depending on which you would like to display) followed by the number of the slideshow or photo in the order they are set.

For example, `[`photo 3`]` would display the third photo of the slideshow.  `[`slideshow 2`]` would show the second slideshow.

To show an individual photo from a slideshow when there are multiple slideshows present, specify the slideshow number, then the photo number.  For example, `[`slideshow 3, photo 2`]` would show the second photo from the third slideshow.

![http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot8.png](http://ipm-wordpress.googlecode.com/svn/trunk/wp-content/plugins/ipm-wordpress-slideshow/screenshot8.png)

The photos/slideshows you specify with machine tags will appear in the location where their respective machine tags are located when you are editing a post.

Note that choosing to use machine tags overrides the normal WPSS behavior of automatically displaying a photo or slideshow at the top of the post.  If you wish to have a slideshow or image appear at the top, use a machine tag before the main text of the article.