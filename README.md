# jquery树形结构动画jqtreeanimate
效果如下：
![](images/img.gif)

all code:
```
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>树形动画</title>
	<style>
		ul.list{display: none;}
	</style>
</head>
<body>
	<div>
		<ul class="title">
			<li>水果
				<ul class="list">
					<li>苹果</li>
					<li>苹果</li>
					<li>苹果</li>
				</ul>
			</li>
			<li>蔬菜
				<ul class="list">
					<li>白菜</li>
					<li>白菜</li>
					<li>白菜</li>
				</ul>
			</li>
			<li>干果
				<ul class="list">
					<li>核桃</li>
					<li>核桃</li>
					<li>核桃</li>
				</ul>
			</li>
		</ul>
	</div>
</body>
</html>
<script type="text/javascript" src="js/jquery-2.1.4.js"></script>
<script>
	$(function(){
		$("ul.title li").click(
				function(){
					var $css = $(this).children('ul').css('display');
					if($css=="none"){
						$(this).children('ul').css('display','block')
					}else{
						$(this).children('ul').css('display','none')
					}
				})
	})
</script>
```

