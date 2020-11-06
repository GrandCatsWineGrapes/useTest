<template>
    <div class="uc-top-menu">
        <div class="logo-container">
            <h2 class="logo">useTest()</h2>
        </div>
        <div class="menu-items">
            <uc-top-menu-button v-for="(item, index) in menuItems" :key="index" 
                    v-bind:name="item.name" v-bind:href="item.href"/>
        </div>
    </div>
</template>

<script>
import topButton from './uc-top-menu-button'

export default {
    name: 'uc-top-menu',
    components: {
        'uc-top-menu-button': topButton
    },
    data() {
        return {
            menuItems: [
                {
                    name: 'Home',
                    href: '/'
                }
            ]
        }
    }
}
</script>

<style lang="scss">
    .uc-top-menu {
        display: flex;
        align-items: center;
        height: 100px;
        background-color: #181818;
        color: #ffffff;

        .logo-container {
            padding: 25px 22px;
        }

        h2.logo {
            font-size: 36px;
            font-weight: 400;
            // padding: 0;
            margin: 0;
        }
    }
</style>