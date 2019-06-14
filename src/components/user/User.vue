<template>
<div>
    <h1>The User Page</h1>
    <hr>
   <!-- Este comando vincula o número ID, que está na minha URL ao dado "id" em "User.vue" e é apresentado na minha pagína 
        <p>Load ID: {{ id }}</p> -->
    <button class="btn btn-primary" @click="goToHome">Go to Home</button>
    <hr>
    <router-view></router-view>
</div>
</template>
<script>
export default {

   /* Este comando vincula o número ID, que está na minha URL ao dado "id" em "User.vue" e é apresentado na minha pagína  
   data(){
        return{
            id: this.$route.params.id,
        }
    },
    watch: {
        '$route' (to, from) {
            this.id = to.params.id;
        }
    }, */
    methods: {
        goToHome(){
            this.$router.push({name:'home'});
        }
    }
}
</script>
