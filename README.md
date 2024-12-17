<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Iron House Garage</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            color: #333;
        }

        header {
            background-color: #333;
            color: white;
            padding: 20px;
            text-align: center;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #333;
            padding: 10px;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            padding: 5px 10px;
            border-radius: 5px;
            transition: background-color 0.3s;
        }

        nav a:hover {
            background-color: #333;
        }

        .content {
            padding: 20px;
            text-align: center;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        .hidden {
            display: none;
        }

        .visible {
            display: block;
            animation: fadeIn 0.5s;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        .payment-options {
            margin-top: 20px;
            text-align: left;
        }

        .payment-options ul {
            list-style: none;
            padding: 0;
        }

        .payment-options ul li {
            margin: 10px 0;
        }

        .product-item {
            border: 1px solid #ddd;
            margin: 10px;
            padding: 15px;
            border-radius: 5px;
            text-align: left;
        }

        .product-actions {
            margin-top: 10px;
        }

        .product-actions button {
            padding: 10px 20px;
            margin-right: 10px;
            background-color: #e83838;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .product-actions button:hover {
            background-color: #d73030;
        }

        .payment-modal {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: white;
            padding: 20px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
            z-index: 1000;
            display: none;
        }

        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            z-index: 999;
            display: none;
        }
    </style>
</head>
<body>

<header>
    <h1>The Iron House Garage</h1>
</header>

<nav>
    <a href="#" onclick="showPage('home')">Home</a>
    <a href="#" onclick="showPage('product')">Products</a>
    <a href="#" onclick="showPage('about')">About Us</a>
    <a href="#" onclick="showPage('contact')">Contact</a>
</nav>

<div id="home" class="content visible">
    <h2>Welcome to Our Shop</h2>
    <p>Explore our latest products!</p>
    <div>
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\bolts1.jpg" alt="Product 1" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\rim2.jpg" alt="Product 2" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\sidemirror3.jpg" alt="Product 3" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\mags4.jpg" alt="Product 4" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\headlight5.jpg" alt="Product 5" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\chainset6.jpg" alt="Product 6" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\tire7.jpg" alt="Product 7" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\beastire8.jpg" alt="Product 8" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\horns9.jpg" alt="Product 9" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\gearshifter10.jpg" alt="Product 10" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\seatcover11.jpg" alt="Product 11" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\signalights12.jpg" alt="Product 12" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\handlegrip13.jpg" alt="Product 13" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\handleswitch14.jpg" alt="Product 14" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\lightendisc15.jpg" alt="Product 15" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\dunlop16.jpg" alt="Product 16" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\helmet17.jpg" alt="Product 17" style="width: 150px; margin: 10px;">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\mdl18.jpg" alt="Product 18" style="width: 150px; margin: 10px;">
        <img src="Motor Accessories/break fluid19.jpg" alt="Product 19" style="width: 150px; margin: 10px;">
        <img src="Motor Accessories/led20.jpg" alt="Product 20" style="width: 150px; margin: 10px;">
    </div>
</div>

<div id="product" class="content hidden">
    <h2>Our Products</h2>
    <p>Check out our amazing deals on high-quality items!</p>
    <div class="product-item">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\bolts1.jpg" alt="Product1" style="width: 150px; margin: 10px;">
        <h3>Bolts</h3>
        <p>₱3000</p>
        <div class="product-actions">
            <button onclick="addToCart('bolts1')">Add to Cart</button>
            <button onclick="showPaymentOptions('bolts1')">Buy Now</button>
        </div>
    </div>
    <div class="product-item">
        <img src="C:\Users\faye angelie\OneDrive\Desktop\Iron House Garage\Motor Accessories\rim2.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>Rim</h3>
            <p>₱5000</p>
        <div class="product-actions">
            <button onclick="addToCart('Product 2')">Add to Cart</button>
            <button onclick="showPaymentOptions('Product 2')">Buy Now</button>
        </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/sidemirror3.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>sidemirror</h3>
            <p>₱1500</p>
        <div class="product-actions">
            <button onclick="addToCart('sidemirror3')">Add to Cart</button>
            <button onclick="showPaymentOptions('sidemirror3')">Buy Now</button>
        </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/mags4.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>mags</h3>
            <p>₱1000</p>
        <div class="product-actions">
            <button onclick="addToCart('mags4')">Add to Cart</button>
            <button onclick="showPaymentOptions('mags4')">Buy Now</button>
            </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/headlight5.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>headlight</h3>
            <p>₱999</p>
        <div class="product-actions">
            <button onclick="addToCart('headlight5')">Add to Cart</button>
            <button onclick="showPaymentOptions('headlight5')">Buy Now</button>
            </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/chainset6.jpg" alt="Product1" style="width: 150px; margin: 10px;">
           <h3>chainset</h3>
           <p>₱700</p>
        <div class="product-actions">
           <button onclick="addToCart('chainset6')">Add to Cart</button>
           <button onclick="showPaymentOptions('chainset6')">Buy Now</button>
           </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/tire7.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>tire</h3>
            <p>₱2000</p>
        <div class="product-actions">
            <button onclick="addToCart('tire7')">Add to Cart</button>
            <button onclick="showPaymentOptions('tire7')">Buy Now</button>
            </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/beastire8.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>Beast Tire</h3>
            <p>₱1200</p>
        <div class="product-actions">
            <button onclick="addToCart('beastire8')">Add to Cart</button>
            <button onclick="showPaymentOptions('beastire8')">Buy Now</button>
            </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/clutchlever9.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>Clutch Lever</h3>
            <p>₱1300</p>
        <div class="product-actions">
            <button onclick="addToCart('clutchlever9')">Add to Cart</button>
            <button onclick="showPaymentOptions('clutchlever9')">Buy Now</button>
            </div>
    </div>       
    <div class="product-item">
        <img src="Motor Accessories/gearshifter10.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>Gear Shifter</h3>
            <p>₱500</p>
        <div class="product-actions">
            <button onclick="addToCart('gearshifter10')">Add to Cart</button>
            <button onclick="showPaymentOptions('gearshifter10')">Buy Now</button>
            </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/seatcover11.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>Seat Cover</h3>
            <p>₱400</p>
        <div class="product-actions">
            <button onclick="addToCart('seatcover11')">Add to Cart</button>
            <button onclick="showPaymentOptions('seatcover11')">Buy Now</button>
            </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/signalights12.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>Signal Light</h3>
            <p>₱150</p>
        <div class="product-actions">
            <button onclick="addToCart('signalights12')">Add to Cart</button>
            <button onclick="showPaymentOptions('signalights12')">Buy Now</button>
            </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/handlegrip13.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>Handle Grip</h3>
            <p>₱200</p>
        <div class="product-actions">
            <button onclick="addToCart('handlegrip13')">Add to Cart</button>
            <button onclick="showPaymentOptions('handlegrip13')">Buy Now</button>
            </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/handleswitch14.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>Handle Switch</h3>
            <p>₱150</p>
        <div class="product-actions">
            <button onclick="addToCart('handleswitch14')">Add to Cart</button>
            <button onclick="showPaymentOptions('handleswitch14')">Buy Now</button>
            </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/lightendisc15.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>Ligthen Disc</h3>
            <p>₱250</p>
        <div class="product-actions">
            <button onclick="addToCart('lightendisc15')">Add to Cart</button>
            <button onclick="showPaymentOptions('lightendisc15')">Buy Now</button>
            </div>
    </div>       
    <div class="product-item">
        <img src="Motor Accessories/dunlop16.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>Dunlop</h3>
            <p>₱800</p>
    <div class="product-actions">
            <button onclick="addToCart('dunlop16')">Add to Cart</button>
            <button onclick="showPaymentOptions('dunlop16')">Buy Now</button>
            </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/helmet17.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>Helmet</h3>
            <p>₱2000</p>
        <div class="product-actions">
            <button onclick="addToCart('helmet17')">Add to Cart</button>
            <button onclick="showPaymentOptions('helmet17')">Buy Now</button>
            </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/mdl18.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>MDL</h3>
            <p>₱300</p>
        <div class="product-actions">
            <button onclick="addToCart('mdl18')">Add to Cart</button>
            <button onclick="showPaymentOptions('mdl18')">Buy Now</button>
            </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/break fluid19.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>Break Fluid</h3>
            <p>₱200</p>
        <div class="product-actions">
            <button onclick="addToCart('break fluid19')">Add to Cart</button>
            <button onclick="showPaymentOptions('break fluid19')">Buy Now</button>
            </div>
    </div>
    <div class="product-item">
        <img src="Motor Accessories/led20.jpg" alt="Product1" style="width: 150px; margin: 10px;">
            <h3>LED</h3>
            <p>₱250</p>
        <div class="product-actions">
            <button onclick="addToCart('led20')">Add to Cart</button>
            <button onclick="showPaymentOptions('led20')">Buy Now</button>
            </div>
    </div>
</div>

<div id="about" class="content hidden">
    <h2>About Us</h2>
    <p>We are a company dedicated to providing the best products and services to our customers.</p>
</div>

<div id="contact" class="content hidden">
    <h2>Contact Us</h2>
    <p>Email: theironhousegarage@gmail.com</p>
    <p>Phone: +123 456 7890</p>
</div>

<div id="paymentModal" class="payment-modal">
    <h3>Select Payment Option</h3>
    <ul>
        <li><a href="https://example.com/cod" target="_blank">Cash on Delivery (COD)</a></li>
        <li><a href="https://www.gcash.com" target="_blank">GCash</a></li>
        <li><a href="https://www.paymaya.com" target="_blank">PayMaya</a></li>
    </ul>
    <button onclick="closePaymentModal()">Close</button>
</div>
<div id="modalOverlay" class="modal-overlay" onclick="closePaymentModal()"></div>

<footer>
    &copy; 2024 The house of Garage
</footer>

<script>
    function showPage(pageId) {
        const pages = document.querySelectorAll('.content');
        pages.forEach(page => page.classList.remove('visible'));
        pages.forEach(page => page.classList.add('hidden'));

        const activePage = document.getElementById(pageId);
        activePage.classList.remove('hidden');
        activePage.classList.add('visible');
    }

    function addToCart(product) {
        alert(`${product} has been added to your cart!`);
    }

    function showPaymentOptions(product) {
        document.getElementById('paymentModal').style.display = 'block';
        document.getElementById('modalOverlay').style.display = 'block';
    }

    function closePaymentModal() {
        document.getElementById('paymentModal').style.display = 'none';
        document.getElementById('modalOverlay').style.display = 'none';
    }
</script>

</body>
</html>
