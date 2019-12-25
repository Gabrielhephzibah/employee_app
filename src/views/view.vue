<template>
<div class="container">
    <div class="wrapper">
      <div class="top">
        <table class="table table-striped table-dark" id="first">
  <thead>
    <tr>
      <th scope="col">id</th>
      <th scope="col">Name</th>
      <th scope="col">Salary</th>
      <th scope="col">Age</th>
      <th scope="col">image</th>
    </tr>
  </thead>
  <tbody>
    <tr v-if="employee">
      <th scope="row">{{employee.id}}</th>
      <td>{{ employee.employee_name}}</td>
      <td><button>{{employee.employee_salary}}</button></td>
      <td><button>{{employee.employee_age}}</button></td>
      <td><button>{{employee.profile_image }}</button></td>
    </tr>
    
  </tbody>
</table> 








      </div>
    </div>
  </div>
  </template>










  <script>
  export default{
    name:'home',
    props: ['id'],
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
    }
  };

  
  
  </script>



  <style>
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
