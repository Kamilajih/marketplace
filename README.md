<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Discover products from independent sellers on our online marketplace.">
  <title>MarketHub</title>
  <link rel="stylesheet" href="style.css">
  <script src="script.js" defer></script>
</head>
<body>
  <header class="header">
    <a href="#" class="logo">Market<span>Hub</span></a>

    <form class="search-bar" id="searchForm">
      <input
        type="search"
        id="searchInput"
        placeholder="Search products..."
        aria-label="Search products"
      >
      <button type="submit" aria-label="Search">⌕</button>
    </form>

    <nav class="header-actions">
      <button class="nav-link" id="sellerButton">Sell on MarketHub</button>
      <button class="cart-button" id="cartButton">
        🛒 Cart <span id="cartCount">0</span>
      </button>
    </nav>
  </header>

  <main>
    <section class="hero">
      <div class="hero-content">
        <p class="eyebrow">YOUR MARKETPLACE, YOUR CHOICE</p>
        <h1>Discover more.<br>Shop smarter.</h1>
        <p>
          Explore products from different sellers, compare your options,
          and find what you need in one place.
        </p>
        <a href="#products" class="primary-button">Start shopping →</a>
      </div>
      <div class="hero-visual" aria-hidden="true">
        <span class="hero-icon">🛍️</span>
        <span class="floating-item item-one">👟</span>
        <span class="floating-item item-two">🎧</span>
        <span class="floating-item item-three">⌚</span>
      </div>
    </section>

    <section class="categories section">
      <div class="section-heading">
        <div>
          <p class="eyebrow">EXPLORE</p>
          <h2>Shop by category</h2>
        </div>
      </div>
      <div class="category-list" id="categoryList">
        <button class="category-chip active" data-category="All">All products</button>
        <button class="category-chip" data-category="Electronics">Electronics</button>
        <button class="category-chip" data-category="Fashion">Fashion</button>
        <button class="category-chip" data-category="Home">Home & Living</button>
        <button class="category-chip" data-category="Beauty">Beauty</button>
      </div>
    </section>

    <section class="products-section section" id="products">
      <div class="section-heading">
        <div>
          <p class="eyebrow">HANDPICKED FOR YOU</p>
          <h2>Explore products</h2>
        </div>
        <span class="product-total" id="productTotal">0 products</span>
      </div>

      <div class="product-grid" id="productGrid"></div>

      <div class="empty-state" id="emptyState" hidden>
        <h3>No products found</h3>
        <p>Try another search or choose a different category.</p>
      </div>
    </section>

    <section class="seller-banner">
      <div>
        <p class="eyebrow">GROW YOUR BUSINESS</p>
        <h2>Have products to sell?</h2>
        <p>Reach more customers by bringing your products to MarketHub.</p>
      </div>
      <button class="primary-button" id="sellerBannerButton">
        Become a seller →
      </button>
    </section>
  </main>

  <footer class="footer">
    <a href="#" class="logo">Market<span>Hub</span></a>
    <p>A marketplace connecting buyers and independent sellers.</p>
    <p>© <span id="year"></span> MarketHub. All rights reserved.</p>
  </footer>

  <div class="toast" id="toast" role="status" aria-live="polite"></div>

</body>
</html>
