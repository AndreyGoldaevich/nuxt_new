<template>
  <div id="profile" class="panel">
    <img
      id="photo"
      src="/avatar39.jpg"
      loading="lazy"
      alt="Muhaddis Profile Image"
    />

    <div class="box">
      <div class="in">
        <div class="one-half no-margin">
          <h5>Давайте знакомиться!</h5>

          Меня зовут Андрей мне 33 года 3 из которых я занимаюсь разработкой. Оцените мои работы
          <a href="#works">Portoflio</a> так же вы можете посмотреть данный сайт как одна из моих работ.
        </div>

        <div class="one-half no-margin column-last">
          <h5>Что же я умею?</h5>

          За все это время основной фреймворк который я использовал был Vue с php  на бэке.
          Я Активно развиваюсь по направлению Full stack developer.
        </div>
      </div>
    </div>

  </div>
</template>

<script>
export default {}
</script>

<style scoped>
#profile #photo {
  margin-bottom: 20px;
}

#profile p {
  margin-bottom: 0;
}

#photo,
.box .in {
  max-width: 100%;
  border-radius: 3px;
  -moz-border-radius: 3px;
  -webkit-border-radius: 3px;
  -webkit-box-shadow: 0px 1px 7px 0px rgba(00, 00, 00, 0.7);
  box-shadow: 0px 1px 7px 0px rgba(00, 00, 00, 0.7);
}
</style>
