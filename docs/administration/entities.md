# Customize entities

## Introduction

A variety of entity customization options are available to optimize data representation, workflow management, and enhance overall user experience. Whether you're fine-tuning processing statuses, configuring entities' attributes, or hiding entities, OpenCTI's customization capabilities provide the flexibility you need to create a tailored environment for your threat intelligence and cybersecurity workflows.

The following chapter aims to provide readers with an understanding of the available customization options by entity type. Customize entities can be done in "Settings > Customization".

![Customization menu](./assets/customization-window.png)


## Hidden in interface

This configuration allows to hide a specific entity type throughout the entire platform. It provides a potent means to simplify the interface and tailor it to your domain expertise. For instance, if you have no interest in disinformation campaigns, you can conceal related entities such as Narratives and Channels from the menus.

You can specify which entities to hide on a platform-wide basis from "Settings > Customization" and from "Settings > Parameters", providing you with a list of hidden entities. Furthermore, you can designate hidden entities for specific Groups and Organizations from "Settings > Security > Groups/Organizations" by editing a Group/Organization.

An overview of hidden entity types is available in the "Hidden entity types" field in "Settings > Parameters."


## Automatic references at file upload

This configuration enables an entity to automatically construct an external reference from the uploaded file.


## Enforce references

This configuration enables the requirement of a reference message on an entity creation or modification. This option is helpful if you want to keep a strong consistency and traceability of your knowledge and is well suited for manual creation and update.

![Entity configuration](./assets/entity-configuration.png)


<a id="workflow-section"></a>
## Workflow

For now, OpenCTI has a simple workflow approach. They're represented by the "Processing status" field embedded in each object. By default, this field is disabled for most objects but can be activated through the platform settings:

1. Navigate to "Settings > Customization > Entity types > [Desired object type]."
2. Click on the small pink pen icon next to "Workflow" to access the object customization window.
3. Add and configure the desired statuses, defining their order within the workflow.

![Workflow status](./assets/workflow-configuration.png)

In addition, the available statuses are defined by a collection of status templates visible in "Settings > Taxonomies > Status templates". This collection can be customized.


<a id="fintelTemplates-section"></a>
## Fintel templates

In Entreprise Edition, you can now define templates for your containers.
You can access this feature via the Customization page (Setting/Customization/Entity types). As a result, you are required to have the Manage customization capability (or the Bypass capability) to either create, update, view, export or delete a template.

![Fintel templates](./assets/fintelTemplates-list.png)

Clicking on a fintel template line redirects to its edition page.
In the 'Content editor' tab, you can write and format the content of your template via CK Editor.
![Fintel templates edition](./assets/fintelTemplates-edition.png)

In the 'Content Preview' tab, you can preview what a file generated from your Fintel template will look like for a given container.
![Fintel templates preview](./assets/fintelTemplates-preview.png)

### Fintel template widgets

In the right panel, the widgets saved in your template are displayed.
![Fintel templates widgets](./assets/fintelTemplates-widgets.png)

To add an existing widget in your content, copy the variable name and paste it in your content.

To add a widget, click on the 'Add data related to the container' button and follow the steps to create a visualization. For more information on how to create a widget, please read  [Widget creation](../usage/widgets.md).

To add an attribute of the container where the Fintel template will be used, click on the 'Add data of the container' button. In the opened pop-up you can manage the attributes you want to use in your template content.
Note that every template has a built-in widget of type 'attribute' that can't be deleted. This widget enables to display attributes of the container for which the template will be used.
![Fintel templates self attribute widget edition](./assets/fintelTemplates-widget-attributes.png)

You can only delete widgets that are not used in your content (they are highlighted with a warning icon).


<a id="attributes-section"></a>
## Attributes

Each attribute in an Entity offers several customization options:

- It can be set as mandatory if not already defined as such in the STIX standard.
- A default value can be established to streamline entity creation through the creation forms.
- Different thresholds and their corresponding labels for scalable attributes can be defined.

![Mandatory attributes and default values](./assets/mandatory_and_default_attributes.png)


### Confidence scale configuration

Confidence scale can be customized for each entity type by selecting another scale template or by editing directly the scale values.
Once you have customized your scale, click on "Update" to save your configuration.

![Mandatory attributes and default values](./assets/confidence_scale_configuration.png)

!!! note "Max confidence level"

    The above scale also needs to take into account the confidence level per user. To understand the concept, please navigate to this [page](../usage/reliability-confidence.md)


### Overview layout customization
At the platform level, the Overview layout tab of the containers can be rearranged to fit the users needs.
The widgets can be reordered or extended to their full width.

![Overview layout customization settings](assets/overview-layout-customization.png)

To reset the layout to its default version, click the button next to the section title.