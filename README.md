# Projeto Amigo Secreto

![Status](https://img.shields.io/badge/status-concluído-brightgreen)

Uma aplicação web elegante e funcional para realizar sorteios de Amigo Secreto (ou Amigo Oculto) de forma simples e rápida. O projeto foi desenvolvido com foco em boas práticas de programação, utilizando HTML5, CSS3 e JavaScript puro (Vanilla JS), e possui um design responsivo que se adapta a diferentes tamanhos de tela.

## 🖼️ Demonstração Visual
![image](https://github.com/user-attachments/assets/db25d99e-8ce6-4234-8281-07f29a3e1b0a)

## ✨ Funcionalidades Principais

* **Adicionar Participantes:** Inclua quantos amigos quiser na lista para o sorteio.
* **Validação de Duplicidade:** O sistema impede a adição de nomes idênticos, garantindo a integridade da lista.
* **Sorteio Inteligente:** Realiza o sorteio utilizando o algoritmo de embaralhamento Fisher-Yates, garantindo que ninguém tire a si mesmo e que todos os participantes tirem alguém em um ciclo fechado.
* **Reiniciar Sorteio:** Limpe a lista de participantes e o resultado do sorteio com um único clique para começar de novo.
* **Requisito Mínimo:** O sorteio só é habilitado com um número mínimo de 4 participantes para garantir a dinâmica da brincadeira.

## 🚀 Tecnologias Utilizadas

* **HTML5:** Estrutura semântica e bem organizada.
* **CSS3:** Estilização moderna e responsiva, utilizando:
    * **Flexbox** para alinhamento dos layouts.
    * **Unidades Relativas (`rem`)** para garantir escalabilidade e adaptabilidade a diferentes zooms e tamanhos de tela.
    * **Fontes Externas** via Google Fonts (`Chakra Petch` e `Inter`).
* **JavaScript (ES6+):** Lógica do sorteio, manipulação dinâmica do DOM e interatividade com o usuário, sem a necessidade de frameworks externos.

## 🧠 Lógica do Sorteio

A função de sorteio foi cuidadosamente implementada para ser justa e à prova de erros:

1.  **Embaralhamento (Shuffle):** A lista de participantes é embaralhada aleatoriamente usando o algoritmo **Fisher-Yates**, que é um método eficiente e imparcial para criar uma permutação aleatória de uma sequência finita.
2.  **Atribuição em Ciclo:** Após o embaralhamento, a atribuição é feita de forma sequencial, garantindo que o último participante da lista sorteie o primeiro, fechando o ciclo e assegurando que ninguém fique de fora.
