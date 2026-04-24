# Empilha Smurfs

## {Introduction @unplugged}

Tem alguma coisa muito smurfante acontecendo por aqui!

<img src="https://arcade.makecode.com/static/tutorials/stackem-smurfs/stackem-smurfs.gif" alt="Crie um jogo estrelado pelos Smurfs"/>

Neste tutorial, você vai criar seu próprio jogo de arcade em estilo retrô, inspirado no universo dos Smurfs.

## Step 1: Primeiro Smurf
### Vamos começar colocando um Smurf no chão para iniciar o jogo.

- :gear: Abra a categoria ``||Smurfy:Smurfy||`` na caixa de ferramentas e pegue o bloco ``||Smurfy:set first Smurf||``.
- :mouse pointer: Encaixe esse bloco dentro do ``||loops:on start||`` que já está na área de trabalho.

> Você pode clicar na imagem do Smurf para escolher outro personagem, se quiser.

## Step 2: Testando o projeto
### Agora vamos ver o que já apareceu no jogo.

- :binoculars: Olhe para a janela do jogo para ver o que o seu código fez.
- :mouse pointer: Você deve ver um Smurf parado no chão.

## Step 3: Cor de fundo
### Está um pouco escuro. Vamos adicionar um pouco de cor!

- :tree: Abra a categoria ``||scene:Scene||`` e pegue o bloco ``||scene:set background color to ()||``.
- :mouse pointer: Coloque esse bloco dentro do ``||loops:on start||``.

> Você pode clicar no círculo de cor do bloco para escolher outra cor de fundo, se quiser.

```blocks
Smurfy.setFirstSmurf()
 //@highlight
scene.setBackgroundColor(8)
```

## Step 4: Mais um Smurf
### Agora precisamos de outro Smurf para empilhar.

- :tree: Na categoria ``||Smurfy:Smurfy||``, arraste o bloco ``||Smurfy:new floating Smurf||``.
- :mouse pointer: Encaixe esse bloco no final do ``||loops:on start||``.

#### Por que no final?
O código dentro do ``||loops:on start||`` roda de cima para baixo.  
Como o Smurf que está caindo precisa de outro Smurf para pousar, precisamos colocar esse bloco **depois** do bloco onde definimos o primeiro Smurf.

```blocks
Smurfy.setFirstSmurf()
scene.setBackgroundColor(8)
//@highlight
Smurfy.newFloatingSmurf()
```