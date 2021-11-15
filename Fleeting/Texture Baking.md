Baking de um normal map:



Para aplicar o normal map gerado:

- Salve o map como um arquivo de imagem (ALT + S) no UV Editor
- Abra o workspace Shading com o modelo LOW POLY selecionado
- Conecte a Image texture com o normal mapa em um node "Normal Map" e conecte esse node no campo normal to BSDF
- Ative a visão Rendered e modidifuque o material para ser mais Metallic e ter menos Roughness para ver o efeito do Normal map criado

O mesmo processo vale para criar outros tipos de mapa, basta mudar o bake type de “Normal” para “Diffuse”, “Specular”, etc.

