<template>
  <footer>
    <nav>
      <ul>
        <a href=""><li>Destinations</li></a>
        <a href=""><li>Travel</li></a>
        <a href=""><li>Destinations</li></a>
        <a href=""><li>Destinations</li></a>
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
    </div>

    <div id="footer-item">
      <div class="logo-item">
        <img src="../assets/icons/icon-sun.svg" alt="Logo of sun">
        <span>
          Always outdors
        </span>
      </div>

      <div class="copy-right">
        &copy; 2021, Always Outside
      </div>
    </div>
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
    font-size: 12px;
    justify-content: center;
    padding: 20px 15px;

      a {
        margin: 10px;
        color: white;
        text-decoration: none;

        li {
          list-style: none;
        }
      }
    }
  }
}

@include tablet {
  footer {
    flex-direction: row;
    justify-content: center;

    a {
      margin: 0 10px;
    };
  };
};

@include laptop {
  footer {
    font-size: 1rem;
  };
};
</style>