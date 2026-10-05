🖼️ Dynamic Gallery – HTML & CSS

A simple Dynamic Gallery project created using HTML and CSS. The project displays multiple images in four vertical columns, with each column containing the same set of images arranged in a different order.

This project is useful for practicing Flexbox, image layouts, CSS sizing, and webpage structure.

📸 Project Overview

The webpage contains:

- A centered Dynamic Gallery heading
- Four equal-width gallery columns
- Four images in each column
- Different image arrangements in each column
- A simple black border around each column

Gallery Layout

┌────────────┬────────────┬────────────┬────────────┐
│   Image 1  │   Image 4  │   Image 3  │   Image 2  │
│   Image 2  │   Image 2  │   Image 1  │   Image 4  │
│   Image 3  │   Image 1  │   Image 4  │   Image 1  │
│   Image 4  │   Image 3  │   Image 2  │   Image 3  │
└────────────┴────────────┴────────────┴────────────┘

Each column uses the same four images but in a different sequence.

🛠️ Technologies Used

- HTML5
- CSS3
- Flexbox

No external libraries or frameworks are required.

📂 Project Structure

dynamic-gallery/
│
├── index.html
├── img1.png.png
├── img2.png.png
├── img3.png.png
├── img4.png.png
└── README.md

«Make sure all four image files are located in the same folder as the HTML file.»

🎨 CSS Features

Main Container

The gallery container uses Flexbox:

.container {
    height: 600px;
    border: 1px solid black;
    display: flex;
}

"display: flex" places the four gallery boxes horizontally.

Gallery Boxes

Each gallery column uses:

.box {
    height: 100%;
    width: 25%;
    border: 1px solid black;
}

Since each box has a width of 25%, four boxes fit across the container.

Image Width

The images are styled with:

.img {
    width: 100%;
}

This sets the image width to 100% of its containing element.

🖼️ Image Arrangement

Column 1

<img src="img1.png.png" alt="">
<img src="img2.png.png" alt="">
<img src="img3.png.png" alt="">
<img src="img4.png.png" alt="">

Order:

Image 1 → Image 2 → Image 3 → Image 4

Column 2

<img src="img4.png.png" alt="">
<img src="img2.png.png" alt="">
<img src="img1.png.png" alt="">
<img src="img3.png.png" alt="">

Order:

Image 4 → Image 2 → Image 1 → Image 3

Column 3

<img src="img3.png.png" alt="">
<img src="img1.png.png" alt="">
<img src="img4.png.png" alt="">
<img src="img2.png.png" alt="">

Order:

Image 3 → Image 1 → Image 4 → Image 2

Column 4

<img src="img2.png.png" alt="">
<img src="img4.png.png" alt="">
<img src="img1.png.png" alt="">
<img src="img3.png.png" alt="">

Order:

Image 2 → Image 4 → Image 1 → Image 3

🔄 Why Is It Called a Dynamic Gallery?

The gallery gives the appearance of a dynamic arrangement because the same images are displayed in different sequences across multiple columns.

However, the current implementation is static because the image arrangement is written directly in HTML.

A truly dynamic gallery could use JavaScript to randomly change image positions or automatically update the gallery.

▶️ How to Run

1. Create a folder named "dynamic-gallery".
2. Save the HTML code as "index.html".
3. Place the following images in the same folder:
   - "img1.png.png"
   - "img2.png.png"
   - "img3.png.png"
   - "img4.png.png"
4. Open "index.html" in a modern web browser.

🎯 Learning Objectives

This project helps beginners understand:

- HTML document structure
- "<div>" elements
- "<img>" elements
- Image paths
- CSS Flexbox
- Percentage-based widths
- Borders
- CSS reset
- Basic gallery layouts
- Organizing images into multiple columns

💡 Possible Improvements

The project could be improved by:

- Adding image hover effects
- Adding transitions and animations
- Making the gallery responsive
- Adding image captions
- Using JavaScript to randomly arrange images
- Adding a lightbox for viewing images
- Adding CSS Grid for a more advanced gallery layout
- Adding lazy loading to images
- Providing meaningful "alt" text for accessibility

Example Hover Effect

img {
    transition: transform 0.3s ease;
}

img:hover {
    transform: scale(1.05);
}

⚠️ Note

The current CSS defines:

.img {
    width: 100%;
}

but the images do not have the "img" class:

<img src="img1.png.png" alt="">

Therefore, the ".img" styling will not be applied to the images as written.

To apply it, you could use:

<img class="img" src="img1.png.png" alt="">

or change the CSS selector to:

img {
    width: 100%;
}

👨‍💻 Author

Created as a beginner-friendly HTML & CSS Dynamic Gallery project for practicing Flexbox, image layouts, and basic webpage styling.# Dynamic-Gallery
