# Generate Modifiers - MOC
Criado: 14/11/2021 - 15:18

tags: 

---

- [[Array Modifier]]: Permite criar cópias do objeto. Trabalha com três tipos de offset:
  - Constant: A distância entre a origem de cada cópia é sempre a mesma
  - Relative: Utiliza o tamanho em X Y Z para calcular a distância entre as cópias
  - Object: Permite utilizar outro objeto para determinar a distância, direção e escala entre as cópias
  - Permite usar opções para controlar o tamanho do array de acordo com o tamanho do objeto ou uma curve
  - É possível dar um merge em vértices próximos ao ativar a opção merge
- [[Bevel Modifier]]: Criar bevel, ou perfis, nas arestas da mesh. Permite que opção como suavização, número de segmentos grupo de vértices sejam modificadas
- [[Boolean Modifier]]: Permite criar interação entre duas meshes.
  - A mesh primária possui o modificador que deve ser configurado com uma mesh secundária
  - Aplica um cálculo de Addition, Intersect e Differencenas áreas onde ambas as meshes se tocam
  - Addition: A mesh resultante é a soma das áreas ocupadas pelas meshes na operação
  - Intersect: A mesh resultante é composta pelas áreas comuns a ambas as meshes.
  - Difference: A mesh secundária serve como uma “faca” e cortar uma parte da mesh primária
- [[Build Modifier]]: Criar uma “animação” em que a mesh é construída face a face, dando um efeito em que ela aparece aos poucos.
- [[Decimate Modifier]]: Serve para realizar uma operação de simplificação na mesh, diminuindo a quantia de vértices que a compõem.
- [[Split Edge Modifier]]: Especifica um ângulo para fazer um recorte de arestas, podem assim separar as faces. No caso de um cubo, ao se especificar o ângulo 90 graus,  todas as faces são separadas por estarem 90 graus umas das outras
- [[Mask Modifier]]: Permite especificar um Vertex Group como uma mascara, escondendo todos os vertices do grupo
- [[Mirror Modifier]]: Espelha as modificações feitas de um lado da mesh para outro
  - Pode fazer espelhamento em qualquer um dos eixos (X,Y e Z)
  - O espelhamento é feito em relação a origem do mesh
  - Os eixos usados são os eixos locais
- [[Multiresolution Modifier]]: Permite subdividir a mesh com mais parâmetros que o Subdivision modifier
- [[Remesh Modifier]]: Muda a topologia do objeto para um dos três tipo. A modificação tenta preservar o formato do objeto o maximo possível. A topologia anterior é totalmente perdida ao aplicar este modifier
- [[Screw Modifier]]: Permite pegar um objeto e criar cópias rotacionadas e incrementais afim de criar algo semelhante a uma mola ou a rosca de um parafuso (screw).
  - Para criar uma mola, basta aplicar o Screw modifier em um Circle com um offset positivo
- [[Skin Modifier]]: Criar geometria em volta de vértices e arestas. É util para criar uma “gordura” em cima de vertices e arestas individuais. Quando aplicado em uma mesh como faces, as faces anteriores são deletadas para criar a nova geometria
  - Pode ser util para criar coisas como arvores low-poly. Basta arrastar vertices e arestras e aplicar um skin modifier a eles
- [[Solidify Modifier]]: Aumenta grossura de um objeto 2D. Facilita o trabalho de criação pois permite manipular o objeto 2D original e o Solidify Modifier cuida de criar o aspecto 3D do objeto final
- [[Subdivision Surface Modifier]]: Duplica e subdividide a quantia de vertices, arestas e faces, fazendo com que o modelo tenha mais topologia e mais detalhes. Tende a suavizar as bordas, fazendo com que detalhes mais angulares sejam perdidos
- [[Triangulate Modifier]]: Transform todas as faces em faces triangulares. Ideal para jogos
- [[Wireframe Modifier]]: PArecido com o Skin, permite criar um novo “esqueleto” em volta dos vertices, arestas e faces. Parmaetros como grossura desse novo esqueleto e resolução também estão presentes
- [[Weld Modifier]]: Realiza a operação Merge By Distance (Remove Doubles) na mesh inteira, juntando vertices que estejam muito próximos a partir de um valor especificado no modifier.

---
## Referências
1.