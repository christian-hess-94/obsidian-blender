- Texture Baking é o ato de salvar as informações de uma textura aplicada a uma mesh em um arquivo
  - Permite que a textura possa ser facilmente usada em outros locais e melhora a performance.
- O Baking funciona com qualquer tipo de textura (Diffuse, Normal, Specular, etc)
- Necessita que a mesh esteja UV Unwrappdr para traduzir as informações da textura a um arquivo de imagem
- Muito útil quando se tem um modelo High poly com muitos detalhes e deseja-se transferir os detalhes para um modelo low-poly através de um Normal Map

Baking de um normal map:

- Para fazer o baking deve-se primeiro criar o modelo low-poly.
- Crie uma cópia do modelo low-poly e adicione detalhes com ajuda de brushes no modo sculpting
  - Tenha cuidado para não mover os modelos de lugar. Faça com que ambos fiquem exatamente no mesmo local para facilitar o processo de baking no futuro.
  - Certifique-se também dos pontos de origem de ambos.
  - Use o modo Dyntopo (Dynamic Topology) para adicionar novos vertices ao inves de apenas altearar os ja presentes
- **Após adicionados os detalhes, pode-se iniciar o processo de baking**
- Garanta que os objetos estão intercalados na mesma posição
- Certifique de estar no Cycles
- Abra o workspace UV Editing
- Caso haja alguma imagem aberta, remova-a e crie uma nova imagem 
- Selecione o objeto LOW POLY e aplique um material a ele
- Modifique a opção Color para ser uma Image Texture
- Selecione a imagem recém-criada e aplique-a como textura do objeto
- Aproveite para se certificar que o UV Map da mesh esta inteiro dentro da área designada no UV Editor
  - Caso não tenha sido feito o UV Map, utilize o SMART UV UNWRAP
- Após feito isso, abra a aba Render Properties.
- Procure o sub-conjunto "bake"
- Modifique Bake type para "normal"
- Deixe as demais opções como padrão e ative "Selected to Active"
  - Ative essa opção sempre que for passar detalhes de um high-poly para um low-poly
- Em seguide, selecione na seguinte ordem:
- `    `PRIMEIRO a HIGH POLY 
- `    `DEPOIS selecione a LOW POLY
  - A configuração "SELECTED TO ACTIVE" pega os detalhes de todos os objetos "SELECIONADO"
- e os transfere para o objeto "ATIVO". O Objeto ATIVO sempre é o ultimo objeto selecionado.
  - Basicamente, sempre selecione o objeto que for receber os detalhes por último para que ele seja o objeto ATIVO
- Clique em bake e espere para ver o resultado.
- Caso a mesh possua muitos espaços "verdes" ou "mostarda" o bake não foi bem sucedido
- Expanda a caixa do SELECT TO ACTIVE e incremente a opção "Ray Distance" e tente novamente
  - Aumente e diminua essa opção até obter um resultado satisfatório (totalmente roxo com vermelho e azul)

Para aplicar o normal map gerado:

- Salve o map como um arquivo de imagem (ALT + S) no UV Editor
- Abra o workspace Shading com o modelo LOW POLY selecionado
- Conecte a Image texture com o normal mapa em um node "Normal Map" e conecte esse node no campo normal to BSDF
- Ative a visão Rendered e modidifuque o material para ser mais Metallic e ter menos Roughness para ver o efeito do Normal map criado

O mesmo processo vale para criar outros tipos de mapa, basta mudar o bake type de “Normal” para “Diffuse”, “Specular”, etc.

