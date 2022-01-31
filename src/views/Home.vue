<template>
  <div class="home">
    <div class="card">
      <div class="container">
        <div id="qoute-of-day-title">
        <h2><b>Qoute of the Day</b></h2>     
        <div id="qoute-creator">
              <h6>By Etricia Seko</h6> 
        </div>
    
        </div>
        <p>
     Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

        </p>
    
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
  }
}
</script>
<style scoped>
.container {
  padding: 6rem 5rem;
  /* margin: 150px 159px; */
}
.home {
    display: grid;  
    grid-template-columns: 1fr 1fr 1fr;  
    grid-template-rows: 50px 50px;  
}
.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  grid-column-start: 2;
  margin: auto;
}
.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}
#qoute-of-day-title {
   margin-bottom: 10px;
}
#qoute-creator {
  margin-bottom: 20px;
  margin-top: 10px;
}

</style>
