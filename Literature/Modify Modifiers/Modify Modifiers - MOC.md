# Modify Modifiers - MOC
Criado: 14/11/2021 - 15:18

tags:  #modify_modifiers

---

Modifiers Modificadores realizam operações que alteram diretamente a geometria do objeto sendo construído.

Essas alterações são chamadas de [[Modelagem não destrutiva]].

### Lista de modifiers
- [[Data Transfer Modifier]]: 
- [[Mesh Cache Modifier]]: 
- [[Mesh Sequence Modifier]]: 
- [[Normal Edit Modifier]]: 
- [[Weighted Normal Modifier]]: 
- [[UV Project Modifier]]: 
- [[UV Wrap Modifier]]: Permite usar objetos externos para alterar a projeção da textura no mapa UV do objeto com o modificador
- [[Vertex Weight Edit Modifier]]: Permite realizar alterações ao weight painting feito em uma mesh. Permite alterar coisas como Default Weight e modificar o weight painting ativo de maneira procedural
- [[Vertex Weight Mix Modifier]]: Permite realizar um mix dos weight paintings de diferentes Vertex Groups. Oferece a opção de realizar diversas operações como Add, Subtract, Difference, dentre outros.
- [[Vertex Weight Proximity Modifier]]: Permite a criação de Vertex Groups e Weight Paintings dinâmicos. Associa um objeto ao modificador que cria um vertex group a partir da localização do objeto. Outros parâmetros podem ser mexidos para ajustar o tamanho e intensidade do Weight Paint que é originado.
  - Pode fazer um efeito de fade com ajude de um Wireframe Modifier (explicado abaixo)

---
## Referências
1. [[Modifiers - MOC]]