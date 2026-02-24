# Ex02 Commercial Website
## Date: 24.02.2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM

# index.html
```
<!DOCTYPE html>
<html>
<head>
    <title>FoodZone</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<!-- Navbar -->
<nav>
    <div class="logo">FoodZone</div>
    <div>
        <a href="#home">Home</a>
        <a href="#menu">Menu</a>
        <a href="#order">Order</a>
    </div>
</nav>

<!-- HERO -->
<section id="home" class="section hero">
    <h1>Delicious Food Delivered Fast 🍕</h1>
    <a href="#menu" class="btn">Explore Menu</a>
</section>

<!-- MENU -->
<section id="menu" class="section">
    <h2>Our Popular Dishes</h2>

    <div class="card-container">

        <div class="card">
            <h3>Burger Combo</h3>
            <p>₹199</p>
            <a href="#burger" class="btn">ORDER NOW</a>
        </div>

        <div class="card">
            <h3>Chicken Biryani</h3>
            <p>₹249</p>
            <a href="#biryani" class="btn">ORDER NOW</a>
        </div>

        <div class="card">
            <h3>Pizza Special</h3>
            <p>₹299</p>
            <a href="#pizza" class="btn">ORDER NOW</a>
        </div>

    </div>
</section>

<!-- BURGER DETAILS -->
<section id="burger" class="section">
    <h2>Burger Combo</h2>
    <div class="details-box">
        <p><strong>Price:</strong> ₹199</p>
        <p><strong>Includes:</strong> Burger + Fries + Coke</p>
        <p><strong>Type:</strong> Veg / Non-Veg</p>
        <a href="#order" class="btn">Order Now</a>
    </div>
</section>

<!-- BIRYANI DETAILS -->
<section id="biryani" class="section">
    <h2>Chicken Biryani</h2>
    <div class="details-box">
        <p><strong>Price:</strong> ₹249</p>
        <p><strong>Quantity:</strong> Full Plate</p>
        <p><strong>Spice Level:</strong> Medium</p>
        <a href="#order" class="btn">Order Now</a>
    </div>
</section>

<!-- PIZZA DETAILS -->
<section id="pizza" class="section">
    <h2>Pizza Special</h2>
    <div class="details-box">
        <p><strong>Price:</strong> ₹299</p>
        <p><strong>Size:</strong> Medium</p>
        <p><strong>Toppings:</strong> Cheese + Veggies</p>
        <a href="#order" class="btn">Order Now</a>
    </div>
</section>

<!-- ORDER SECTION -->
<section id="order" class="section">
    <h2>THANKS FOR ORDERING</h2>


        <a href="#home" class="btn">✨❤️</a>
    </div>
</section>

</body>
</html>
```

# style.css
```
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial;
    scroll-behavior:smooth;
}

nav{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:15px 40px;
    background:rgba(0,0,0,0.9);
    color:white;
    position:fixed;
    width:100%;
    z-index:1000;
}

nav a{
    color:white;
    text-decoration:none;
    margin-left:20px;
}

.section{
    min-height:100vh;
    padding:120px 50px;
    text-align:center;
    color:white;
}

/* HERO BACKGROUND */
.hero{
    background:
    linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)),
    url("https://images.unsplash.com/photo-1504674900247-0877df9cc836");
    background-size:cover;
    background-position:center;

    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
}

/* MENU BACKGROUND */
#menu{
    background:
    linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)),
    url("https://images.unsplash.com/photo-1540189549336-e6e99c3679fe");
    background-size:cover;
    background-position:center;
}

/* CARDS */
.card-container{
    display:flex;
    justify-content:center;
    gap:20px;
    margin-top:30px;
    flex-wrap:wrap;
}

.card{
    background:rgba(255,255,255,0.9);
    color:black;
    padding:20px;
    width:250px;
    border-radius:10px;
    transition:0.3s;
}

.card:hover{
    transform:scale(1.05);
}

/* DETAILS */
.details-box{
    background:rgba(255,255,255,0.9);
    color:black;
    padding:30px;
    max-width:400px;
    margin:auto;
    border-radius:10px;
}

/* ORDER */
#order{
    background:
    linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)),
    url("https://images.unsplash.com/photo-1498837167922-ddd27525d352");
    background-size:cover;
    background-position:center;
}

.order-box{
    display:flex;
    flex-direction:column;
    gap:15px;
    max-width:300px;
    margin:auto;
}

.order-box input{
    padding:10px;
}

.price-display{
    background:black;
    color:white;
    padding:10px;
    border-radius:5px;
}

/* BUTTON */
.btn{
    display:inline-block;
    margin-top:10px;
    padding:8px 15px;
    background:black;
    color:white;
    text-decoration:none;
    border-radius:5px;
}
```


## OUTPUT

<img width="1876" height="1013" alt="image" src="https://github.com/user-attachments/assets/2b5ba336-73bd-45a2-9963-b472829bfd39" />

<img width="1880" height="1018" alt="image" src="https://github.com/user-attachments/assets/e9d8cda9-5ec6-45b8-ac00-833fa07379ad" />

<img width="1879" height="1016" alt="image" src="https://github.com/user-attachments/assets/3746804b-ed87-4efc-969e-a4259ba2142f" />




## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
