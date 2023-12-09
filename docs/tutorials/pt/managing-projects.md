---
title: 'Gerenciando Projetos'
id: 42IpDFqTVTESH8DCypJMPM
status: PUBLISHED
createdAt: 2023-11-01T13:45:57.091Z
updatedAt: 2023-11-16T14:44:11.820Z
publishedAt: 2023-11-16T14:44:11.820Z
firstPublishedAt: 2023-11-01T19:38:50.237Z
contentType: tutorial
productTeam: VTEX IO
author: 4oTZzwYoyhy1tDBwLuemdG
slug: gerenciando-projetos
locale: pt
legacySlug: gerenciando-projetos
subcategory: 27t6x0lngvjI3bnUg5AgEO
---

Projetos é uma funcionalidade do VTEX Headless CMS que simplifica o gerenciamento de vários projetos de frontend, como aplicativos móveis, sites e email marketing em uma única tela.

![Projects pages](//images.ctfassets.net/alneenqid6w5/5sXlS9M78whzUVdSxJiKpX/b5bd29ece472c96fceb0aefb71a5365a/projects-one-pt-certo.gif)

Cada projeto tem suas configurações, conteúdo e marca personalizados de acordo com públicos ou objetivos específicos.

Neste guia, você aprenderá como gerenciar cada projeto de frontend da sua loja.

## Antes de começar
Certifique-se de que você tenha acesso ao VTEX Headless CMS. Entre em contato com os administradores da conta para verificar se seu perfil de acesso tem permissão para gerenciar conteúdo no VTEX Headless CMS no VTEX Admin. Para saber mais, consulte o guia [Perfis de acesso](https://help.vtex.com/pt/tutorial/roles--7HKK5Uau2H6wxE1rH5oRbc).

## Visão geral
Para acessar a página de **Projetos**, entre no VTEX Admin e clique em **Storefront > Headless CMS**.

![Projects overview](//images.ctfassets.net/alneenqid6w5/3RgVmOuLr7SJmEfots0KMZ/c5a1f1ba3077c11504d9f78c1712c59e/projects-two-pt.png)

| Opção               | Descrição                                              |
| ------------------- | ------------------------------------------------------ |
| Cartão projeto      | Abre o projeto selecionado, para que você possa criar e editar páginas do conteúdo dele.       |
| Configurações (⚙️) | Abre um modal com as configurações do projeto separadas em duas abas: <ul><li>**Geral:** permite editar o ID do projeto e as configurações de API ou arquivar o projeto.</li> <li>**Build:** permite conectar o projeto CMS ao código-fonte via webhooks, configurando os tipos de conteúdo e as seções.</li></ul> |
| Criar novo       | Abre uma página para configurar um novo projeto.       |

## Criar novo projeto

Crie um novo projeto para sua loja definindo as configurações gerais, como **ID do projeto** e **URL base de produção**. Para conectar um projeto Headless CMS ao código-fonte do seu projeto, você também precisará definir webhooks e configurações de build, como *URL de build do webhook* e * URL de pré-visualização*.

O webhook é um endpoint HTTP que permite a comunicação automatizada entre o VTEX Headless CMS e o código-fonte do projeto. Ele permite, por exemplo, que o CMS notifique um projeto FastStore sobre alterações de conteúdo ou outros eventos, desencadeando ações como a sincronização de conteúdo em tempo real.

1. Na página **Projetos**, clique em `Criar novo`.

2. Na página **Novo projeto**, preencha os campos de acordo com a seção [Configurações do projeto](#configurações-do-projeto).

3. Depois de definir cada campo da página, clique em `Criar` e uma mensagem de sucesso será exibida na tela.

Depois de criar um novo projeto, você poderá criar páginas para ele com todas as rotas de URL e modelos de página compatíveis com a sua loja, como páginas iniciais, de produtos e de login.

Para criar uma nova página, siga os passos em [Gerenciando páginas no Headless CMS](https://help.vtex.com/tutorial/managing-pages--3DO6rBhZ1p3zndnFu5BgRt)

## Configurações do projeto
As configurações do projeto permitem que você o configure de acordo com duas categorias principais:

- [Geral](#geral): permite editar o ID do projeto e as configurações de API, além de arquivar o projeto.
- [Build](#build): permite estabelecer a conexão entre o projeto CMS e o código do seu projeto.

### Geral

| Nome do campo               | Descrição      | Exemplo de valor |
| --------------------------- | -------------- | ---------------- |
| ID do projeto (obrigatório) | ID do projeto. | `Sales App`      |
| API                         | URL base de produção do site. | `https://{nomedaconta}.vtex.com/` |

### Build

| Nome do campo               | Descrição      | Exemplo de valor |
| ---------- | ---------- | ---------- |
| URL das seções | URL do webhook para receber e salvar as seções criadas no código-fonte no Headless CMS.      | `https://infra.io.vtex.com/vbase/v0/{nomedaconta}/master/buckets/vtex.admin-cms-graphql-rc/store/files/{builderId}/sections`       |
| URL dos tipos de conteúdo      | URL do webhook para receber e salvar os tipos de conteúdo criados no código-fonte no Headless CMS.       | `https://infra.io.vtex.com/vbase/v0/{nomedaconta}/master/buckets/vtex.admin-cms-graphql-rc/store/files/{builderId}/content-types`       |
| URL de build do webhook       | URL do webhook para iniciar um novo build no Headless CMS quando uma página ou conteúdo é adicionado ou editado.       | `https://app.io.vtex.com/vtex.cms-builder-sf-jamstack/v1/{nomedaconta}/{workspace}/build-releases`       |
| Salvar URL do webhook       | URL do webhook para permitir pré-visualizações do projeto em tempo real, enviando uma notificação para que você atualize a página para refletir as alterações mais recentes no Headless CMS.       |  -       |
| URL de pré-visualização       | URL do webhook que permite a pré-visualização de páginas no Headless CMS.       | `https://{nomedaconta}.vtex.app/api/preview`       |

## Editar projeto
Após criar o projeto, você também pode editar todas as informações que definiu durante a [criação do projeto](#criar-novo-projeto).
Na página principal **Projetos**, clique em **Configurações** (⚙️). Em seguida, um modal aparecerá com duas guias de configurações: [Geral](#geral) e [Build](#build).

## Arquivar projeto
O arquivamento de um projeto desativa a API e o acesso ao seu conteúdo.
Para arquivar um projeto, siga os passos abaixo:

1. Acesse **Storefront > Projetos**.

2. Escolha o projeto que deseja arquivar e clique em **Configurações** (⚙️). Isso abrirá um modal.

3. No modal, clique em `Arquivar projeto` na página `Geral`. Uma mensagem pop-up aparecerá confirmando se você deseja arquivar o projeto.
![Arquivar projeto](//images.ctfassets.net/alneenqid6w5/3FkQ3UCU68HH8QkP4LH91I/c7410dbcff84549da3a15720a0ce68ed/projects-three-pt.png)
4. Clique em `Arquivar`. Em seguida, será exibida uma mensagem informando que o projeto foi arquivado com sucesso.

Para restaurar um projeto arquivado, siga os passos em [Restaurar projeto](#restaurar-projeto).

### Restaurar projeto
Ao restaurar um projeto, sua API é reativada e o conteúdo do projeto pode ser acessado novamente. Para restaurar um projeto, siga os passos abaixo:

1. Acesse **Storefront > Projetos**.

2. Clique no cartão do projeto arquivado.

3. Clique em `Restaurar projeto`. Uma mensagem pop-up aparecerá confirmando se você deseja restaurar o projeto.

4. Clique em `Restaurar`. Em seguida, será exibida uma mensagem informando que o projeto foi restaurado com sucesso.

