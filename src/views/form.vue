<template>
	<div class="wrapper">
		<div class="head">
		<div class="text3">
			<ul class="text2 ">
				<li><router-link :to="{name:'home'}"> Dashboard </router-link></li>
				<li>Shiftplans</li>
				<li>Positions</li>
				<li>Employee</li>
			</ul>
			<h3 class="text4">Employee</h3>
		</div>
	</div>
	<div class="below">
		<div class="circle">
			<img class="img2" src="../assets/circle.png">
			
		</div>
		<br><br><br>
		<div class="below2">
		<div class="search">
			<img src="../assets/searching.png"><span>Search</span>
			
		</div>
		<div class="list3">
			<ul class="list2">
				<li class="filter">Filter<i class="fa fa-caret-down" style="margin-left:12px; color: rgba(47, 54, 68, 0.5);"></i></li>
				<li class="position"> Position:</li>
				<li class="all">All <i class="fa fa-caret-down" style="margin-left:12px;"></i></li>
				
			</ul>
			
		</div>
		<div class="table1">
			<table class="table">
			  <thead>
			    <tr class="tableRow">
			      <th  class="name" scope="col">NAME</th>
			      <th class="mail" scope="col">MAIL</th>
			      <th class="status" scope="col">STATUS</th>
			      <th scope="col"></th>
			    </tr>
			  </thead>
			  <tbody>
			    <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active" ><i class="fa fa-circle" id="smallCircle"></i> active </td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>


			    
			    </tr>



			    <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle"></i>   active</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>


			    
			    </tr>



			    <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle"></i>   active</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>
			    
			    </tr>


			     <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle"></i>   active</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>


			    
			    </tr>

			     <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle1"></i>   inactive</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>


			    
			    </tr>

			     <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle"></i>   active</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>


			    
			    </tr>

			     <tr class="tableRow">
			      <th class="alan"  scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle"></i>   active</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>
			    
			    </tr>
			     <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle2"></i> deleted</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>


			    
			    </tr>

			     <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle"></i>   active</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>

			    </tr>

			     <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle"></i>   active</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>


			    
			    </tr>


			    <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle1"></i>   inactive</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>


			    
			    </tr>



			    <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle"></i>   active</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>


			    
			    </tr>




			    <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle"></i>   active</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>


			    
			    </tr>







			    <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle"></i>   active</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>


			    
			    </tr>





			    <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle2"></i> deleted</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>


			    
			    </tr>





			    <tr class="tableRow">
			      <th class="alan" scope="row" style="font-weight:12px;">Alan Scott</th>
			      <td class="lantern">green@lantern.com</td>
			      <td class="active"><i class="fa fa-circle" id="smallCircle"></i>   active</td>
			 		<td class="myTable">
      				<ul class="myList">
	      				<li ><img style="width:20px;" src="../assets/edit.png"><li>
	      				<li ><img style="width:20px;" src="../assets/edit1.png"></li>
	      				<li ><img style="width:20px;" src="../assets/delete.png"></li>
	      				
	      			</ul>
      			</td>


			    
			    </tr>

			  </tbody>
			</table>
						
		</div>





		</div>
		
	</div>






	</div>







	<!-- <div class="header">
		<div class="nav">
			<div class="list">
		<ul class="top">
			<li>Dashboard</li>
			<li>Shiftplans</li>
			<li>Positions</li>
			<li>Employee</li>
		</ul>
		</div>
			
		</div>
		
	</div> -->
	

</template>

<style scoped>
	.head{
		background-color: #3B3F4F;
		height: 14vh; 
	}
	.below{
		height: 200vh;
	}

	.text{
		color: #ffff;
		padding-top: 100px;
	}
	.text3{
		width:30%;
		float: left;
		margin-left: 80px;
	}
	.text2{
		color: #ffff;
		display: right;

		display: flex;
	justify-content: space-between;
list-style: none;
font-size: 15px;
	font-family: Roboto;
font-style: normal;
font-weight: normal;
font-size: 20px;
line-height: 23px;

color: #F9F9FB;
opacity: 0.8;


	 
	}


	.text4 {
		color: #ffff;
		font-size: 20px;
		text-align: left;
		margin-left: 35px;
		font-family: Lato;
font-style: normal;
font-weight: normal;
font-size: 36px;
line-height: 43px;


color: rgba(255, 255, 255, 0.8);
	
	}

	.below{
		background-color: #F9F9FB; 
	}

	.circle{
		margin-left: 900px;
	}
	.img2{
		position: absolute;
		margin-top: -40px;
	}
	.search{
		text-align: left;
		margin-left: 120px;
		font-family: Lato;
font-style: normal;
font-weight: normal;
font-size: 18px;
line-height: 22px;
/* identical to box height */


color: #3B3F4F;

	}
	
	.list2{
	
		display: right;

		display: flex;
	justify-content: space-between;
list-style: none;
font-size: 15px;
margin-right: 90px;



	}
	.list3{
		width:30%;
		float:right;
		margin-top: 0px;

	}

	.table1{
	
		width: 85%;

		
		margin: auto;
		margin-top: 80px;
	}
	.myList{
		display: flex;
		justify-content: space-between;
		list-style: none;
	}
	.myTable{
		width:150px;

	}

	#smallCircle{
		color: blue;
		margin-right: 4px;
		font-size: 12px;
 
	}

	#smallCircle1{
		margin-right: 4px;
		font-size: 12px;
		color: #F5A625;
	}

	#smallCircle2{
		margin-right: 4px;
		font-size: 12px;
		color: #F9495E;
	}

	.filter{
		font-family: Lato;
font-style: normal;
font-weight: normal;
font-size: 18px;
line-height: 22px;
/* identical to box height */
color: #4c4c4c;
opacity: 0.9


/*color: rgba(47, 54, 68, 0.5);*/


	}
.position{
	font-family: Lato;
font-style: normal;
font-weight: normal;
font-size: 18px;
line-height: 22px;
/* identical to box height */
color: #4c4c4c;
opacity: 0.9;


/*color: rgba(70, 70, 84, 0.5);*/


}

.all{
	font-family: Lato;
font-style: normal;
font-weight: normal;
font-size: 18px;
line-height: 22px;
/* identical to box height */
color: #4c4c4c;
opacity: 0.9;


/*color: rgba(0, 0, 0, 0.5);
*/

}

.name{
	font-family: Lato;
font-style: normal;
font-weight: normal;
font-size: 18px;
line-height: 22px;
/* identical to box height */


color: #000000;



}

.mail{
	font-family: Lato;
font-style: normal;
font-weight: normal;
font-size: 18px;
line-height: 22px;
/* identical to box height */


color: #000000;
width: 330px;


margin-left:9.6em;


}

.status{
	font-family: Lato;
font-style: normal;
font-weight: normal;
font-size: 18px;
line-height: 22px;
/* identical to box height */


color: #000000;

width: 420px;


}

.alan{
	font-family: Lato;
font-style: normal;
font-weight: normal;
font-size: 21px;
line-height: 26px;
color: #000000;




/*color: rgba(0, 0, 0, 0.5);*/

}

.lantern{
	font-family: Lato;
font-style: normal;
font-weight: normal;
font-size: 21px;
line-height: 26px;
 color: #000000;
opacity: 0.6;



/*color: rgba(0, 0, 0, 0.5);

*/

}

.active{
	font-family: Lato;
font-style: normal;
font-weight: normal;
font-size: 21px;
line-height: 15px;

color: #000000;
opacity: 0.6;


/*color: rgba(0, 0, 0, 0.5);
*/
}

.tableRow{
	text-align: left;
}
	

</style>