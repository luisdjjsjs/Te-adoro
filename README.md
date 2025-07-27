# Te-adoro
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Te adoro</title>
  <style>
    body {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
      background-color: #fdf6e3;
      margin: 0;
      font-family: Arial, sans-serif;
      line-height: 1.5;
      cursor: pointer;
    }
    .container {
      width: 80%;
      max-width: 600px;
      text-align: center;
    }
    p {
      margin: 4px 0;
      font-size: 1.2rem;
      color: #d33682;
    }
  </style>
</head>
<body>
  <div class="container" id="container">
  </div>

  <script>
    const container = document.getElementById('container');
    function appendTeAdoro() {
      const p = document.createElement('p');
      p.textContent = 'Te adoro';
      container.appendChild(p);
    }
    for (let i = 0; i < 100; i++) {
      appendTeAdoro();
    }
    document.body.addEventListener('click', () => {
      appendTeAdoro();
    });
  </script>
</body>
</html>
