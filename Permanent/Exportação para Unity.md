# Exportação para Unity
Criado: 15/11/2021 - 14:41
links: [[FBX]] - [[Modelagem]] - [[Exportação]]
tags: #done 

---

Crie o objeto a ser importado dentro do Blender

1. Salve o objeto como arquivo .blend
   1. Use o arquivo .blend dentro do projeto da Unity para prototipar coisas simples como tamanho do objeto em relação ao resto do jogo
1. Caso o objeto tenha múltiplas animações crie-as como Actions:
   1. Abra o workspace de Animation
   1. Troque o modo da DopeSheet para Actions Editor
   1. Crie os keyframes da primeira animação
   1. 4 Após feito isso, renomeie o nome da animação no topo do Actions Editor
   1. 5 Clique no símbolo de Escudo chamado "Fake User" do lado do nome
   1. 6 Crie uma nova animação ao duplicar a animação anterior
      1. Resete a animação caso necessário
      1. Abra a armature da animação no Pose Mode
      1. Selecione todos os bones com A
      1. Clique com botão direito em qualquer bone e selecione "Revert user transforms"
   1. Crie novas animações conforme necessário

#### Exportando objeto para ser usado na Unity:

1. A Unity recomenda o uso de objeto no formato [[FBX]]
   1. Arquivos [[FBX]] são compactadores. Eles compactam texturas, materiais, animações e meshes em um só arquivo
   1. Usar [[FBX]] permite que todas as animações e textures sejam automaticamente associadas ao objeto ao ser adicionado na Unity
1. Selecione o Objeto e a Armature de animação, se houver
1. Vá em File -> Export e selecione a opção [[FBX]]
   1. Do lado direito na opções de exportação:
   1. Path Mode: Copy
   1. Habilite o botão ao lado do Path Mode: EmbedTextures
   1. Habilite Selected Objects
1. Exporte o objeto [[FBX]] para dentro do seu projeto Unity

#### Configurando o objeto dentro da Unity

1. Arraste o arquivo [[FBX]] para dentro da Scene
   1. O arquivo [[FBX]] é tratado como um Prefab, quaisuqer configurações devem ser feitas direto no arquivo através da interface da Unity
1. Expanda o arquivo [[FBX]] e certifique que os objetos, animações e materials estão todos empacotados corretamente 
1. Caso os materiais estejam vazios, veja o proximo passo
   1. No [[FBX]] abra a opção "Materials"
   1. Clique no botão Extract Textures
   1. Aparecerão cópias das imagens usadas nas texturas do objeto e as texturas serão corrigidas
1. Na aba Animations do [[FBX]], verifique que todas as animações foram importadas corretamente (preview no final do Inspector)
   1. Caso a animação deva ficar em loop, selecione-a na lista e habilite "Loop Time"

#### Configurando animações para funcionar com o Animator da Unity:

1. Expanda o [[FBX]]
1. Segure e arreste alguma animação (de preferencia a animação inicial) para o objeto na Scene
1. Um novo arquivo do tipo Animator será criado com o mesmo nome do objeto na Scene
1. Abra a visão do Animator e use o sistema de animações normalmente
1. Para adicionar as demais animações, se houverem:
   1. Arraste os arquivos de animação de dentro do [[FBX]] para a janela do Animator
   1. Crie transições conforme necessário
1. Caso alguma animação configurada como Loop (seção anterior - 1) esteja loopando antes de finalizar
   1. Selecione a transição que leva à animação dentro do Animator
   1. Desablite a opção "Can Transition to self"

---
## Referências
1.



