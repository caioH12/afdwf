<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Venda de Aviões</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }
        header {
            background-color: #007bff;
            color: white;
            padding: 20px;
            text-align: center;
        }
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 20px auto;
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }
        .plane-card {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            width: calc(33.333% - 20px);
            box-sizing: border-box;
            overflow: hidden;
        }
        .plane-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        .plane-card .details {
            padding: 15px;
        }
        .plane-card h2 {
            margin: 0 0 10px;
        }
        .plane-card p {
            margin: 0 0 15px;
        }
        .plane-card .price {
            font-size: 20px;
            color: #007bff;
            margin-bottom: 15px;
        }
        .plane-card button {
            background-color: #007bff;
            color: white;
            border: none;
            padding: 10px;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }
        .plane-card button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <header>
        <h1>Venda de Aviões</h1>
    </header>

    <div class="container">
        <!-- Avião 1 -->
        <div class="plane-card">
            <img src="https://via.placeholder.com/600x400" alt="Avião 1">
            <div class="details">
                <h2>Avião SuperJet 500</h2>
                <p>Um jato executivo de alta performance com capacidade para 8 passageiros. Ideal para viagens internacionais.</p>
                <div class="price">R$ 20.000.000</div>
                <button onclick="buyPlane('Avião SuperJet 500')">Comprar</button>
            </div>
        </div>

        <!-- Avião 2 -->
        <div class="plane-card">
            <img src="https://via.placeholder.com/600x400" alt="Avião 2">
            <div class="details">
                <h2>Avião Cargo XL</h2>
                <p>O Avião Cargo XL é perfeito para transporte de grandes cargas. Capacidade de carga de 50 toneladas.</p>
                <div class="price">R$ 15.000.000</div>
                <button onclick="buyPlane('Avião Cargo XL')">Comprar</button>
            </div>
        </div>

        <!-- Avião 3 -->
        <div class="plane-card">
            <img src="https://via.placeholder.com/600x400" alt="Avião 3">
            <div class="details">
                <h2>Avião de Passeio SkyDreamer</h2>
                <p>Ideal para viagens de lazer com capacidade para 4 passageiros. Equipado com a mais moderna tecnologia.</p>
                <div class="price">R$ 5.000.000</div>
                <button onclick="buyPlane('Avião de Passeio SkyDreamer')">Comprar</button>
            </div>
        </div>
    </div>

    <script>
        function buyPlane(planeName) {
            alert('Você selecionou o ' + planeName + '. Entre em contato para mais informações.');
        }
    </script>
</body>
</html>

