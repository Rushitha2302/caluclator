# caluclator
<!DOCTYPE html>
<html>
<head>
	<title>Calculator</title>

	<style>
		* { margin: 0; padding: 0; box-sizing: border-box; }
        
        body{
        	background-image: url('image/image.jpg');
        	background-size: 110% 110%;
        }

        form{
        	width: 400px;
        	height: 520px;box-shadow: 0 0 10px 1px grey;
        }

		.centercalcy{
			height: 100vh;
			display: flex;
			justify-content: center;
			align-items: center;
		}

		#app{
			width: inherit;
			font-size: 
			background-colour:#000000;
			border: none;
			color: blue;

		}

		#display{
			width: inherit;height: 140px;
			background-color: grey;
			text-align: right;
			color: white;
			font-size: 30px;
			outline: none;
		}

		.layer{
			width: inherit;
			display: flex;
			justify-content: center;
			height: 90px;

		}

		.layer1{
			width: inherit;
			display: flex;
			justify-content: center;
			height: 90px;

		}
		


		input{ flex: 1; }


		input:hover {
			background-color: blue;

		}
        .mainnumber{
        	background-color: red;
        }


	</style>
</head>
<body>
	<div class="centercalcy">
		<form name="calcy">
			
			<input type="text" name="answers" id="display">

			<div class="layer1">
				<input type="button"  name=""   value="C" id="clear" onclick="calcy.answers.value = '' ">
				<input type="button"  name=""   value="=" id="clear" onclick="calcy.answers.value = eval(calcy.answers.value) ">
			</div>
			<div class="layer">
				<input type="button"  name="" class="mainnumber"  value="7" onclick="calcy.answers.value += '7' ">

				<input type="button"  name="" class="mainnumber"  value="8" onclick="calcy.answers.value += '8' ">
				
				<input type="button"  name="" class="mainnumber"  value="9" onclick="calcy.answers.value += '9' ">
				
				<input type="button" name="" class="operator" value="" onclick="calcy.answers.value += '' ">
			</div>

			<div class="layer">
				<input type="button"  name="" class="mainnumber"  value="4" onclick="calcy.answers.value += '4' ">

				<input type="button"  name="" class="mainnumber"  value="5" onclick="calcy.answers.value += '5' ">
				
				<input type="button"  name="" class="mainnumber"  value="6" onclick="calcy.answers.value += '6' ">
				
				<input type="button" name="" class="operator" value="-" onclick="calcy.answers.value += '-' ">
			</div>

			<div class="layer">
				<input type="button"  name="" class="mainnumber"  value="1" onclick="calcy.answers.value += '1' ">

				<input type="button"  name="" class="mainnumber"  value="2" onclick="calcy.answers.value += '2' ">
				
				<input type="button"  name="" class="mainnumber"  value="3" onclick="calcy.answers.value += '3' ">
				
				<input type="button" name="" class="operator" value="+" onclick="calcy.answers.value += '+' ">
			</div>

			<div class="layer">
				<input type="button"  name="" class="mainnumber"  value="." onclick="calcy.answers.value += '.' ">

				<input type="button"  name="" class="mainnumber"  value="0" onclick="calcy.answers.value += '0' ">
				
				<input type="button"  name="" class="mainnumber"  value="%" onclick="calcy.answers.value += '%' ">
				
				<input type="button" name="" class="operator" value="/" onclick="calcy.answers.value += '/' ">
			</div>


		</form>
	</div>

</body>
</html>
