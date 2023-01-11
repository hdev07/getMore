<template>
  <div class="container-footer">
    <div class="footer">
      <div class="text">
        <p>Inicio</p>
        <p>Acerca de nosotros</p>
        <p>Historia</p>
        <p>Contacto</p>
      </div>
      <div class="img">
        <img src="../assets/images/F1.png" alt="" />
        <img src="../assets/images/F2.png" alt="" />
        <img src="../assets/images/F3.png" alt="" />
        <img src="../assets/images/F4.png" alt="" />
        <img src="../assets/images/F5.png" alt="" />
      </div>
    </div>
    <div class="logo">
      <img src="../assets/images/logo.png" alt="" />
    </div>
  </div>
</template>

<script></script>

<style lang="scss" scoped>
div .container-footer {
  display: flex;
  background-color: $--sickly-yellow;
  justify-content: space-between;
  align-items: center;
  height: 24vh;
  .footer {
    width: 35vw;
    padding-left: 16 * $--spacing-xxs;
    .text {
      margin-top: 16 * $--spacing-xxs;
      display: flex;
      justify-content: space-between;
      font-family: HelveticaNeue;
      font-size: 13px;
      font-weight: normal;
      font-stretch: normal;
      font-style: normal;
      line-height: normal;
      letter-spacing: 1.14px;
    }
  }
}

div .footer .img {
  display: flex;
  margin-top: 3vh;
  img {
    width: 2rem;
    padding-right: 3 * $--spacing-xxs;
  }
}
.logo img {
  margin-right: 3vw;
  width: 55px;
}
@media screen and (max-width: 864px) {
  div .container-footer {
    flex-direction: column;
    .footer {
      margin-top: -10px;
      width: 100vw;
      padding: 0 20px 0 20px;
      .img {
        justify-content: center;
      }
      img {
        width: 12vw;
      }
    }
  }
  .logo img {
    padding: 5%;
    width: 60px;
  }
}
</style>
