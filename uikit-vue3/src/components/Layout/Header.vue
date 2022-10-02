<template>
  <header class="header">
    <div class="header__top">
      <div class="container">
        <div class="header__content">
          <router-link class="header__logo" to="/"><img class="img" src="@/assets/icon.png" alt="icon"></router-link>
          <div class="header__region">
            <button class="header__btn">Москва и область</button>
          </div>
          <nav class="header__nav">
            <router-link class="header__link" to="#">Магазины</router-link>
            <router-link class="header__link" to="#">Сервесные центры</router-link>
            <router-link class="header__link" to="#">Для бизнеса</router-link>
            <router-link class="header__link" to="#">Оплата и доставка</router-link>
            <router-link class="header__link" to="#">Блог</router-link>
          </nav>
          <div class="header__cabinet">
            <img src="@/assets/cabinet.png" alt="logo cabinet" class="logo__cabinet">
            <span>Личный кабинет</span>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.header{
  &__content{
    display: flex;
    align-items: center;
  }
  background-color: #000;
  position: relative;
  width: 100%;
  z-index: 150;
  &__top{
    padding: 12px 0 14px;
  }
  &__logo{
    margin-right: 60px;
  }
  &__btn{
    background: #000;
    border: none;
    color: white;
    &::after{
      content: " ";
      background: url("../../assets/arrow.png") no-repeat;
      padding-left: 14px;
      margin-left: 9px;
    }
  }
  &__nav{
    margin-left: 40px;
  }
  &__link{
    margin-left: 25px;
    color: white;
    &:first-child{
      margin-left: 0;
    }
  }
  &__cabinet{
    color: #9999;
    margin-left: auto;
  }
}
.container{
  margin: 0 auto;
  max-width: 1440px;
  padding-left: 20px;
  padding-right: 20px;
}
.img{
  width: 130px;
}
.link{
  color: white;
}
.logo__cabinet{
  background: white;
  width: 15px;
  border-radius: 25px;
  border: 1px solid white;
  margin-right: 5px;
}
</style>
