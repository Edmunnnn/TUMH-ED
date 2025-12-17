# TUMH-ED
Sainuu, busduudd medegdku geed ingej bnshd bvvr , H
<!DOCTYPE html>
<html lang="mn">
<head>
  <meta charset="UTF-8">
  <title>Mongolian Cipher Decryptor</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">

  <style>
    body {
      font-family: system-ui, -apple-system, BlinkMacSystemFont, sans-serif;
      padding: 20px;
      max-width: 800px;
      margin: auto;
      background: #f7f7f7;
    }

    textarea {
      width: 100%;
      height: 140px;
      font-size: 16px;
      padding: 10px;
      margin-top: 10px;
      box-sizing: border-box;
    }

    button {
      margin: 15px 0;
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
    }
  </style>
</head>
<body>

<h2>Mongolian Cipher Decryptor</h2>

<textarea id="input">
Цгупфхдоуялг дпзлгду. Щпшшззр шл, пууджгг плпл юйц, рпегррй йхпм плпл.
</textarea>

<button onclick="decrypt()">Decrypt</button>

<textarea id="output" readonly></textarea>

<script>
const mapping = {
  "Ц":"Х","г":"а","у":"р","п":"а","ф":"м","х":"с","д":"л","о":"г",
  "я":"й","л":"ү","з":"ө","р":"ь","ш":"ч","Щ":"Ө","П":"М","ю":"з",
  "й":"и","ц":"н","е":"ж","м":"г",
  "Г":"А","Д":"Л","О":"Г","Л":"Ү"
};

function decrypt() {
  const input = document.getElementById("input").value;
  let result = "";

  for (const char of input) {
    result += mapping[char] ?? char;
  }

  document.getElementById("output").value = result;
}
</script>

</body>
</html>
