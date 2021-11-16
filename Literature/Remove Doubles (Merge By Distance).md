# Remove Doubles (Merge By Distance)
Criado: 16/11/2021 - 19:02

tags: #modelling 

---

Remove doubles é uma técnica para remoção vértices que tenham sido criados muito proximos durante o processo de [[Modelagem]].

Esse tipo de vertice duplicado pode aparecer durante a aplicação de alguns processos de subdivisão dos #modify_modifiers, sendo bastante importante que sejam corrigido para que não ocorram glitches durante uma possível animação ou aplicação de [[Material]].

Para usar, abre o [[Edit Mode]], aperte M e selecione "Merge By Distance"
![[Merge By Distance.png]]
Controle a distancia que deseja que os vértices se juntem. Cuidado ao alterar esse valor para que o objeto em si não fique distrocido

![[Remove Doubles Demo.png]]

Esquerda: original | Meio: 0.0601m | Direita: 0.14m

O processo é um pouco parecido com o [[Decimate Modifier]], mas as mudanças feitas pelo Remove Doubles são permanentes após a operação ser finalizada.

---
## Referências
1.