<template>
			
		<div class="container">
			<div class="row">
			<div class="col-sm-6">
				<div class="form2 mt-4">
       			<form @submit.prevent="upDate" class="mt-2">
		        	
				    <!-- <div class="form-group col-md-6"> -->
  <div class="form-group row mt-4">
    <label for="inputEmail3" class="col-sm-2 col-form-label ml-3" style="color:#ffff; font-weight:bold;font-size:24px;">Name</label>
    <div class="col-sm-8">
      <input type="text" v-model="employee.employee_name" class="form-control" id="inputEmail3" placeholder="employee name">
    </div>
  </div>
  <div class="form-group row pt-3">
    <label for="inputPassword3" class="col-sm-2 col-form-label ml-3" style="color:#ffff; font-weight:bold; font-size:25px;">Age</label>
    <div class="col-sm-8">
      <input type="text" v-model="employee.employee_age" class="form-control" id="inputPassword3" placeholder="employee age">
    </div>
  </div>

  <div class="form-group row pt-3">
    <label for="inputPassword3" class="col-sm-2 col-form-label ml-3" style="color:#ffff; font-weight:bold;font-size:25px;">Salary</label>
    <div class="col-sm-8">
      <input type="text" v-model="employee.employee_salary" class="form-control"  placeholder="employee salary">
    </div>
  </div>

   
  
 




				      <!-- <label  style=" color:#ffff; font-size:20px;">name</label>
				      <input type="text" v-model="employee.employee_name"class="form-control"placeholder="employee name"  autofocus>
				    </div>
				    <div class="form-group col-md-6">
				      <label for="inputPassword4" style=" color:#ffff; font-size:20px;">Salary</label>
				      <input type="number" v-model="employee.employee_salary"class="form-control" id="inputPassword4" placeholder="employee salary">
				  </div>
			
				      <div class="form-group col-md-6">
				      <label for="inputPassword4" style=" color:#ffff; font-size:20px;">Age</label>
				      <input type="number" v-model=" employee.employee_age"class="form-control" id="inputPassword4" placeholder="employee Age" >
				  </div>

				      <div class="form-group col-md-6">
				      <label for="inputPassword4" style=" color:#ffff; font-size:20px;">image</label>
				      <input type="number" v-model="employee.employee_image"class="form-control" id="inputPassword4" placeholder="employee.image" >
				  </div> -->
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























<style>
	.form2{
		border: 2px solid #b2b3b3;
		height: 50vh;
		box-shadow: 5px 5px #b3b3b3;
		background-color: #1f2628
	}

	.me{
		margin-left:15px;
		padding-top: 20px;
	}
	


</style>



<script>
  export default{
    name:'home',
    data() {
      return{
        apiResponse:{},
        employee: null,
        error:{}

      }
    },

    components:{},
    mounted() {
      let id = this.$route.params.id
      this.$http.get('http://dummy.restapiexample.com/api/v1/employee/'+id)
      .then(response =>{
        console.log(response)
        this.employee = response.data
        console.log(this.employee)
      })
    },



    methods:{
    upDate:function(){
		this.$http.put('http://dummy.restapiexample.com/api/v1/update/'+this.employee.id,this.employee)
		.then(response=>{
			console.log(response)
			alert('employee list is successfully updated')
	
		})   	
    }


    }
    
    
  };

  
  


	




</script>