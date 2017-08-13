# This is a level 1 heading


```
<h1>Hello World</h1>

<p>The rain in Spain<br>
Falls mainly on the plain.
</p>

```
This is some javascript code `alert("Hello there")` texting testing. And some `<b>HTML code</b>` test. 
```
	<script>
		$(document).ready(function () {
			$("p.ans").click(function () {
				//Get the id of the div
				var qnum = "#" + $(this).parent().attr("id");
				//Clear previous freeback:
				$(qnum + " p.ans").removeClass("right wrong");
				$(qnum + " p span").css("display", "none");
				//Apply right or wrong class to p and span.
				var applyclass = "wrong"
				var spancolor = "red"
				if ($(this).hasClass("correct")) {
					applyclass = "right";
					spancolor = "green"
				}
				$(this).addClass(applyclass);
				$(this).children(":first").css("display", "block").css("color", spancolor);
			})
		});
	</script>
    ```