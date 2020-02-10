<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xmlns:og="http://ogp.me/ns#" xmlns:fb="http://www.facebook.com/2008/fbml">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
    <title>Trang chuyển hướng</title>

</head>
<body>
	<script type="text/javascript">
	var count = 7;
	var redirect = "https://vithuong7.blogspot.com";
	function countDown(){
		var timer = document.getElementById("timer");
		if(count > 0){
			count--;
			timer.innerHTML = "Trang web bạn muốn đến sẽ tự động chuyển tới trong <b>"+count+"</b> giây.";
			setTimeout("countDown()", 1000);
		}else{
			window.location.href = redirect;
		}
	}
	</script>
	<style>
	.wrap {
		width: 600px;
		margin: 250px auto;
		padding: 20px;
		border-radius: 10px;
		border: 1px solid #ddd;
		font-size: 20px;
		line-height: 1.3em;
		text-align: center;
	}
	</style>
    <div class="wrap">
        <p id="timer"><script type="text/javascript">countDown();</script></p>
	</div>
</body>
</html>
