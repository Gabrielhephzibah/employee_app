<template>
	<div class="container">
		<div class="row">
			<div class="col-sm-6">
				<div class="add mt-3">
				<form @submit.prevent="add" >
		        	
				    <!-- <div class="form-group col-md-6"> -->
  <div class="form-group row mt-4">
    <label class="col-sm-2 col-form-label ml-3" style="color:#ffff; font-weight:bold;font-size:24px;">Name</label>
    <div class="col-sm-8">
      <input type="text" v-model="employee.employee_name" class="form-control"placeholder="employee name">
    </div>
  </div>
  <div class="form-group row pt-3">
    <label for="inputPassword3" class="col-sm-2 col-form-label ml-3" style="color:#ffff; font-weight:bold; font-size:25px;">Age</label>
    <div class="col-sm-8">
      <input type="text" v-model="employee.employee_age"  class="form-control" id="inputPassword3" placeholder="employee age">
    </div>
  </div>

  <div class="form-group row pt-3">
    <label for="inputPassword3" class="col-sm-2 col-form-label ml-3" style="color:#ffff; font-weight:bold;font-size:25px;">Salary</label>
    <div class="col-sm-8">
      <input type="text" v-model="employee.employee_salary"  class="form-control"  placeholder="employee salary">
    </div>
  </div>

				   <div class="form-row justify-content-center mt-3">
				  	<div class=" me form-group">
		  				<button  type="submit"class="btn btn-primary">Save</button>
		  			</div>
		  		</div>
		  	
		  
		</form>
					
				</div>

				
			</div>
			
		</div>
		
	</div>
</template>

<script>
  export default{
    name:'home',
    data() {
      return{
        apiResponse:{},
        employee: {},
        error:{}

      }
    },

    components:{},
    mounted() {
      this.$http.post('http://dummy.restapiexample.com/api/v1/create',this.employee)
     .then(response =>{
        console.log(response)
        this.employee = response.data
        console.log(this.employee)
      })
    },
    methods:{
      add:function(){
        this.$http.post('http://dummy.restapiexample.com/api/v1/create',this.employee)
      .then(response=>{
      console.log(response)
      alert('employee list is successfully updated')

    })
  
      }
    }

  };

  




</script>









<style>
.add{
		border: 2px solid #b2b3b3;
		height: 50vh;
		box-shadow: 5px 5px #b3b3b3;
		background-color: #1f2628
	}

	
</style>