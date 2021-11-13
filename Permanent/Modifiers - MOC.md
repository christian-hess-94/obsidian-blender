# Modifiers - MOC
Criado: 13/11/2021 - 18:01

tags: #modifiers

---

Modificadores ou Modifier são efeitos que alteram de forma não destrutiva a geometria de um objeto.
A forma como são adicionados ao objeto influenciam a forma como são aplicados ao mesmo.
Existem três tipos de Modifiers:
## Modificadores #modify_modifiers

## Geradores #generate_modifiers

## Deform #deform_modifiers
Modificadores deformadores são responsáveis por modificar a estrutura da geometria já existente. Não adicionam e nem removem complexidade da geometria, apenas modificam a posição de seus diversos vértices, arestas e faces.
- [[Armature Modifier]]
- [[Cast Modifier]]
- [[Curve Modifier]]
- [[Displace Modifier]]
- [[Hook Modifier]]: 
  
  - Isso permite que possamos criar uma animação no objeto externo para deformar o objeto com o modifier, coisa que não pode ser feita no Edit Mode
  
- [[Laplacian Deform Modifier]]:  Realiza um processo mais automatizado de Hooking. Permite que diversos hooks sejam associados à mesh para que possam alterar o formato durante um animação, por exemplo.
- [[Lattice Modifier]]: Utiliza um objeto do tipo Lattice (SHIFT + A) para envelopar uma mesh. Ao aplicar o modifier, se modificarmos a Lattice no Edit Mode, a Mesh envelopada é modificada de acordo.
  - Basicamente agrupa vários hooks em um formato de Grid (Lattice) e os utiliza para deformar a Mesh
- [[Mesh Deform Modifier]]: Mesma coisa do Lattice porém permite utilizar qualquer outra Mesh. Mais intensivo computacionalmente
- [[ShrinkWrap Modifier]]: Muito usado em retopologia
---
## Referências
1. [[Fleeting/Modifiers]]