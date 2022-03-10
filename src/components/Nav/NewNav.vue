<template>

<div>
    <nav class="navbar">
        <div class="container">
              <ul>
  <li><router-link class="active" to="/">Home</router-link></li>
  <li><router-link  to="/Profile">Profile</router-link></li>
  <li><router-link href="#contact">Contact</router-link></li>
  <li><router-link href="#about">About</router-link></li>
</ul>
        </div> <router-view></router-view>
    </nav>
        
</div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: rgb(217, 230, 223);
  position: fixed;
  top: 0;
  width: 100%;
}
li {
  float: left;
}

li a {
  display: block;
  color: rgb(40, 28, 209);
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: rgb(245, 240, 240);
}

.active {
  background-color: #04AA6D;
}
</style>
