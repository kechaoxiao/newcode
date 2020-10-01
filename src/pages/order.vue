<template>
  <div>
    <oreder-header></oreder-header>
    order
    <router-view></router-view>
    <nav-footer></nav-footer>
  </div>
</template>
<script>
import OrederHeader from '../components/OrderHeader'
import NavFooter from '../components/NavFooter'
export default {
  name: 'oreder',
  components: {
    OrederHeader,
    NavFooter
  }
}
</script>
