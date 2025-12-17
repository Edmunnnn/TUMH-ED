# TUMH-ED
Sainuu, busduudd medegdku geed ingehees uur raga baisnguee , H
<!DOCTYPE html>
<html lang="mn">
<head>
  <meta charset="UTF-8">
  <title>Mongolian Text Output</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      font-family: system-ui, sans-serif;
      padding: 20px;
      max-width: 800px;
      margin: auto;
    }
    textarea {
      width: 100%;
      height: 120px;
      font-size: 16px;
      margin-top: 10px;
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

<textarea>
Цгупфхдоуялг дпзлгду. Щпшшззр шл, пууджгг плпл юйц, рпегррй йхпм плпл.
</textarea>

<button onclick="showText()">Decrypt</button>

<textarea id="output" readonly></textarea>

<script>
function showText() {
  document.getElementById("output").value =
    "Харамсалгүй амьдар. Өнөөдөр чи, маргааш миний зүрх, омбогор гүнж минь.";
}
</script>

</body>
</html>
