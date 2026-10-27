
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Desafio Drauzio Varella</title>

<style>
* { box-sizing: border-box; }

body {
  margin: 0;
  padding: 20px;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: Arial, sans-serif;
  color: white;
  background:
    linear-gradient(#06101bdc, #06101be8),
    url("https://www.sicredi.com.br/media/coop/filer_public/2020/09/29/drauzio_varella_-_credito_ana_bogaciovas_-_03-9407233801773830658.jpg")
    center/cover fixed;
}

.game {
  width: 100%;
  max-width: 540px;
  padding: 24px;
  border-radius: 20px;
  background: #14243aee;
  border: 1px solid #4fffc1;
  box-shadow: 0 15px 50px #0009;
}

header {
  display: flex;
  align-items: center;
  gap: 15px;
}

.foto {
  width: 85px;
  height: 85px;
  object-fit: cover;
  border-radius: 50%;
  border: 3px solid #4fffc1;
}

h1 { color: #4fffc1; font-size: 25px; }
.sub { color: #c5d5e5; font-size: 13px; }

.info {
  display: flex;
  justify-content: space-between;
  margin-top: 22px;
}

.barra {
  height: 8px;
  background: #39485b;
  border-radius: 20px;
  overflow: hidden;
  margin: 12px 0;
}

#progresso {
  height: 100%;
  width: 0;
  background: #4fffc1;
}

.timer {
  display: flex;
  align-items: center;
  gap: 10px;
  margin: 15px 0;
}

#tempoBarra {
  height: 10px;
  width: 100%;
  background: #4fffc1;
  border-radius: 20px;
}

#tempoBarra.fim { background: #ff4055; }

#tempo {
  font-size: 22px;
  font-weight: bold;
  color: #4fffc1;
}

#pergunta {
  font-size: 20px;
  line-height: 1.5;
  min-height: 100px;
}

button {
  width: 100%;
  padding: 15px;
  margin-top: 10px;
  border: none;
  border-radius: 10px;
  font-size: 16px;
  font-weight: bold;
  cursor: pointer;
}

button:disabled { opacity: .5; }

.v { background: #13865b; color: white; }
.f { background: #c0394b; color: white; }
.proximo { background: #4fffc1; color: #07111f; }

#feedback {
  padding: 14px;
  background: #253951;
  border-radius: 10px;
  margin-top: 15px;
  line-height: 1.5;
}

.escondido { display: none; }

#final { text-align: center; }

@media(max-width: 400px) {
  .game { padding: 17px; }
  h1 { font-size: 21px; }
  #pergunta { font-size: 18px; }
}
</style>
</head>

<body>
<div class="game">

<header>
  <img class="foto"
    src="https://www.sicredi.com.br/media/coop/filer_public/2020/09/29/drauzio_varella_-_credito_ana_bogaciovas_-_03-9407233801773830658.jpg"
    alt="Drauzio Varella">
  <div>
    <h1>Verdadeiro ou Falso</h1>
    <div class="sub">DESAFIO DIFÍCIL — DRAUZIO VARELLA</div>
  </div>
</header>

<div id="jogo">
  <div class="info">
    <span id="contador">Pergunta 1 de 10</span>
    <span id="pontos">Pontos: 0</span>
  </div>

  <div class="barra">
    <div id="progresso"></div>
  </div>

  <div class="timer">
    <span>⏱️</span>
    <div class="barra" style="flex:1">
      <div id="tempoBarra"></div>
    </div>
    <span id="tempo">10</span>
  </div>

  <h2 id="pergunta"></h2>

  <button class="v" id="btnV"
    onclick="responder(true)">VERDADEIRO</button>

  <button class="f" id="btnF"
    onclick="responder(false)">FALSO</button>

  <div id="feedback" class="escondido"></div>

  <button class="proximo escondido" id="btnProximo"
    onclick="proxima()">Próxima pergunta →</button>
</div>

<div id="final" class="escondido">
  <h1>🏆 Fim de jogo!</h1>
  <h2 id="resultado"></h2>
  <p id="mensagem"></p>
  <button class="proximo" onclick="reiniciar()">
    JOGAR NOVAMENTE
  </button>
</div>

</div>

<script>
const perguntas = [
  {
    texto: "Drauzio Varella formou-se em Medicina pela USP em 1967.",
    resposta: true,
    explicacao: "Verdadeiro! Ele se formou na Faculdade de Medicina da Universidade de São Paulo em 1967."
  },
  {
    texto: "O trabalho voluntário de Drauzio Varella no Carandiru começou em 1989.",
    resposta: true,
    explicacao: "Verdadeiro! O trabalho começou em 1989 e envolveu ações de prevenção do HIV."
  },
  {
    texto: "O livro Estação Carandiru foi publicado antes de 1989.",
    resposta: false,
    explicacao: "Falso! O livro foi publicado em 1999, dez anos depois do início do trabalho no Carandiru."
  },
  {
    texto: "O filme Carandiru, lançado em 2003, foi dirigido por Hector Babenco.",
    resposta: true,
    explicacao: "Verdadeiro! Hector Babenco dirigiu a adaptação cinematográfica."
  },
  {
    texto: "Drauzio Varella estudou Medicina na Unicamp, e não na USP.",
    resposta: false,
    explicacao: "Falso! Sua formação médica ocorreu na USP."
  },
  {
    texto: "Carcereiros e Prisioneiras também estão entre as obras relacionadas à experiência prisional de Drauzio Varella.",
    resposta: true,
    explicacao: "Verdadeiro! Os dois livros fazem parte de sua produção sobre o sistema prisional."
  },
  {
    texto: "Drauzio Varella trabalhou exclusivamente como cirurgião, sem se dedicar à pesquisa médica.",
    resposta: false,
    explicacao: "Falso! Ele também atuou em pesquisa e dirigiu o Serviço de Imunologia do Hospital do Câncer."
  },
  {
    texto: "Além da medicina, Drauzio Varella é conhecido por divulgar informações de saúde ao público.",
    resposta: true,
    explicacao: "Verdadeiro! Ele comunica temas médicos na televisão, na imprensa e na internet."
  },
  {
    texto: "Drauzio Varella nunca teve interesse por corrida de longa distância.",
    resposta: false,
    explicacao: "Falso! Ele pratica corrida e já participou de maratonas."
  },
  {
    texto: "A trajetória de Drauzio Varella inclui trabalho sobre prevenção do HIV e divulgação de informações sobre AIDS.",
    resposta: true,
    explicacao: "Verdadeiro! A prevenção do HIV fez parte de seu trabalho no Carandiru e de suas ações de comunicação pública."
  }
];

let atual = 0;
let pontuacao = 0;
let segundos = 10;
let intervalo;
let respondeu = false;

const el = id => document.getElementById(id);

function iniciarTempo() {
  clearInterval(intervalo);
  segundos = 10;
  atualizarTempo();

  intervalo = setInterval(() => {
    segundos--;
    atualizarTempo();

    if (segundos <= 0) {
      clearInterval(intervalo);
      responder(null, true);
    }
  }, 1000);
}

function atualizarTempo() {
  el("tempo").textContent = segundos;
  el("tempoBarra").style.width = (segundos * 10) + "%";
  el("tempoBarra").classList.toggle("fim", segundos <= 3);
  el("tempo").style.color =
    segundos <= 3 ? "#ff4055" : "#4fffc1";
}

function mostrarPergunta() {
  respondeu = false;

  el("contador").textContent =
    `Pergunta ${atual + 1} de ${perguntas.length}`;

  el("pergunta").textContent = perguntas[atual].texto;
  el("pontos").textContent = "Pontos: " + pontuacao;
  el("progresso").style.width =
    (atual / perguntas.length * 100) + "%";

  el("feedback").classList.add("escondido");
  el("btnProximo").classList.add("escondido");
  el("btnV").disabled = false;
  el("btnF").disabled = false;

  iniciarTempo();
}

function responder(escolha, acabouTempo = false) {
  if (respondeu) return;

  respondeu = true;
  clearInterval(intervalo);

  const p = perguntas[atual];
  const acertou = !acabouTempo && escolha === p.resposta;

  if (acertou) pontuacao++;

  el("btnV").disabled = true;
  el("btnF").disabled = true;
  el("pontos").textContent = "Pontos: " + pontuacao;

  el("progresso").style.width =
    ((atual + 1) / perguntas.length * 100) + "%";

  el("feedback").innerHTML =
    `<strong>${acabouTempo ? "⏰ Tempo esgotado!" :
    acertou ? "✅ Acertou!" : "❌ Errou!"}</strong><br>
    ${p.explicacao}`;

  el("feedback").classList.remove("escondido");

  el("btnProximo").textContent =
    atual === perguntas.length - 1
    ? "Ver resultado 🏆"
    : "Próxima pergunta →";

  el("btnProximo").classList.remove("escondido");
}

function proxima() {
  atual++;

  if (atual < perguntas.length) {
    mostrarPergunta();
  } else {
    clearInterval(intervalo);
    el("jogo").classList.add("escondido");
    el("final").classList.remove("escondido");
    el("resultado").textContent =
      pontuacao + " / " + perguntas.length + " pontos";

    el("mensagem").textContent =
      pontuacao === 10 ? "Perfeito! Você acertou tudo!" :
      pontuacao >= 8 ? "Excelente resultado!" :
      pontuacao >= 5 ? "Muito bem! Tente melhorar sua pontuação." :
      "Continue estudando e tente novamente!";
  }
}

function reiniciar() {
  atual = 0;
  pontuacao = 0;
  el("jogo").classList.remove("escondido");
  el("final").classList.add("escondido");
  mostrarPergunta();
}

mostrarPergunta();
</script>
</body>
</html>
