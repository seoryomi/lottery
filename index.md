<html>
<script>

function aaa() {
	fir = new Array(999999);
	sec = new Array(1);
	for (i = 0; i < 999999; i++) fir[i] = i;
	for (i = 0; i < 1; i++) {
		ran = parseInt(Math.random()*fir.length);
		sec[i] = fir[ran];

		for (h = fir.length; h; h -= 1) {
			j = Math.floor(Math.random() * h);
			x = fir[h - 1];
			fir[h - 1] = fir[j];
			fir[j] = x;
		}
	}
	for (i = 0; i < 6; i++) {
		for (j = 0; j <= i; j++) {
			if(sec[i] <= sec[j]) {
				k = sec[i];
				sec[i] = sec[j];
				sec[j] = k;
			}
		}
	}
	document.getElementById('ddd').innerHTML = sec;
}
</script>
<h1> ٩(๑• ₃ -๑)۶♥ 아수라 발발타... 부자가 되고 싶니?</h1>
<h2> 뚝딱 나온다! 연금복권 번호! </h2>

https://user-images.githubusercontent.com/69951427/116185776-3bae2e00-a75d-11eb-8b14-03dbc22a5358.PNG

<h2> 이거이 니 정주영이고! 이병철이야! </h2>
<input id="button1" type="button" onclick="aaa()" value="너, 패 한번 쥐어보라" style="width:300px;height:50px;font-size:25px;">
<br/><br/>
<div id="ddd" style="font-size:30px;border:1px solid;width:300px;height:50px;text-align:center;padding:10px;"></div>
</html>
