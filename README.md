<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Coffee Haven — Modern Coffee Shop</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --accent:#d89c4f;
      --bg:#0f1113;
      --card:#141516;
      --muted:#9aa0a6;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:'Poppins',sans-serif;background:var(--bg);color:#fff}

    /* NAVBAR */
    .brand {
  display: flex;
  align-items: center;
  gap: 10px;
}

.brand .logo {
  height: 36px;
  width: auto;
  object-fit: contain;
}
    header.site-header{position:fixed;inset:0 0 auto 0;height:70px;display:flex;align-items:center;justify-content:space-between;padding:0 32px;z-index:1200}
    header.site-header .brand{font-weight:700;letter-spacing:1px}
    header.site-header nav a{color:#fff;text-decoration:none;margin-left:18px;opacity:0.95}
    header.site-header{backdrop-filter:blur(8px);background:rgba(10,10,10,0.45)}

    main{margin-top:70px}

    /* HERO */
    .hero{height:92vh;display:grid;place-items:center;position:relative;overflow:hidden}
    .hero::before{content:"";position:absolute;inset:0;background:url('https://images.unsplash.com/photo-1509042239860-f550ce710b93?auto=format&fit=crop&w=1600&q=80') center/cover fixed no-repeat;filter:brightness(0.45) saturate(0.9)}
    .hero__card{position:relative;z-index:2;padding:44px 56px;border-radius:18px;background:linear-gradient(135deg,rgba(255,255,255,0.04),rgba(255,255,255,0.02));box-shadow:0 12px 40px rgba(0,0,0,0.6);text-align:center;max-width:980px}
    .hero__title{font-size:44px;line-height:1.02;margin:0 0 12px;font-weight:800}
    .hero__subtitle{color:var(--muted);font-size:18px;margin-bottom:18px}
    .hero .cta{display:inline-block;padding:12px 26px;border-radius:999px;background:var(--accent);color:#081217;font-weight:700;border:none;cursor:pointer}

    /* Typing small */
    .typing{display:inline-block;white-space:nowrap;overflow:hidden;border-right:3px solid rgba(255,255,255,0.8);animation:typing 3s steps(40,end) forwards,blink 0.8s infinite}
    @keyframes typing{from{width:0}to{width:420px}}@keyframes blink{50%{border-color:transparent}}

    /* SECTIONS */
    section{padding:72px 6%}
    .title{text-align:center;font-size:28px;margin-bottom:30px;font-weight:700}

    /* MENU GRID */
    .menu{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:28px}
    .card{background:var(--card);border-radius:14px;overflow:hidden;box-shadow:0 6px 20px rgba(0,0,0,0.6);transition:transform .28s,box-shadow .28s;padding-bottom:18px;text-align:center}
    .card:hover{transform:translateY(-8px);box-shadow:0 18px 40px rgba(0,0,0,0.6)}
    .card img{width:100%;height:180px;object-fit:cover;display:block}
    .card h3{margin:14px 10px 6px;font-size:18px}
    .card p.desc{color:var(--muted);font-size:14px;margin:0 12px 10px}
    .price{color:var(--accent);font-weight:700;margin-bottom:8px}
    .rating{color:gold;margin-bottom:8px}

    /* Center order button */
    .order-btn{display:inline-block;margin:8px auto 0 auto;padding:10px 18px;border-radius:12px;border:none;background:var(--accent);color:#071017;font-weight:700;cursor:pointer}
    .order-btn:hover{transform:scale(1.03)}

    /* About & Gallery */
    .about p{max-width:880px;margin:0 auto;color:var(--muted);line-height:1.6}
    .gallery{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:14px}
    .gallery img{width:100%;height:200px;object-fit:cover;border-radius:10px}

    /* Footer */
    footer{padding:24px 6%;text-align:center;color:var(--muted);background:linear-gradient(180deg,rgba(0,0,0,0.0),rgba(0,0,0,0.2))}

    /* Floating utilities */
    .whatsapp{position:fixed;right:22px;bottom:22px;background:#25D366;color:#fff;padding:14px 18px;border-radius:50px;font-weight:700;text-decoration:none;z-index:1300;box-shadow:0 8px 30px rgba(0,0,0,0.45)}
    .cart{position:fixed;right:22px;bottom:90px;background:var(--accent);color:#071017;padding:12px 14px;border-radius:50%;z-index:1300;cursor:pointer;box-shadow:0 8px 30px rgba(0,0,0,0.45)}
    .dark-toggle{position:fixed;left:22px;bottom:22px;padding:10px 12px;border-radius:10px;background:#222;border:none;color:#fff;cursor:pointer;z-index:1300}

    /* Loading screen */
    #loading{position:fixed;inset:0;display:flex;align-items:center;justify-content:center;background:#070707;z-index:2000;color:#fff;font-size:20px}

    /* Responsive tweaks */
    @media(max-width:640px){.hero_title{font-size:26px}.hero_card{padding:22px}.typing{animation:typing 2.4s steps(30,end) forwards}}

    /* small helpers */
    .muted{color:var(--muted)}
  </style>
</head>
<body>

  <!-- Loading -->
  <div id="loading">Loading Manchester coffee...</div>

  <!-- Header / Navbar -->
  <header class="site-header">
    <div class="brand">
  <img src="https://static.vecteezy.com/system/resources/thumbnails/002/412/377/small/coffee-cup-logo-coffee-shop-icon-design-free-vector.jpg" 
       alt="Logo" class="logo">
  <span>Manchester Coffee</span>
  
</div>

</div>

    <nav>
      <a href="#home">Home</a>
      <a href="#menu">Menu</a>
      <a href="#about">About</a>
      <a href="#gallery">Gallery</a>
    </nav>
  </header>

  <main>
    <!-- HERO -->
    <section class="hero" id="home">
      <div class="hero__card" role="banner">
        <h2 class="hero__title">Experience Coffee Like Never Before</h2>
        <p class="hero__subtitle"><span class="typing">Fresh beans — modern brews — cozy vibes.</span></p>
        <button class="cta" onclick="document.getElementById('menu').scrollIntoView({behavior:'smooth'})">Explore Menu</button>
      </div>
    </section>

    <!-- MENU -->
    <section id="menu">
      <h3 class="title">Our Menu</h3>
      <div class="menu">

        <div class="card">
          <img src="https://awsimages.detik.net.id/community/media/visual/2024/12/01/khasiat-espresso.jpeg?w=600&q=90" alt="Espresso">
          <h3>Espresso</h3>
          <p class="desc">Rich, bold, and aromatic espresso brewed from premium beans.</p>
          <div class="price">Rp 18.000</div>
          <div class="rating">★★★★☆ (4.6)</div>
          <button class="order-btn" onclick="addToCart('Espresso')">Order Now</button>
        </div>

        <div class="card">
          <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSnF5zVmTn3cy-eu0OgSTgQpaPY53tV7wFkpQ&s" alt="Cappuccino">
          <h3>Cappuccino</h3>
          <p class="desc">Perfect blend of espresso, steamed milk, and foam.</p>
          <div class="price">Rp 22.000</div>
          <div class="rating">★★★★★ (4.8)</div>
          <button class="order-btn" onclick="addToCart('Cappuccino')">Order Now</button>
        </div>

        <div class="card">
          <img src="https://images.unsplash.com/photo-1541167760496-1628856ab772?auto=format&fit=crop&w=800&q=80" alt="Latte">
          <h3>Latte</h3>
          <p class="desc">Silky smooth latte with a touch of art in every cup.</p>
          <div class="price">Rp 24.000</div>
          <div class="rating">★★★★★ (4.9)</div>
          <button class="order-btn" onclick="addToCart('Latte')">Order Now</button>
        </div>

        <div class="card">
          <img src="https://ichef.bbci.co.uk/food/ic/food_16x9_1600/recipes/the_perfect_mocha_coffee_29100_16x9.jpg" alt="Mocha">
          <h3>Mocha</h3>
          <p class="desc">Chocolate-infused coffee drink with a rich and creamy taste.</p>
          <div class="price">Rp 26.000</div>
          <div class="rating">★★★★☆ (4.7)</div>
          <button class="order-btn" onclick="addToCart('Mocha')">Order Now</button>
        </div>

        <div class="card">
          <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQP7PzXpj11ISpb2pI5WjxOaFayqiv2w4qZxA&s" alt="Americano">
          <h3>Americano</h3>
          <p class="desc">Smooth espresso diluted with hot water for a lighter flavor.</p>
          <div class="price">Rp 20.000</div>
          <div class="rating">★★★★☆ (4.5)</div>
          <button class="order-btn" onclick="addToCart('Americano')">Order Now</button>
        </div>

        <div class="card">
          <img src="https://img.freepik.com/free-photo/hot-caramel-macchiato_1339-6096.jpg" alt="Caramel Macchiato">
          <h3>Caramel Macchiato</h3>
          <p class="desc">Sweet blend of espresso, milk, and caramel drizzle.</p>
          <div class="price">Rp 28.000</div>
          <div class="rating">★★★★★ (4.9)</div>
          <button class="order-btn" onclick="addToCart('Caramel Macchiato')">Order Now</button>
        </div>

        <div class="card">
          <img src="https://images.squarespace-cdn.com/content/v1/677f0f6e06c79b1759fe25ab/57ad1f4d-b2b8-43e3-bb9f-9380b0b8c61f/IMG_6375.jpg" alt="Flat White">
          <h3>Flat White</h3>
          <p class="desc">Smooth microfoam milk poured over rich espresso.</p>
          <div class="price">Rp 25.000</div>
          <div class="rating">★★★★★ (5.0)</div>
          <button class="order-btn" onclick="addToCart('Flat White')">Order Now</button>
        </div>

        <div class="card">
          <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT7BUhLFQod_-Sy8gNY_AomaugSocYQYnYyNA&s" alt="Macchiato">
          <h3>Macchiato</h3>
          <p class="desc">Espresso marked with milk foam.</p>
          <div class="price">Rp 23.000</div>
          <div class="rating">★★★★☆ (4.6)</div>
          <button class="order-btn" onclick="addToCart('Macchiato')">Order Now</button>
        </div>

        <div class="card">
          <img src="https://dfrnt.coffee/cdn/shop/articles/affogato-la-combinacion-perfecta-entre-cafe-y-helado-911187.png?v=1733918360" alt="Affogato">
          <h3>Affogato</h3>
          <p class="desc">Vanilla ice cream drowned in espresso.</p>
          <div class="price">Rp 30.000</div>
          <div class="rating">★★★★★ (4.9)</div>
          <button class="order-btn" onclick="addToCart('Affogato')">Order Now</button>
        </div>

        <div class="card">
          <img src="https://dfrnt.coffee/cdn/shop/articles/cold-brew-cafe-frio-y-refrescante-para-cualquier-momento-del-dia-170904.png?v=1733918359&width=1024" alt="Cold Brew">
          <h3>Cold Brew</h3>
          <p class="desc">Slow-brewed coffee served cold with bold flavor.</p>
          <div class="price">Rp 27.000</div>
          <div class="rating">★★★★☆ (4.7)</div>
          <button class="order-btn" onclick="addToCart('Cold Brew')">Order Now</button>
        </div>

      </div>
    </section>

    <!-- ABOUT -->
    <section id="about">
      <h3 class="title">About Us</h3>
      <div class="about"><p>Manchester Coffee adalah coffee shop modern yang menghadirkan nuansa cozy, minimalis, dan kekinian. Kami hanya menggunakan biji kopi premium dan setiap racikan dibuat oleh barista profesional untuk menghadirkan kopi terbaik tiap hari.</p></div>
    </section>

    <!-- GALLERY -->
    <section id="gallery">
      <h3 class="title">Gallery</h3>
      <div class="gallery">
        <img src="https://images.unsplash.com/photo-1461988091159-192b6df7054f?auto=format&fit=crop&w=800&q=80S" alt="gallery1">
        <img src="https://images.unsplash.com/photo-1495474472287-4d71bcdd2085" alt="gallery2">
        <img src="https://images.unsplash.com/photo-1498804103079-a6351b050096" alt="gallery3">
        <img src="https://images.unsplash.com/photo-1481391032119-d89fee407e44" alt="gallery4">
      </div>
    </section>

  </main>
  <!-- POPUP QUANTITY -->
<div id="qtyPopup" style="
  position: fixed;
  inset: 0;
  display: none;
  align-items: center;
  justify-content: center;
  background: rgba(0,0,0,0.55);
  backdrop-filter: blur(4px);
  z-index: 5000;
">
  <div style="
    background: #fff;
    color: #000;
    padding: 24px 30px;
    border-radius: 14px;
    width: 300px;
    text-align: center;
    box-shadow: 0 10px 40px rgba(0,0,0,0.4);
  ">
    <h3 id="popupTitle" style="margin-top:0">Jumlah Pesanan</h3>

    <input type="number" id="popupQty" value="1" min="1" style="
      width: 80px;
      font-size: 20px;
      padding: 6px;
      border-radius: 8px;
      border: 1px solid #aaa;
      text-align: center;
      margin-top: 10px;
    ">

    <div style="margin-top: 20px; display: flex; gap: 10px; justify-content: center;">
      <button onclick="confirmQty()" style="
        background: #d89c4f;
        border: none;
        padding: 10px 18px;
        border-radius: 10px;
        font-weight: bold;
        cursor: pointer;
      ">OK</button>

      <button onclick="closeQtyPopup()" style="
        background: #ccc;
        border: none;
        padding: 10px 18px;
        border-radius: 10px;
        cursor: pointer;
      ">Cancel</button>
    </div>
  </div>
</div>

</body>
</html>


  <!-- Footer + utilities -->
  <footer>© 2025 Manchester Coffee • All Rights Reserved</footer>

  <a class="whatsapp" href="https://wa.me/6281547232757" target="_blank">Order via WhatsApp</a>
  <button class="cart" id="cartBtn" title="Cart">🛒</button>
  <button class="dark-toggle" id="darkToggle">Dark</button>

  <!-- Background music (will play after user interaction) -->
  <audio id="bgMusic" loop preload="none">
    <source src="https://www2.cs.uic.edu/~i101/SoundFiles/StarWars60.wav" type="audio/wav">
  </audio>

  <script>
  // Loading screen hide
  window.addEventListener('load', ()=>{document.getElementById('loading').style.display='none'})

  // Dark mode
  const toggle=document.getElementById('darkToggle');
  toggle.addEventListener('click',()=>{
    document.documentElement.style.setProperty('--bg',
      document.documentElement.style.getPropertyValue('--bg') === '#0f1113' ? '#f7f7f7' : '#0f1113'
    );
    document.documentElement.style.setProperty('--card',
      document.documentElement.style.getPropertyValue('--card') === '#141516' ? '#ffffff' : '#141516'
    );

    if(document.body.style.background==='rgb(247, 247, 247)'){
      document.body.style.background='var(--bg)';
      document.body.style.color='#fff';
      toggle.textContent='Dark';
    } else {
      document.body.style.background='#f7f7f7';
      document.body.style.color='#111';
      toggle.textContent='Light';
    }
  });

  // music play on first interaction
  const music=document.getElementById('bgMusic');
  function resumeMusic(){music.play().catch(()=>{});window.removeEventListener('click',resumeMusic)}
  window.addEventListener('click',resumeMusic)

/* ===========================
      CART SYSTEM WITH QTY
   =========================== */

const cart = [];
const prices = {
  "Espresso": 18000,
  "Cappuccino": 22000,
  "Latte": 24000,
  "Mocha": 26000,
  "Americano": 20000,
  "Caramel Macchiato": 28000,
  "Flat White": 25000,
  "Macchiato": 23000,
  "Affogato": 30000,
  "Cold Brew": 27000
};

function addToCart(item){
  const qty = parseInt(prompt(`Berapa ${item} yang ingin dipesan?`, 1));

  if (!qty || qty <= 0){
    alert("Jumlah tidak valid.");
    return;
  }

  // cek apakah item sudah ada di cart
  const existing = cart.find(x => x.name === item);

  if(existing){
    existing.qty += qty;
  } else {
    cart.push({ name: item, qty: qty });
  }

  alert(`${item} (${qty}) masuk ke keranjang!`);
}

document.getElementById('cartBtn').addEventListener('click', showCart);

function showCart(){
  if(cart.length === 0){
    alert("Keranjang masih kosong.");
    return;
  }

  let list = "";
  let total = 0;

  cart.forEach(item=>{
    const subtotal = prices[item.name] * item.qty;
    list += `• ${item.name} x ${item.qty} = Rp ${subtotal.toLocaleString()}\n`;
    total += subtotal;
  });

  const message =
    "🛒 *KERANJANG ANDA*\n\n" +
    list +
    `\nTotal: *Rp ${total.toLocaleString()}*\n\n` +
    "Checkout sekarang?";

  if(confirm(message)){
    checkoutWA(list, total);
  }
}

function checkoutWA(list, total)
{
  const text =
    "Halo, saya ingin memesan:\n\n" +
    list +
    `\nTotal: Rp ${total.toLocaleString()}`;

  const url = `https://wa.me/6281547232757?text=${encodeURIComponent(text)}`;
  window.open(url, "_blank");

}
</script>
