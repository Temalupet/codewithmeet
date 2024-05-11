<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link
      href="https://cdn.jsdelivr.net/npm/remixicon@4.1.0/fonts/remixicon.css"
      rel="stylesheet"
    />
    <link
      rel="stylesheet"
      href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css"
    />
    <link rel="stylesheet" href="styles.css" />
    <title>Web Design Mastery | Foodman</title>
  </head>
 <style>
   @import url("https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap");

:root {
  --primary-color: #fc7f09;
  --primary-color-light: #fffcfa;
  --primary-color-dark: #db6e09;
  --text-dark: #18181b;
  --text-light: #6b7280;
  --white: #ffffff;
  --max-width: 1200px;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.section__container {
  max-width: var(--max-width);
  margin: auto;
  padding: 5rem 1rem;
}

.section__header {
  margin-bottom: 1rem;
  font-size: 2.5rem;
  font-weight: 700;
  line-height: 3rem;
  color: var(--text-dark);
  text-align: center;
}

.section__description {
  color: var(--text-light);
  line-height: 1.75rem;
  text-align: center;
}

.btn {
  padding: 0.75rem 1.5rem;
  outline: none;
  border: none;
  white-space: nowrap;
  font-size: 1rem;
  color: var(--white);
  background-color: var(--primary-color);
  border-radius: 10px;
  transition: 0.3s;
  cursor: pointer;
}

.btn:hover {
  background-color: var(--primary-color-dark);
}

.logo a {
  font-size: 1.5rem;
  font-weight: 700;
  color: var(--primary-color);
}

.logo a span {
  color: var(--text-dark);
}

img {
  display: flex;
  width: 100%;
}

a {
  text-decoration: none;
  transition: 0.3s;
}

ul {
  list-style: none;
}

html,
body {
  scroll-behavior: smooth;
}

body {
  font-family: "Poppins", sans-serif;
}

nav {
  position: fixed;
  isolation: isolate;
  width: 100%;
  z-index: 9;
}

.nav__header {
  width: 100%;
  padding: 1rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: var(--primary-color);
}

.nav__logo a {
  color: var(--white);
}

.nav__menu__btn {
  font-size: 1.5rem;
  color: var(--white);
  cursor: pointer;
}

.nav__links {
  position: absolute;
  top: 68px;
  left: 0;
  width: 100%;
  padding: 2rem;
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 2rem;
  background-color: var(--primary-color-light);
  transition: 0.5s;
  z-index: -1;
  transform: translateY(-100%);
}

.nav__links.open {
  transform: translateY(0);
}

.nav__links a {
  font-weight: 500;
  color: var(--primary-color);
}

.nav__links a:hover {
  color: var(--text-dark);
}

.nav__btn {
  display: none;
}

.header__container {
  display: grid;
  gap: 2rem;
  overflow: hidden;
}

.header__image img {
  max-width: 500px;
  margin-inline: auto;
  border-radius: 2rem;
  
}

.header__content h1 {
  margin-bottom: 1rem;
  font-size: 3.5rem;
  font-weight: 700;
  line-height: 4.5rem;
  color: var(--text-dark);
  text-align: center;
}

.header__content h1 span {
  color: var(--primary-color);
}

.header__content .section__description {
  margin-bottom: 2rem;
}

.header__btn {
  text-align: center;
}

.special__container :is(.section__header, .section__description) {
  max-width: 600px;
  margin-inline: auto;
}

.special__grid {
  margin-top: 4rem;
  display: grid;
  gap: 1rem;
}

.special__card {
  padding: 1rem;
  text-align: center;
  border-radius: 2rem;
  transition: 0.3s;
}

.special__card:hover {
  box-shadow: 10px 10px 40px rgba(0, 0, 0, 0.1);
}

.special__card img {
  width: 200px;
  height: 200px;
  margin-inline: auto;
  margin-bottom: 1rem;
  filter: drop-shadow(10px 10px 20px rgba(0, 0, 0, 0.3));
  border-radius: 2rem;
}

.special__card h4 {
  margin-bottom: 0.5rem;
  font-size: 1.5rem;
  font-weight: 700;
  color: var(--text-dark);
}

.special__card p {
  margin-bottom: 0.5rem;
  color: var(--text-light);
  line-height: 1.75rem;
}

.special__ratings {
  margin-bottom: 1rem;
  font-size: 1rem;
  color: goldenrod;
}

.special__footer {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
}

.special__footer .price {
  font-size: 1.2rem;
  font-weight: 600;
  color: var(--text-dark);
}

.explore__container {
  display: grid;
  gap: 2rem;
  overflow: hidden;
}

.explore__image img {
  max-width: 350px;
  margin-inline: auto;
  filter: drop-shadow(0 0 50px rgba(252, 127, 9, 0.4));
  border-radius:2rem;
}

.explore__content .section__description {
  margin-bottom: 2rem;
}

.explore__btn {
  text-align: center;
}

.banner__container {
  display: grid;
  gap: 1rem;
}

.banner__card {
  padding: 2rem;
  box-shadow: 5px 5px 20px rgba(0, 0, 0, 0.1);
  border-radius: 3rem;
  transition: 0.3s;
}

.banner__card:hover {
  box-shadow: 10px 10px 40px rgba(0, 0, 0, 0.1);
}

.banner__card .banner__icon {
  display: inline-block;
  margin-bottom: 1rem;
  padding: 5px 11px;
  font-size: 2rem;
  color: var(--white);
  border-radius: 1rem;
}

.banner__card:nth-child(1) .banner__icon {
  background-color: #62b15c;
  box-shadow: 5px 5px 30px #62b15cd0;
}

.banner__card:nth-child(2) .banner__icon {
  background-color: #ff3e67;
  box-shadow: 5px 5px 30px #ff3e67d0;
}

.banner__card:nth-child(3) .banner__icon {
  background-color: #185adb;
  box-shadow: 5px 5px 30px #185adbd0;
}

.banner__card h4 {
  margin-bottom: 0.5rem;
  font-size: 1.5rem;
  font-weight: 600;
  color: var(--text-dark);
}

.banner__card p {
  margin-bottom: 1rem;
  color: var(--text-light);
  line-height: 1.75rem;
}

.banner__card a {
  display: flex;
  align-items: center;
  gap: 10px;
  font-size: 500;
  color: var(--primary-color);
}

.banner__card a span {
  font-size: 1.25rem;
  transition: 0.3s;
}

.banner__card a:hover span {
  transform: translateX(10px);
}

.chef {
  position: relative;
  isolation: isolate;
  overflow: hidden;
}

.chef__bg {
  position: absolute;
  z-index: -1;
  max-width: 275px;
  left: -4rem;
  bottom: -2rem;
}

.chef__container {
  padding-bottom: 10rem;
  display: grid;
  gap: 2rem;
}

.chef__content .section__description {
  margin-bottom: 1rem;
}

.chef__image {
  position: relative;
  isolation: isolate;
}

.chef__image img {
  max-width: 500px;
  border-radius: 100%;
  margin-inline: auto;
}

.chef__image::after {
  position: absolute;
  content: "";
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
  height: 100%;
  width: 100%;
  max-width: 500px;
  background-color: var(--primary-color);
  border-radius: 100%;
  z-index: -1;
}

.chef__list {
  display: grid;
  gap: 0.5rem;
}

.chef__list li {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  font-weight: 500;
  color: var(--text-dark);
}

.chef__list li span {
  font-size: 1.5rem;
}

.chef__list li:nth-child(1) span {
  color: #62b15c;
}
.chef__list li:nth-child(2) span {
  color: #ff3e67;
}
.chef__list li:nth-child(3) span {
  color: #185adb;
}

.client__container {
  padding-top: 0;
}

.client__container :is(.section__header, .section__description) {
  max-width: 600px;
  margin-inline: auto;
  text-align: center;
}

.client__swiper {
  margin-top: 2rem;
  max-width: 750px;
  margin-inline: auto;
  padding: 3rem 1rem;
  overflow: hidden;
  border: 2px solid rgba(252, 127, 9, 0.5);
  box-shadow: 5px 5px 30px rgba(252, 127, 9, 0.2);
  border-radius: 3rem;
}

.swiper {
  padding-bottom: 3rem;
  width: 100%;
}

.client__card {
  text-align: center;
}

.client__card p {
  margin-bottom: 2rem;
  color: var(--text-dark);
  line-height: 1.75rem;
}

.client__card img {
  margin-bottom: 1rem;
  max-width: 70px;
  margin-inline: auto;
  border-radius: 100%;
  box-shadow: 5px 5px 20px rgba(0, 0, 0, 0.2);
}

.client__card h4 {
  font-size: 1.2rem;
  font-weight: 600;
  color: var(--text-dark);
}

.client__card h5 {
  font-size: 1rem;
  font-weight: 500;
  color: var(--text-light);
}

.swiper-pagination-bullet-active {
  background-color: var(--primary-color);
}

.footer {
  background-color: var(--primary-color-light);
}

.footer__container {
  display: grid;
  gap: 4rem 2rem;
}

.footer__logo {
  margin-bottom: 1rem;
}

.footer__col .section__description {
  text-align: left;
}

.footer__col h4 {
  margin-bottom: 1rem;
  font-size: 1.2rem;
  font-weight: 600;
  color: var(--text-dark);
}

.footer__links {
  display: grid;
  gap: 0.75rem;
}

.footer__links a {
  color: var(--text-light);
}

.footer__links a:hover {
  color: var(--primary-color);
}

.footer__bar {
  padding: 1rem;
  font-size: 0.9rem;
  color: var(--text-light);
  text-align: center;
}

@media (width > 540px) {
  .special__grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .banner__container {
    grid-template-columns: repeat(2, 1fr);
  }

  .footer__container {
    grid-template-columns: 3fr 2fr;
  }
}

@media (width > 768px) {
  nav {
    position: static;
    padding: 2rem 1rem;
    max-width: var(--max-width);
    margin-inline: auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 2rem;
  }

  .nav__header {
    flex: 1;
    padding: 0;
    background-color: transparent;
  }

  .nav__logo a {
    color: var(--primary-color);
  }

  .nav__menu__btn {
    display: none;
  }

  .nav__links {
    position: static;
    padding: 0;
    flex-direction: row;
    background-color: transparent;
    transform: none;
  }

  .nav__links a {
    color: var(--text-dark);
  }

  .nav__links a:hover {
    color: var(--primary-color);
  }

  .nav__btn {
    display: flex;
    flex: 1;
  }

  .nav__btn .btn {
    padding: 8px 10px;
    font-size: 1.5rem;
    border-radius: 100%;
  }

  .header__container {
    grid-template-columns: 2fr 3fr;
    align-items: center;
  }

  .header__content h1,
  .header__content .section__description,
  .header__btn {
    text-align: left;
  }

  .header__image {
    grid-area: 1/2/2/3;
  }

  .special__grid {
    grid-template-columns: repeat(3, 1fr);
  }

  .explore__container {
    grid-template-columns: repeat(2, 1fr);
    align-items: center;
  }

  .explore__content .section__header {
    max-width: 500px;
  }

  .explore__content :is(.section__header, .section__description),
  .explore__btn {
    text-align: left;
  }

  .banner__container {
    grid-template-columns: repeat(3, 1fr);
  }

  .chef__bg {
    max-width: 300px;
  }

  .chef__container {
    grid-template-columns: repeat(2, 1fr);
    align-items: center;
  }

  .chef__image {
    grid-area: 1/2/2/3;
  }

  .chef__content :is(.section__header, .section__description) {
    text-align: left;
  }

  .chef__list li {
    justify-content: flex-start;
  }

  .client__swiper {
    padding: 3rem 2rem;
  }

  .footer__container {
    grid-template-columns: 2fr repeat(3, 1fr);
  }
}

@media (width > 1024px) {
  .special__grid {
    gap: 2rem;
  }

  .special__card {
    padding: 2rem;
    border-radius: 3rem;
  }

  .banner__container {
    gap: 2rem;
  }

  .chef__bg {
    max-width: 375px;
  }
}</style>
  <body>
    <nav>
      <div class="nav__header">
        <div class="logo nav__logo">
          <a href="#">PINOY D'<span>ORIHINAL</span></a>
        </div>
        <div class="nav__menu__btn" id="menu-btn">
          <span><i class="ri-menu-line"></i></span>
        </div>
      </div>
      <ul class="nav__links" id="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#special">Special</a></li>
        <li><a href="#chef">Chef</a></li>
        <li><a href="#client">Clients</a></li>
        <li><a href="#contact">Contact Us</a></li>
      </ul>
      <div class="nav__btn">
        <button class="btn"><i class="ri-shopping-bag-fill"></i></button>
      </div>
    </nav>
    <header class="section__container header__container" id="home">
      <div class="header__image">
        <img src="/header.jpg" alt="header" />
      </div>
      <div class="header__content">
        <h1>Meet, Eat & Enjoy The <span>True Taste</span>.</h1>
        <p class="section__description">
          
          
          Discover the true essence of Filipino culinary delight as you meet, eat, and
          savor the authentic Filipino flavors that define our passion for food.
        </p>
        <div class="header__btn">
          <button class="btn">Get Started</button>
        </div>
      </div>
    </header>

    <section class="section__container special__container" id="special">
      <h2 class="section__header">Our Special Dish</h2>
      <p class="section__description">
        Each dish promises an unforgettable dining experience, blending
        innovation with tradition to delight your senses.
      </p>
      <div class="special__grid">
        <div class="special__card">
          <img src="/assets/Kare-Kare.jpg" alt="special" />
          <h4>Kare - Kare</h4>
          <p>
             A Filipino stew made with  beef stew meat cooked in a rich peanut sauce.It's traditionally served with a side of bagoong. It's a beloved dish in Filipino cuisine, known for its complex flavors and creamy texture.
          </p>
          <div class="special__ratings">
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
          </div>
          <div class="special__footer">
            <p class="price">350 PESOS</p>
            <button class="btn">Add to Cart</button>
          </div>
        </div>
        <div class="special__card">
          <img src="bulalo.jpg" alt="special" />
          <h4>Beef Bulalo</h4>
          <p>
             A  Filipino soup made with beef shanks and marrow bones, the broth is rich and savory. Bulalo is a comforting and satisfying dish, especially popular during colder months or rainy days.
          </p>
          <div class="special__ratings">
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
          </div>
          <div class="special__footer">
            <p class="price">350 PESOS</p>
            <button class="btn">Add to Cart</button>
          </div>
        </div>
        <div class="special__card">
          <img src="sinigang.jpg" alt="special" />
          <h4>Sinigang na Baboy</h4>
          <p>
             traditional Filipino sour soup made with pork, typically pork belly or ribs, simmered with tamarind broth. It's known for its tangy and savory flavor profile and is often enjoyed with steamed rice.
          </p>
          <div class="special__ratings">
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
          </div>
          <div class="special__footer">
            <p class="price">350 PESOS</p>
            <button class="btn">Add to Cart</button>
          </div>
        </div>
         <div class="special__card">

          <img src="lumpia.jpg" alt="special" />

          <h4>Lumpiang Shanghai</h4>
          <p>
             Filipino version of spring rolls  wrapped in thin spring roll wrappers and deep-fried until crispy. It's commonly served as an appetizer or snack, often accompanied by a sweet and sour dipping sauce.
          </p>
          <div class="special__ratings">
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
          </div>
          <div class="special__footer">
            <p class="price">150 PESOS</p>
            <button class="btn">Add to Cart</button>
          </div>
        </div>
    <div class="special__card">

          <img src="Crispy pata.jpg" alt="special" />

          <h4>Crispy Pata</h4>
          <p>
             A Filipino dish consisting of deep-fried pig trotters or knuckles. It's often served with a dipping sauce made from vinegar, soy sauce, and garlic, and it's a popular dish for special occasions and gatherings.
          </p>
          <div class="special__ratings">
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
          </div>
          <div class="special__footer">
            <p class="price">650 PESOS</p>
            <button class="btn">Add to Cart</button>
          </div>
        </div>
    <div class="special__card">

          <img src="sisig-2.jpg" alt="special" />

          <h4>Pork Sisig</h4>
          <p>
            A flavorful Filipino dish made from chopped pig's face and ears, seasoned with calamansi (Philippine lime), onions, and chili peppers. It's commonly enjoyed as a savory appetizer or main course.
          </p>
          <div class="special__ratings">
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
          </div>
          <div class="special__footer">
            <p class="price">250 PESOS</p>
            <button class="btn">Add to Cart</button>
          </div>
        </div>
        

        <div class="special__card">

          <img src="LECHE FLAN.jpg" alt="special" />
          <h4>Leche Flan</h4>
          <p>
            Leche flan is a classic Filipino dessert that resembles a caramel custard.  Leche flan has a smooth and creamy texture with a sweet and slightly bitter caramel flavor, making it a popular treat for special occasions and celebrations.
          </p>
          <div class="special__ratings">
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
          </div>
          <div class="special__footer">
            <p class="price">80 PESOS</p>
            <button class="btn">Add to Cart</button>
          </div>
        </div>
  
     <div class="special__card">
.     <img src="halo halo.jpg" alt="special" />
          <h4>Halo-Halo</h4>
          <p>
             A delightful Filipino dessert that typically consists of a mixture of shaved ice, sweetened fruits, jellies, beans, and topped with evaporated milk and sometimes ice cream. It's a refreshing and colorful treat!
          </p>
          <div class="special__ratings">
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
          </div>
          <div class="special__footer">
            <p class="price">100 PESOS</p>
            <button class="btn">Add to Cart</button>
          </div>
        </div>
        
        <div class="special__card">



          <img src="turon.jpg" alt="special" />
          <h4>Turon</h4>
          <p>
             A popular Filipino snack made with ripe plantains (saba bananas), brown sugar and wrapped in a spring roll wrapper and fried until crispy. It's typically enjoyed as a sweet treat with a crunchy exterior and soft, sweet interior.
          </p>
          <div class="special__ratings">
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
            <span><i class="ri-star-fill"></i></span>
          </div>
          <div class="special__footer">
            <p class="price">100 PESOS</p>
            <button class="btn">Add to Cart</button>
          </div>
        </div>
 
 

 
 

      </div>
    </section>
        
   
  
  
        
    
 <section class="section__container explore__container">
      <div class="explore__image">
        <img src="pinoy cuisine.jpg" alt="explore" />
      </div>
      <div class="explore__content">
        <h1 class="section__header">We Serve Healthy & Tasty Filipino Food</h1>
        <p class="section__description">
          Indulge guilt-free with our commitment to serving wholesome and
          delicious Filipino meals. Explore a menu curated to balance taste and
          nutrition, ensuring every bite is both satisfying and nourishing.
        </p>
        <div class="explore__btn">
          <button class="btn">
            Explore Story <span><i class="ri-arrow-right-line"></i></span>
          </button>
        </div>
      </div>
    </section>

    <section class="section__container banner__container">
      <div class="banner__card">
        <span class="banner__icon"><i class="ri-bowl-fill"></i></span>
        <h4>Order Your Food</h4>
        <p>
          Seamlessly place your food orders online with just a few clicks. Enjoy
          convenience and efficiency as you select from our diverse menu of
          delectable dishes.
        </p>
        <a href="#">
          Read more
          <span><i class="ri-arrow-right-line"></i></span>
        </a>
      </div>
      <div class="banner__card">
        <span class="banner__icon"><i class="ri-truck-fill"></i></span>
        <h4>Pick Your Food</h4>
        <p>
          Customize your dining experience by choosing from a tantalizing array
          of options. For savory, sweet, or in between craving, find the perfect
          meal to satisfy your appetite.
        </p>
        <a href="#">
          Read more
          <span><i class="ri-arrow-right-line"></i></span>
        </a>
      </div>
      <div class="banner__card">
        <span class="banner__icon"><i class="ri-star-smile-fill"></i></span>
        <h4>Enjoy Your Food</h4>
        <p>
          Sit back, relax, and savor the flavors as your meticulously prepared
          meal arrives. Delight in the deliciousness of every bite, knowing that
          your satisfaction is our top priority.
        </p>
        <a href="#">
          Read more
          <span><i class="ri-arrow-right-line"></i></span>
        </a>
      </div>
    </section>

    <section class="chef" id="chef">
      <img src= "" alt="topping" class="chef__bg" />
      <div class="section__container chef__container">
        <div class="chef__image">
          <img src="arvin.jpg" alt="chef" />
        </div>
        <div class="chef__content">
          <h2 class="section__header">Cooked By The Best Chefs In The Country</h2>
          <p class="section__description">
            Experience culinary excellence crafted by master chefs from around
            the globe. Our team of culinary virtuosos brings together expertise,
            innovation, and passion to create unforgettable dining experiences
            that redefine gastronomy.
          </p>
          <ul class="chef__list">
            <li>
              <span><i class="ri-checkbox-fill"></i></span>
              Savour culinary brilliance from master chefs worldwide.
            </li>
            <li>
              <span><i class="ri-checkbox-fill"></i></span>
              Experience innovative creations with attention to detail.
            </li>
            <li>
              <span><i class="ri-checkbox-fill"></i></span>
              Enjoy dishes crafted with an unwavering passion for perfection.
            </li>
          </ul>
        </div>
      </div>
    </section>

    <section class="section__container client__container" id="client">
      <h2 class="section__header">What Our Customers Are Saying</h2>
      <p class="section__description">
        Discover firsthand experiences and testimonials from our valued patrons.
        Explore the feedback and reviews that showcase our commitment to
        quality, service, and customer satisfaction.
      </p>
      <div class="client__swiper">
        <!-- Slider main container -->
        <div class="swiper">
          <!-- Additional required wrapper -->
          <div class="swiper-wrapper">
            <!-- Slides -->
            <div class="swiper-slide">
              <div class="client__card">
                <p>
                  MASAYANG KAINAN's culinary expertise never fails to impress! Every
                  dish is a masterpiece, bursting with flavor and freshness.
                </p>
                <img src="jose.jpg" alt="client" />
                <h4>Jose Gavina</h4>
                <h5>Student </h5>
              </div>
            </div>
            <div class="swiper-slide">
              <div class="client__card">
                <p>
                  I always turn to PINOY D' ORIHINAL for a quick and delicious meal. Their
                  efficient service and mouthwatering options never disappoint!
                </p>
                <img src="kevin.jpg" alt="client" />
                <h4>Kevin Dexter Rolusta</h4>
                <h5>Student</h5>
              </div>
            </div>
            <div class="swiper-slide">
              <div class="client__card">
                <p>
                  PINOY D' ORIHINAL has become my go-to for all my catering needs. Their
                  attention to detail and exceptional customer service make
                  every event a success.
                </p>
                <img src="carlyn.jpeg" alt="client" />
                <h4>Carlyn Morales</h4>
                <h5>Student</h5>
              </div>
            </div>
          </div>
          <!-- If we need pagination -->
          <div class="swiper-pagination"></div>
        </div>
      </div>
    </section>

    <footer class="footer" id="contact">
      <div class="section__container footer__container">
        <div class="footer__col">
          <div class="logo footer__logo">
            <a href="#">MASAYANG<span>KAINAN</span></a>
          </div>
          <p class="section__description">
             Reflects the joy and gratitude we feel when indulging in delicious food, but it also symbolizes the bonds we strengthen and the memories we create with loved ones. It's a celebration of life's simple pleasures and the warmth of companionship around the table.
          </p>
        </div>
        <div class="footer__col">
          <h4>Product</h4>
          <ul class="footer__links">
            <li><a href="#">Menu</a></li>
            <li><a href="#">Specials</a></li>
            <li><a href="#">Meal Deals</a></li>
            <li><a href="#">Catering Options</a></li>
            <li><a href="#">Seasonal Offerings</a></li>
          </ul>
        </div>
        <div class="footer__col">
          <h4>Information</h4>
          <ul class="footer__links">
            <li><a href="#">About Us</a></li>
            <li><a href="#">Contact Us</a></li>
            <li><a href="#">Nutrition Information</a></li>
            <li><a href="#">Allergen Information</a></li>
          </ul>
        </div>
        <div class="footer__col">
          <h4>Company</h4>
          <ul class="footer__links">
            <li><a href="#">Our Story</a></li>
            <li><a href="#">Careers</a></li>
            <li><a href="#">Terms of Service</a></li>
            <li><a href="#">Privacy Policy</a></li>
          </ul>
        </div>
      </div>
      <div class="footer__bar">
        Copyright © 2024 Web Design Mastery. All rights reserved.
      </div>
    </footer>

    <script src="https://unpkg.com/scrollreveal"></script>
    <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
    <script src="main.js"></script>
  </body>
</html>
