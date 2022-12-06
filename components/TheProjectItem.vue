<template>
  <li>
  </li>
</template>

<script scoped>
export default {

}

</script>

<style scoped>
.animation-view {
  max-width: 100%;
  width: 100%;
  border-radius: 3px;
  -moz-border-radius: 3px;
  -webkit-border-radius: 3px;
  overflow: hidden;
  position: relative;
  text-align: center;
  background: #fff;
  margin-top: 5px;
}
.animation-view .mask,
.animation-view .content {
  width: 100%;
  height: 100%;
  position: absolute;
  overflow: hidden;
  top: 0;
  left: 0;
}
.animation-view img {
  display: block;
  position: relative;
}
.animation-view h2 {
  display: none;
  text-transform: uppercase;
  color: #fff;
  text-align: center;
  position: relative;
  font-size: 17px;
  padding: 10px;
  background: rgba(0, 0, 0, 0.8);
  margin: 20px 0 0 0;
}
.animation-view p {
  display: none;
  font-style: italic;
  font-size: 12px;
  position: relative;
  color: #fff;
  line-height: normal;
  padding: 5px 5px 5px;
  margin-bottom: unset;
  text-align: center;
}
.animation-view button.info,
.animation-view svg.info {
  display: none;
  line-height: 24px;
}

.animation-view button.info a,
.animation-view svg.info a {
  font-style: normal;
}

.animation img {
  transition: all 0.2s linear;
}
.animation .mask {
  opacity: 0;
  background-color: rgba(18, 18, 18, 0.7);
  transition: all 0.4s ease-in-out;
}
.animation h2 {
  transform: translateY(-100px);
  opacity: 0;
  transition: all 0.2s ease-in-out;
}
.animation p {
  transform: translateY(100px);
  opacity: 0;
  transition: all 0.2s linear;
}
.animation button.info,
.animation svg.info {
  opacity: 0;
  transition: all 0.2s ease-in-out;
}
.animation button.info:hover {
  background-color: #ff4343;
}

.animation svg.info:hover {
  opacity: 1;
  cursor: pointer;
}

.animation:hover img {
  transform: scale(1.1);
}
.animation:hover .mask {
  opacity: 1;
}
.animation:hover h2,
.animation:hover p,
.animation:hover button.info,
.animation:hover svg.info {
  opacity: 0.8;
  transform: translateY(0px);
}

.animation:hover svg {
  padding: 5px;
}

.animation:hover svg.info:hover {
  opacity: 1;
}
.animation:hover h2 {
  display: block;
}
.animation:hover p {
  transition-delay: 0.1s;
  display: block;
}
.animation:hover button.info,
.animation:hover svg.info {
  display: inline-block;
}
@media only screen and (max-width: 600px) {
  .animation-view p {
    line-height: normal;
    margin-bottom: unset;
  }
}
</style>
