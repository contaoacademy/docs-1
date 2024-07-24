---
title: 'Select menu'
description: 'The shop configuration - Select menu.'
aliases:
    - /en/backend-configuration/store-configuration/products/attributes/select-menu/
weight: 110
---

## Attribute Name &amp; Type

<table>
    <thead>
        <tr>
            <th>Setting</th>
            <th>Default</th> 
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Use for variants</td>
            <td>-</td>
            <td>Here you can provide the attribute for configuring product variants.</td> </tr><tr><td>Selectable by the customer</td> <td>-</td> <td>You must 
                select this field if the customer should be able to make an entry in the frontend.</td>
            </tr>
    </tbody>
</table>


## Description

<table>
    <thead>
        <tr>
            <th>Setting</th>
            <th>Default Setting</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Description</td> 
            <td>-</td>
            <td>This description serves as a hint for the backend user and is displayed below the input field.</td>
        </tr>
    </tbody>
</table>


## Options

<table>
    <thead>
        <tr>
            <th>Setting</th>
            <th>Default setting</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Options Source</td>
            <td>-</td>
            <td>Here you can select where the options for this field should be taken from. You can choose from:
                <ul>
                    <li>Options Manager</li>
                    <li>Own database table (foreignKey)</li>
                    <li>Options Wizard (deprecated)</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td colspan="3">Options Manager</td>
        </tr>
        <tr>
            <td>Edit Option</td> 
            <td>-</td> 
            <td>Add an option to the field.</td> 
        </tr>
        <tr>
            <td>New Option</td>
            <td>-</td> 
            <td>Create a new option.</td> 
        </tr>
        <tr>
            <td>Group</td>
            <td>-</td>
            <td>Here you can group option (adds a <code>optgroup</code> to the option).</td> 
        </tr>
        <tr>
            <td>Default</td> 
            <td>-</td> 
            <td>Here you can pre-select an option (adds <code>selected</code> to the option).</td> 
        </tr>
        <tr>
            <td>Label</td>
            <td>-</td>
            <td>Here you can specify which label the option should be displayed in the backend or frontend.</td>
        </tr>
        <tr>
            <td>Price markups or markdowns</td>
            <td>-</td> 
            <td>You can enter a positive or negative value to change the product price when this option is selected.</td> 
        </tr>
        <tr>
            <td>Published</td> 
            <td>-</td> 
            <td>Make this option available in the product.</td>
        </tr>
        <tr>
            <td colspan="3">Own database table (foreignKey)</td> 
        </tr>
        <tr>
            <td>Foreign table and field</td> 
            <td>-</td> 
            <td>Instead of options you can also read data from the database. A possible query, after creating the database table and data 
                fields, could look like this: 
                <br><code># Database field for the fallback language</code>
                <br><code>tl_my_table.my_field</code>
                <br><code># Database field for the German language</code>
                <br><code>de=tl_my_table.my_field_de</code>
                <br><code># Database field for the French language</code>
                <br><code>fr=tl_my_table.my_field_fr</code>
            </td> 
        </tr>
        <tr>
            <td colspan="3">Options Wizard (deprecated)</td> 
        </tr>
        <tr>
            <td>Value</td> 
            <td>-</td> 
            <td>Here you can enter the value of the option, which should be transferred when submitting the form.</td> 
        </tr>
        <tr>
            <td>Name</td> 
            <td>-</td> 
            <td>Here you can specify which label the option should be displayed in the backend or frontend.</td>
        </tr>
        <tr>
            <td>Default</td> 
            <td>-</td> 
            <td>Here you can pre-select an option (adds a <code>selected</code> to the option).</td>
        </tr>
        <tr>
            <td>Group</td> 
            <td>-</td> 
            <td>Here you can group an option (adds <code>optgroup</code> to the option).</td>
        </tr>
        <tr>
            <td colspan="3"></td> 
        </tr>
        <tr>
            <td>Insert empty selection</td>
            <td>-</td> 
            <td>Here you can define an empty selection for the select menu.</td>
        </tr>
        <tr>
            <td>Label for the empty selection</td> 
            <td>-</td> 
            <td>Here you can define the label for the empty selection.</td>
        </tr>
    </tbody>
</table>

{{% notice info %}}<p>Tip: <a href="https://now.metamodel.me/" target="_blank">MetaModels</a>  is anexcellent tool for creating 
and maintaining external tables and fields.{{% /notice %}}


## Attribute configuration

<table>
    <thead>
        <tr>
            <th>Setting</th>
            <th>Default setting</th>
            <th>Description</th> 
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Mandatory field</td> 
            <td>-</td> 
            <td>If <code>Selectable by the customer</code> is selected, the product cannot be added to the shopping cart without 
                this information. Otherwise, the field will be displayed as a required field in the backend when creating a product.</td> 
        </tr>
        <tr>
            <td>Use the JavaScript plugin "Chosen"</td> 
            <td>-</td> 
            <td>This option enables the use of the JavaScript plugin "Chosen" for the selection field, allowing you to select 
                multiple values using a search function. {{< version "2.6" >}}</td>
        </tr>
        <tr>
            <td>Multiple Selection</td> 
            <td>-</td> 
            <td>Allows the user to select more than one option.</td> 
        </tr>
        <tr>
            <td>List Size</td> 
            <td>5</td> 
            <td>Once <code>Multiple Selection</code> is selected, you can set the size of the selection box here.</td>
        </tr>
    </tbody>
</table>


## Search &amp; Filter Settings

<table>
    <thead>
        <tr>
            <th>Setting</th> 
            <th>Default setting</th> 
            <th>Description</th> 
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Filterable in frontend</td> 
            <td>-</td> 
            <td>Once this field is selected, this attribute can be used as a filter in the frontend.</td> 
        </tr>
        <tr>
            <td>Add to "Sort by" option list.</td> 
            <td>-</td> 
            <td>Makes the field, if maintained in the backend and visible to the customer, sortable in the list module.</td> 
        </tr>
        <tr>
            <td>Filterable in the backend</td>
            <td>-</td> 
            <td>Once this field is selected, this attribute can be used as a filter in the backend.</td>
        </tr>
    </tbody>
</table>

The output of the created attribute in the backend is through the [product types](en/backend-configuration/store-configuration/products/product-types/). 
If you have made the select menu <code>Selectable by the customer</code> it will be displayed automatically in the frontend (using <code>$this->options</code> 
in the template). Otherwise you can output the attribute in the desired isotope template with the following code <code><?= $this->generateAttribute('InternerName'); ?></code>.
