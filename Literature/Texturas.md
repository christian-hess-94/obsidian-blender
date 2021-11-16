# Texturas
Criado: 16/11/2021 - 19:01

tags: #texturing 

---

Texturas são imagens que podem ser aplicadas em um [[Material]] para configurar as diversas caracteristicas que o objeto pode ter.

Em geral são consideradas as seguintes:
- Color: Essa textura representa a cor da superficie do objeto
	- Albedo: Essa textura também possui as cores porém remove as sombras que possam existir afim de dar um resultado mais específico.
	- ![[Color Map.png]]
- [[Normal Map]] ou Bump Map: Essa textura indica imperfeições na superficie do objeto, e faz com que sombras sejam renderizadas de acordo com a direção da luz, sem a necessidade de aumentar a complexidade da geometria
	- ![[Normal Map.png]]
- Specular Map: Esta textura preto e branco indica o quão refletiva e brilhosa é a superficie. Basicamente indica se a superficie pode ou não refletir algo e com que intensidade.
	- ![[Specular Map.png]]
- Roughness Map: Tambem chamado de "rugosidade", indica o quao detalhado é o reflexo da luz (um espelho fosco vs um espelho comum)
	- ![[Roughness Map.png]]
- Metalness: Um tipo de mapa especial que indica quais parte da superficie devem ser consideradas metálicas, alterando a forma como refletem a luz
	- ![[Metalness Map.png]]
- [[Ambient Occlusion]]: Normalmente gerado a partir do processo de [[Texture Baking]], adiciona sombras em locais de proximidade na geometria, dando uma maior sensação de profundidade
- Emission: indica quais parte da geometria emitem luz que afeta outros objetos na cena
	- ![[Emission Map.png]]

---
## Referências
1. https://help.poliigon.com/en/articles/1712652-what-are-the-different-texture-maps-for
2. https://pt.wikipedia.org/wiki/Normal_map
3. http://wedesignvirtual.com/what-does-a-specular-map-do/#:~:text=Specular%20maps%20are%20black%20and,realism%20of%20the%20object's%20texture.