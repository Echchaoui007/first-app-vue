<script>

export default {
    name :'Home',
    data(){
        return {
            name: 'ZEDKA',
            color: '',
            youname:''
        }
    },
    methods:{
        alerting(){
            this.color = 'heading'
        },
        changeName(){
            this.name ='eCHaoui'
        }
    }
}
</script>

<template>
<h1 :class="color" @mouseover="alerting" > {{ name }}</h1>

</template>

<style>
.heading {
    @apply text-green-500;
}
</style>