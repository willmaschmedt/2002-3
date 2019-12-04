# 2002-3
second day of mf software dvlmpt

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<link rel="shortcut icon" type="image/x-icon" href="https://static.codepen.io/assets/favicon/favicon-aec34940fbc1a6e787974dcd360f2c6b63348d4b1f4e06c77743096d55480f33.ico" />
<link rel="mask-icon" type="" href="https://static.codepen.io/assets/favicon/logo-pin-8f3771b1072e3c38bd662872f6b673a722f4b3ca2421637d5596661b4e2132cc.svg" color="#111" />
<title>CodePen - 2002-3</title>
<style>
  h1{
  color:rgb(255,100,100);
}
#mainList{
    font-size:250%;
}
.odd{
  background-color:rgba(225,225,225,.3)
}
.even{
  background-color:rgba(100,100,100,.3);
}
.aList{
  color:#FFFFA0;
  font-size:25px;
  background-image:url("https://www.healthyplace.com/sites/default/files/ShareTasksHaveMoreFun.jpg")
}
</style>
</head>
<body translate="no">
<h1 id="mainList">To do list</h1>
<ul class="aList" id="myList">
<li class="odd">Do math homework</li>
<li class="even">Eat dinner</li>
</ul>
<button id="add">Add</button>
<input id="item">
<script id="rendered-js">
      console.clear();
console.log("hello world");
const addBtn = document.getElementById("add");
addBtn.addEventListener("click", addItem);
function addItem(e) {
  const theItem = document.getElementById("item").value;
  console.log("add item", theItem);
  var node = document.createElement("li");
  var textnode = document.createTextNode(theItem);
  node.appendChild(textnode);
  document.getElementById("myList").appendChild(node);
}
    </script>
</body>
</html>
