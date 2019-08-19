<h1>TuomasKoo Watch Site</h1>
<p><img src="https://tuomaskoo.github.io/UI/Button_L.png" alt="Button_L" /> <img src="https://tuomaskoo.github.io/Files/Seiko 7s26-0020_1.jpg" alt="test" width="436" height="585" /><img src="https://tuomaskoo.github.io/UI/Button_R.png" alt="Button_R" width="78" height="78" /></p>
<p>https://tuomaskoo.github.io/Files/Seiko_7S26-0020.txt</p>

<html>
  <head>
    <title>reading file<https://tuomaskoo.github.io/Files/Seiko_7S26-0020.txt>
   </head>
<body>


<input type="file" id="myFile">
<hr>
<textarea style="width:500px;height: 400px" id="output"></textarea>

<script>
var input = document.getElementById("myFile");
var output = document.getElementById("output");

input.addEventListener("change", function () {
  if (this.files && this.files[0]) {
    var myFile = this.files[0];
    var reader = new FileReader();

    reader.addEventListener('load', function (e) {
      output.textContent = e.target.result;
    });

    reader.readAsBinaryString(myFile);
  }
});
</script>
  </body>
</html>
