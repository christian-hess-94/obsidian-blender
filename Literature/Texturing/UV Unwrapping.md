# UV Unwrapping
Criado: 15/11/2021 - 15:40

tags: #texturing  

---

UV Unwrapping é um processo executado em cima de um objeto 3D que cria um [[UV Map]] vazio.

O processo pode ser feito manualmente pelo artista, selecionando trechos do objeto 3D e fazendo o Unwrap de cada parte, mas também pode ser feito de forma automatizada podendo ser alterado diretamente com a criação de [[Seams]].

![[UV Mapping Algorithms.png]]

- **Smart UV** é um processo que faz o unwrap completo da imagem e automaticamente cria o [[UV Map]] correpondente. Isso facilita o processo de [[Texture Paint]] que necessita de um [[UV Map]] associado ao objeto.
- **Cube Projection** realiza um Smart UV porém transforma todas as ilhas em formas quadráticas afim de organizar o [[UV Map]] gerado
- **Project From View** gera uma ilha no [[UV Map]] nas exatas dimensões em que o objeto está sendo visto pela camera no ambiente 3D

---
## Referências
1.