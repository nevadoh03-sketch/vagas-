<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vagas Americanas - Encontre Seu Emprego</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Vagas Americanas</h1>
        <nav>
            <a href="#vagas">Vagas</a>
            <a href="#inscrever">Inscrever-se</a>
            <a href="#sobre">Sobre</a>
        </nav>
    </header>

    <section id="hero">
        <h2>Encontre a Vaga dos Seus Sonhos</h2>
        <p>Estilo americano: Simples, direto e eficaz. Assine por $15/mês e receba novas vagas instantaneamente!</p>
        <button onclick="window.location.href='#inscrever'">Começar Agora</button>
    </section>

    <section id="vagas">
        <h2>Vagas Disponíveis</h2>
        <div class="filtros">
            <input type="text" id="localizacao" placeholder="Localização (ex.: São Paulo)">
            <select id="tipo">
                <option value="">Tipo de Emprego</option>
                <option value="full-time">Tempo Integral</option>
                <option value="part-time">Meio Período</option>
                <option value="remote">Remoto</option>
            </select>
            <button onclick="filtrarVagas()">Filtrar</button>
        </div>
        <div id="lista-vagas">
            <!-- Vagas simuladas; no backend real, carregue do DB -->
            <div class="vaga">
                <h3>Desenvolvedor Full-Stack</h3>
                <p>Empresa: TechCorp | Local: São Paulo | Salário: $5.000/mês</p>
                <p>Descrição: Trabalhe com tecnologias modernas. Requer experiência em React e Node.js.</p>
                <button class="inscrever-btn" onclick="alert('Assine para candidatar-se!')">Candidatar-se</button>
            </div>
            <div class="vaga">
                <h3>Designer Gráfico</h3>
                <p>Empresa: Creative Inc | Local: Rio de Janeiro | Salário: $3.500/mês</p>
                <p>Descrição: Crie designs incríveis para campanhas digitais.</p>
                <button class="inscrever-btn" onclick="alert('Assine para candidatar-se!')">Candidatar-se</button>
            </div>
            <!-- Mais vagas podem ser adicionadas dinamicamente -->
        </div>
        <p class="aviso">Novas vagas são enviadas apenas para assinantes ($15/mês).</p>
    </section>

    <section id="inscrever">
        <h2>Inscreva-se e Receba Novas Vagas</h2>
        <p>Pague $15 mensais e seja notificado instantaneamente quando novas vagas forem publicadas.</p>
        <form id="form-inscrever">
            <input type="email" id="email" placeholder="Seu Email" required>
            <input type="text" id="nome" placeholder="Seu Nome" required>
            <button type="submit">Pagar $15/mês e Inscrever</button>
        </form>
        <p id="mensagem"></p>
    </section>

    <section id="sobre">
        <h2>Sobre Nós</h2>
        <p>Estilo americano: Foco em eficiência e oportunidades. Nosso site conecta talentos a empregos de qualidade.</p>
    </section>

    <footer>
        <p>&copy; 2023 Vagas Americanas. Todos os direitos reservados.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
