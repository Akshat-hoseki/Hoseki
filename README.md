
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Hoseki - Shop Delicious Products</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        /* General Styles */
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f4f4f4;
            color: #333;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
        }

        a {
            color: inherit;
            text-decoration: none;
        }

        /* Navbar Styles */
        header {
            background-color: #001f3f;
            padding: 20px 0;
            color: #fff;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        nav ul {
            list-style: none;
            padding: 0;
        }

        nav ul li {
            display: inline-block;
            margin: 0 15px;
        }

        nav ul li a {
            color: #fff;
            font-weight: bold;
            font-size: 16px;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: #ff9f43;
        }

        /* Hero Section */
        .hero {
            background-color: #ff9f43;
            color: #001f3f;
            text-align: center;
            padding: 80px 20px;
            margin-bottom: 20px;
            border-radius: 8px;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
        }

        /* Sections */
        section {
            padding: 40px 20px;
            transition: all 0.3s ease;
            border-radius: 8px;
            margin: 20px auto;
            max-width: 1200px;
            background-color: #e0e0e0;
            display: none; /* Hide all sections initially */
        }

        section.active {
            display: block; /* Show active section */
        }

        /* Fade In Animation */
        .fade-in {
            animation: fadeIn 0.5s ease-in;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
            }

            to {
                opacity: 1;
            }
        }

        /* Products Section */
        .products {
            display: flex;
            overflow-x: auto;
            padding: 20px;
        }

        .product {
            min-width: 200px;
            margin-right: 20px;
            background-color: #FFD700;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            padding: 10px;
            text-align: center;
            transition: transform 0.2s;
        }

        .product:hover {
            transform: scale(1.05);
        }

        /* Cart Section */
        .cart-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin: 10px 0;
        }

        /* Contact Form */
        form {
            display: flex;
            flex-direction: column;
            max-width: 400px;
            margin: 0 auto;
        }

        form label {
            margin-bottom: 5px;
        }

        form input,
        form textarea {
            margin-bottom: 15px;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }

        .button {
            background-color: #001f3f;
            color: #fff;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .button:hover {
            background-color: #ff9f43;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 20px;
            background-color: #000000;
            color: #fff;
        }

        /* Review Section */
        .review {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .review-item {
            margin: 10px 0;
            text-align: center;
        }

        /* Google Rating */
        .google-rating {
            display: inline-block;
            margin-top: 10px;
            font-size: 24px;
            color: gold;
        }

        /* Contact Box */
        .contact-box {
            border: 2px solid #001f3f;
            padding: 15px;
            border-radius: 8px;
            background-color: #87CEEB;
            text-align: center;
            margin: 20px auto;
            width: fit-content;
        }

        /* FAQs */
        .faq {
            margin: 10px 0;
        }
    </style>
</head>

<body>

    <header>
        <h1>Hoseki</h1>
        <nav>
            <ul>
                <li><a href="#" onclick="showSection('home')">Home</a></li>
                <li><a href="#" onclick="showSection('products')">Products</a></li>
                <li><a href="#" onclick="showSection('cart')">Cart</a></li>
                <li><a href="#" onclick="showSection('about')">About Us</a></li>
                <li><a href="#" onclick="showSection('contact')">Contact</a></li>
                <li><a href="#" onclick="showSection('faq')">FAQs</a></li>
                <li><a href="#" onclick="showSection('reviews')">Reviews</a></li>
            </ul>
        </nav>
    </header>

    <div class="hero">
        <h1>Welcome to Hoseki</h1>
        <p>Your one-stop shop for delicious treats made with love!</p>
    </div>

    <section id="home" class="fade-in active">
        <h2>Welcome to Hoseki</h2>
        <p>We are thrilled to have you here! At Hoseki, we believe that food is more than just a meal; it's a celebration of flavors, memories, and connections. Our passion for crafting delightful treats shines through in every product we offer, from our irresistible Dora cakes to our rich brownies and everything in between. We take pride in using only the highest quality ingredients, ensuring that each bite is a journey of taste and joy.

        As you explore our website, you'll discover a world of deliciousness designed to bring a smile to your face and warmth to your heart. Whether you’re treating yourself or looking for the perfect gift, we invite you to experience the magic of Hoseki. Join us on this delicious journey, and let’s create unforgettable moments together! Thank you for choosing us, and we can't wait for you to savor our creations.

</p>
        <p>Join us on a delightful journey where every product tells a story. We prioritize quality, sourcing only the finest ingredients to craft our delightful offerings. Whether it's the warmth of fresh cookies or the richness of our chocolates, we promise a taste that will make you return for more.</p>
    </section>

    <section id="products" class="fade-in">
        <h2>Our Products</h2>
        <div class="products">
            <div class="product">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT8CzO_vLU5Vfj4FFsvVJs_k4S8_ReiaEZPaw&s" alt="Chocolates" style="width: 100%; height: 150px; object-fit: cover;">
                <h3>Chocolates</h3>
                <p>Delicious handcrafted chocolates.</p>
                <p>Price: ₹150</p>
                <button class="button" onclick="addToCart('Chocolates', 150)">Add to Cart</button>
            </div>
            <div class="product">
                <img src="https://chefsavvy.com/wp-content/uploads/the-best-double-chocolate-cookies.jpg" alt="Cookies" style="width: 100%; height: 150px; object-fit: cover;">
                <h3>Cookies</h3>
                <p>Crunchy and chewy cookies with chocolate chips.</p>
                <p>Price: ₹100</p>
                <button class="button" onclick="addToCart('Cookies', 100)">Add to Cart</button>
            </div>
            <div class="product">
                <img src="https://baranbakery.com/wp-content/uploads/2023/06/Crinkle-Top-Brownies-11.jpg" alt="Brownies" style="width: 100%; height: 150px; object-fit: cover;">
                <h3>Brownies</h3>
                <p>Rich and fudgy brownies for chocolate lovers.</p>
                <p>Price: ₹120</p>
                <button class="button" onclick="addToCart('Brownies', 120)">Add to Cart</button>
            </div>
            <div class="product">
                <img src="https://www.mostlovelythings.com/wp-content/uploads/2023/10/homemade-potato-chips.jpg" alt="
                    Chips" style="width: 100%; height: 150px; object-fit: cover;">
                    <h3>Chips</h3>
                    <p>Crispy and crunchy potato chips.</p>
                    <p>Price: ₹80</p>
                    <button class="button" onclick="addToCart('Chips', 80)">Add to Cart</button>
                    </div>
                    <div class="product">
                    <img src="https://www.seriouseats.com/thmb/YKFVj42G9BWsHMQDczr9o1IRnVA=/1500x0/filters:no_upscale%2Cmax_bytes(150000)%2Cquality(90)/20230720-chocolate-chocolate-chip-cookies-vicky-wasik-6-3a4e60cb1b0344c7b6d0c60f99ec6284.jpg" alt="Dora Cakes" style="width: 100%; height: 150px; object-fit: cover;">
                    <h3>Dora Cakes</h3>
                    <p>Delicious cream-filled cakes.</p>
                    <p>Price: ₹200</p>
                    <button class="button" onclick="addToCart('Dora Cakes', 200)">Add to Cart</button>
                    </div>
                    </div>
                    </section>

                    <section id="cart" class="fade-in">
                    <h2>Your Cart</h2>
                    <div id="cart-items"></div>
                    <div class="cart-item">
                    <strong>Total:</strong> <span id="total-price">₹0</span>
                    </div>
                    <button class="button" onclick="placeOrder()">Place Order</button>
                    </section>

                    <section id="about" class="fade-in">
                    <h2>About Us</h2>
                    <p>At Hoseki, we believe that food is not just a source of nourishment but a medium to create connections and memories. Founded as a school project by a group of nine enthusiastic individuals, Hoseki has evolved into a vibrant startup dedicated to crafting delightful treats that bring joy to people's lives. Our team is passionate about quality and flavor, ensuring that every product we create—whether it's our fluffy Dora cakes, indulgent brownies, crispy cookies, or rich chocolates—is made with the utmost care and attention to detail. We are committed to using the finest ingredients, striving for perfection in every bite. Our journey is fueled by the joy of sharing our creations with the world and the desire to make each moment special for our customers. As we grow, we remain dedicated to our mission of providing delicious products that cater to a wide range of tastes and preferences. Thank you for being a part of our story; we look forward to serving you and making your taste buds dance with delight!.</p>
                    <h3>Our Story</h3>
                    <p>Hoseki began as a simple idea in a classroom, born out of a shared passion for creating delicious treats and a desire to bring people together through food. What started as a school project for a group of nine friends quickly blossomed into a vibrant startup. Our journey has been fueled by the belief that food is not just sustenance; it’s an experience that connects us, evokes memories, and fosters joy.

                    From our very first batch of Dora cakes to our rich, fudgy brownies, each product reflects our commitment to quality and craftsmanship. We take pride in sourcing the finest ingredients, ensuring that every treat we offer is made with love and care. As we experimented in our kitchen, we discovered the magic that happens when creativity meets dedication, and we have been driven by this passion ever since.

                    Hoseki is not just a brand; it is a testament to our journey of learning, growth, and connection. We aim to create delightful experiences with every product we offer, inviting our customers to be a part of our story. As we continue to innovate and expand our range, we remain deeply committed to our core values: quality, flavor, and the joy of sharing.

                    Join us as we explore new flavors, celebrate culinary creativity, and continue to build a community that values the art of good food. Thank you for being a part of our story—here’s to many more delicious moments together!

</p>
                    </section>

                    <section id="contact" class="fade-in">
                    <h2>Contact Us</h2>
                    <div class="contact-box">
                    <h3>Get in Touch</h3>
                    <form id="contact-form" onsubmit="submitForm(event)">
                        <p> Number- 9718153305 </p>
                        <p> Mail id- s.15.115@slps.one</p>
                    <label for="name">Name:</label>
                    <input type="text" id="name" required>

                    <label for="email">Email:</label>
                    <input type="email" id="email" required>

                    <label for="message">Message:</label>
                    <textarea id="message" rows="4" required></textarea>

                    <button type="submit" class="button">Send Message</button>
                    </form>
                    </div>
                    </section>

                    <section id="faq" class="fade-in">
                    <h2>Frequently Asked Questions</h2>
                    <div class="faq">
                    <h3>1. What are your delivery options?</h3>
                    <p>We offer standard and express delivery options. Check our website for more details!</p>
                    </div>
                    <div class="faq">
                    <h3>2. Do you offer vegan options?</h3>
                    <p>Yes, we have a range of vegan-friendly products available.</p>
                    </div>
                    <div class="faq">
                    <h3>3. Can I customize my order?</h3>
                    <p>Absolutely! Contact us for more details on customizing your orders.</p>
                    </div>
                    </section>

                    <section id="reviews" class="fade-in">
                    <h2>Reviews</h2>
                    <div class="review">
                    <div class="review-item">
                    <p>"The best brownies I've ever had!" - John Doe</p>
                    <div class="google-rating">★★★★☆</div>
                    </div>
                    <div class="review-item">
                    <p>"Absolutely love the chips!" - Jane Smith</p>
                    <div class="google-rating">★★★★★</div>
                    </div>
                    </div>
                    <form id="review-form" onsubmit="submitReview(event)">
                    <label for="review-name">Name:</label>
                    <input type="text" id="review-name" required>

                    <label for="review-text">Your Review:</label>
                    <textarea id="review-text" rows="3" required></textarea>

                    <button type="submit" class="button">Submit Review</button>
                    </form>
                    </section>

                    <footer>
                    
                    <p>Contact: <a href="mailto:s.15.115slps.one">s.15.115slps.one</a> | Phone: <a href="tel:+919718153305">+91 97181 53305</a></p>
                    </footer>

                    <script>
                    let cart = [];
                    let total = 0;

                    function showSection(sectionId) {
                    // Hide all sections
                    const sections = document.querySelectorAll('section');
                    sections.forEach(section => {
                    section.classList.remove('active');
                    });

                    // Show the selected section
                    const activeSection = document.getElementById(sectionId);
                    activeSection.classList.add('active');
                    activeSection.classList.add('fade-in');
                    }

                    function addToCart(productName, price) {
                    cart.push({ productName, price });
                    total += price;
                    updateCart();
                    }

                    function updateCart() {
                    const cartItemsContainer = document.getElementById('cart-items');
                    cartItemsContainer.innerHTML = '';
                    cart.forEach((item, index) => {
                    cartItemsContainer.innerHTML += `<div class="cart-item">${item.productName} - ₹${item.price} <button class="button" onclick="removeFromCart(${index})">Remove</button></div>`;
                    });
                    document.getElementById('total-price').textContent = `₹${total}`;
                    }

                    function removeFromCart(index) {
                    total -= cart[index].price;
                    cart.splice(index, 1);
                    updateCart();
                    }

                    function placeOrder() {
                    alert('Your order has been placed successfully!');
                    cart = [];
                    total = 0;
                    updateCart();
                    showSection('home');
                    }

                    function submitForm(event) {
                    event.preventDefault();
                    alert('Message sent! We will get back to you shortly.');
                    document.getElementById('contact-form').reset();
                    }

                    function submitReview(event) {
                    event.preventDefault();
                    const name = document.getElementById('review-name').value;
                    const reviewText = document.getElementById('review-text').value;
                    const reviewsSection = document.querySelector('#reviews .review');
                    reviewsSection.innerHTML += `<div class="review-item"><p>"${reviewText}" - ${name}</p><div class="google-rating">★★★★☆</div></div>`;
                    document.getElementById('review-form').reset();
                    }

                    // Show the home section by default
                    showSection('home');
                    </script>
                    </body>

                    </html>
