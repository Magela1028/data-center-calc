# data-center-calc
数据中心空调节能计算
html
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>计算数据中心年度节电费用</title>
</head>
<body>
<h1>计算数据中心年度节电费用</h1> 
<form>
<p>空调制冷量(千瓦): <input type="text" id="cooling_capacity"></p> 
<p>空调性能系数(COP): <input type="text" id="cop"></p>
<p>空调数量: <input type="text" id="ac_num"></p>
<p>电价(元/千瓦时): <input type="text" id="elec_price"></p>
<p>空调节能率: <input type="text" id="ac_eff"></p>
<p><button type="button" onclick="calculate()">计算</button></p>
</form>
<div id="output"></div>

<script>
function calculate() {
  // 获取用户输入
  var cooling_capacity = document.querySelector('#cooling_capacity').value; 
  var cop = document.querySelector('#cop').value;
  var ac_num = document.querySelector('#ac_num').value;
  var elec_price = document.querySelector('#elec_price').value;
  var ac_eff = document.querySelector('#ac_eff').value;
  
  // 计算年耗电量、年度电费、节省电量和节省电费
  // ......
  
  // 将结果输出到HTML页面
  document.querySelector('#output').innerText = '';
  document.querySelector('#output').innerText += '数据中心一年总耗电量:' + elec_year + '千瓦时\n';
  // ......
}
</script>
</body>
</html>
