<template>
  <footer>
      <nav>
        <ul>
          <a href="#"><li>Destinations</li></a>
          <a href="#"><li>Travel styles</li></a>
          <a href="#"><li>Travel Deal</li></a>
          <a href="#"><li>Gear</li></a>
        </ul>
      </nav>

      <div class="media">
        <div class="icon-media">
          <img src="../assets/icons/icon-twitter.svg" alt="Twitter">
        </div>
        <div class="icon-media">
          <img src="../assets/icons/icon-instagram.svg" alt="Instagram">
        </div>
        <div class="icon-media">
          <img src="../assets/icons/icon-facebook.svg" alt="Facebook">
        </div>
      </div><!-- .media -->

      <div id="footer-item">
        <div class="container">
          <div class="logo-item">
            <img src="../assets/icons/icon-sun.svg" alt="Logo of sun">
            <span>Always outdors</span>
          </div><!-- logo-item -->

          <div class="copy-right">
            &copy; 2021, Always Outside
          </div><!-- copy-right -->
        </div><!-- container -->
      </div><!-- id=footer-item -->
  </footer>
</template>
<script>
export default {
  name: "footer"
};
</script>
<style lang="scss">
footer {
  background-color: color(footer-color);

    nav {
      padding: 30px 0;
  
      ul {
        display: flex;
        flex-direction: row;
        font-size: 0.95rem;
        justify-content: space-around;
        padding: 20px 0px;
  
          a {
            text-decoration: none;
  
            li {
              color: white;
              list-style: none;
            }
          }
        }
      }
      
    .media {
      display: flex;
      align-items: center;
      justify-content: center;
      padding-bottom: 40px;
      
      .icon-media {
        text-align: center;
        border-radius: 50px;
        width: 35px;
        height: 35px;
        background-color: #0193af;
        margin: 0 5px;
        
        img {
          width: 20px;
          margin-top: 8px;
        }
      }
      
    }
    
    #footer-item {
      padding: 20px 15px;
      background-color: #1b373b;
      font-size: 12px;

      .container {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .logo-item {
          display: flex;
          align-items: center;
    
          span {
            color: white;
          }
          img {
            margin-right: 15px;
          }
        }
    
        .copy-right {
          color: white;
        }
      }
      
    }

}

@include tablet {
  footer {
    flex-direction: row;
    justify-content: center;

      nav {
        ul {
          justify-content: center
        }
      }
 
     a {
       margin: 0 10px;
     };
    }
};

@include laptop {
  footer {
    font-size: 1rem;
    
    nav {
      ul {
        font-size: 1rem;
      }
    }

     #footer-item {
       font-size: 1rem;
     }
  };
};
</style>