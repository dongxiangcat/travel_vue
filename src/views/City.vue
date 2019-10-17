<template>
  <div>
    <city-header></city-header>
    <city-list :cities="cities" :hotCities="hotCities"></city-list>
  </div>
</template>

<script>
import CityHeader from '@/components/city/CityHeader'
import CityList from '@/components/city/CityList'
import axios from 'axios'
export default {
  name: 'City',
  components: {
    CityHeader,
    CityList
  },
  data () {
    return {
      cities: {},
      hotCities: []
    }
  },
  mounted () {
    axios.get('/data/city.json').then(this.handleGetCityInfoSucc)
  },
  methods: {
    handleGetCityInfoSucc (res) {
      res = res.data
      if (res.ret && res.data) {
        const data = res.data
        this.cities = data.cities
        this.hotCities = data.hotCities
      }
    }
  }
}
</script>

<style scoped>

</style>
