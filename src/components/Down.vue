<template>
	<div class="wrapper">
		<div class="text3">
			<ul class="text2 ">
				<li>Home</li>
				<li> Policy details</li>
				<li>My Member</li>
				<li>E-Card</li>
				<li> Network Empires</li>
				<li>Change password</li>
				<li> Log Out</li>
			</ul>
		</div>


		<div class="text">
			<h1 class="good">A good smile and a long Sleep</h1>
			<h5 class="best">are the best cures in the Doctor's book</h5>
		</div>
		<div class="head">
			<div class="first" id="green">
				<img class="img"src="../assets/network.png" >
				<h4  class="imgText">Network</h4>
				
			</div>
			<div class="first ml-5" id="blue">
				<router-link :to="{name:'form'}">
				<img class="img" src="../assets/worker.png">
				<h4 class="imgText" style="padding-top:15px;">Employee</h4>
			</router-link>
			</h4>
				
			</div>
			<div class="first ml-5 " id="red">
				<img class="img" src="../assets/sun.png" style="padding-top:12px; width:80px;">
				<h4 class="imgText" style="padding-top:15px;">Marketing</h4>
				
			</div>
			
		</div>

		
	</div>
	
</template>



<style scoped>
	.wrapper{
		background-color: #3B3F4F;
		height: 100vh; 
	}

	.text{
		color: #ffff;
		padding-top: 100px;
	}
	.text3{
		width:50%;
		float: right;
		margin-right: 96px;
	}
	.text2{
		color: #ffff;
		display: right;

		display: flex;
	justify-content: space-between;
list-style: none;
font-family: sans-serif;
font-family: Lato;
font-style: normal;
font-weight: bold;
font-size: 14px;
line-height: 17px;
/* identical to box height */


color: #FFFFFF;

		
	 
	}

	.head{
		display: flex;
	}

	.first{
		height: 150px;
		width: 150px;
		background-color: red;


	}
	.head{
		margin-top: 120px;
		margin-left: 400px;
	}

	#green{
		background-color: #946A66;
	}

	#blue{
		background-color: #36395F;


	}
	#red{
		background-color: #336184;
	}
	.img{
		padding-top:16px;

	}
	.imgText{
		font-size:18px; 
		padding-top:25px;
		color: #ffff;
		font-weight: 30px;
		font-family: Roboto;
font-style: normal;
font-weight: normal;
font-size: 24px;
line-height: 28px;

color: #FFFFFF;

	}

	.good{
		font-family: Lato;
font-style: normal;
font-weight: 500;
font-size: 48px;
line-height: 58px;
letter-spacing: 0.05em;

color: #FFFFFF;

	}

.best{
	font-family: Lato;
font-style: normal;
font-weight: 500;
font-size: 24px;
line-height: 29px;
letter-spacing: 0.05em;

color: #FFFFFF;

}




</style>