<template>
  <div id="app">
    <main>
      <div>
        <input 
          type="text" 
          placeholder="Search..."
        />
      </div>
      <div>{{ weather.name }}, {{ weather.sys.country }}</div>
      <div> dateBuilder() }}</div>
      <div>{{ Math.round(weather.main.temp) }}°c</div>
      <div>{{ weather.weather[0].main }}</div>
    </main>
  </div>
</template>

<script>
export default {
  name: 'Weather',
  setup(){
    const api_key= '19bedb32e1849ab76d6185b2c3123fd4',
      url_base= 'https://api.openweathermap.org/data/2.5/'


    return {api_key,url_base}
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

</style>
