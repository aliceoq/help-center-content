---
title: 'Creating a form in Master Data'
id: tutorials_1047
status: PUBLISHED
createdAt: 2017-04-27T21:57:35.614Z
updatedAt: 2023-12-08T18:36:08.521Z
publishedAt: 2023-12-08T18:36:08.521Z
firstPublishedAt: 2017-04-27T23:03:43.083Z
contentType: tutorial
productTeam: Master Data
author: authors_3
slug: creating-form-in-master-data
locale: en
legacySlug: creating-form-in-master-data
subcategory: WpbGhubuRZaNZilJSXnqu
---

A form serves as an interface for the visualization and manipulation of a data entity. Essentially, it acts as a field aggregator. Although always associated with an entity, it is not mandatory for it to contain all the fields related to it; it can be customized according to demand. This way, it is possible to create different forms for the same entity, adapting to various needs. For example, a purchase form may include fields such as ID, customer, and date.

To create a form, follow the steps below:

1. In the VTEX Admin, access **Store Settings** > **Storefront** > **Master Data.**
2. Click on the **Aplicações** tab.
3. In the application in which you want to create the form, click on the gear icon.
4. After opening the list of forms, click on the **Novo** button.
5. Fill in the fields as below (fields are divided by section).
6. Click on the **Salvar** button.

## Fields for the new form

- **Nome:** Form name.
- **Filtros:** Fields marked as entity filters; these fields will make up the side filters of the form. The internal name of the field must be entered. If there is more than one field, separate them with comas. For example: campo1,campo2.
- **Entidade de Dados:** This is the data entity in which the form will save and display the data.
- **Destaques de busca:** Fields that will be listed in the search results. The internal name of the field must be entered. If there is more than one field, separate them with comas. For example: when searching for a customer, the list of results must include the customer’s CPF and name; so, the field must be filled out with “cpf,nome.”
- **Consultas na visualização:** Enables a new section in the display form with the records of an entity related to the form’s entity. The information displayed will relate to the record that is being viewed.   

   For example, the __Atendimento__ entity includes a field related to the __Cliente__ entity. So, in the __Consultas na visualização__ field of the __Cliente__ form, you must enter the __Atendimento__ field that refers to the __Cliente__. if the acronym of the __Atendimento__ entity is __AT__, and the name of the field is __Cliente__, you must enter: `AT.Cliente` to upload the customer service that is being viewed in the form. ![registrosRelacionados2](//images.contentful.com/alneenqid6w5/2NrlYdzzR66Og4waCIekGe/e4d47ef3e257c749c09c0c9151383c45/registrosRelacionados2.png)![registrosRelacionados](//images.contentful.com/alneenqid6w5/3j6iBpbL7ao6soYaME4e2a/d80177bdf01586c97f1321c74c881ac3/registrosRelacionados-1.png)

After filling out the mandatory fields, the tabs available for configuration will be displayed. See below the fields of these tabs.

- **Campos da Listagem:** Select the fields included in the records list when clicking to view the form. To this end, just select the check boxes appearing at the side of the fields that you want to appear on the list. It is also possible to set up the width of the field on the list (column width), the display order and the ordering.

   The order of the fields on the list will follow the order viewed in this screen, that is, for a field to appear in the first column, click on the up arrow until it becomes the first field. Ordering is defined by one field. Select one field and choose between ascending (Asc) or descending (Desc) order.
- **Schemas de Layout:** definition of how the fields will be displayed in the form, both for viewing, and for editing and creating the fields. That is, the position of each field in the form will be set up in this phase, and they also be divided by sections.

   1. Click on the `Incluir nova seção` button.
   2. Fill out the __Nome__ field.
   3. Drag one field from the **Campos disponíveis** list to the **Campos da coluna 1** column. The same can be made regarding the **Campos da coluna 2** column.

   Repeat these 3 steps until you reach the format desired for the form. You can include several fields in a single column, as well as create several sections.

- **Consultas:** This tab is only intended to show the [queries created on the list](/en/tutorial/creating-a-personalized-master-data-query/).
- **Folha de Estilo:** Place to enter the CSS for editing the front-end of the form.

<video class="wp-video-shortcode" id="video-1047-3" width="840" height="411" preload="metadata" controls="controls"><source type="video/mp4" src="//assets.contentful.com/alneenqid6w5/7oRARnBsVamuk8iQ0mogQa/438e55214f38f7f16634da4fbc238d68/CriandoFormulario-1.mp4?_=3" /></video>
