- 👋 Hi, I’m @Sandbless
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Sandbless/Sandbless is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
//comandos
//while = enquanto, if = se, let = deixe, else = se não, prompt = escrever, alert = mensagem. breack = parar
// o while, Math.random = número aleatorio abaixo de 0, parseInt = bloquear os números abaixo não inteiros,
//

//condições
alert('Boas vindas ao Game Charada');
let numeroMaximo = 5000;
let numeroSecreto = parseInt(Math.random() * numeroMaximo + 1);
console.log (numeroSecreto);
let chute;
let tentativas = 1;

//enquanto o chute não for igualao N.S
while (chute != numeroSecreto) {
    chute = prompt (`escolha um número entre 1 a ${numeroMaximo}`);
    //se chute for igual ao nuemro secreto
    if (chute == numeroSecreto) {
        break;
    } else {
        if (chute > numeroSecreto) {
            alert(`O número secreto é menor que ${chute}`);
        } else {
            alert(`O número secreto é maior que ${chute}`);
        }
        tentativas++;
    }
}

    let palavratentativa = tentativas > 1 ? 'tentitivas.' : 'tentativa.'
    alert(`Parabéns! você acertou o numero secreto! (${numeroSecreto}) com ${tentativas} ${palavratentativa}`);
    //if (tentativas > 1) {
    //    alert(`Parabéns! você acertou o numero secreto! (${numeroSecreto}) com ${tentativas} tentativas!`);
    // } else {
    //     alert(`Parabéns! você acertou o numero secreto! (${numeroSecreto}) com ${tentativas} tentativa!`);

    //}
