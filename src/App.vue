<template>
    <div class="wrapper">
        <uc-top-menu />
    </div>
</template> 

<script>
import 'normalize.css'
import './styles/main.scss'

import topMenu from './components/uc-top-menu'

export default {
    name: 'App',
    components: {
        'uc-top-menu': topMenu
    }
}
</script>

<style lang="scss" scoped>


</style>
