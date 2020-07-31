<template>
<h5>Example Component</h5>
</template>

<script>
    export default {
        mounted() {
            Echo.channel('test')
            .listen('Test',(e)=>{
                console.log('echo tings-e=',e)
            })
            console.log('Component mounted.')
        }
    }
</script>
