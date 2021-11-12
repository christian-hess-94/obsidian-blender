Material:

- Nome de algo que dá cor, textura a uma mesh
- Os materiais são aplicados nas faces de uma mesh
- Materiais podem ser de vários tipos
  - Imagem, Vídeo ou Geradas
- Materiais do tipo Imagem pegam informações de cor e textura de um arquivo externo 
  - jpg, png, por exemplo
- Materiais do tipo vídeo mostram um vídeo na superfície onde são aplicados
- Materiais gerados usam o sistemas de nodes para criar cores e texturas

Pintando com Texture Paint:

- Texture paint permite que a textura da mesh possa ser pintada digitalmente
- As informações de cores feitas pela pintura são salvas em uma imagem
  - Textura pintada sempre é aplicada a um material do tipo Imagem
- A mesh precisa ser mapeada no arquivo de imagem (UV Unwrap)

**Como fazer:**

- Certificar que o objeto foi UV Unwrapped 
  - Usar SMART UV UNWRAP para um quickstart
- Abrir workspace de texture paint (Image Editor / 3D viewport + Texture Paint)
- Selecionar objeto a ser pintado
- No Image Editor (esquerda) clicar em "New +" para criar uma nova imagem vazia.
  - Especifique a resolução e o nome
  - Essa imagem irá receber a textura pintada usando o UV Unwrap do objeto
- Abra o painel de Materials
- Associe um novo material ao objeto
- Na opção Base Color, clicar na bolinha do lado da cor e escolha Image Texture
- No dropdown, escolha a imagem gerada nos passos anteriores

Propriedades de Materials: 

- Volume: Afeta como a luz interage com o volume do objeto
- Volume Absorption: Usado para aumentar refratação causada pelo volume do objeto 
  - Aparência de água turva, café, etc

Aplicando múltiplos materiais:

- Crie todos os materiais na aba de materiais usando o + ou o botão de duplicar
- Abra o objeto em modo de edição
- Seleciona as faces que vão usar determinado material
- Com as faces selecionadas, selecione o material a ser aplicado
- Clicar no botão "ASSIGN" logo abaixo
- Certifique de estar no moto "Material Preview" ou "Rendered" para ver 
  - Se o material for modificado, as mudanças afetarão todos as meshes e seções de meshes com o material aplicado

