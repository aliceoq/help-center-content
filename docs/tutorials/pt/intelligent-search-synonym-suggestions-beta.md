---
title: 'Sugestões de Sinônimos do Intelligent Search (Beta)'
id: 18A9JTCPrMsHWpFntNoKEr
status: PUBLISHED
createdAt: 2023-06-01T20:18:10.087Z
updatedAt: 2024-01-18T22:11:46.309Z
publishedAt: 2024-01-18T22:11:46.309Z
firstPublishedAt: 2023-06-01T20:33:35.148Z
contentType: tutorial
productTeam: Others
author: 1malnhMX0vPThsaJaZMYm2
slug: sugestoes-de-sinonimos-do-intelligent-search-beta
locale: pt
legacySlug: sugestoes-de-sinonimos-do-intelligent-search-beta
subcategory: 23WdCYqmn2V2Z7SDlc14DF
---

<div class="alert alert-info">
  <p>Essa funcionalidade está na fase Beta fechado, o que significa que somente clientes selecionados têm acesso a ela no momento. Caso tenha interesse em implementá-la futuramente, entre em contato com <a href="https://support.vtex.com/hc/pt-br/requests">nosso Suporte</a>.</p>
  <p>Para os clientes selecionados, a funcionalidade está disponível para uso gratuito no Admin VTEX durante seu período Beta, ou até decidido pela VTEX. É possível que taxas extras se apliquem futuramente.</p>
</div>

A funcionalidade de [Sinônimos](https://help.vtex.com/pt/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/1pxAWPEglBey1UFdvcetZV) do [VTEX Intelligent Search](https://help.vtex.com/pt/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/3qgT47zY08biLP3d5os3DG) permite cadastrar palavras, ou expressões de mesmo sentido, para termos de busca utilizados pelos clientes ao realizar pesquisas na sua loja, aumentando a chance deles obterem resultados relevantes nas buscas.

A página de **Sinônimos** no Admin VTEX apresenta sugestões inteligentes de termos para cadastro, além da configuração manual de sinônimos. A plataforma sugere sinônimos a partir de inteligência artificial, com base no comportamento de busca de clientes na sua loja.

Para isso, o VTEX Intelligent Search contabiliza quantas vezes nos últimos 30 dias os clientes pesquisaram por um termo que resultou em poucos ou nenhum resultado de busca e substituíram o termo original por outro. 

> _Exemplo:_ imagine que cinco clientes escreveram `sabonete rosto` e, em seguida, alteraram a pesquisa para `sabão rosto`. O sistema registra esse comportamento e os termos mais reescritos vão aparecer como sugestão de sinônimos.

Você pode revisar as sugestões geradas e optar por uma das três ações: recusar, editar ou aprovar. Confira o passo a passo na seção a seguir.

## Revisar sugestões

Siga as instruções para visualizar as sugestões de sinônimos e definir se elas serão recusadas, editadas ou aprovadas:

1. No Admin VTEX, acesse **Storefront**, ou digite **Storefront** na barra de busca no topo da página.
2. Em **Intelligent Search**, clique em **Sinônimos**.
3. Ao acessar a página de **Sinônimos**, existem dois cenários possíveis:

    * Se existirem sugestões ainda não visualizadas, um modal vai surgir, indicando a quantidade de sugestões geradas. Nesse caso, clique em `Revisar`.
    * Se existirem sugestões já visualizadas que ainda não revisadas, você verá um aviso no topo da página, indicando a quantidade de sugestões geradas. Nesse caso, clique em `Iniciar revisão`.

   Você verá um modal com a primeira sugestão de sinônimo. Cada sugestão indica o termo buscado e o termo que será adicionado como sinônimo, bem como a quantidade de vezes em que clientes da sua loja reescreveram o termo original para o segundo termo nos últimos 30 dias.

   ![syn-sug-pt-2](//images.ctfassets.net/alneenqid6w5/6cHj0ZfxftInJFwJNWdJET/571016f8129c3a58a6e49dd55ed491be/806shots_so.png)

4. Para revisar cada sugestão, escolha uma das ações a seguir:
    * <i class="fas fa-times-circle"></i> **Recusar**: descarta a sugestão proposta.
    * <i class="fas fa-pencil-alt"></i> **Editar**: altera campos da configuração dos sinônimos sugeridos. Depois de editar, é preciso clicar em <i class="fas fa-check-circle"></i> para salvar. Para mais informações sobre os campos disponíveis, leia [Configurar Sinônimos](https://help.vtex.com/pt/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/3ExbC3QKNF4zH7Gs8jD1cL).
    * <i class="fas fa-check-circle"></i> **Aprovar**: aplica e salva a sugestão proposta.
5. Após revisar todas as sugestões, feche o modal para acessar a listagem de sinônimos configurados na sua loja.

<div class="alert alert-error">
  <p>Uma vez que uma ação é realizada, não é possível desfazê-la, pois a próxima sugestão disponível é exibida imediatamente.</p>
</div>

## Saiba mais

* [Sinônimos](https://help.vtex.com/pt/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/1pxAWPEglBey1UFdvcetZV)
* [Configurar Sinônimos](https://help.vtex.com/pt/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/3ExbC3QKNF4zH7Gs8jD1cL)
* [VTEX Intelligent Search](https://help.vtex.com/pt/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/3qgT47zY08biLP3d5os3DG)
