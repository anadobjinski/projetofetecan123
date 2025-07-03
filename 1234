<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Cidade Inteligente</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #f0f2f5;
      color: #333;
    }

    header {
      background-color: #004d99;
      color: #fff;
      padding: 20px;
      text-align: center;
    }

    .container {
      padding: 20px;
    }

    .card {
      background: white;
      border-radius: 8px;
      padding: 15px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
      margin-bottom: 20px;
    }

    .toggle {
      margin-top: 10px;
    }

    label {
      display: inline-block;
      margin-right: 10px;
    }

    input[type="checkbox"] {
      transform: scale(1.2);
    }

    .dashboard-data {
      display: flex;
      justify-content: space-between;
      margin-top: 10px;
    }

    .dashboard-item {
      flex: 1;
      padding: 10px;
      background: #e6f2ff;
      margin: 5px;
      border-radius: 5px;
      text-align: center;
    }

    button {
      padding: 10px 20px;
      background-color: #0077cc;
      color: white;
      border: none;
      border-radius: 5px;
      margin-top: 10px;
      cursor: pointer;
    }

    button:hover {
      background-color: #005fa3;
    }
  </style>
</head>
<body>
  <header>
    <h1>Painel da Cidade Inteligente</h1>
    <p>Monitoramento e controle urbano em tempo real</p>
  </header>

  <div class="container">
    <div class="card">
      <h2>Iluminação Pública</h2>
      <label for="lampToggle">Ativar Iluminação Noturna</label>
      <input type="checkbox" id="lampToggle" onchange="atualizarStatus('lampToggle')"/>
    </div>

    <div class="card">
      <h2>Sistema de Coleta</h2>
      <p>Status da coleta: <span id="coletaStatus">Agendada</span></p>
      <button onclick="alterarColeta()">Alterar Coleta</button>
    </div>

    <div class="card">
      <h2>Tráfego Urbano</h2>
      <div class="dashboard-data">
        <div class="dashboard-item">
          <h3>Semáforos</h3>
          <p id="semaforoStatus">Sincronizados</p>
        </div>
        <div class="dashboard-item">
          <h3>Fluxo</h3>
          <p id="fluxoStatus">Moderado</p>
        </div>
      </div>
      <button onclick="atualizarTrafego()">Atualizar Dados</button>
    </div>
  </div>

  <script>
    function atualizarStatus(id) {
      const estado = document.getElementById(id).checked ? 'ativo' : 'inativo';
      alert("Iluminação está agora " + estado);
    }

    function alterarColeta() {
      const status = document.getElementById("coletaStatus");
      status.innerText = (status.innerText === "Agendada") ? "Em andamento" : "Agendada";
    }

    function atualizarTrafego() {
      const fluxo = ["Moderado", "Pesado", "Leve"];
      const semaforos = ["Sincronizados", "Desincronizados"];
      document.getElementById("fluxoStatus").innerText = fluxo[Math.floor(Math.random() * fluxo.length)];
      document.getElementById("semaforoStatus").innerText = semaforos[Math.floor(Math.random() * semaforos.length)];
    }
  </script>
</body>
</html>
