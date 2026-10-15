
- Convert the tags in the text fields into a UI menu that shows up where you can install various tags to the text by selecting that text. The menu will appear when you select the text, or we can have a menu that exists all the time. 
- Change the video and images to an image/video picker. I don't know how it will work, since we don't know the directory where the images or videos will reside or how we can upload it to the AWS server once the image has been uploaded. 

#### Decision made

- Small toolbar that stays visible all the time for the text fields
- Video and image picker for all the media files in the form

#### Suggestions

- [x] For the entire interface, use the _look and feel_ of the style we selected for our entire system.
- [x] If the user tries to close the page without saving, warn them that there are unsaved changes.
- [x] When editing add a link at the top to the actual page. For example the link is [pand.ai.dsgr/](https://pand.dsgr.nl/brunssum) . Brunssum is the slug (page link) in it.
- [x] Where `<em>` is. blue on the actual page, also show it in blue on `edit.php`
- [x] Let's remove any buttons that reads `Line break`. Rather, just allow the user to type a line break.
- [x] Please remove any `Choose existing` buttons (so, both for images and videos). When someone removes an image or an image carousel item, just remove those images from the server, but keep the thumbnails as I believe they may be shared. You can therefor also remove the sentence `_The red × never deletes a file from the server_`. That entire `_Choose an existing image_` popup can go.
- [x] Make the image captions text also rich-editable. Just linebreaks will do. (You can exclude the "HTML" view for these.)
- [ ] I believe that you show the uncompressed images under `Gallery` in `edit.php`. Use thumbnails instead ― ask AI to review how `/home/tristan/git/pand/index.php` generates them (various sizes) with `/home/tristan/git/shared/thumb.php` . They'll end up in `/home/tristan/git/shared/thumbs`

                                         