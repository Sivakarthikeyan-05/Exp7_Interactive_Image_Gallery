# Ex.07 Design of Interactive Image Gallery
## Date:17/12/2025

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title> 
<style> 
         .gallery-container  
{ 
            position: relative; 
            max-width: 600px; 
            margin: auto; 
            background: white; 
            padding: 10px; 
            border-radius: 10px; 
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2); 
         } 
         .gallery-image  
{ 
            width: 100%; 
            height: 600px; 
            object-fit: cover; 
            border-radius: 10px; 
         } 
         .caption  
{ 
            margin-top: 10px; 
            font-size: 18px; 
         } 
         .gallery-buttons  
{ 
            display: flex; 
            justify-content: space-between; 
            margin-top: 15px; 
         } 
         button  
{ 
            padding: 10px 20px; 
            cursor: pointer; 
            border: none; 
            border-radius: 5px; 
            background-color: #007BFF; 
            color: white; 
            transition: 0.3s; 
         } 
     </style> 
</head>  
<body> 
<div class="gallery-container"> 
<img id="galleryImage" class="gallery-image" src="flag.jpg" height="40%" width="40%"> 
<div id="caption" class="caption">Caption for Image 1</div> 
<div class="gallery-buttons"> 
<button onclick="prevImage()">Previous</button> 
<button onclick="nextImage()">Next</button> 
</div> 
</div> 
<script> 
const images = [ 
{ src: "flag.jp", caption: "Caption for Image 1" }, 
{ src: "roger.jpg", caption: "Caption for Image 2" }, 
{ src: "download.jpg", caption: "Caption for Image 3" }, 
{ src: "flag1.jpg", caption: "Caption for Image 4" } 
]; 
let currentIndex = 0; 
function updateGallery( )  
{ 
document.getElementById("galleryImage").src = images[currentIndex].src; 
document.getElementById("caption").textContent = images[currentIndex].caption; 
} 
function nextImage( )  
{ 
currentIndex = (currentIndex + 1) % images.length; 
updateGallery( ); 
} 
function prevImage( )  
{ 
currentIndex = (currentIndex - 1 + images.length) % images.length; 
updateGallery( ); 
} 
</script> 
</body>
</html>
```
## OUTPUT:
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/0ced3c58-b17a-45fb-992b-7e75f9cb6d1c" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/5a872006-3e3a-40dd-bc17-e096550e99b5" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/6eaa7c3e-d08c-4625-a689-d46534667758" />
<img width="1906" height="1079" alt="image" src="https://github.com/user-attachments/assets/f5ab7947-5fd7-48bf-88c6-c00fd7af641c" />



## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
