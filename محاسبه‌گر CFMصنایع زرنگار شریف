<!DOCTYPE html>
<html lang="fa">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>محاسبه‌گر CFM</title>
  <style>
    body {
      font-family: sans-serif;
      direction: rtl;
      padding: 20px;
      background: #f7f7f7;
      color: #333;
    }
    .container {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      max-width: 400px;
      margin: auto;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }
    label {
      display: block;
      margin-top: 15px;
    }
    input {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
    }
    button {
      margin-top: 20px;
      padding: 10px;
      width: 100%;
      background: #2196f3;
      color: white;
      border: none;
      border-radius: 5px;
    }
    #result {
      margin-top: 20px;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <h1>شرکت صنایع زرنگار شریف - تولید کننده مکندهای صنعتی</h1>
  <div class="container">
    <label for="length">طول (متر):</label>
    <input type="number" id="length" />

    <label for="width">عرض (متر):</label>
    <input type="number" id="width" />

    <label for="height">ارتفاع (متر):</label>
    <input type="number" id="height" />

    <label for="ach">تعداد تعویض هوا در ساعت (ACH):</label>
    <input type="number" id="ach" />

    <button onclick="calculateCFM()">محاسبه CFM</button>

    <div id="result"></div>
  </div>

  <script>
    function calculateCFM() {
      const length = parseFloat(document.getElementById("length").value);
      const width = parseFloat(document.getElementById("width").value);
      const height = parseFloat(document.getElementById("height").value);
      const ach = parseFloat(document.getElementById("ach").value);

      if (isNaN(length) || isNaN(width) || isNaN(height) || isNaN(ach)) {
        alert("لطفاً همه مقادیر را به‌درستی وارد کنید");
        return;
      }

      const volume = length * width * height;
      const cfm = (volume * ach) / 60;
      document.getElementById("result").innerText = `مقدار CFM مورد نیاز: ${cfm.toFixed(2)}`;
    }
  </script>
</body>
</html>
