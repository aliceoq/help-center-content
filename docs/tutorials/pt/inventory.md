---
title: 'Inventário Data Pipeline (Beta)'
id: 2IvKMZV9SNrE6ipBRQr8h2
status: DRAFT
createdAt: 2024-02-02T17:41:24.979Z
updatedAt: 2024-02-02T18:15:06.757Z
publishedAt: 
firstPublishedAt: 
contentType: tutorial
productTeam: Others
author: 2p7evLfTcDrhc5qtrzbLWD
slug: inventario-data-pipeline-beta
locale: pt
legacySlug: inventario-data-pipeline-beta
subcategory: QPnz120TdtLcXSh65c4Gs
---

# Inventário

O conjunto de dados composto pela tabela `item_inventory` fornece informações sobre a disponibilidade de itens no inventário. Ele detalha a quantidade total e disponível de itens, reservas ativas, possibilidade de estoque infinito, além de incluir identificações de SKU e estoque. A tabela também registra atualizações com registro de data e hora e IDs de controle.

Nesta seção você encontra as seguintes informações:

- [Características dos dados de inventário](#caracteristicas-dos-dados-de-inventario)
- [Tabela item_inventory](#tabela-item-inventory)
- [Análise com item_inventory](#analises-com-item-inventory)
- [Correlações com outros dados](#correlacoes-com-outros-dados)

## Características dos dados de inventário

| **Característica** | **Descrição** |
|:---:|:---:|
| **Origem do dado** | Alimentado por informações do **módulo de logística**. |
| **Disponibilidade** | Admin da VTEX. |
| **Histórico** | Os dados são mantidos por dois anos, a partir de 2024 para clientes que já utilizam a plataforma VTEX. |
| **Menor intervalo de atualização possível** | Uma hora. |

## Tabela `item_inventory`

Conheça a seguir os campos que constituem a tabela:  

| **Nome da Coluna** | **Tipo de Coluna** | **Descrição da Coluna** |
|:---:|:---:|:---:|
| account_name | character varying(256) | Nome da conta relacionada ao item. |
| seller_account_name | character varying(256) | Nome da conta do vendedor associada ao item. |
| parent_account_name | character varying(256) | Nome da conta mãe associada ao item. |
| quantity | double precision | Quantidade total de itens disponíveis. |
| available_quantity | double precision | Quantidade de itens disponíveis para venda. |
| reserved_quantity | double precision | Quantidade de itens reservados e não disponíveis para venda imediata. |
| is_unlimited_quantity | boolean | Indica se o item tem inventário ilimitado. |
| item | character varying(256) | ID do SKU. |
| container | character varying(256) | ID do estoque onde o item está armazenado. |
| ts | timestamp without time zone | Registro de data e hora da última atualização do item. |
| batch_id | character varying(13) | ID de controle do lote de ingestão de dados. |

## Análises com `item_inventory`

Veja abaixo algumas das análises possíveis com a tabela de inventário:

**- Análise de níveis de inventário:** avalie se o inventário atende à demanda e identificar itens com risco de esgotamento.  
**- Tendências de reserva de inventário:** analise a quantidade de itens reservados ao longo do tempo para identificar padrões e ajustar estratégias de gestão de inventário.  
**- Análise de distribuição de inventário por conta:** otimize a gestão de inventário em várias contas e entender como o inventário é distribuído.  

## Correlações com outros dados

Os dados de inventário se correlacionam com os conjuntos de pedidos e produtos, e proporcionam análises mais abrangentes para compras, vendas e marketing. Veja alguns exemplos:  

**- Interação com dados de pedidos:** a análise conjunta com os dados de pedidos oferece insights sobre a eficiência em atender às demandas dos clientes e ajuda a prever necessidades de reabastecimento.  
**- Relação com os SKUs:** a integração com os dados de SKUs ajuda a gerenciar o inventário com base na popularidade e disponibilidade dos produtos.  
**- Dados de compras e fornecedores:** a coordenação com os dados de compras permite manter um equilíbrio ideal no inventário, evitando superlotação ou escassez.  
**- Análises de vendas e marketing:** a compreensão do inventário impacta diretamente as estratégias de marketing e vendas, alinhando promoções e campanhas com a disponibilidade de produtos.  

