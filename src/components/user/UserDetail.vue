<template>
<div>
    <h3>Some User Details</h3>
    <p>User loaded has ID: {{ $route.params.id}}</p>
    <!-- Primeiro metodo 
        <router-link 
    tag="button" 
    :to="'/user/' + $route.params.id + '/edit'"
    class="btn btn-primary">Edit User</router-link> -->

    <!-- Segundo método-->
    <router-link 
    tag="button" 
    :to="link"
    class="btn btn-primary">Edit User</router-link>

</div>
</template>

<script>
export default {
    data(){
        return{
            link: {name: 'editUser', params:{id: this.$route.params.id}, query:{ locale:'en', q:'100' },
            hash:'#data' }
        }
    },
    //Este comando serve para autenticar a entrada do usuário a esta página
    beforeRouteEnter(to,from,next){
        if(true){
            next();
        }else{
            next(false);
        }
    }
}

</script>
