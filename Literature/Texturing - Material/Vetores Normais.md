# Vetores Normais
Criado: 15/11/2021 - 16:01
links: [[Texturas]] - [[Material]]
tags: #done 

---

A Normal é um vetor calculado a partir de cada face de um objeto 3D. Esse vetor é perpendicular a essa superfície.

O caso de uso mais comum do Vetor Normal é para renderização de materiais na face.  o processo de renderização a engine apenas renderiza a face caso o seu Vetor Normal seja positivo e aponte para a camera que está realizando a renderização.

Isso significa que a engine não renderiza as faces opostas (ou "de dentro") da geometria, aumentando sua performance.  Esse processo se chama **Face Culling**

![[Face Culling.png]]

Em contrapartida, isso faz com o ladooposto  do objeto "não exista" e seja transparente, o que pode trazer problemas dependo do que deve ser mostrado.

![[Face Culling 2.png]]

---
## Referências
1.