
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title>replit</title>
  <link href="style.css" rel="stylesheet" type="text/css" />
</head>

<body>
  <input type="number" id="numeroInput">
  <button onclick="bottoneNumero()">Stampa numeri</button>
  <div id="output"></div>

  <script>
    function bottoneNumero() {
      const numeroInput = document.getElementById("numeroInput").value;
      stampaNumeri(numeroInput);
    }

    function stampaNumeri(numero) {
      let outputDiv = document.getElementById("output");
      outputDiv.innerHTML = "";
      for (let i = 1; i <= numero; i++) {
        outputDiv.innerHTML += i + "<br>";
      }
      outputDiv.innerHTML += "10% del numero: " + (numero * 0.1);
    }
  </script>
  <script src="script.js"></script>
  <script src="https://replit.com/public/js/replit-badge-v2.js" theme="dark" position="bottom-right"></script>
</body>

</html>
