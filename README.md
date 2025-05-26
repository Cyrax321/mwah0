# For-my-baby-Pumpkin-pie
Kisses for my lil Biscuitttt
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Mwah Counter</title>
  <style>
    body {
      background-color: pink;
      color: white;
      font-family: 'Arial', sans-serif;
      overflow-x: hidden;
      padding: 20px;
    }
    #counter {
      position: fixed;
      top: 10px;
      right: 20px;
      background: hotpink;
      padding: 10px 15px;
      border-radius: 10px;
      font-size: 20px;
      font-weight: bold;
      z-index: 999;
    }
    #mwahContainer {
      font-size: 24px;
      white-space: pre-wrap;
    }
  </style>
</head>
<body>
  <div id="counter">Mwahs: 0</div>
  <div id="mwahContainer"></div>

  <script>
    let count = 0;
    const mwahContainer = document.getElementById('mwahContainer');
    const counter = document.getElementById('counter');

    function addMwah() {
      mwahContainer.textContent += 'mwah ';
      count++;
      counter.textContent = 'Mwahs: ' + count;
      window.scrollTo(0, document.body.scrollHeight);
    }

    setInterval(addMwah, 100); // adds a new "mwah" every 100ms
  </script>
</body>
</html>
