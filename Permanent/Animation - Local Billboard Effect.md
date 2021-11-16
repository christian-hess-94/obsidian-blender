# Animation - Local Billboard effect
Criado: 16/11/2021 - 18:23

tags: #animation 

---

Como criar um Billboard effect controlada pela camera usando o [[UV Project Modifier]]

- Adicione um plano ou qualquer outra geometria e a posicione na camera da forma que deseja
	- ![[Pasted image 20211116182854.png]]
- Crie um [[Material]] para a geometria, pode ser de qualquer tipo
- Ative o [[Node Wrangler]]
- Na aba de Shading, adicione nodes para usar o [[UV Map]] na renderização da textura no objeto
	- ![[Pasted image 20211116182817.png]]
- Adicione o [[UV Project Modifier]] no objeto
	- Selecione UV Map
	- Selecione a Camera como projetor
- A camera vai controlar os parametros de Transform do UV Map, assim a texutra sempre aponta na direção da camera
![[0001-0030.mp4]]


---
## Referências
1.