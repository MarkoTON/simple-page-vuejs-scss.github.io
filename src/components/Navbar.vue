<template>
  <header>
    <div class="container">
      <div class="logo">
        <a href="#"><img src="../assets/icons/icon-sun.svg" alt="Logo icon">Always outdors</a>
      </div>
      <nav>
        <a href="#"><li>Destionations</li></a>
        <a href="#"><li>Travel Style</li></a>
        <a href="#"><li>Travel Deals</li></a>
        <a href="#"><li>Gear</li></a>
      </nav>
      <div class="search">
        <img src="../assets/icons/icon-search.svg" alt="Search icon">
        <input type="text" placeholder="Search">
      </div>
    </div>
  </header>
</template>
<script>

</script>
<style lang="scss">
header {
  position: fixed;
  top:0;
  z-index: 100;
  width: 100%;
  background-color: color(primary);
  color: white;

  .container {
    display: flex;
    justify-content: space-between;
    flex-direction: column;
    

    .logo {
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 1rem;
  
      a {
        color:white;
        display: flex;
        align-items: center;
        text-decoration: none;
        text-transform: uppercase;
        font-size: 1.5rem;
  
        img {
          margin-right: 1rem;
        }
      }
  
    }
  
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      list-style: none;
      padding: 0 1rem;
  
      a {
        font-size: 0.95rem;
        text-decoration: none;
        
        li {
          color:white;
        }
      }
    }
  
    .search {
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 1rem;
      
      img {
        height: 1.5rem;
        margin-right: 5px;
      }
  
      input {
        color: white;
        background-color: rgba(0,0,0,0);
        border:none;
        height: 32px;
        width: 80px;
        font-size: 1.2rem;
  
        &::-webkit-input-placeholder {
          font-size: 1.5rem;
          color: white;
          font-weight: 400;
          opacity: 1; 
        }
  
        &:focus {
          outline: none;
        }
      }
    }
  }


}

@include tablet {
  header {
    .container {
      flex-direction: row;
  
      .logo {
        width: 200px;
      }
  
      nav {
        width: 55%;
      }
    }
  }
}

@include laptop {
  header{
    .container {

      .logo {
        width: 300px;
      }
  
      nav {
        justify-content: center;
        padding: 0 0.5rem;
  
        a {
          padding: 0 0.25rem;
        }
      }
  
      .search {
        input {
          color: white;
          background-color: rgba(0,0,0,0);
          border:none;
          height: 32px;
          width: 80px;
          font-size: 1.2rem;
  
          &::-webkit-input-placeholder {
            font-size: 1.3rem;
            color: white;
            font-weight: 400;
            opacity: 1; 
          }
        }
      }
    }

  }
}
</style>