<template>
  <div>
    <oreder-header></oreder-header>
    cart
    <router-view></router-view>
    <nav-footer></nav-footer>
  </div>
</template>
<script>
import OrederHeader from '../components/OrderHeader'
import NavFooter from '../components/NavFooter'
export default {
  name: 'cart',
  components: {
    OrederHeader,
    NavFooter
  }
}
</script>
