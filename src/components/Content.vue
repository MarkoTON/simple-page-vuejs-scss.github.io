<template>
  <main>
    <section class="connect-to-world">
      <h1>Connect to the world</h1>
      <div class="main-content-world">
        <article>
          <h3>Out world deservers more you</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit, officiis necessitatibus quod ea sapiente quis nostrum quas eos. Ut a laboriosam amet, repudiandae placeat adipisci! Esse, rem explicabo sequi eveniet magnam aspernatur id enim repellendus, eos ea architecto, cupiditate sapiente.
          </p>
          <h3>Whatever your style, see it your way</h3>
          <p>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Voluptatum ducimus, provident omnis repellendus adipisci reprehenderit nobis, ab itaque dolores dolore architecto consectetur quas molestias odio vitae a quibusdam deserunt. Amet?
          </p>
        </article>
        <div class="img-content">
          <!-- <img src="../assets/images/img-connect.jpg" alt="City image"> -->
        </div>
      </div>
    </section><!-- connect-to-world -->
    <section class="adventure-travel bg-cover-gradient">
      <h1>Why adventure travel?</h1>
      <div class="card-section">
        <div class="card">
          <div>
            <span class="icon icon-airplane"></span>
          </div>
          <div class="card-body">
            <h2>Explore The World</h2>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas illo porro, perspiciatis optio excepturi praesentium dolorum itaque earum temporibus? Aut!
            </p>
          </div><!-- card-body -->
        </div><!-- card -->
        <div class="card">
          <img src="../assets/icons/icon-earth.svg" alt="Icon airplane">
          <div class="card-body">
            <h2>Meet nature</h2>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas illo porro, perspiciatis optio excepturi praesentium dolorum itaque earum temporibus? Aut!
            </p>
          </div><!-- card-body -->
        </div><!-- card -->
        <div class="card">
          <img src="../assets/icons/icon-compass.svg" alt="Icon airplane">
          <div class="card-body">
            <h2>Know your way</h2>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas illo porro, perspiciatis optio excepturi praesentium dolorum itaque earum temporibus? Aut!
            </p>
          </div><!-- card-body -->
        </div><!-- card -->
        <div class="card">
          <img src="../assets/icons/icon-heart.svg" alt="Icon airplane">
          <div class="card-body">
            <h2>Live a healthier life</h2>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas illo porro, perspiciatis optio excepturi praesentium dolorum itaque earum temporibus? Aut!
            </p>
          </div><!-- card-body -->
        </div><!-- card -->
      </div><!-- card-section -->
    </section><!-- adventure-travel -->
  </main>
</template>
<script>

</script>
<style lang="scss">
main {
  margin-top: 149px;

  section.connect-to-world {
    padding: 1rem;

    h1 {
      padding: 0.5rem 0;
      text-align: center;
      text-transform: uppercase;
      letter-spacing: 2px;
      color: color(primary);
    };

    .main-content-world {
      display: flex;
      flex-direction: column;

      article {
        display: inline-block;
        padding-bottom: 1rem;
        h3 {
          padding: 0.5rem 0;
          color: color(primary);
        }
      }

      .img-content {
        display: inline-block;
        width: 100%;
        height: 300px;
        background: url("../assets/images/img-connect.jpg") center center;
        background-size: cover;
      }
    }

  }

  section.adventure-travel.bg-cover-gradient {
    position: relative;
    background: url("../assets/images/img-bg-adventure.jpg") center center;
    background-size: cover;
    clip-path: polygon(100% 0, 100% 98%, 0 100%, 0 2%);
    padding: 1rem;

    h1 {
      text-transform: uppercase;
      text-align: center;
      color: white;
      padding: 1rem 0;
    }

    &::after {
      content: "";
      z-index: -10;
      position: absolute;
      top: 0;
      left:0;
      width: 100%;
      height: 100%;
      background:linear-gradient(90deg, rgba(27,167,190,0.8186624991793592) 0%, rgba(27,167,190,0.5413515748096114) 53%, rgba(0,212,255,0.4433123591233369) 100%);;
    }

    .card-section {
      display: flex;
      flex-direction: column;

      .card {
        background-color: white;
        margin-bottom: 1rem;
        text-align: center;
        padding: 2rem 1rem;

        h2 {
          text-transform: uppercase;
          color: color(primary);
          padding: 0.5rem 0;
        }

        .icon {
          display: inline-block;
          width: 35px;
          height: 35px;
          background-size: cover;
        }
        .icon-airplane {
          background-image: icons(airplane);
        }
      }
    }
  }
}

@include tablet {
  main {
    margin-top: 97px;
  }
}

@include laptop {
  main {
    margin-top: 65px;
    section {
      .main-content-world {
        flex-direction: row;

        article {
          width: 100%;
        }
      }
    }

    section.adventure-travel.bg-cover-gradient {
      .card-section {
        justify-content: space-between;
        flex-direction: row;
        .card {
          margin-right: 1rem;

          &:last-child {
            margin-right: 0;
          }
        }
      }
    }
  }
}
</style>