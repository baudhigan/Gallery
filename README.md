# Ex.08 Design of Interactive Image Gallery
# Date: 13.05.2025
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
### gallery.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Interactive Image Gallery</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #121212;
      color: #fff;
    }

    

    header {
      text-align: center;
      padding: 40px 20px;
      background: #1e1e1e;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.5);
      border-bottom: 2px solid #e63946
    }

    header h1 {
      margin: 0;
      font-size: 3.5em;
      color: #e63946;
    }

    button:hover {
      background-color: #c5303d;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 40px 20px;
      max-width: 1200px;
      margin: auto;
    }

    .gallery img {
      width: 100%;
      height: auto;
      border-radius: 10px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.5);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      cursor: pointer;
    }

    .gallery img:hover {
      transform: scale(1.05);
      box-shadow: 0 6px 20px rgba(0, 0, 0, 0.8);
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #1a1a1a;
      font-size: 0.9em;
      color: #777;
    }

    .lightbox {
      display: none;
      position: fixed;
      z-index: 999;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      background: rgba(0, 0, 0, 0.9);
      align-items: center;
      justify-content: center;
    }

    .lightbox img {
      max-width: 90%;
      max-height: 90%;
      border-radius: 10px;
      box-shadow: 0 0 20px rgba(0, 0, 0, 0.8);
    }

    .lightbox:target {
      display: flex;
    }

    .close-btn {
      position: absolute;
      top: 20px;
      right: 40px;
      font-size: 2rem;
      color: #fff;
      text-decoration: none;
      background: rgba(0,0,0,0.5);
      padding: 8px 16px;
      border-radius: 4px;
    }

    .close-btn:hover {
      background: rgba(255, 255, 255, 0.1);
    }
  </style>
</head>
<body>

  <header>
    <h1>INTERACTIVE IMAGE GALLERY</h1>
  </header>

  <div class="gallery">
    <a href="#img1"> <img src="IMG_2552.jpg" alt="Image 1" /> </a>
    <a href="#img2"> <img src="IMG_2687.JPG" alt="Image 2" /> </a>
    <a href="#img3"> <img src="IMG_5214.JPG" alt="Image 3" /> </a>
    <a href="#img4"> <img src="IMG_3903.JPG" alt="Image 4" /> </a>
    <a href="#img5"> <img src="IMG_3970.JPG" alt="Image 5" /> </a>
    <a href="#img6"> <img src="IMG_3975.jpg" alt="Image 6" /> </a>
  </div>

  <div id="img1" class="lightbox">
    <a href="#" class="close-btn">&times;</a>
    <img src="IMG_2552.jpg" alt="Full Image 1">
  </div>

  <div id="img2" class="lightbox">
    <a href="#" class="close-btn">&times;</a>
    <img src="IMG_2687.JPG" alt="Full Image 2">
  </div>

  <div id="img3" class="lightbox">
    <a href="#" class="close-btn">&times;</a>
    <img src="IMG_5214.JPG" alt="Full Image 3">
  </div>

  <div id="img4" class="lightbox">
    <a href="#" class="close-btn">&times;</a>
    <img src="IMG_3903.JPG" alt="Full Image 4">
  </div>

  <div id="img5" class="lightbox">
    <a href="#" class="close-btn">&times;</a>
    <img src="IMG_3970.JPG" alt="Full Image 5">
  </div>

  <div id="img6" class="lightbox">
    <a href="#" class="close-btn">&times;</a>
    <img src="IMG_3975.JPG" alt="Full Image 6">
  </div>

  <footer>
    &copy; 2025 BAUDHIGAN. All rights reserved.
  </footer>

</body>
</html>

```
# OUTPUT:
![Alt text](<Screenshot 2025-05-13 115342.png>)
![Alt text](<Screenshot 2025-05-13 115357.png>)
![Alt text](<Screenshot 2025-05-13 115409.png>)
![Alt text](<Screenshot 2025-05-13 115422.png>)
![Alt text](<Screenshot 2025-05-13 115438.png>)
![Alt text](<Screenshot 2025-05-13 115449.png>)
![Alt text](<Screenshot 2025-05-13 115512.png>)
# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
