<template>
  <header>
    <div class="wrapper">
      <nav>
        <RouterLink class="logo" to="/">
          <img src="./../assets/images/logo.png" alt="">
          <h1>Taobao</h1>
        </RouterLink>

        
        <div class="category-wrapper">
          <RouterLink class="category" to="/about">Trending</RouterLink>
          <a href="" class="category-separator">|</a>
          <RouterLink class="category" to="/product">Products</RouterLink>
          <a href="" class="category-separator">|</a>
          <RouterLink class="category" to="/about">More</RouterLink>

          <!-- <button @click="$emit('checkout')">Go to checkout</button> -->
        </div>

        <div class="right-Wrapper">

          <div id="search">
            <input type="text" placeholder="Search">
            <button>
              <svg width="30" height="30" viewBox="0 0 36 37" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M35.0473 30.2617L27.1164 22.3307C28.4972 20.0947 29.3321 17.4864 29.3321 14.666C29.3321 6.56587 22.7662 0 14.666 0C6.56587 0 0 6.56587 0 14.666C0 22.7662 6.56587 29.3321 14.666 29.3321C17.4864 29.3321 20.0947 28.4972 22.3285 27.1186L30.2617 35.0496C30.9001 35.6669 31.7556 36.0086 32.6436 36.001C33.5317 35.9935 34.3812 35.6372 35.0091 35.0091C35.6369 34.381 35.9927 33.5313 35.9999 32.6432C36.007 31.7551 35.6649 30.8998 35.0473 30.2617ZM14.666 24.8194C9.05909 24.8194 4.51262 20.273 4.51262 14.666C4.51262 9.05909 9.05909 4.51262 14.666 4.51262C20.273 4.51262 24.8194 9.05909 24.8194 14.666C24.8194 20.273 20.273 24.8194 14.666 24.8194Z" fill="#F16573"/>
              </svg>
            </button>
          </div>
          
          <a href="">

              <img src="./../assets/images/carticon.svg" alt="">
              <p>Cart(1)</p>
          </a>
          
        </div>

      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Jua&display=swap');

  nav {
    position: static;
    top: 0px;
    left: 0px;
    right: 0px;
    height: 100px;
    
    display: flex;
    font-family: 'Jua', sans-serif;
    background-color: #FFD7CB;

    padding: 20px;
    padding-left: 50px;
    padding-right: 50px;
    box-shadow: 0px 10px 4px rgba(0, 0, 0, 0.25);
  }
  

  .logo img {
    margin-top: -35px;
    display: inline-block;
  }

  .logo h1 {
    display: inline-block;
    font-size: 40px;
    font-family: 'Inter', sans-serif;

    font-weight: 700;
    color: #D06325;

    margin-left: 20px;
  }

  .category-wrapper {
    display: inline-block;

    margin-left: 50px;
    margin-top: auto;
    margin-bottom: auto;
    margin-right: auto;

    font-size: 25px;
  }

  .category-wrapper .category-separator {
    margin-left: 15px;
    margin-right: 15px;
    color: #D06325;
  }
  .category-wrapper a {
    color: black;
  }

  .right-Wrapper {
    display: inline-flex;
    align-self: center;
    width: 50%;
    
    margin-top: 7px;
    margin-left: auto;
    justify-content: right;
    gap: 10px;
    
  }

  .right-Wrapper img {
    display: inline-block;
  }

  #search {
    position: relative;
    width: 85%;
    margin-right: 20px;
  }

  #search input {
    width: 100%;
    height: 45px;
    font-size: large;
    
    padding-left: 20px;
    padding-right: 60px;

    border-radius: 28px;
    border-width: 3px;
    border-color: #33345D;
  }

  #search button {
    position: absolute;
    top: 3px;
    height: 40px;
    right: 20px;

    display: flex;
    align-items: center;
  }

  .right-Wrapper a {
    display: inline-block;
    font-size: xx-large;
    display: flex;
    justify-content: space-between;
    height: 55px;
  }
  .right-Wrapper a p {
    display: inline-block;
    align-self: center;
    margin-left: 20px;
    font-family: 'Jua', sans-serif;
  }

</style>