---
title: 'Como escrever um ticket completo para o suporte VTEX'
id: 6u4ehk6F0ksuDgYuCbFDRX
status: PUBLISHED
createdAt: 2023-03-23T22:00:24.560Z
updatedAt: 2023-07-27T20:50:02.235Z
publishedAt: 2023-07-27T20:50:02.235Z
firstPublishedAt: 2023-03-23T22:57:50.828Z
contentType: tutorial
productTeam: Others
author: 46G4yHIZerH7B9Jo0Iw5KI
slug: como-escrever-um-ticket-completo-para-o-suporte-vtex
locale: pt
legacySlug: como-escrever-um-ticket-completo-para-o-suporte-vtex
subcategory: 1VvCpaa8NCA6a0MK6W6oWg
---

Todos os clientes e parceiros têm acesso a atendimento fornecido pelo time de especialistas do [Suporte VTEX](https://help.vtex.com/pt/faq/como-funciona-o-suporte-da-vtex--3kACEfni4m8Yxa1vnf2ebe). Para contatá-los, é necessário abrir um chamado por meio do sistema de tickets. 

Os especialistas estão preparados para proporcionar a melhor experiência possível para a solução dos chamados. Porém, para garantir um atendimento mais rápido e objetivo, existem algumas orientações que devem ser seguidas durante a abertura do ticket. 

Lembre-se que, quanto mais contexto os especialistas tiverem, mais rápido será possível chegar a uma resolução para o problema. 

Este artigo orienta os clientes e parceiros a abrirem os tickets com informações relevantes para agilizar o processo de investigação dos nossos especialistas. Ele está dividido nas seguintes seções:

- [Orientações gerais](#orientacoes-gerais)
- [Informações relevantes por cenário](#informacoes-relevantes-por-cenario)

Para saber como abrir um chamado na VTEX, leia o artigo [Abrir chamados para o suporte VTEX](https://help.vtex.com/pt/tutorial/abrir-chamados-para-o-suporte-vtex--16yOEqpO32UQYygSmMSSAM).

## Orientações gerais

Antes de abrir um ticket, é importante conferir se o problema está relacionado às customizações da loja. 

Para fazer a verificação, é necessário executar duas principais ações, veja abaixo.

**Para loja CMS**

1. Bloqueie arquivos no devtools da página (`.js` e `.css`).

![Ferramenta do desenvolvedor](//images.ctfassets.net/alneenqid6w5/1BXRvp3Ogpx83gJnB5kFeG/8611c6f0da93808db6e5f588bcb184e9/devtolls.png)  

2. Execute a ação que apresentava erro no carrinho ou checkout.

**Para loja VTEX IO**

1. Linke o tema padrão do VTEX IO a um workspace de desenvolvimento.  
2. No workspace, reproduza o processo que apresenta erro no site.  

Se o erro persistir, abra um ticket para o time VTEX seguindo as orientações da tabela abaixo. Se o erro não acontece após o bloqueio dos arquivos ou no tema padrão do VTEX IO, significa que o erro é relacionado às customizações presentes no site e para a resolução, você deve entrar em contato com a equipe responsável pelo frontend da sua loja. 

### Preenchendo um ticket  

Para preencher um ticket de forma completa, siga as orientações abaixo:  

| Informações | Orientações |
| ----------- | ----------- |
| Assunto e descrição do problema | <p> - Resuma o problema ou dúvida em poucas palavras. Preencha o campo **Assunto da solicitação** de forma concisa e direta para ajudar o time de especialistas a entender rapidamente o cenário. </p> <p> - Preencha o campo **Assunto da solicitação** com a descrição completa do que foi observado, incluindo o quê, como e onde está acontecendo o problema, para que o time de especialistas possa investigar e reproduzir o cenário. Não esqueça de informar caso o passo a passo para reprodução do cenário inclua alguma ação atípica que precisa ser tomada ou permissão de acesso restrita. </p>  |
| Evidências | Inclua qualquer material que o problema possa ser observado, sempre que disponível. Por exemplo, capturas ou gravações da tela, [arquivos HAR](https://help.vtex.com/pt/tutorial/gerar-arquivo-har-para-debugar-problemas-na-loja--15xVlw8nuakk2k6Cao4k2Q), logs gerados pela plataforma, respostas do servidor, o texto ou o ID do erro apresentado. |
| Cenário esperado | Forneça detalhes do cenário que era esperado, em comparação ao que está acontecendo. |
| Testes e validações | Se você já tentou solucionar o problema, detalhe as ações já executadas, quais documentações foram consultadas e seus resultados. |
| Escopo do ticket | <p> - Não enderece mais de um problema no mesmo ticket. </p> <p> - Não crie mais de um ticket para o mesmo problema. </p> |
| Prioridade | Verifique a [prioridade](https://help.vtex.com/pt/faq/suporte-vtex-brasil--5q861sTw1n7H2BENOu7ls9#prioridade-de-chamados) correta de acordo com  a natureza do problema, para que o [SLA](https://help.vtex.com/pt/faq/suporte-vtex-brasil--5q861sTw1n7H2BENOu7ls9#disponibilidade-e-sla-de-atendimento) correto seja aplicado. |

## Informações relevantes por cenário

Existem vários cenários que podem levar à abertura de um ticket. Nessa seção, serão elencados os cenários mais comuns com informações básicas necessárias para abertura do ticket em cada cenário.

Você pode adaptar essas informações ao seu cenário específico e também usá-las como guia  em sua própria investigação antes da abertura de ticket.

| Cenários | Informações |
| ----------- | ----------- |
| Pedidos | <p> - ID do pedido ou do <code> orderForm </code>. </p> <p> - URL do pedido no <strong> Gerenciamento de pedidos </strong> ou no <strong> Bridge </strong> (em casos de pedidos de marketplaces com integrações nativas). </p> |
| Checkout | <p> - URL do carrinho gerado pelo <a href="https://help.vtex.com/pt/tutorial/configurar-o-cartman--1ACMTStZYkMqB0lTgwg451">Cartman</a>. </p> <p> - IDs dos SKUs e CEP para reprodução do carrinho. </p>
| Logística | <p> - ID do seller. </p> <p> - URL de estoque, doca ou transportadora do seller. </p> <p> - Informações para simular entrega, como IDs dos SKUs e CEP </p> |
| Pagamentos | <p> - ID da transação. </p> <p> - Link da transação, acessando no Admin VTEX <em> Pagamentos > Transações. </em> </p>
| VTEX IO | <p> - Nome e versão do aplicativo utilizado. </p> <p> - Workspace utilizado. </p> <p> - Arquivo ZIP com o <a href="https://developers.vtex.com/docs/guides/vtex-io-documentation-3-settingyourstoretheme">store-theme</a> em caso de tema linkado e não instalado. </p> |
| Promoções | <p> - Nome da promoção. </p> <p> - URL da promoção. </p> <p> - Produto e CEP aplicáveis à promoção para testes. </p> |
| Integrações (aplicável aos parceiros de integração) | <p> - Explicação sobre o produto e o papel dele na VTEX. </p> <p> - Seu objetivo final antes do problema ocorrer. </p> <p> - Em caso de chamadas para APIs da VTEX que falharam: endpoint utilizado, request body e response body. </p> <p> - ID e URL do afiliado (se o problema for na integração com um marketplace externo). </p>

#### Saiba mais

- [Abrir chamado no suporte VTEX](https://help.vtex.com/pt/tutorial/abrir-chamados-para-o-suporte-vtex--16yOEqpO32UQYygSmMSSAM)
- [Como funciona o suporte da VTEX ?](https://help.vtex.com/pt/faq/como-funciona-o-suporte-da-vtex--3kACEfni4m8Yxa1vnf2ebe)
- [Suporte VTEX - Brasil](https://help.vtex.com/pt/faq/suporte-vtex-brasil--5q861sTw1n7H2BENOu7ls9)
