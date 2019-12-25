<template>
	<div class="container">
		<div class="wrapper mt-4">
			<div class="top">
	
		<table  id="first" class="table table-striped table-dark">
        <thead>
            <tr>
                <th>#</th>
      			<th style="text-align:centre;">Name</th>
      			<th> Actions</th>
      			<th ></th>
            </tr>
        </thead>
        <tbody>
                <tr v-for="(employee,hephzibah) in employees">
      			<th scope="row">{{ hephzibah+1}}</th>
      			<td>{{ employee.employee_name}}</td>
      			<td colspan="3">
      				<ul class="list-inline">
	      				<li class="list-inline-item"><router-link :to="{name:'view', params:{id: employee.id}
	      				}" class="btn btn-primary">view</router-link></li>
	      				<li class="list-inline-item"><router-link :to="{name:'edit',params:{id: employee.id}}" class="btn btn-secondary">edit</router-link></li>
	      				<li @click.prevent="Del(employee)" class="list-inline-item"><button class="btn btn-info">delete</button></li>
	      				
	      			</ul>
      			</td>
      			<!-- <td></td>
      			<td></td> <router-link :to="{name: 'about'}" class="nav-link">About</router-link> -->
    	</tr>
        </tbody>
    </table>




			<!-- <table class="table table-striped table-dark" id="first">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col" style="text-align:centre;">Name</th>
      <th scope="col"></th>
      <th scope="col"></th>
    </tr>
  </thead>
  <tbody>
    <tr v-for="(employee,hephzibah) in employees">
      <th scope="row">{{ hephzibah+1}}</th>
      <td>{{ employee.employee_name}}</td>
      <td><button>view</button></td>
      <td><button>edit</button></td>
      <td><button>delete</button></td>
    </tr>
    
  </tbody>
</table> -->
			
		</div>
	</div>
		
	</div>


	
</template>


// 	export default{
//     name:'home',
//     data() {
//       return{
//         apiResponse:{},
//         employee: {},
//         error:{}

//       }
//     },

//     components:{},
//     mounted() {
//       let id = this.$route.params.id
//       this.$http.get('http://dummy.restapiexample.com/api/v1/delete/2/'+id)
//       .then(response =>{
//         console.log(response)
//         this.employee = response.data
//         console.log(this.employee)
//       })

//     },
    

// };






<style>
body{
	background-image: url(https://images.pexels.com/photos/1092364/pexels-photo-1092364.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500); 
		
		}
.wrapper{
	height:auto;
	width:auto;
	border: 2px solid #000000;
}
.top {
	height:inherit;
	width:inherit;
	border: 2px solid #000000;

}
	

</style>

<script>
	export default{
		name:'home',
		data() {
			return{
				apiResponse:{},
				employees: [],
				error:{}
				


			}
		},

		components:{},
		mounted() {
			this.$http.get('http://dummy.restapiexample.com/api/v1/employees')
			.then(response =>{
				// console.log(response)
				this.employees = response.data
				console.log(this.employees)
			})
			    $('table#first').DataTable();
		},
		methods:{
      	Del: function(employee){
	      	if (confirm("do you want to delete?")) {
				this.$http.delete('http://dummy.restapiexample.com/api/v1/delete/'+employee.id)
				.then(response=>{
					console.log(response)
					alert("record sucessfully deleted")
				})
	      	}
      	}
    }
};
</script>

<!-- this.employees = response.body.employees,error=> this.error =error.body  -->