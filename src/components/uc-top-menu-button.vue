<template>
    <div class="uc-top-menu-button">
        <router-link :to="this.href" class="link">
            {{this.name}}        
        </router-link>
    </div>
</template>

<script>
export default {
    name: 'uc-top-menu-button',
    props: ['name', 'href'],
    methods: {
        get_props() {
            console.log(this.name)
        }
    }
}


</script>

<style lang="scss">
    .uc-top-menu-button {
        height: 100px;
        background-color: #181818;
        .link {
            padding: 35px;
            text-align: center;
            text-decoration: none;
            line-height: 100px;
            color: #ffffff;
        }
        padding: auto 35px;
        &:hover {
            animation: button-hover .5s;
            background-color: #515151;
        }
    }

    @keyframes button-hover {
        from {background-color: #181818}
        to {background-color: #515151}
    }
</style>