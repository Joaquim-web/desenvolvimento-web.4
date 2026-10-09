# desenvolvimento-web.4
entregavel de desenvolvimento web semana 4
const nomes = ["Ana", "Bruno", "Carla"];

nomes.forEach((nome) => console.log(`Olá, ${nome}!`));

const nomesMaiusculos = nomes.map((nome) => nome.toUpperCase());
console.log(nomesMaiusculos);

const precos = [10, 25, 40, 5, 60];

const precosMaioresQue20 = precos.filter((preco) => preco > 20);
console.log(precosMaioresQue20);

const totalPrecos = precos.reduce((acumulador, preco) => acumulador + preco, 0);
console.log(totalPrecos);

const produtos = [
  { nome: "Caderno", preco: 15 },
  { nome: "Mochila", preco: 120 },
  { nome: "Caneta", preco: 5 },
  { nome: "Estojo", preco: 30 }
];

const nomesProdutos = produtos.map((produto) => produto.nome);
console.log(nomesProdutos);

const produtosBaratos = produtos.filter((produto) => produto.preco < 50);
console.log(produtosBaratos);

const totalProdutos = produtos.reduce((acumulador, produto) => acumulador + produto.preco, 0);
console.log(totalProdutos);

produtos.forEach((produto) => console.log(`${produto.nome}: R$ ${produto.preco}`));
