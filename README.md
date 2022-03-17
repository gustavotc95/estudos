## Estudando teorias 🧠

Neste repositório deixarei por escrito algumas questões teóricas necessárias para a evolução profissional

### JS 
- [Como funciona o JS](#how-js-works)
- [O que é o JS](#what-is-js)
- [Hoisting](#hosting)
- [Promises](#promises)
- [Pure Functions](#pure-functions)
- [Higher-Order Functions](#higher-order-functions)
- [foreach vs map](#foreach-vs-map)
- [Tipos primitivos](#tipos-primitivos)

### NODE
- [Como funciona o NODE](#how-node-works)
- [Call Stack](#call-stack)
- [Middleware](#middleware)

### ReactJS
- [Como funciona o React](#how-react-works)
- [Arquitetura flux](#flux-architecture)
- [Componentes funcionais](#componentes-funcionais)
- [Higher-Order components](#higher-order-components)
- [Render Props (ou render functions)](#render-props)
- [Context API vs Redux](#context-vs-redux)
- [O que faz um componete ser atualizado?](#compontente-ser-atualizado)
- [Prop drilling](#prop-drilling)
- [O que é um componente controlado?](#componente-controlado)
- [Real DOM vs Virtual DOM](#componente-controlado)
- [Class components vs Functional components](#class-vs-functional)
- [O que são keys?](#keys)
- [Life cycle do react](#life-cycle)

### Testes
- [TDD](#tdd)

### Outros
- [POO](#poo)
- [Pilares POO](#poo-pillars)
- [Pilares Programação Funcional](#functional-programming-pillars)

#### <a name="hoisting"></a> Hoisting
Hoisting é o içamento de funções e variáveis para o topo do código, isso declara as variáveis e funções em memória e permite que você use uma função/variável antes mesmo de declara-la.
```javascript
sayHello();
// a função foi chamada antes de ser declarada
    
functionSayHello() {
    console.log("Say Hello");
}
```
O mesmo é acontece para variáveis, as quais podem ser inicializadas antes de serem declaradas. Porém, o js eleva somente a declaração não a inicialização.
```javascript 
console.log(num); // undefined -> nesse caso num é undefined porque só foi declarada
num = 6;
console.log(num); // 6 -> agora num já foi inicializada
var num;
```
