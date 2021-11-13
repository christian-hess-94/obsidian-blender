# Deformadores (Deform)
Criado: 13/11/2021 - 18:03

tags: #modifier

---

Modificadores deformadores são responsáveis por modificar a estrutura da geometria já existente. Não adicionam e nem removem complexidade da geometria, apenas modificam a posição de seus diversos vértices, arestas e faces.

Os modificadores são:

- [[Armature]]: Permite adicionar um esqueleto (Armature) ao objeto. Normalmente esse processo não é feito através do Modifier. O modifier é colocado automaticamente ao se dar parent da mesh na armature.
- [[Cast]]: Modifier que se especializa em transformar a mesh para que tenha um formato de esfera, cilindro ou cuboide.
- [[Curve]]: Permite associar a mesh a uma Curve. Pode-se criar um combo de modifier para que a mesh se duplique em volta da Curve
  - Crie a Curve a ser usada
  - Crie e modifique o objeto a ser duplicado
  - Adicione o Array Modifier para começar a criar cópias
  - No fit type, selecione Fit Curve e escolha a Curve criada
    - Isso faz com que o objeto seja duplicado até o resultado ser do tamanho da Curve
  - Adicione o Curve Modifier **após** o Array Modifier e selecione a Curve
    - O objeto e suas cópias seguem o contorno da Curva
- [[Displace]]: Permite aplicar uma Imagem ou Textura Procedural para mover os vértices da mesh. Muito útil para criar ondulações e dar um efeito mais natural e imperfeito a uma mesh.
- [[Hook]]: Permite que um objeto externo possa modificar a geometria do objeto que possui o modifier.
  - Normalmente a geometria só pode ser modificada manualmente no Edit Mode
  - Ao colocar um Hook de uma parte da geometria a um objeto externo, podemos mover e alterar o objeto externo para alterar a geometria
  - Isso permite que possamos criar uma animação no objeto externo para deformar o objeto com o modifier, coisa que não pode ser feita no Edit Mode
  - O atalho para fazer isso diretamente do Edit Mode é CTRL + H
    - Isso cria um novo hook onde fica o 3D Cursor e associa todos os vértices, arestas e faces selecionado a ele (cria o Hook modifier automaticamente)
    - Para fazer com que o novo Hook seja criado junto da geometria que ele move, use CTRL + S e escolha 3D Cursor to Active
- [[Laplacian Deform]]:  Realiza um processo mais automatizado de Hooking. Permite que diversos hooks sejam associados à mesh para que possam alterar o formato durante um animação, por exemplo.
- [[Lattice]]: Utiliza um objeto do tipo Lattice (SHIFT + A) para envelopar uma mesh. Ao aplicar o modifier, se modificarmos a Lattice no Edit Mode, a Mesh envelopada é modificada de acordo.
  - Basicamente agrupa vários hooks em um formato de Grid (Lattice) e os utiliza para deformar a Mesh
- [[Mesh Deform]]: Mesma coisa do Lattice porém permite utilizar qualquer outra Mesh. Mais intensivo computacionalmente
- [[ShrinkWrap]]: Muito usado em retopologia

---
## Referências
1. [[Literature/Modifiers]]