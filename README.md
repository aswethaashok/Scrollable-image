# Scrollable-image
DATE:22-03-2025
NAME:SWETHA A
Design and implement an interactive image gallery using JavaScript, HTML, and CSS. The gallery should meet the following requirements:

Display multiple images in a horizontal scrollable layout.
Each image must have a caption that appears when hovered over.
Include Next and Previous buttons to navigate through the images.
Use JavaScript to enhance interactivity (e.g., smooth sliding animations, hover effects).
Style the gallery using CSS for a visually appealing and responsive design.
Include a footer at the bottom of the page with the text "Learner's Name and Register Number".
Your solution should include well-structured HTML, CSS, and JavaScript code, ensuring smooth user experience and navigation.
##Program
```
assign.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Scrollable Image Gallery</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h2> IT Companies in Bangalore</h2>
    <div class="gallery-container">
        <button class="btn prev" onclick="scrollGallery(-300)">&#10094;</button>
        <div class="gallery" id="gallery">
            <div class="image-container">
                <img src="c:\Users\admin\Documents\go.avif" alt="Image 1">
                <div class="caption">Google is a multinational technology company</div>
            </div>
            <div class="image-container">
                <img src="c:\Users\admin\Documents\am.jpeg" alt="Image 2">
                <div class="caption">Amazon's office in Bagmane Capital Tech</div>
            </div>
            <div class="image-container">
                <img src="c:\Users\admin\Documents\TCS.avif" alt="Image 3">
                <div class="caption">Tata Consultancy Services (TCS)</div>
            </div>
            <div class="image-container">
                <img src="c:\Users\admin\Documents\ad.jpeg" alt="Image 4">
                <div class="caption">Adobe</div>
            </div>
            <div class="image-container">
                <img src="c:\Users\admin\Documents\info.jpeg" alt="Image 5">
                <div class="caption">Infosys</div>
            </div>
        </div>
        <div class="scroll-container">
            <img src="c:\Users\admin\Documents\wipro.jpg" alt="Cinque Terre">
            <div class="caption">Infosys</div>
            <img src="c:\Users\admin\Documents\img2.jpeg" alt="Forest">
            <img src="c:\Users\admin\Documents\img3.jpeg" alt="Northern Lights">
            <img src="c:\Users\admin\Documents\img4.jpeg" alt="Mountains">
            <img src="c:\Users\admin\Documents\img5.jpeg" alt="Himaliyas">
        </div>
        <div class="image-container">
            <img src="c:\Users\admin\Documents\go.avif" alt="Image 1">
            <div class="caption">Google is a multinational technology company</div>
        </div>
        <div class="image-container">
            <img src="c:\Users\admin\Documents\am.jpeg" alt="Image 2">
            <div class="caption">Amazon's office in Bagmane Capital Tech</div>
        </div>
        <div class="image-container">
            <img src="c:\Users\admin\Documents\TCS.avif" alt="Image 3">
            <div class="caption">Tata Consultancy Services (TCS)</div>
        </div>
        <div class="image-container">
            <img src="c:\Users\admin\Documents\ad.jpeg" alt="Image 4">
            <div class="caption">Adobe</div>
        </div>
        <div class="image-container">
            <img src="c:\Users\admin\Documents\info.jpeg" alt="Image 5">
            <div class="caption">Infosys</div>
        </div>
    </div>
        <button class="btn next" onclick="scrollGallery(300)">&#10095;</button>
    </div>
    <footer>SWETHA A 212223220114</footer>
    <script src="img.js"></script>
</body>
</html>


styles.css

body {
    font-family: Arial, sans-serif;
    text-align: center;
    margin: 0;
    padding: 0;
    background-color: #eec9e0;
}
.gallery-container {
    position: relative;
    width: 100%;
    margin: auto;
    overflow: hidden;
}
.gallery {
    display: flex;
    overflow-x: auto;
    scroll-behavior: smooth;
    scrollbar-width: none;
    -ms-overflow-style: none;
}
.gallery::-webkit-scrollbar {
    display: none;
}
.gallery img {
    width: 300px;
    height: 200px;
    margin: 10px;
    border-radius: 10px;
    transition: transform 0.3s ease;
}
.gallery img:hover {
    transform: scale(1.1);
}
.caption {
    position: absolute;
    bottom: 10px;
    left: 50%;
    transform: translateX(-50%);
    background-color: rgba(0, 0, 0, 0.7);
    color: white;
    padding: 5px 10px;
    border-radius: 5px;
    opacity: 0;
    transition: opacity 0.3s;
}
.image-container {
    position: relative;
    display: inline-block;
}
.image-container:hover .caption {
    opacity: 1;
}
.btn {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background-color: rgba(0, 0, 0, 0.5);
    color: white;
    border: none;
    padding: 10px;
    cursor: pointer;
    border-radius: 5px;
}
div.scroll-container {
    background-color: #333;
    overflow: auto;
    white-space: nowrap;
    padding: 10px;
    }
    
    div.scroll-container img {
    padding: 10px;
    }
.prev { left: 0; }
.next { right: 0; }
footer {
    margin-top: 20px;
    padding: 10px;
    background-color: #222;
    color: white;
    text-align: center;
}

img.js

function scrollGallery(amount) {
    document.getElementById('gallery').scrollBy({
        left: amount,
        behavior: 'smooth'
    });
}

```

#output
![Screenshot 2025-03-22 094231](https://github.com/user-attachments/assets/89724437-5a89-44b7-b054-2f134917c965)

![Screenshot 2025-03-22 094256](https://github.com/user-attachments/assets/c03c24a6-f8bb-4817-8c72-ed869c5230c1)

![Screenshot 2025-03-22 094410](https://github.com/user-attachments/assets/728d37a8-d7cd-4399-a1ce-bc91c61d7f12)

#Result
This experiment is implemented using HTML,CSS and JS.


