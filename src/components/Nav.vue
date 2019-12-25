<template>
	<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <a class="navbar-brand" href="#"><strong>Employee List</strong></a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
    <div class="navbar-nav">
      <button <router-link :to="{name:'home'}" class="btn btn-primary ml-5">Homepage </router-link><span class="sr-only">(current)</span></button>
    </div>
  </div>

  <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
    <div class="navbar-nav">
      <button <router-link :to="{name:'add'}" class="btn btn-danger ml-5">Add New </router-link></button>
    </div>
  </div>
</nav>
</template>
<!-- <td></td> <router-link :to="{name: 'about'}" class="nav-link">About</router-link> --> 
<style scoped>
	
	nav{
		
		border: 1px solid #b2b2b2;
		box-shadow: 5px 5px #b3b3;
		background-color: #b3b3
	}



	
</style>