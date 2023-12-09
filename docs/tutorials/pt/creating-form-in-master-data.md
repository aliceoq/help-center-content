---
title: 'Criar formulário no Master Data'
id: tutorials_1047
status: PUBLISHED
createdAt: 2017-04-27T21:57:35.614Z
updatedAt: 2023-12-08T18:36:08.521Z
publishedAt: 2023-12-08T18:36:08.521Z
firstPublishedAt: 2017-04-27T23:03:43.083Z
contentType: tutorial
productTeam: Master Data
author: authors_3
slug: criando-formulario-no-master-data
locale: pt
legacySlug: criando-formulario-no-master-data
subcategory: WpbGhubuRZaNZilJSXnqu
---

Um formulário serve como interface para visualização e manipulação de uma entidade de dados. Em essência, ele atua como um agrupador de campos. Embora esteja sempre associado a uma entidade, não é obrigatório que contenha todos os campos relacionados a ela, podendo ser personalizado conforme a demanda. Dessa forma, é possível criar diferentes formulários para uma mesma entidade, adaptando-se às distintas necessidades. Por exemplo, um formulário de compra pode incluir campos como ID, cliente e data.

Para criar um formulário, siga os passos abaixo:

1. No Admin VTEX, acesse **Configurações da loja** > **Storefront** > **Master Data**.
2. Clique na aba **Aplicações**.
3. Na aplicação em que deseja criar o formulário, clique no símbolo de engrenagem.
4. Na listagem de formulários, clique no botão `Novo`.
5. Preencha os campos descritos na seção [Campos do formulário](#campos-do-formulario).
6. Clique no botão `Salvar`.

## Campos do novo formulário

- **Nome:** Nome do formulário.
- **Filtros:** Campos marcados como filtro da entidade, esses campos formarão os filtros laterais do formulário. Deve ser inserido o nome interno do campo. Para mais de um campo, separe-os por vírgulas. Exemplo: campo1,campo2.
- **Entidade de Dados:** A entidade de dados para a qual o formulário vai salvar e exibir os dados. 
- **Destaques de busca:** Os campos que serão listados nos resultados de busca. Deve ser inserido o nome interno do campo. Para mais de um campo, separe-os por vírgulas. Exemplo: para buscar por cliente e fazer com que na listagem de resultado apareça o CPF do cliente e o nome, é necessário preencher o campo com CPF e nome.
- **Consultas na visualização:** Habilita uma nova seção no formulário de exibição, com registros de uma entidade relacionada à entidade do formulário. As informações exibidas serão relacionadas ao registro que está sendo visualizado.

   Por exemplo, na entidade __Atendimento__, existe um campo relacionado com a entidade __Cliente__. Então, no formulário __Cliente__, no campo __Consultas__ na visualização, insira este campo de atendimento que faz referência à entidade __Cliente__. Se a sigla da entidade __Atendimento__ for __AT__ e o nome do campo for __Cliente__, deve ser inserido `AT.Cliente` para carregar os atendimentos do cliente que está sendo visualizado no formulário. ![registrosRelacionados2](//images.contentful.com/alneenqid6w5/2NrlYdzzR66Og4waCIekGe/e4d47ef3e257c749c09c0c9151383c45/registrosRelacionados2.png) ![registrosRelacionados](//images.contentful.com/alneenqid6w5/3j6iBpbL7ao6soYaME4e2a/d80177bdf01586c97f1321c74c881ac3/registrosRelacionados-1.png)

Após preencher os campos obrigatórios, aparecerão as abas disponíveis para configuração. Seguem abaixo os campos para cada uma delas.

- **Campos da Listagem:** Aqui, devem ser selecionados os campos que aparecerão na listagem de registros, ao clicar para visualizar o formulário. Para isso, basta marcar as caixas de seleção ao lado dos campos que você deseja que apareçam na listagem. Além disso, é possível configurar a largura do campo na listagem (a largura da coluna), a ordem de exibição e a ordenação.

   A ordem de exibição dos campos da listagem seguirá a ordem dessa tela, ou seja, para que um campo apareça na primeira coluna, clique na seta para cima, até que este seja o primeiro campo. A ordenação é definida por um campo, você deve selecioná-lo e escolher entre ordenação ascendente (Asc) ou descendente (Desc).
- **Schemas de Layout:** neste campo, será feita a definição de como realmente os campos serão exibidos no formulário, tanto para visualização quanto para edição e criação. Ou seja, nesta parte você deve configurar onde cada campo ficará dentro do formulário e como os campos serão divididos por seções. Para isso, siga os passos abaixo:

   1. Clique no botão `Incluir nova seção`.
   2. Preencha o campo **Nome**.
   3. Arraste um campo da lista **Campos disponíveis** para a coluna **Campos da coluna 1**. O mesmo pode ser feito para a coluna **Campos da coluna 2**. 

  Esses três passos podem ser repetidos até que se tenha o formulário no formato em que se deseja. É possível inserir vários campos na mesma coluna, assim como é possível criar várias seções. 

- **Consultas:** Essa aba serve apenas para exibir as [consultas criadas na listagem](/pt/tutorial/criando-uma-consulta-personalizada-no-master-data/).
- **Folha de Estilo:** Local para inserção de CSS para edição do front-end do formulário.

<video class="wp-video-shortcode" id="video-1047-3" width="840" height="411" preload="metadata" controls="controls"><source type="video/mp4" src="//assets.contentful.com/alneenqid6w5/7oRARnBsVamuk8iQ0mogQa/438e55214f38f7f16634da4fbc238d68/CriandoFormulario-1.mp4?_=3" /></video>
