<template>
  <div class="honors panel box">
    <div id="works" class="in">
      <h2>Works</h2>

      <div>
        <p>
          <i
            >Вот список проектов над которыми я работал(Скоро будет наполнен)
            <a href="#">GitHub</a> Открытые проекты</i
          >
        </p>

        <ul>
          <TheProjectItem
          />
          <TheProjectItem
          />

<!--          <TheProjectItem-->
<!--            project-cover-image="AS_Earning.png"-->
<!--            project-caption="Developed AS Earnings for a client using Laravel and MySQL. This is an online earning platform based on watching youtube videos. This website is currently functional only in Pakistan."-->
<!--            project-title="AS Earnings"-->
<!--            project-url="https://asearnings.com"-->
<!--          />-->
        </ul>
      </div>
    </div>
  </div>
</template>
<script>
import TheProjectItem from './TheProjectItem'
export default {
  components: {
    TheProjectItem
  }
}
</script>
