# Anotações sobre CSS Flexbox
Flexbo vem pra resolver o problema de alinhamento dos componentes de um layout de um modo nativo e responsivo.

### Flex Container
É a tag que envolve os itens. Pode ser aplicada a qualquer tag do HTML que enha itens filhos.

* **display: flex**: é a propriedade inicializadora do sistema flexbox e atribuída ao container;
* **flex-direction**: indica se a direção dos itens filhos do container que pode ser linha (row) ou coluna (column);
* **flex-wrap**: indica se que haverá quebra de linha;
* **flex-flow**: é um atalho para as propriedades **flex-direction** e **flex-wrap**;
* **justify-content**: alinha os itens filhos do container conforme a sua direção;
* **align-items**: alinha os itens de acordo com o eixo do container;
* **align-content**: define o alinhamentos das linhas do container;

### Flex Item
Os itens de um container flex também podem ser um flex container, envolvendo seus itens filhos, que por sua vez, _podem ser_ flex containers _também_ e assim por diante.

De qualquer forma, os itens de um **flex container** possuem propriedades específicas que definem seu posicionamento:

* **flex-grow**: fator de crescimento, aumentando o tamanho dos itens progressivamente ao longo da distribuição no espaço disponível no container;
* **flex-basis**: define o fator inicial antes da distribuição do item no espaço disponível;
* **flex-shrink**: define a capacidade de redução;
* **flex**: trata-se de um atalho para as 3 propriedades acima;
* **order**: ordem de distribuição;
* **align-self**: alinhamento de um item específico;

#### Dicas
1. Quando o item contém um valor definido para flex-grow, o align-basis não terá efeito.

Para esse curso foi utilizado:
* VSCODE
    * [Live HTML Previewer](https://marketplace.visualstudio.com/items?itemName=hdg.live-html-previewer)
    * [HTML Snippets](https://marketplace.visualstudio.com/items?itemName=abusaidm.html-snippets)

