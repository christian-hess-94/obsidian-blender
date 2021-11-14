# Modify Modifiers - MOC
Criado: 14/11/2021 - 15:18

tags:  #modify_modifiers

---

Modifiers Modificadores realizam operações que alteram diretamente a geometria do objeto sendo construído.

Essas alterações são chamadas de [[Modelagem não destrutiva]].

- [[Data Transfer Modifier]]: Serve para transferir dados de uma mesh para outra, coisas como posição e direção dos vetores normais
- [[Mesh Cache Modifier]]: Permite associar animações externas aos objetos. Um dos tipos possíveis é MDD
- [[Mesh Sequence Modifier]]: Faz a mesma coisa que o Mesh Cache mas usando arquivos.alembic
- [[Normal Edit Modifier]]: Permite alterar a direção das normais de um objeto a partir de outro objeto. **Pode servir para direcionar as normais de um sistema de particulas para a camêra fazendo com que cada particula fique mais visível**
- [[Weighted Normal Modifier]]: Faz uma interpolação dos vetores normais do vértices para que apontem na direção dos vetores normais das faces que compõem. Pode aumentar a fidelidade gráfica de um objeto sem precisar aumentar a taxa de vértices.
- [[UV Project Modifier]]: Permite utilizar um objeto como um “projetor” que projeta a textura em cima do UV Map do objeto com o modificador.
- [[UV Wrap Modifier]]: Permite usar objetos externos para alterar a projeção da textura no mapa UV do objeto com o modificador
- [[Vertex Weight Edit Modifier]]: Permite realizar alterações ao weight painting feito em uma mesh. Permite alterar coisas como Default Weight e modificar o weight painting ativo de maneira procedural
- [[Vertex Weight Mix Modifier]]: Permite realizar um mix dos weight paintings de diferentes Vertex Groups. Oferece a opção de realizar diversas operações como Add, Subtract, Difference, dentre outros.
- [[Vertex Weight Proximity Modifier]]: Permite a criação de Vertex Groups e Weight Paintings dinâmicos. Associa um objeto ao modificador que cria um vertex group a partir da localização do objeto. Outros parâmetros podem ser mexidos para ajustar o tamanho e intensidade do Weight Paint que é originado.
  - Pode fazer um efeito de fade com ajude de um Wireframe Modifier (explicado abaixo)

---
## Referências
1. [[Modifiers - MOC]]