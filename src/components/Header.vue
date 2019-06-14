<template>
    <ul class="nav nav-pills">
     <router-link  to="/" tag="li" active-class="active" exact><a> Home</a> </router-link>
      <router-link to="/user" tag="li" active-class="active"><a> User </a></router-link>

<!--   Este comando vincula o número ID, que está na minha URL ao dado "id" em "User.vue" e é apresentado na minha pagína 
       <router-link to="/user/2" tag="li" active-class="active"><a> User 2</a></router-link> -->
    </ul>
</template>
