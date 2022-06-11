// let tipoTransacao = document.querySelector('#type').value;
// let nomeMercadoria = document.querySelector('#nomeMercadoria').value;
// let valor = document.querySelector('#valor').value;
let button = document.querySelector('.button');

let formMercadoria = document.querySelector('#formMercadoria');
let items = JSON.parse(localStorage.getItem('items')) || [];

\***\*\*\*\***pt2
formMercadoria.addEventListener('submit', event => {
event.preventDefault();

const tipoTransacao = event.target.elements['type'];
const nomeMercadoria = event.target.elements['nomeMercadoria'];
const valor = event.target.elements['valor'];

items.push({
tipoTransacao: tipoTransacao.value,
nomeMercadoria: nomeMercadoria.value,
valor: valor.value
});

//localStorage.setItem('items', JSON.stringify(items));
//nomeMercadoria.value = '';
//valor.value = '';
//});
