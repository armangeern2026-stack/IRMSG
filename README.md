# IRMSG
گالری سنگ مجیدی
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>گالری سنگ مجیدی | اونیکس مشکی جواهری</title>
    <!-- لوگو در تب مرورگر (فاوآیکون) -->
    <link rel="icon" href="logo.png" type="image/png">
    
    <!-- سئو برای گوگل: معرفی کسب و کار برای نمایش لوگو -->
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Organization",
      "name": "گالری سنگ مجیدی",
      "url": "https://your-website.com",
      "logo": "https://your-website.com/logo.png",
      "contactPoint": {
        "@type": "ContactPoint",
        "telephone": "+98-991-382-7998",
        "contactType": "customer service"
      }
    }
    </script>

    <link href="https://cdn.jsdelivr.net/gh/rastikerdar/vazirmatn@v33.003/Vazirmatn-font-face.css" rel="stylesheet" type="text/css" />
    <style>
        :root {
            --primary-green: #a8e6cf;
            --secondary-green: #dcedc1;
            --light-green: #f2faf2;
            --white: #ffffff;
            --dark-text: #333333;
        }

        body { font-family: 'Vazirmatn', sans-serif; background-color: var(--white); color: var(--dark-text); margin: 0; padding: 0; direction: rtl; }
        header { background-color: var(--primary-green); padding: 20px; display: flex; justify-content: space-between; align-items: center; box-shadow: 0 2px 10px rgba(0,0,0,0.1); }
        .logo { display: flex; align-items: center; gap: 10px; }
        .logo img { width: 50px; height: 50px; border-radius: 50%; }
        nav a { margin: 0 15px; text-decoration: none; color: var(--dark-text); font-weight: bold; }
        .cart-btn { cursor: pointer; background-color: var(--white); border: none; padding: 10px 20px; border-radius: 20px; font-weight: bold; }

        .container { max-width: 1200px; margin: 0 auto; padding: 20px; }
        
        /* Hero Section */
        .hero { background: linear-gradient(135deg, var(--secondary-green), var(--white)); text-align: center; padding: 80px 20px; border-radius: 15px; margin-bottom: 50px; }
        .hero h1 { font-size: 3rem; color: #2c5e3f; }
        .hero p { font-size: 1.2rem; color: #555; margin-bottom: 30px; }
        .cta-btn { background-color: #2c5e3f; color: white; text-decoration: none; padding: 15px 30px; border-radius: 30px; font-size: 1.2rem; }

        /* Pricing Slider */
        .pricing-section { background-color: var(--light-green); border-radius: 15px; padding: 40px; text-align: center; margin-bottom: 60px; }
        .price-display { display: flex; justify-content: space-around; margin: 30px 0; font-size: 1.5rem; font-weight: bold; }
        .slider-container { margin: 20px auto; width: 80%; }
        input[type=range] { width: 100%; cursor: pointer; }
        .toman { color: #2c5e3f; }

        /* Products */
        .products-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px; margin-bottom: 60px; }
        .product-card { background: var(--white); border: 1px solid var(--secondary-green); border-radius: 15px; padding: 20px; text-align: center; box-shadow: 0 5px 15px rgba(0,0,0,0.05); }
        .product-card img { width: 100%; height: 250px; object-fit: cover; border-radius: 10px; }
        .product-price { font-size: 1.2rem; font-weight: bold; margin: 15px 0; }
        .add-btn { background-color: var(--primary-green); border: none; padding: 10px; width: 100%; cursor: pointer; border-radius: 8px; font-weight: bold; }

        /* Lab Tests */
        .lab-section { background: #f9f9f9; padding: 40px; border-radius: 10px; margin-bottom: 60px; }
        table { width: 100%; border-collapse: collapse; }
        th, td { border: 1px solid #ddd; padding: 12px; text-align: center; }
        th { background-color: var(--primary-green); }

        /* Comments */
        .comment-form { background: var(--white); border: 1px solid var(--secondary-green); padding: 30px; border-radius: 15px; margin-bottom: 50px; }
        .comment-form textarea, .comment-form input { width: 100%; margin-bottom: 15px; padding: 10px; border-radius: 8px; border: 1px solid #ddd; }
        .submit-btn { background: #2c5e3f; color: white; border: none; padding: 10px 20px; border-radius: 8px; cursor: pointer; }
        .review-list .review-item { border-bottom: 1px solid #eee; padding: 15px 0; }

        /* Social Media and Footer */
        .social-links { text-align: center; padding: 30px; background-color: var(--primary-green); }
        .social-links a { display: inline-block; margin: 0 10px; padding: 10px 20px; background-color: white; color: #333; text-decoration: none; border-radius: 20px; font-size: 0.9rem; }
        footer { background-color: #2c5e3f; color: white; text-align: center; padding: 20px; }

        /* Cart Drawer */
        .cart-drawer { position: fixed; left: 0; top: 0; height: 100%; width: 300px; background-color: white; box-shadow: -5px 0 15px rgba(0,0,0,0.2); transform: translateX(100%); transition: transform 0.3s ease-in-out; padding: 20px; z-index: 1000; }
        .cart-drawer.open { transform: translateX(0); }
    </style>
</head>
<body>

    <header>
        <div class="logo">
            <!-- تصویر لوگو را در پوشه سایت با نام logo.png قرار دهید -->
            <img src="logo.png" alt="گالری سنگ مجیدی">
            <h1>گالری سنگ مجیدی | IR.MSG</h1>
        </div>
        <nav>
            <a href="#pricing">قیمت‌گذاری</a>
            <a href="#products">محصولات</a>
            <a href="#lab-tests">آزمایشگاه</a>
            <a href="#contact">تماس</a>
        </nav>
        <button class="cart-btn" onclick="toggleCart()">🛒 سبد خرید (<span id="cartCount">0</span>)</button>
    </header>

    <div class="container">
        <!-- Hero Section -->
        <section class="hero">
            <h1>بهترین سنگ، اونیکس ایران</h1>
            <p>فقط و فقط اونیکس مشکی جواهری، با تراش‌های اختصاصی بر روی انگشترهای نقره ۹۲۵ طبیعی.</p>
            <p>برای اطلاع از قیمت و مشاوره رایگان تماس بگیرید: <b>0991 382 7998</b></p>
            <a href="#pricing" class="cta-btn">مشاهده قیمت و خرید</a>
        </section>

        <!-- Interactive Pricing Slider -->
        <section id="pricing" class="pricing-section">
            <h2>قیمت‌گذاری هوشمند</h2>
            <p>با کشیدن اسلایدر به چپ و راست، قیراط و قیمت سنگ را ببینید. (قیمت لحظه‌ای دلار: ۲۴۰,۰۰۰ تومان)</p>
            <div class="slider-container">
                <input type="range" id="priceSlider" min="800" max="10000" step="100" value="800" oninput="updatePricing()">
            </div>
            <div class="price-display">
                <div>
                    <span>قیمت به دلار: </span>
                    <span id="usdPrice">$800</span>
                </div>
                <div>
                    <span>معادل تومان: </span>
                    <span id="tomanPrice" class="toman">0 تومان</span>
                </div>
                <div>
                    <span>وزن سنگ: </span>
                    <span id="caratValue">5.0 قیراط</span>
                </div>
            </div>
            <div class="social-links" style="background:transparent;">
                <p>قیمت دلار امروز: <b>۲۴۰,۰۰۰ تومان</b> (این قیمت به‌صورت لحظه‌ای قابل به‌روزرسانی با اتصال به API است)</p>
            </div>
        </section>

        <!-- Product Section -->
        <h2 style="text-align:center; margin-bottom: 30px;">مدل‌های انگشتر نقره ۹۲۵ با نگین اونیکس جواهری</h2>
        <section id="products" class="products-grid">
            <!-- مدل ۱ -->
            <div class="product-card">
                <img src="YOUR_IMAGE_PATH_HERE_1.jpg" alt="انگشتر اونیکس تراش زمردی">
                <h3>تراش زمردی (Emerald Cut)</h3>
                <p>وزن: 5 قیراط</p>
                <p class="product-price">$800</p>
                <button class="add-btn" onclick="addToCart('انگشتر تراش زمردی', 800)">افزودن به سبد خرید</button>
            </div>
            <!-- مدل ۲ -->
            <div class="product-card">
                <img src="YOUR_IMAGE_PATH_HERE_2.jpg" alt="انگشتر اونیکس تراش برلیان">
                <h3>تراش برلیان (Brilliant Cut)</h3>
                <p>وزن: 10 قیراط</p>
                <p class="product-price">$2,500</p>
                <button class="add-btn" onclick="addToCart('انگشتر تراش برلیان', 2500)">افزودن به سبد خرید</button>
            </div>
            <!-- مدل ۳ -->
            <div class="product-card">
                <img src="YOUR_IMAGE_PATH_HERE_3.jpg" alt="انگشتر اونیکس تراش گلابی">
                <h3>تراش گلابی (Pear Cut)</h3>
                <p>وزن: 15 قیراط</p>
                <p class="product-price">$4,500</p>
                <button class="add-btn" onclick="addToCart('انگشتر تراش گلابی', 4500)">افزودن به سبد خرید</button>
            </div>
            <!-- مدل ۴ -->
            <div class="product-card">
                <img src="YOUR_IMAGE_PATH_HERE_4.jpg" alt="انگشتر اونیکس تراش لوکس">
                <h3>تراش لوکس سلطنتی (Luxury Cut)</h3>
                <p>وزن: 30 قیراط</p>
                <p class="product-price">$10,000</p>
                <button class="add-btn" onclick="addToCart('انگشتر تراش لوکس', 10000)">افزودن به سبد خرید</button>
            </div>
        </section>

        <!-- Lab Tests Section -->
        <h2 style="text-align:center;">آنالیز و آزمایشگاه تخصصی سنگ</h2>
        <section id="lab-tests" class="lab-section">
            <p><strong>توضیحات تخصصی:</strong> اونیکس سیاه جواهری ارائه شده در گالری سنگ مجیدی، از خلوص بسیار بالایی برخوردار است. سنگ شما تحت آزمایش‌های XRD و XRF قرار گرفته و نتایج زیر را به همراه دارد:</p>
            <ul>
                <li>ساختار اصلی: ۹۸٪ کوارتز (SiO2)</li>
                <li>کلسیت: کمتر از ۱٪</li>
                <li>جذب آب: ۰.۱٪ (تخلخل فوق‌العاده پایین)</li>
                <li>سختی موس: ۷.۵</li>
                <li>وزن مخصوص حقیقی: ۲.۶۳۶</li>
                <li>pH محیط: ۱۰.۰۴</li>
            </ul>
            <table>
                <tr>
                    <th>عنصر آزمایش‌شده</th>
                    <th>مقدار (ppm)</th>
                </tr>
                <tr><td>U</td><td>7.4</td></tr>
                <tr><td>V</td><td>57</td></tr>
                <tr><td>Zn</td><td>90</td></tr>
                <tr><td>Zr</td><td>26</td></tr>
                <tr><td>As</td><td>13.4</td></tr>
                <tr><td>Ba</td><td>341</td></tr>
                <tr><td>Hg (جیوه)</td><td>< 0.1</td></tr>
                <tr><td>کلر (Cl-)</td><td>308</td></tr>
            </table>
            <p style="margin-top:20px; color:#555;">این نتایج نشان‌دهنده یک سنگ فوق‌العاده مقاوم، خالص و بدون رگه‌های مزاحم است که برای تراش‌های ظریف جواهری ایده‌آل می‌باشد.</p>
        </section>

        <!-- Comments Section -->
        <h2 style="text-align:center;">نظرات مشتریان</h2>
        <section class="comment-form">
            <h3>دیدگاه خود را بنویسید</h3>
            <form onsubmit="addComment(event)">
                <input type="text" id="userName" placeholder="نام شما" required>
                <textarea id="userComment" rows="4" placeholder="نظر شما درباره سنگ و خدمات ما..." required></textarea>
                <button type="submit" class="submit-btn">ثبت دیدگاه</button>
            </form>
            <div id="reviewsList" class="review-list">
                <!-- نظرات نمونه -->
                <div class="review-item">
                    <strong>علی رضایی:</strong> کیفیت سنگ فوق‌العاده است، دقیقاً مطابق آنالیز آزمایشگاهی بود. پیشنهاد می‌کنم!
                </div>
                <div class="review-item">
                    <strong>مریم احمدی:</strong> مشاوره رایگان عالی و قیمت‌ها منصفانه‌ترین قیمتی بود که پیدا کردم.
                </div>
            </div>
        </section>
    </div>

    <!-- Social Links -->
    <section class="social-links">
        <h3>ما را در شبکه‌های اجتماعی دنبال کنید</h3>
        <a href="https://t.me/Majidi_Stone_Galleryy" target="_blank">تلگرام</a>
        <a href="https://www.instagram.com/majidi_stone_gallery?igsh=MXhlend4eDd5aTl5eA==" target="_blank">اینستاگرام</a>
        <a href="https://eitaa.com/Majidi_Stone_Gallery" target="_blank">ایتا</a>
        <a href="https://ble.ir/majidi_stone_gallery" target="_blank">بله</a>
        <a href="https://rubika.ir/Majidi_Stone_Gallery" target="_blank">روبیکا</a>
        <a href="https://splus.ir/Majidi_Stone_Gallery" target="_blank">سروش</a>
        <a href="https://chat.whatsapp.com/BcEVtBt5wfmAuyLTOxWblU?s=cl&p=a&mlu=4&ilr=4" target="_blank">واتساپ</a>
        <a href="https://www.facebook.com/share/1HPvrL5oDf/" target="_blank">فیسبوک</a>
        <a href="https://x.com/majidistone" target="_blank">ایکس (توییتر)</a>
    </section>

    <!-- Footer -->
    <footer id="contact">
        <p>تماس برای سفارش: 0991 382 7998</p>
        <p>گالری سنگ مجیدی | بهترین سنگ اونیکس ایران | IR.MSG</p>
    </footer>

    <!-- Cart Drawer -->
    <div id="cartDrawer" class="cart-drawer">
        <h3>سبد خرید شما</h3>
        <ul id="cartItems"></ul>
        <p>جمع کل: <span id="cartTotal">$0</span></p>
        <button onclick="closeCart()">بستن</button>
    </div>

    <script>
        // قیمت دلار امروز (۲۴۰,۰۰۰ تومان)
        const dollarRate = 240000;

        function updatePricing() {
            const slider = document.getElementById('priceSlider');
            const price = parseInt(slider.value);
            
            // محاسبه قیراط: 5 قیراط برای 800 دلار، 30 قیراط برای 10000 دلار
            const carat = 5 + ((price - 800) / (10000 - 800)) * 25;
            
            document.getElementById('usdPrice').innerText = `$${price.toLocaleString()}`;
            document.getElementById('caratValue').innerText = `${carat.toFixed(1)} قیراط`;
            document.getElementById('tomanPrice').innerText = `${(price * dollarRate).toLocaleString()} تومان`;
        }

        function toggleCart() {
            document.getElementById('cartDrawer').classList.toggle('open');
        }

        function closeCart() {
            document.getElementById('cartDrawer').classList.remove('open');
        }

        let cart = [];

        function addToCart(productName, price) {
            cart.push({ name: productName, price: price, toman: price * dollarRate });
            renderCart();
            document.getElementById('cartCount').innerText = cart.length;
        }

        function renderCart() {
            const list = document.getElementById('cartItems');
            list.innerHTML = '';
            let total = 0;
            cart.forEach(item => {
                total += item.price;
                const li = document.createElement('li');
                li.innerHTML = `${item.name} - ${item.price} دلار (${item.toman.toLocaleString()} تومان)`;
                list.appendChild(li);
            });
            document.getElementById('cartTotal').innerText = `$${total.toLocaleString()}`;
        }

        function addComment(e) {
            e.preventDefault();
            const name = document.getElementById('userName').value;
            const comment = document.getElementById('userComment').value;
            const div = document.createElement('div');
            div.className = 'review-item';
            div.innerHTML = `<strong>${name}:</strong> ${comment}`;
            document.getElementById('reviewsList').prepend(div);
            document.querySelector('form').reset();
            alert("نظر شما ثبت شد!");
        }

        // فراخوانی اولیه برای محاسبه اولیه
        updatePricing();
    </script>
</body>
</html>
