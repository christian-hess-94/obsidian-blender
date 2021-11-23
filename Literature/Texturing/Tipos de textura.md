# Tipos de textura
Criado: 16/11/2021 - 19:05
links: [[Texturas]]
tags: #wip 

---

Em geral são consideradas as seguintes:
- **[[Color]]**: Essa textura representa a cor da superficie do objeto
	- **[[Albedo]]**: Essa textura também possui as cores porém remove as sombras que possam existir afim de dar um resultado mais específico.
	- ![[Color Map.png]]
- **[[Normal Map]]** ou Bump Map: Essa textura indica imperfeições na superficie do objeto, e faz com que sombras sejam renderizadas de acordo com a direção da luz, sem a necessidade de aumentar a complexidade da geometria
	- ![[Normal Map.png]]
- **[[Specular Map]]**: Esta textura preto e branco indica o quão refletiva e brilhosa é a superficie. Basicamente indica se a superficie pode ou não refletir algo e com que intensidade.
	- ![[Specular Map.png]]
- **[[Roughness Map]]**: Tambem chamado de "rugosidade", indica o quao detalhado é o reflexo da luz (um espelho fosco vs um espelho comum)
	- ![[Roughness Map.png]]
- **[[Metalness Map]]**: Um tipo de mapa especial que indica quais parte da superficie devem ser consideradas metálicas, alterando a forma como refletem a luz
	- ![[Metalness Map.png]]
- **[[Ambient Occlusion Map]]**: Normalmente gerado a partir do processo de [[Texture Baking]], adiciona sombras em locais de proximidade na geometria, dando uma maior sensação de profundidade
- **[[Emission Map]]**: indica quais parte da geometria emitem luz que afeta outros objetos na cena
	- ![[Emission Map.png]]

---
## Referências
1.