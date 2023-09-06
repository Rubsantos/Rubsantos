- 👋 Hi, I’m @Rubsantos
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Rubsantos/Rubsantos is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<!-- 
Código escrito por MTHS1901 em um tutorial no YouTube
Confira: https://www.youtube.com/watch?v=zxxB9SFh9p4
Este arquivo já esta pronto e você pode mandar para quem quiser
-->
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Namora comigo?</title>
</head>

<body>
    <div id="conteudo">
        <h2>Aceita namorar comigo?</h2>
        <div style="margin: auto;width: 170px;">
            <button style="position: fixed;display: block;" class="btn" onclick="sim()">SIM</button>
            <button class="btn" onclick="desvia(this)" onmouseover="desvia(this)" style="position: absolute;">NÃO</button>
        </div>
    </div>
</body>
<style>
    #conteudo {
        background: #ff7a7a;
        width: 100%;
        height: 100%;
        position: fixed;
        top: 0;
        left: 0;
        padding: 10px;
        text-align: center;
        font-family: sans-serif;
    }

    .btn {
        background: black;
        color: white;
        border: none;
        padding: 10px;
        width: 80px;
        border-radius: 5px;
    }
</style>

<script>
    function sim() {
        alert("Você aceitou namorar comigo! :)");
        // redireciona para um URL após clicar no SIM
        location.href = "https://music.youtube.com/watch?v=izGwDsrQ1eQ";
    }

    function desvia(btn) {
        // btn declarado na função
        btn.style.position = 'absolute';
        btn.style.bottom = geraPosicao(10, 90);
        btn.style.left = geraPosicao(10, 90);
        console.log('opa, desviei...');
    }

    function geraPosicao(min, max) {
        return (Math.random() * (max - min) + min) + "%";
    }

    /* Apague se quiser, isso apenas escreve MTHS1901 e o link para o tutorial no console */
    const o = "MTHS1901", e = 90, l = "bold"; console.log(`%c${o}`, "font-size: 90px; font-weight: bold; background: linear-gradient(90deg, red, yellow);"), console.log("Tutorial: https://www.youtube.com/watch?v=zxxB9SFh9p4");

</script>

</html>
