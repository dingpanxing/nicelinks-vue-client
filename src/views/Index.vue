<template>
  <div class="wrapper">
    <search class="mobile-search" v-if="$isMobileScreen()" />
    <HomeLotus class="$isMobileScreen() ? mobile-search-serving : ''"></HomeLotus>
    <NiceFantasy></NiceFantasy>
    <Introduction></Introduction>
    <LinkCountup></LinkCountup>
  </div>
</template>

<script>
import HomeLotus from 'components/homepage/HomeLotus'
import NiceFantasy from 'components/homepage/NiceFantasy'
import Introduction from 'components/homepage/Introduction'
import LinkCountup from 'components/homepage/LinkCountup'
import pageMixin from 'mixins/pageMixin.js'
import metaMixin from 'mixins/metaMixin.js'

export default {
  name: 'Index',

  mixins: [pageMixin, metaMixin],

  data () {
    return {
      title: ''
    }
  },

  components: {
    HomeLotus,
    NiceFantasy,
    Introduction,
    LinkCountup
  },

  beforeCreate () {
  },

  created () {
  },

  mounted () {
  },

  methods: {
  }
}
</script>
