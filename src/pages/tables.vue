<template>
    <div>
        <f7-page :cached="false" class="current-padding">
            <!--<navbar/>    -->

            <waiters-tables/>
        </f7-page>
    </div>
</template>
<style scoped lang="less">
    .current-padding {
        padding-top: 70px;
    }
</style>
<script>
    import navbar from '../components/navbar-main.vue';
    import waitersTables from '../components/table-in-work';

    export default {
        data() {
            return {
                name: 'this component'
            }
        },
        mounted() {
        },
        components: {
            navbar,
            'waiters-tables': waitersTables
        },
        methods: {
            reload() {
                console.log('reload');
            }
        }
    }


</script>