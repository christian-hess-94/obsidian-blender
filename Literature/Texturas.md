# Texturas
Criado: 16/11/2021 - 19:01

tags: #texturing #wip 

---

Texturas são imagens que podem ser aplicadas em um [[Material]] para configurar as diversas caracteristicas que o objeto pode ter.

Em geral são consideradas as seguintes:
- Color: Essa textura representa a cor da superficie do objeto
	- Albedo: Essa textura também possui as cores porém remove as sombras que possam existir afim de dar um resultado mais específico.
	- ![[Pasted image 20211116193232.png]]
- [[Normal Map]] ou Bump Map: Essa textura indica imperfeições na superficie do objeto, e faz com que sombras sejam renderizadas de acordo com a direção da luz, sem a necessidade de aumentar a complexidade da geometria
- Specular Map: Esta textura preto e branco indica o quão refletiva e brilhosa é a superficie. Interaje com a luz ambiente da cena e a reflete de acordo com os valores presentes na imagem
- Roughness Map: Tambem chamado de "rugosidade", indica o quao detalhado é o reflexo da luz (um espelho fosco vs um espelho comum)
- ![[Roughness Map.png]]
- Metalness: Um tipo de mapa especial que indica quais parte da superficie devem ser consideradas metálicas, alterando a forma como refletem a luz
- [[Ambient Occlusion]]: Normalmente gerado a partir do processo de [[Texture Baking]], 

---
## Referências
1. https://help.poliigon.com/en/articles/1712652-what-are-the-different-texture-maps-for
2. https://pt.wikipedia.org/wiki/Normal_map
3. http://wedesignvirtual.com/what-does-a-specular-map-do/#:~:text=Specular%20maps%20are%20black%20and,realism%20of%20the%20object's%20texture.