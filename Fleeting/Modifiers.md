# Modify
- Data Transfer: Serve para transferir dados de uma mesh para outra, coisas como posição e direção dos vetores normais
- Mesh Cache: Permite associar animações externas aos objetos. Um dos tipos possíveis é MDD
- Mesh Sequence: Faz a mesma coisa que o Mesh Cache mas usando arquivos.alembic
- Normal Edit: Permite alterar a direção das normais de um objeto a partir de outro objeto. **Pode servir para direcionar as normais de um sistema de particulas para a camêra fazendo com que cada particula fique mais visível**
- Wighted Normal: Faz uma interpolação dos vetores normais do vértices para que apontem na direção dos vetores normais das faces que compõem. Pode aumentar a fidelidade gráfica de um objeto sem precisar aumentar a taxa de vértices.
- UV Project: Permite utilizar um objeto como um “projetor” que projeta a textura em cima do UV Map do objeto com o modificador.
- UV Warp: Permite usar objetos externos para alterar a projeção da textura no mapa UV do objeto com o modificador
- Vertex Weight Edit: Permite realizar alterações ao weight painting feito em uma mesh. Permite alterar coisas como Default Weight e modificar o weight painting ativo de maneira procedural
- Vertex Weight Mix: Permite realizar um mix dos weight paintings de diferentes Vertex Groups. Oferece a opção de realizar diversas operações como Add, Subtract, Difference, dentre outros.
- Vertex Weight Proximity: Permite a criação de Vertex Groups e Weight Paintings dinâmicos. Associa um objeto ao modificador que cria um vertex group a partir da localização do objeto. Outros parâmetros podem ser mexidos para ajustar o tamanho e intensidade do Weight Paint que é originado.
  - Pode fazer um efeito de fade com ajude de um Wireframe Modifier (explicado abaixo)

# Generate
- Array: Permite criar cópias do objeto. Trabalha com três tipos de offset:
  - Constant: A distância entre a origem de cada cópia é sempre a mesma
  - Relative: Utiliza o tamanho em X Y Z para calcular a distância entre as cópias
  - Object: Permite utilizar outro objeto para determinar a distância, direção e escala entre as cópias
  - Permite usar opções para controlar o tamanho do array de acordo com o tamanho do objeto ou uma curve
  - É possível dar um merge em vértices próximos ao ativar a opção merge
- Bevel: Criar bevel, ou perfis, nas arestas da mesh. Permite que opção como suavização, número de segmentos grupo de vértices sejam modificadas
- Boolean: Permite criar interação entre duas meshes.
  - ` `A mesh primária possui o modificador que deve ser configurado com uma mesh secundária
  - Aplica um cálculo de Addition, Intersect e Differencenas áreas onde ambas as meshes se tocam
  - Addition: A mesh resultante é a soma das áreas ocupadas pelas meshes na operação
  - Intersect: A mesh resultante é composta pelas áreas comuns a ambas as meshes.
  - Difference: A mesh secundária serve como uma “faca” e cortar uma parte da mesh primária
- Build: Criar uma “animação” em que a mesh é construída face a face, dando um efeito em que ela aparece aos poucos.
- Decimate: Serve para realizar uma operação de simplificação na mesh, diminuindo a quantia de vértices que a compõem.
- Split Edge: Especifica um ângulo para fazer um recorte de arestas, podem assim separar as faces. No caso de um cubo, ao se especificar o ângulo 90 graus,  todas as faces são separadas por estarem 90 graus umas das outras
- Mask: Permite especificar um Vertex Group como uma mascara, escondendo todos os vertices do grupo
- Mirror: Espelha as modificações feitas de um lado da mesh para outro
  - Pode fazer espelhamento em qualquer um dos eixos (X,Y e Z)
  - O espelhamento é feito em relação a origem do mesh
  - Os eixos usados são os eixos locais
- Multiresolution: Permite subdividir a mesh com mais parâmetros que o Subdivision modifier
- Remesh: Muda a topologia do objeto para um dos três tipo. A modificação tenta preservar o formato do objeto o maximo possível. A topologia anterior é totalmente perdida ao aplicar este modifier
- Screw: Permite pegar um objeto e criar cópias rotacionadas e incrementais afim de criar algo semelhante a uma mola ou a rosca de um parafuso (screw).
  - Para criar uma mola, basta aplicar o Screw modifier em um Circle com um offset positivo
- Skin: Criar geometria em volta de vértices e arestas. É util para criar uma “gordura” em cima de vertices e arestas individuais. Quando aplicado em uma mesh como faces, as faces anteriores são deletadas para criar a nova geometria
  - Pode ser util para criar coisas como arvores low-poly. Basta arrastar vertices e arestras e aplicar um skin modifier a eles
- Solidify: Aumenta grossura de um objeto 2D. Facilita o trabalho de criação pois permite manipular o objeto 2D original e o Solidify Modifier cuida de criar o aspecto 3D do objeto final
- Subdivision Surface: Duplica e subdividide a quantia de vertices, arestas e faces, fazendo com que o modelo tenha mais topologia e mais detalhes. Tende a suavizar as bordas, fazendo com que detalhes mais angulares sejam perdidos
- Triangular: Transform todas as faces em faces triangulares. Ideal para jogos
- Wireframe: PArecido com o Skin, permite criar um novo “esqueleto” em volta dos vertices, arestas e faces. Parmaetros como grossura desse novo esqueleto e resolução também estão presentes
- Weld: Realiza a operação Merge By Distance (Remove Doubles) na mesh inteira, juntando vertices que estejam muito próximos a partir de um valor especificado no modifier.

# Deform

