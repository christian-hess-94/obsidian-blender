# UV Map
Criado: 15/11/2021 - 15:32

tags: #texturing  

---

O UV Map é uma imagem que representa a geometria 3D de um objeto em um plano 2D. 

```
UV são os nomes das coordenadas horizontal e vertical da imagem, visto que XYZ já são usadas no espaço 3D.
```

No momento de aplicação de uma Textura, ou de [[Texture Paint]], o UV Map é utilizado para identificar quais partes da imagem da textura devem ser aplicados na geometria do objeto.

O UV Map também é utilizado em processos de [[Texture Baking]], para que possa salvar as informações das cores sendo geradas durante o processo de acordo com a geometria do mesmo.

O ato de criar uma UV Map a partir de um objeto 3D se chama [[UV Unwrapping]] e pode ser feito de forma manual ou automática, usando diversos algoritmos.

---
## Referências
1. https://pt.wikipedia.org/wiki/Mapeamento_UV
2. https://conceptartempire.com/uv-mapping-unwrapping/