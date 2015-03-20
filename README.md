# project02A-Diksha
<html>
<head>
<title>
Determination of Productivity Rating Index
</title>
<style type="text/css">

#header {
      background-color:Crimson;
      width:1345px;
      height:255px;
	  font-size:175%;
	  font-family:Calibri(body);
	  font-color:White;
}
#container {
      background-color:WhiteSmoke;
	  width:1345px;
	  height:355px;
	  font-size:150%;
	  }
#footer {
      background-color:whitesmoke;
	  width:1335px;
	  font-size:175%;
	  }
</style>
<script type="text/javascript">
function myfunction(){
var x = parseInt(document.getElementById("a").value);
var y = parseInt(document.getElementById("b").value);
var z = document.getElementById("c");
z.value=(x/y)*100;
suitability();
}
</script>
</head>
<body>
<div id="header">
</br></br>
<h1 align="center"> Calculation Of Productivity Rating Index(PRI)</h1>
</div>
<div id="container">
<form name = "01" align="right"></br>
Expected or Actual yield of crop:<input type="text" id="a" /></br></br>
Standard yield of crop:<input type="text" id="b" /></br>
<input type="button" onclick="javascript:myfunction()" value="Calculate PRI" /></br></br>
Productivity Rating Index(PRI): <input type="text" id="c" /></br>
<div>
</form>
<div id="footer">
<p id="demo" align="center"></p>
<script type="text/javascript">
function suitability(){
var z= parseInt(document.getElementById("c").value);
var myclass;
if (z<20){
myclass=" Suitability Class:N";
}
else if (z<40){
myclass="Suitability Class:S3";
}
else if (z<80){
myclass="Suitability Class:S2";
}
else {
myclass="Suitability Class:S1";
}
document.getElementById("demo").innerHTML=myclass;
}
</script>
</div>
</body>
</html>
