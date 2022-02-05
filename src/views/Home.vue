<template>
  <div class="home">
    <div class="card">
      <div class="container">
        <div id="qoute-of-day-title">
        <h2><b>Qoute of the Day</b></h2>     
        <div id="qoute-creator">
              <h6>By {{author}}</h6> 
        </div>
    
        </div>
        <p>
          {{quoteOfDay}}
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
  },
  created() {
    this.fetchQuoteOfDay()
  },
     data: () => ({
      quoteOfDay: '',
      author:'',
    }),
  methods: {
    fetchQuoteOfDay() {
      const uri = 'http://localhost:4000/quoteOfDay';
      this.$http.get(uri)
      .then((result) => {
        console.log(result)
        this.quoteOfDay = result.data[0].text
        this.author = result.data[0].author
      })
    }
  }
}
</script>
<style  lang="scss" scoped>
.container {
  padding: 6rem 5rem;
}
.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  margin: auto;
  margin-top: 3rem;
  width: 70%;
}
.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
  cursor: pointer;
}
#qoute-of-day-title {
   margin-bottom: 10px;
}
#qoute-creator {
  margin-bottom: 20px;
  margin-top: 10px;
}

</style>
