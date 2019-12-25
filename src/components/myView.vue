<div class="container">
    <div class="wrapper">
      <div class="top">
        <table class="table table-striped table-dark" id="first">
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
</table> 








      </div>
    </div>
  </div>







<!--

<table class="table table-striped table-dark" id="first">
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