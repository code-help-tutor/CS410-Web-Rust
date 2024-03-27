# 

A web app was built using Rust, the Axum framework, Postgresql database, and the NASA Image API.
The app allows a registered user to search for images by keyword from NASA. By default the NASA
API returns the top 100 matching results and didn't require a developer key. Thumbnails of the
100 images are displayed. The image description is truncated into a single line and displayed
below each thumbnail -- hovering will display the full description.

There is a link above each thumnail that pops up the image in full size. Clicking on the image 
or checkbox selects it. After selecting the desired images, the user can click on the "Stitch 
Selected Images" button where the web app will combine them into a single (simple) image. The
web app utilizes the Sitchy Core Library. Each "stitched" image is saved to the Postgresql 
database under each user's profile. Clicking on "Display Saved Stitches" shows all the users 
images and a button to delete any if desired.

If an administrator is signed on (using account admin@admin.com), an additional link to "Manage 
Users" is available. This will display all users (without admin permissions) and a checkbox to 
ban them as needed. A banned user attempting to login will be prevented and presented a warning 
that their account has been banned.


2) How it worked, what didn't work?
Almost all the necessary project objectives worked.
- user accounts use passwords and authentication during login (handled via JWT tokens)
- user and administrator roles where administrators can "ban" a user account
- users can save (and delete) their merged images (stored in Postgresql database)
- a cache of NASA API results, storing the following in the database:
  - keyword used to search
  - full URL used to query NASA Image Library API
  - the entire json response returned from the API
 - publishing project to Hetzer cloud servers using Docker images (http://5.78.104.199)


# CS410 Web Rust

# 程序代做代写 CS编程辅导

# WeChat: cstutorcs

# Email: tutorcs@163.com

# CS Tutor

# Code Help

# Programming Help

# Computer Science Tutor

# QQ: 749389476
