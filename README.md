<!DOCTYPE html>
<html lang="ru">
<title>KALKULATORproMAX</title>
<meta charset="UTF-8">
<body class="back" >
  <style>
  .back {
    background-color: black;
    justify-content: center;
            align-items: center;
    width: 75vh; 
    margin-top:450px;
    margin-left:250px
  }
  </style>
</body>
<style>
.znak {
  border-color:green;
  border-width: 10px;
  background-color:black;
  color:white;
}
.inp {
  background-image: linear-gradient(black, black), linear-gradient(to right, rgb(235, 50, 235), rgb(82, 82, 209));
            background-origin: border-box;
            background-clip: content-box, border-box;
border: double 0.1em transparent;
  color:white;
}
.text {
  color:white;
  font-size:50px
}
.del {
  border-color:red;
  border-width:10px;
  background-color:black;
  color:white;
  font-size:100px
}
</style>
<p class="text" >V number 1(X) V_____________V numver 2(X1) V</p>
<input  class="inp" type="number" style="font-size:100px;width:150px;margin-left:100px" id="numOne" placeholder="X"  >
<input class="inp" type="number" style="font-size:100px;width:150px;margin-left:550px" id="numTwo" placeholder="X1" >
<p class="text" style="margin-left:225px">V sign (+-/*) & Response V</p><button class="znak" style="font-size:100px;width:150px;margin-left:225px" onclick="plus()" >+</button> <button class="znak" style="font-size:100px;width:150px" onclick="minus()" >-</button> <button class="znak" style="font-size:100px;width:150px" onclick="dil()" >/</button> <button class="znak" style="font-size:100px;width:150px" onclick="umn()" >*</button>
<p style="margin-left:450px" class="text" >V delete V</p>
<button onclick="duli()" class="del" style="margin-left:150px" >del all</button><button onclick="delX()" class="del">del X</button><button onclick="delXo()" class="del">del X1</button>
<script>
function plus() {
  numOne = parseFloat(document.getElementById("numOne").value);
  numTwo = parseFloat(document.getElementById("numTwo").value);
  otvet = numOne + numTwo;
  alert(`Response: ${otvet}`);
  if(otvet === 1488) {
    alert("PASHALKOOO")
  }
}
function minus() {
  numOne = parseFloat(document.getElementById("numOne").value);
  numTwo = parseFloat(document.getElementById("numTwo").value);
  otvet = numOne - numTwo;
  alert(`Response: ${otvet}`);
  if(otvet === 1488) {
    alert("PASHALKOOO")
  }
}
function umn() {
  numOne = parseFloat(document.getElementById("numOne").value);
  numTwo = parseFloat(document.getElementById("numTwo").value);
  otvet = numOne * numTwo;
  alert(`Response: ${otvet}`);
  if(otvet === 1488) {
    alert("PASHALKOOO")
  }
}
function dil() {
  a = parseFloat(document.getElementById("numOne").value);
  b = parseFloat(document.getElementById("numTwo").value);
  otvet = a / b;
  alert(`Response: ${otvet}`);
  if(otvet === 1488) {
    alert("PASHALKOOO")
  }
}
function duli() {
  x = document.getElementById("numOne");
  x.value = " ";
  y = document.getElementById("numTwo");
  y.value = " "
}
function delX() {
  x = document.getElementById("numOne");
  x.value = " ";
}
function delXo() {
  y = document.getElementById("numTwo");
  y.value = " ";
}

</script>
</html>
