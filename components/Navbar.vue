<template>
  <div>
    <div class="line" />
    <div class="navbar">
      <nav>
        <input type="checkbox" id="nav" class="hidden" />
        <label for="nav" class="nav-btn">
          <i></i>
          <i></i>
          <i></i>
        </label>
        <div class="logo">
          <a><img src="../assets/images/logo.png" alt="logo" /></a>
        </div>
        <div class="nav-wrapper">
          <ul class="nav-items">
            <li><a href="#">Inicio</a></li>
            <li><a href="#">Acerca de nosotros</a></li>
            <li><a href="#">Historia</a></li>
            <li><a href="#">Contacto</a></li>
          </ul>
          <div class="lang">
            <span><b>ES</b></span>
            <span>EN</span>
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.logo {
  float: left;
  margin-top: 25px;
  margin-left: 9 * $--spacing-xxs;
}

.logo img {
  width: 37px;
}

.line {
  width: 1px;
  border: solid 2px #fff;
  position: absolute;
  margin: 0 512px 370px 105px;
  padding-top: 104vh;
}

nav ul {
  float: left;
  margin-top: 11 * $--spacing-xxs;
  margin-left: 25 * $--spacing-xxs;
}

.lang {
  float: right;
  display: flex;
  justify-content: space-around;
  width: 5rem;
  color: white;
  margin: 45px 94px 0 0;
}
nav ul li {
  display: inline-block;
}

nav ul li:not(:first-child) {
  margin-left: 48px;
}

nav ul li:last-child {
  margin-right: 24px;
}

nav ul li a {
  display: inline-block;
  outline: none;
  color: #fff;
  text-decoration: none;
}

@media screen and (max-width: 864px) {
  .logo {
    margin: 7vw;
  }

  .logo img {
    width: 9vw;
  }

  .lang {
    color: #000;
    position: absolute;
    top: 90vh;
    left: 76vw;
  }

  .nav-wrapper {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
    background: #f3f4f8;
    opacity: 0;
    transition: all 0.2s ease;
  }

  .nav-wrapper ul {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    width: 100%;
  }

  .nav-wrapper ul li {
    display: block;
    float: none;
    width: 100%;
    text-align: right;
    margin-bottom: 10px;
  }

  .nav-wrapper ul li:nth-child(1) a {
    transition-delay: 0.2s;
  }

  .nav-wrapper ul li:nth-child(2) a {
    transition-delay: 0.3s;
  }

  .nav-wrapper ul li:nth-child(3) a {
    transition-delay: 0.4s;
  }

  .nav-wrapper ul li:nth-child(4) a {
    transition-delay: 0.5s;
  }

  .nav-wrapper ul li:not(:first-child) {
    margin-left: 0;
  }

  .nav-wrapper ul li a {
    padding: 10px 24px;
    opacity: 0;
    color: #000;
    font-size: 14px;
    font-weight: 600;
    letter-spacing: 1.2px;
    transform: translateX(-20px);
    transition: all 0.2s ease;
  }

  .nav-btn {
    position: fixed;
    right: 15px;
    top: 15px;
    display: block;
    width: 48px;
    height: 48px;
    cursor: pointer;
    z-index: 9998;
    border-radius: 50%;
  }

  .nav-btn i {
    display: block;
    width: 20px;
    height: 2px;
    background: #fff;
    border-radius: 2px;
    margin-left: 14px;
  }

  .nav-btn i:nth-child(1) {
    margin-top: 16px;
  }

  .nav-btn i:nth-child(2) {
    margin-top: 4px;
    opacity: 1;
  }

  .nav-btn i:nth-child(3) {
    margin-top: 4px;
  }
  nav ul {
    margin: 0;
  }
  .line {
    display: none;
  }
}

#nav:checked + .nav-btn {
  transform: rotate(45deg);
}

#nav:checked + .nav-btn i {
  background: #000;
  transition: transform 0.2s ease;
}

#nav:checked + .nav-btn i:nth-child(1) {
  transform: translateY(6px) rotate(180deg);
}

#nav:checked + .nav-btn i:nth-child(2) {
  opacity: 0;
}

#nav:checked + .nav-btn i:nth-child(3) {
  transform: translateY(-6px) rotate(90deg);
}

#nav:checked ~ .nav-wrapper {
  z-index: 9990;
  opacity: 1;
}

#nav:checked ~ .nav-wrapper ul li a {
  opacity: 1;
  transform: translateX(0);
}

.hidden {
  display: none;
}
</style>
