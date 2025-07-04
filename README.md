<!DOCTYPE html>
<html lang="pt-BT">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Extrator de Palavras-Chave</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <div class="container">
        <h1>Extrator de palavras-chave</h1>
        <textarea id="entrada-de-texto" placeholder="Digite ou cole seu texto aqui..."></textarea>
        <button id="botao-palavrachave">Extrair</button>
        <div id="resultado-palavrachave"></div>
    </div>
    <script src="script.js"></script>
   
function processa Texto (Trabalho) {
    let palavras = texto.split(/\P{L}+/u);
    
    let frequencias = [];
    for(let i in palavras) {
        frequencias [i] = 0;
        for (let jin palavras) {
            if (palavras[i]==palavras[j]){
                frequencias[i]++;
            }
        }
    }
    console.log(frequencias);
    
    return palavras;
}
}

function contaVendas(listaVendas) { 
  let produtos = listaVendas.split(/\P{L}+/u); 
  let contagem = {}; 

  for (let i of produtos) { 
    contagem[i] = 0; 
    for (let j of produtos) { 
      if (i == j) { 
        contagem[i]++; 
      } 
    } 
  } 
  console.log(contagem); 
  return contagem; 
}
function tiraPalavrasRuins(palavras) {
    const PALAVRAS_RUINS = ["para", "uma", "nós"];
    const palavrasBoas = [];
    for (let palavra of palavras){
        if (!PALAVRAS_RUINS.has(palavra) && palavra.length > 2) {
    palavrasBoas.push(palavra);
        }
    }
return palavrasBoas;
}
</body>

const texto = "Programar é divertido!"; 

const vogais = texto.match(/[aeiou]/gi); 

console.log(vogais); 
</html>
