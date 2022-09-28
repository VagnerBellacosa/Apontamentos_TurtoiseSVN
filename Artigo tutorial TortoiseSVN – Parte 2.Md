# Enviando arquivos para o repositório - Artigo tutorial TortoiseSVN – Parte 2

## Neste pequeno tutorial irei comentar sobre a utilidade de uma ferramenta usada para compartilhamento arquivos, que no exemplo em questão se trata de códigos fontes de um determinado projeto. Irei de forma simples demonstrar a instalação utilização e configuração do TortoiseSVN, que poderá ser usado para compartilhamento em simples rede de computadores ou até mesmo pela web.



<iframe class="ad-medium" src="https://www.devmedia.com.br/marketing/banners/banner_160x600/" frameborder="0" style="outline: none; -webkit-tap-highlight-color: transparent; max-width: 100%; margin: auto; display: block; height: 600px;"></iframe>

Suporte ao alunoAnotarMarcar como concluído

[Artigos](https://www.devmedia.com.br/artigos/)[Engenharia de Software](https://www.devmedia.com.br/artigos/engenharia-de-software)Enviando arquivos para o repositório - Artigo tutorial TortoiseSVN – Parte 2

No [artigo anterior](http://www.devmedia.com.br/criando-repositorio-e-pasta-de-trabalho-artigo-tutorial-tortoisesvn-parte-1/20979) nos criamos a pasta de repositório e criamos também uma pasta onde nos vamos trabalhar os códigos. Neste artigo vou demonstrar como adicionarmos os projetos criados em nosso micro neste repositório, para que o mesmo fique disponível para todos os outros que porventura venham precisar acessar este projeto.

Primeiramente vamos entender os ícones exibidos pelo tortoiseSVN.



| ![img](https://www.devmedia.com.br/imagens/articles/230527/Tortoise01.jpg) | Quando a pasta local é apresentada desta forma indicada acima, o tortoiseSVN esta indicando a pasta esta atualizada. |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://www.devmedia.com.br/imagens/articles/230527/Tortoise02.jpg) | Quando exibido da forma acima, indica que a pasta do repositório esta com arquivos mais recentes do que a da pasta de trabalho. |
| ![img](https://www.devmedia.com.br/imagens/articles/230527/Tortoise03.jpg) | O ícone ficará desta forma, quando o arquivo local da pasta de trabalho, estiver marcado para ser enviar para o repositório. |
| ![img](https://www.devmedia.com.br/imagens/articles/230527/Tortoise04.jpg) | Indica que o arquivo esta em conflito.                       |



Sabendo disso, agora vamos adicionar um projeto criado ou criar um novo projeto para enviarmos para o repositório. Neste exemplo vou criar um pequeno projeto em delphi apenas para ter os arquivos que iremos usar.

Depois de adicionado os arquivos na pasta, os mesmos ainda não foram para o repositório e não farão diferença alguma nos respectivos ícones. Então agora vamos selecionar todos que desejamos enviar para o repositório e clicar com o botão direito do mouse sobre eles e na sequencia selecionamos a opção “TortoiseSVN->Adicionar”.

![img](https://www.devmedia.com.br/imagens/articles/230527/Tortoise05.jpg)

Observe que ao clicar nesta opção, nos ícones selecionados irá aparecer o sinal de positivo em azul, indicando que na próxima vez que submetermos a atualização, estes irão para o repositório. E é o que faremos na sequencia.

![img](https://www.devmedia.com.br/imagens/articles/230527/Tortoise06.jpg)

Retroceda na raiz da pasta, onde foram adicionados os arquivos do projeto “D:\programa”, e selecione a clicando com o botão direito do mouse sobre a pasta “Meus_Codigos”, a opção “SVN Submeter”.

![img](https://www.devmedia.com.br/imagens/articles/230527/Tortoise07.jpg)

Será exibida a seguinte janela, indicando as alterações que estão pendentes.

![img](https://www.devmedia.com.br/imagens/articles/230527/Tortoise08.jpg)

Confirmado todas as alterações, basta clicar em ok e aguardar o termino do processamento.

![img](https://www.devmedia.com.br/imagens/articles/230527/Tortoise09.jpg)

Com isso concluímos o envio do projeto para o repositório e o mesmo estará disponível para todos os outros que necessitarem acessar o mesmo e que possuírem o acesso. E todas as atualizações que forem disponibilizadas por você, bastará realizar a atualização através do próprio tortoiseSVN, que estas ficarão a disposição de todos.

Devo apenas reforçar que toda e qualquer alteração nos arquivo, inclusive uma possível renomeação do mesmo, deverá ser realizada através do TortoiseSVN, evitando assim problemas.

Na [próxima parte do artigo](http://www.devmedia.com.br/funcionalidades-artigo-tutorial-tortoisesvn-parte-3/21074), vamos conhecer com maiores detalhes, as opções disponibilizadas pelo aplicativo para realização de diferentes tarefas.

AnotarMarcar como concluído

#### Confira outros conteúdos: