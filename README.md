<!DOCTYPE HTML>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width,
  initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Fetch API Sandbox</title>
</head>
<body>
  <button id="getText"> Get Text </button>

  <script>
    document.getElementById('getText').addEventListener('click', getText);
    function getText(){
      fetch('sample.txt')
      .then(function(res){
        return res.text();
      })
      .then(function(data){
        console.log(data);
      })
    }

  </script>
</body>
</html>
