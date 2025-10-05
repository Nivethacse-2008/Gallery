# Ex.08 Design of Interactive Image Gallery
# Date:05/10/2025
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
```
<!DOCTYPE html>
<html>
<head>
  <title>Interactive Photo Gallery</title>
  <style>
    body { font-family: Arial; background: #df6b6b; text-align: center; }
    .gallery { display: flex; flex-wrap: wrap; justify-content: center; gap: 10px; }
    .gallery img { width: 300px; height: 150px; border-radius: 8px; cursor: pointer; transition: transform 0.3s; }
    .gallery img:hover { transform: scale(2.2); }
    #popup { display: none; position: fixed; top:0; left:0; width:100%; height:100%; background:rgba(23, 197, 110, 0.7); justify-content:center; align-items:center; }
    #popup img { max-width:300%; max-height:200%; border-radius:20px; }
    

  </style>
</head>
<body>
  <h1>📸 Interactive Photo Gallery</h1>
  <div class="gallery">
    <img src="https://picsum.photos/200/150?1" onclick="showPopup(this.src)">
    <img src="https://picsum.photos/200/150?2" onclick="showPopup(this.src)">
    <img src="https://picsum.photos/200/150?3" onclick="showPopup(this.src)">
    <img src="https://picsum.photos/200/150?4" onclick="showPopup(this.src)">
    <img src="https://picsum.photos/200/150?5" onclick="showPopup(this.src)">
  </div>

  <div id="popup" onclick="closePopup()">
    <img id="popupImg" src="">
  </div>

  <script>
    function showPopup(src) {
      document.getElementById('popup').style.display = 'flex';
      document.getElementById('popupImg').src = src;
    }
    function closePopup() {
      document.getElementById('popup').style.display = 'none';
    }
  </script>
</body>
</html>
```

# OUTPUT:
<img width="1366" height="720" alt="Screenshot 2025-10-05 125003" src="https://github.com/user-attachments/assets/244d467a-d44b-4dda-984a-850fceddf403" />
<img width="1366" height="709" alt="Screenshot 2025-10-05 125018" src="https://github.com/user-attachments/assets/e8492843-7a9e-47f0-848f-ca4da35f896a" />



# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
