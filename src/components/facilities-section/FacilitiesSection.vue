<template>
  <section class="section">
    <div class="section__top">
      <div class="container-sm">
        <div class="eye-logo">
          <img src="../../assets/img/icon-7.png" alt="eye icon" />
        </div>
        <h1>TOUR OUR FACILITIES</h1>
        <hr />
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil autem
          aspernatur laboriosam cupiditate saepe magnam earum provident
          necessitatibus nesciunt ad, officiis voluptate est, quisquam amet
          culpa illo quia non blanditiis!
        </p>
        <button class="play"></button>
      </div>
    </div>
    <div class="section__bottom">
      <div class="card">
        <div>
          <h4>Emergency Care</h4>
        </div>
        <div>
          <img src="../../assets/img/wave-divider.png" alt="" />
        </div>
        <div>
          <p>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. At,
            nostrum ipsa excepturi perfere
          </p>
        </div>
        <div>
          <button>LEARN MORE</button>
        </div>
      </div>
      <div class="card">
        <div>
          <h4>Expert Diagnostics</h4>
        </div>
        <div>
          <img src="../../assets/img/wave-divider.png" alt="" />
        </div>
        <div>
          <p>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. At,
            nostrum ipsa excepturi perfere
          </p>
        </div>
        <div>
          <button>LEARN MORE</button>
        </div>
      </div>
      <div class="card">
        <div>
          <h4>Superb Rehabilitation</h4>
        </div>
        <div>
          <img src="../../assets/img/wave-divider.png" alt="" />
        </div>
        <div>
          <p>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. At,
            nostrum ipsa excepturi perfere
          </p>
        </div>
        <div>
          <button>LEARN MORE</button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "FacilitiesSection",
};
</script>

<style lang="scss" scoped>
.section {

  &__top {
    background-image: url("../../assets/img/paralax-bg-tour-facilities.jpg");
    // padding: 60px 0;
    height: 500px;
    background-position: center;
    background-size: cover;
    text-align: center;
    color: var(--color-white);
    display: flex;
    align-items: center;

    & h1 {
      font-weight: 400;
    }

    & hr {
      width: 50%;
      margin: 20px auto;
      border: 1px solid var(--color-lightgrey);
      background-color: var(--color-lightgrey);
    }

    .play {
      height: 50px;
      width: 50px;
      border-radius: 50%;
      background-image: url("../../assets/img/play-icon.png");
      background-position: center;
      background-size: cover;
      margin-top: 20px;
      border:none;
      transition:0.25s;
    }

    .play:hover {
      cursor: pointer;
      transform: scale(1.2);
      transition:0.25s;
    }
  }

  &__bottom {
    display: flex;
    text-align: center;
    color: var(--color-white);

    $colors: #3aafbf #3597c3 #327ec7;

    @for $i from 1 through 3 {
      &>div:nth-child(3n + #{$i}) {
        background-color: nth($colors, $i);
      }
    }

    &>div {
      padding: 40px 0;
      display: flex;
      flex-direction: column;
      justify-content: center;
      width: calc(100% / 3);

      button {
        background: none;
        border: 1px solid white;
        color: white;
        padding: 10px 25px;
        transition: 0.25s;
        margin-top: 10px;

        &:hover {
          cursor: pointer;
          transform: scale(1.1);
          background: rgba(0, 0, 0, 25%);
          color: white;
          transition: 0.25s;
        }
      }

      &>* {
        margin-bottom: 5px;
      }
    }
  }
}
</style>