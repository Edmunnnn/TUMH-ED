# TUMH-ED
Sainuu, busduudd medegdku geed ingej bnshd bvvr , H
<!DOCTYPE html>
<html lang="mn">
<head>
  <meta charset="UTF-8">
  <title>Mongolian Cipher Decryptor</title>
  <style>
    body {
      font-family: system-ui, sans-serif;
      padding: 20px;
    }
    textarea {
      width: 100%;
      height: 120px;
      font-size: 16px;
    }
    button {
      margin-top: 10px;
      padding: 8px 16px;
      font-size: 16px;
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
  "й":"и","ц":"н","е":"ж","м":"г","Г":"А","Д":"Л","О":"Г","Л":"Ү"
};

function decrypt() {
  const input = document.getElementById("input").value;
  let result = "";

  for (const char of input) {
    result += mapping[char] || char;
  }

  document.getElementById("output").value = result;
}
</script>

</body>
</html>
