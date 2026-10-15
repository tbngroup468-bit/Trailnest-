<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Kabati Digital Tools — Premium Digital Tools for Small Business</title>
  <meta name="description" content="Practical digital tools for small businesses in Kenya and beyond. Excel templates for inventory, sales, profit and cashbook." />
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            gold: {
              50:  '#fbf8f0',
              100: '#f5edd6',
              200: '#ead9a8',
              300: '#dfc47a',
              400: '#d4af4c',
              500: '#c9a227',   // main gold
              600: '#a8841f',
              700: '#876618',
              800: '#664912',
              900: '#45300c',
            },
            dark: {
              900: '#0a0a0a',
              800: '#121212',
              700: '#1a1a1a',
              600: '#242424',
              500: '#2e2e2e',
            }
          }
        }
      }
    }
  </script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" />
  <style>
    body { font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif; }
    .product-card { transition: transform 0.25s ease, box-shadow 0.25s ease; }
    .product-card:hover { transform: translateY(-6px); box-shadow: 0 20px 40px -12px rgba(201, 162, 39, 0.25); }
    .cart-badge { animation: pop 0.3s ease; }
    @keyframes pop { 0% { transform: scale(1); } 50% { transform: scale(1.35); } 100% { transform: scale(1); } }
    .gold-gradient { background: linear-gradient(135deg, #c9a227 0%, #dfc47a 50%, #c9a227 100%); }
    .text-gold-gradient {
      background: linear-gradient(135deg, #dfc47a, #c9a227);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }
  </style>
</head>
<body class="bg-dark-900 text-gray-100 min-h-screen flex flex-col">

  <!-- Header -->
  <header class="bg-dark-800/95 backdrop-blur border-b border-dark-600 sticky top-0 z-50">
    <div class="max-w-6xl mx-auto px-4 py-3 flex items-center justify-between">
      <a href="#" onclick="showPage('home')" class="flex items-center gap-2.5 font-bold text-xl">
        <span class="gold-gradient text-dark-900 w-9 h-9 rounded-lg flex items-center justify-center text-sm font-black tracking-tight">K</span>
        <span class="text-white">Kabati <span class="text-gold-500">Digital</span></span>
      </a>
      <nav class="hidden md:flex items-center gap-7 text-sm font-medium text-gray-300">
        <a href="#" onclick="showPage('home')" class="hover:text-gold-400 transition">Home</a>
        <a href="#" onclick="showPage('products')" class="hover:text-gold-400 transition">Products</a>
        <a href="#" onclick="showPage('account')" class="hover:text-gold-400 transition">My Account</a>
        <a href="https://kabati-digital-tools.floot.app/" target="_blank" class="hover:text-gold-400 transition">Original Site ↗</a>
      </nav>
      <button onclick="toggleCart()" class="relative p-2.5 rounded-full hover:bg-dark-600 transition">
        <i class="fas fa-shopping-cart text-lg text-gray-200"></i>
        <span id="cart-count" class="absolute -top-0.5 -right-0.5 gold-gradient text-dark-900 text-xs font-bold w-5 h-5 rounded-full flex items-center justify-center hidden">0</span>
      </button>
    </div>
  </header>

  <!-- Main Content -->
  <main class="flex-1">
    <!-- HOME PAGE -->
    <section id="page-home" class="page">
      <!-- Hero -->
      <div class="relative overflow-hidden">
        <div class="absolute inset-0 bg-gradient-to-b from-dark-800 to-dark-900"></div>
        <div class="absolute top-20 left-1/2 -translate-x-1/2 w-[600px] h-[600px] bg-gold-500/5 rounded-full blur-3xl"></div>
        <div class="relative max-w-6xl mx-auto px-4 py-20 md:py-28 text-center">
          <p class="text-gold-400 font-semibold mb-4 tracking-[0.2em] uppercase text-xs">Premium Digital Tools</p>
          <h1 class="text-4xl md:text-6xl font-bold text-white mb-5 leading-tight">
            Run your business.<br>
            <span class="text-gold-gradient">Not after your records.</span>
          </h1>
          <p class="text-lg text-gray-400 max-w-2xl mx-auto mb-10">
            Simple spreadsheets and business toolkits that help you keep track of stock, sales and profit — without the complicated stuff.
          </p>
          <div class="flex flex-wrap justify-center gap-4">
            <button onclick="showPage('products')" class="gold-gradient hover:opacity-90 text-dark-900 px-8 py-3.5 rounded-lg font-bold shadow-lg shadow-gold-500/20 transition">
              Browse Digital Tools
            </button>
            <a href="https://kabati-digital-tools.floot.app/" target="_blank" class="border border-dark-500 hover:border-gold-500 text-gray-200 hover:text-gold-400 px-8 py-3.5 rounded-lg font-semibold transition">
              Visit Main Site
            </a>
          </div>
        </div>
      </div>

      <!-- Features -->
      <div class="max-w-6xl mx-auto px-4 py-16">
        <div class="grid md:grid-cols-3 gap-8 text-center">
          <div class="p-6 rounded-2xl bg-dark-800 border border-dark-600">
            <div class="w-12 h-12 gold-gradient text-dark-900 rounded-xl flex items-center justify-center mx-auto mb-4 text-xl">
              <i class="fas fa-chart-line"></i>
            </div>
            <h3 class="font-bold text-lg mb-2 text-white">Know your numbers</h3>
            <p class="text-gray-400 text-sm">Make better daily decisions with clear sales, expenses and profit snapshots.</p>
          </div>
          <div class="p-6 rounded-2xl bg-dark-800 border border-dark-600">
            <div class="w-12 h-12 gold-gradient text-dark-900 rounded-xl flex items-center justify-center mx-auto mb-4 text-xl">
              <i class="fas fa-boxes-stacked"></i>
            </div>
            <h3 class="font-bold text-lg mb-2 text-white">Stay on top of stock</h3>
            <p class="text-gray-400 text-sm">See what is selling, what is running low and what needs reordering.</p>
          </div>
          <div class="p-6 rounded-2xl bg-dark-800 border border-dark-600">
            <div class="w-12 h-12 gold-gradient text-dark-900 rounded-xl flex items-center justify-center mx-auto mb-4 text-xl">
              <i class="fas fa-download"></i>
            </div>
            <h3 class="font-bold text-lg mb-2 text-white">Instant digital delivery</h3>
            <p class="text-gray-400 text-sm">Download after checkout via Payhip or Gumroad. Ready to use immediately.</p>
          </div>
        </div>
      </div>

      <!-- Featured products -->
      <div class="bg-dark-800 border-t border-dark-600 py-16">
        <div class="max-w-6xl mx-auto px-4">
          <h2 class="text-2xl font-bold text-center text-white mb-2">The Digital Toolbox</h2>
          <p class="text-center text-gray-400 mb-10">Small tools. Big clarity.</p>
          <div id="home-products" class="grid sm:grid-cols-2 lg:grid-cols-4 gap-6"></div>
          <div class="text-center mt-10">
            <button onclick="showPage('products')" class="text-gold-400 font-semibold hover:text-gold-300 transition">View all products →</button>
          </div>
        </div>
      </div>
    </section>

    <!-- PRODUCTS PAGE -->
    <section id="page-products" class="page hidden">
      <div class="max-w-6xl mx-auto px-4 py-12">
        <h1 class="text-3xl font-bold text-white mb-2">All Digital Tools</h1>
        <p class="text-gray-400 mb-8">One-time purchase. Download instantly after payment.</p>
        
        <div class="flex flex-wrap gap-3 mb-8">
          <button onclick="filterProducts('all')" class="filter-btn active px-4 py-1.5 rounded-full text-sm font-medium gold-gradient text-dark-900">All</button>
          <button onclick="filterProducts('inventory')" class="filter-btn px-4 py-1.5 rounded-full text-sm font-medium bg-dark-600 text-gray-300 hover:bg-dark-500">Inventory</button>
          <button onclick="filterProducts('templates')" class="filter-btn px-4 py-1.5 rounded-full text-sm font-medium bg-dark-600 text-gray-300 hover:bg-dark-500">Excel Templates</button>
          <button onclick="filterProducts('toolkit')" class="filter-btn px-4 py-1.5 rounded-full text-sm font-medium bg-dark-600 text-gray-300 hover:bg-dark-500">Toolkits</button>
        </div>

        <div id="products-grid" class="grid sm:grid-cols-2 lg:grid-cols-3 gap-6"></div>
      </div>
    </section>

    <!-- PRODUCT DETAIL -->
    <section id="page-product" class="page hidden">
      <div class="max-w-4xl mx-auto px-4 py-12">
        <button onclick="showPage('products')" class="text-gold-400 mb-6 flex items-center gap-2 hover:text-gold-300 transition">
          <i class="fas fa-arrow-left"></i> Back to products
        </button>
        <div id="product-detail" class="bg-dark-800 rounded-2xl border border-dark-600 p-6 md:p-10"></div>
      </div>
    </section>

    <!-- ACCOUNT PAGE -->
    <section id="page-account" class="page hidden">
      <div class="max-w-2xl mx-auto px-4 py-12">
        <h1 class="text-3xl font-bold text-white mb-2">My Account</h1>
        <p class="text-gray-400 mb-8">Purchases are delivered by Payhip or Gumroad. Check the email you used at checkout.</p>

        <div class="bg-dark-800 rounded-2xl border border-dark-600 p-6 mb-6">
          <h2 class="font-semibold text-lg mb-4 flex items-center gap-2 text-white">
            <i class="fas fa-envelope text-gold-500"></i> How to get your files
          </h2>
          <ol class="list-decimal list-inside space-y-3 text-gray-300">
            <li>Complete checkout on Payhip or Gumroad using the links from this store.</li>
            <li>Use an email address you can access.</li>
            <li>After payment you will receive a download link (or find it in your Payhip/Gumroad library).</li>
            <li>Download the Excel files and start using them right away.</li>
          </ol>
        </div>

        <div class="bg-dark-800 rounded-2xl border border-gold-500/30 p-6">
          <h2 class="font-semibold text-lg mb-2 text-white">Need help?</h2>
          <p class="text-gray-400 mb-4">Questions about a product or your order? Reach out:</p>
          <div class="flex flex-wrap gap-3">
            <a href="https://wa.me/254795302763" target="_blank" class="inline-flex items-center gap-2 bg-green-600 text-white px-4 py-2 rounded-lg text-sm font-medium hover:bg-green-700 transition">
              <i class="fab fa-whatsapp"></i> WhatsApp
            </a>
            <a href="https://www.facebook.com/Exfsashion" target="_blank" class="inline-flex items-center gap-2 bg-blue-600 text-white px-4 py-2 rounded-lg text-sm font-medium hover:bg-blue-700 transition">
              <i class="fab fa-facebook-f"></i> Facebook
            </a>
          </div>
        </div>

        <div class="mt-8 text-center text-sm text-gray-500">
          <p>This storefront links to the same secure checkout as the main site.</p>
          <a href="https://kabati-digital-tools.floot.app/" target="_blank" class="text-gold-400 hover:underline">kabati-digital-tools.floot.app</a>
        </div>
      </div>
    </section>
  </main>

  <!-- Cart Sidebar -->
  <div id="cart-overlay" class="fixed inset-0 bg-black/60 z-50 hidden" onclick="toggleCart()"></div>
  <aside id="cart-sidebar" class="fixed top-0 right-0 h-full w-full max-w-md bg-dark-800 border-l border-dark-600 shadow-2xl z-50 transform translate-x-full transition-transform duration-300 flex flex-col">
    <div class="p-4 border-b border-dark-600 flex items-center justify-between">
      <h2 class="font-bold text-lg text-white">Your Cart</h2>
      <button onclick="toggleCart()" class="p-2 hover:bg-dark-600 rounded-full text-gray-400 hover:text-white transition"><i class="fas fa-times"></i></button>
    </div>
    <div id="cart-items" class="flex-1 overflow-y-auto p-4 space-y-4"></div>
    <div class="p-4 border-t border-dark-600">
      <div class="flex justify-between font-semibold mb-4 text-white">
        <span>Total</span>
        <span id="cart-total" class="text-gold-400">KSh 0</span>
      </div>
      <p class="text-xs text-gray-500 mb-4">Checkout happens on Payhip or Gumroad. You will be redirected for secure payment and instant download.</p>
      <button id="checkout-btn" onclick="startCheckout()" class="w-full gold-gradient hover:opacity-90 text-dark-900 py-3 rounded-lg font-bold disabled:opacity-40 disabled:cursor-not-allowed transition" disabled>
        Proceed to Checkout
      </button>
    </div>
  </aside>

  <!-- Checkout choice modal -->
  <div id="checkout-modal" class="fixed inset-0 bg-black/70 z-[60] hidden flex items-center justify-center p-4">
    <div class="bg-dark-800 rounded-2xl max-w-md w-full p-6 border border-dark-600 shadow-2xl">
      <h3 class="text-xl font-bold text-white mb-2">Choose checkout</h3>
      <p class="text-gray-400 text-sm mb-6">Select your preferred platform. Both deliver the files immediately after payment.</p>
      <div id="checkout-options" class="space-y-3">
        <!-- filled dynamically -->
      </div>
      <button onclick="closeCheckoutModal()" class="mt-6 w-full text-gray-500 hover:text-gray-300 text-sm transition">Cancel</button>
    </div>
  </div>

  <!-- Footer -->
  <footer class="bg-dark-800 border-t border-dark-600 py-10 mt-auto">
    <div class="max-w-6xl mx-auto px-4 grid md:grid-cols-3 gap-8 text-sm">
      <div>
        <div class="font-bold text-white text-lg mb-3">Kabati <span class="text-gold-500">Digital Tools</span></div>
        <p class="text-gray-400">Practical digital tools for small businesses in Kenya and beyond.</p>
      </div>
      <div>
        <div class="font-semibold text-white mb-3">Quick links</div>
        <ul class="space-y-2 text-gray-400">
          <li><a href="#" onclick="showPage('products')" class="hover:text-gold-400 transition">All products</a></li>
          <li><a href="https://kabati-digital-tools.floot.app/" target="_blank" class="hover:text-gold-400 transition">Main website</a></li>
          <li><a href="#" onclick="showPage('account')" class="hover:text-gold-400 transition">My Account / Downloads</a></li>
        </ul>
      </div>
      <div>
        <div class="font-semibold text-white mb-3">Contact</div>
        <ul class="space-y-2 text-gray-400">
          <li><a href="https://wa.me/254795302763" target="_blank" class="hover:text-gold-400 transition"><i class="fab fa-whatsapp mr-2"></i>WhatsApp</a></li>
          <li><a href="https://www.facebook.com/Exfsashion" target="_blank" class="hover:text-gold-400 transition"><i class="fab fa-facebook mr-2"></i>Facebook</a></li>
        </ul>
      </div>
    </div>
    <div class="max-w-6xl mx-auto px-4 mt-8 pt-6 border-t border-dark-600 text-center text-xs text-gray-600">
      © 2026 Kabati Digital Tools. Connected to <a href="https://kabati-digital-tools.floot.app/" class="text-gold-500 hover:underline">the official site</a>.
    </div>
  </footer>

  <script>
    // ========== PRODUCT DATA ==========
    // Replace the payhip / gumroad URLs below with your individual product links
    const products = [
      {
        id: 'shop-inventory',
        name: 'Shop Stock & Sales Tracker',
        category: 'inventory',
        price: 650,
        description: 'Track stock in, stock out, daily sales and reorder needs in one simple Excel workbook.',
        features: ['Automatic stock balance', 'Daily sales and expenses', 'Simple profit snapshot'],
        badge: 'SHOP OWNER PICK',
        icon: 'fa-boxes-stacked',
        payhip: 'https://payhip.com/b/b4uUh',
        gumroad: 'https://tbngroup.gumroad.com/l/mopjlo'
      },
      {
        id: 'profit-calculator',
        name: 'Small Business Profit Calculator',
        category: 'templates',
        price: 450,
        description: 'Understand costs, gross profit and net profit without complicated accounting software.',
        features: ['Revenue and expense tracker', 'Gross and net profit formulas', 'Monthly summary'],
        badge: 'BEGINNER FRIENDLY',
        icon: 'fa-calculator',
        payhip: 'https://payhip.com/b/b4uUh',
        gumroad: 'https://tbngroup.gumroad.com/l/mopjlo'
      },
      {
        id: 'starter-toolkit',
        name: 'Small Shop Starter Toolkit',
        category: 'toolkit',
        price: 1200,
        description: 'Practical templates and checklists to help a small shop get organised and grow.',
        features: ['Inventory workbook', 'Daily records and cashbook', 'Simple business checklists'],
        badge: 'VALUE BUNDLE',
        icon: 'fa-briefcase',
        payhip: 'https://payhip.com/b/b4uUh',
        gumroad: 'https://tbngroup.gumroad.com/l/mopjlo'
      },
      {
        id: 'cashbook',
        name: 'Daily Cashbook & Expense Log',
        category: 'templates',
        price: 350,
        description: 'Keep a clear record of money received, money spent and the cash balance.',
        features: ['Cash-in and cash-out entries', 'Expense categories', 'Running balance'],
        badge: 'QUICK START',
        icon: 'fa-book',
        payhip: 'https://payhip.com/b/b4uUh',
        gumroad: 'https://tbngroup.gumroad.com/l/mopjlo'
      }
    ];

    // ========== CART ==========
    let cart = JSON.parse(localStorage.getItem('kabati_cart') || '[]');

    function saveCart() {
      localStorage.setItem('kabati_cart', JSON.stringify(cart));
      updateCartUI();
    }

    function addToCart(productId) {
      const existing = cart.find(i => i.id === productId);
      if (existing) existing.qty += 1;
      else cart.push({ id: productId, qty: 1 });
      saveCart();
      const badge = document.getElementById('cart-count');
      badge.classList.add('cart-badge');
      setTimeout(() => badge.classList.remove('cart-badge'), 300);
    }

    function removeFromCart(productId) {
      cart = cart.filter(i => i.id !== productId);
      saveCart();
    }

    function changeQty(productId, delta) {
      const item = cart.find(i => i.id === productId);
      if (!item) return;
      item.qty += delta;
      if (item.qty < 1) removeFromCart(productId);
      else saveCart();
    }

    function getCartTotal() {
      return cart.reduce((sum, item) => {
        const p = products.find(pr => pr.id === item.id);
        return sum + (p ? p.price * item.qty : 0);
      }, 0);
    }

    function updateCartUI() {
      const countEl = document.getElementById('cart-count');
      const totalItems = cart.reduce((s, i) => s + i.qty, 0);
      if (totalItems > 0) {
        countEl.textContent = totalItems;
        countEl.classList.remove('hidden');
      } else {
        countEl.classList.add('hidden');
      }

      const container = document.getElementById('cart-items');
      const checkoutBtn = document.getElementById('checkout-btn');
      document.getElementById('cart-total').textContent = 'KSh ' + getCartTotal().toLocaleString();

      if (cart.length === 0) {
        container.innerHTML = '<p class="text-center text-gray-500 py-10">Your cart is empty</p>';
        checkoutBtn.disabled = true;
        return;
      }

      checkoutBtn.disabled = false;
      container.innerHTML = cart.map(item => {
        const p = products.find(pr => pr.id === item.id);
        if (!p) return '';
        return `
          <div class="flex gap-3 border border-dark-600 rounded-xl p-3 bg-dark-700">
            <div class="w-12 h-12 gold-gradient text-dark-900 rounded-lg flex items-center justify-center flex-shrink-0">
              <i class="fas ${p.icon}"></i>
            </div>
            <div class="flex-1 min-w-0">
              <div class="font-medium text-sm text-white truncate">${p.name}</div>
              <div class="text-gold-400 font-semibold text-sm">KSh ${p.price.toLocal# Trailnest-
Digital product store for Kabati Digital Tools | Excel templates for Kenyan small businesses. https://tbngroup468-bit.github.io/kabati-store/
