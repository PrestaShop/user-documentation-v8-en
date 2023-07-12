# The multistore interface

## The Multistore page  <a href="#themultistoreinterface-managingyourstores" id="themultistoreinterface-managingyourstores"></a>

### Understanding the multistore page organization

{% hint style="info" %}
To access the Multistore page, you need to [enable the feature](../#managingmultipleshops-enablingthemultistorefeature) in **Shop Parameters > General** first.
{% endhint %}

A new page is then available in the **Advanced Parameters** menu: the **Multistore page.**

This page is divided into 3 sections:

* **Multistore tree:** The multistore tree gives you an overview of how your stores are organized into different groups.&#x20;
* **Multistore:** This table lists all the store groups you have created, whether they are enabled or not.&#x20;
* **Multistore options:** In this section, you can select the store you want to set as default. &#x20;

{% content-ref url="adding-new-store.md" %}
[adding-new-store.md](adding-new-store.md)
{% endcontent-ref %}

{% content-ref url="adding-new-group-of-stores.md" %}
[adding-new-group-of-stores.md](adding-new-group-of-stores.md)
{% endcontent-ref %}

{% content-ref url="setting-store-url.md" %}
[setting-store-url.md](setting-store-url.md)
{% endcontent-ref %}

## Working in different contexts <a href="#themultistoreinterface-onebackofficetorulethemall" id="themultistoreinterface-onebackofficetorulethemall"></a>

### Knowing what context you are in

When the multistore feature is enabled, you can apply changes to either **all stores**, **a group of stores**, or **a specific store**, depending on the context selected in the drop-down selector or the header.

* **All stores**: Changes will apply to all your stores.
* **Group X**: Changes will only apply to the stores in group X.
* **Store Y**: Changes will only apply to store Y.

#### The drop-down selector (older versions and non-updated pages)

The drop-down selector at the top of each page of the back office indicates the context you are working on (All stores, group, or single store).

![](<../../../.gitbook/assets/57081980 (4) (4) (2).png>)

#### The header

The multistore interface evolves and the drop-down Edit multistore page EN turns into a header on most of the pages. &#x20;

<figure><img src="../../../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
The color of each store or group of stores can be customized on the **Advanced Parameters > Multistore** page. Depending on the store you are working on, the header will change color, allowing you to know at a glance what context you are in.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

### Make changes to a group of stores or to a specific store

To apply changes to a group of stores or to a specific store, switch context with the header and select the group or the store you want to customize.

The interface might be different depending on your version of PrestaShop and the page you are on:

#### The multistore toggle button and checkboxes (older versions and pages)

In a group or single store context, new options will appear on the page, allowing you to customize settings for the specific group or store selected:

* A multistore "Yes/No" toggle button
* A checkbox next to each parameter

To make changes:&#x20;

1. To make all settings for a section editable, set the multistore toggle button to "Yes".  If you only want to customize a specific setting, **check the box** next to it.
2. Once a parameter is editable, make your changes and save.

{% hint style="info" %}
Setting the multistore toggle to yes or checking a box makes the parameter(s) editable but doesn't change their value. It's up to you to make your adjustments and save.
{% endhint %}

#### Checkboxes

Checkboxes are displayed when you are working in a single-store or group context. They allow you to modify a parameter for a specific store, or a group of stores and keep a record of this change.&#x20;

If the box is checked next time you go to the page, it means that the parameter is customized for the store or the group of stores you are working on. Unchecking the box will cancel the customization, and the parameter will take the same value as in the "All stores" context (or the group context, if any).

For example, in the screenshot below, the box next to the maintenance text parameter is checked. This means that this parameter is customized in Store 1.

<figure><img src="../../../.gitbook/assets/image (96).png" alt=""><figcaption></figcaption></figure>

### Keep track of the changes made on a single store

#### The specific settings drop-down

Thanks to the specific settings drop-down, if you make changes to a specific store, and that you then go back to the "All stores" or group context, you'll be able to easily know which parameters have been modified in a specific store.

So, if you see this drop-down next to a parameter, it means that this parameter has been customized in at least one store. Deploy the drop-down to know which store(s) are concerned.

<figure><img src="../../../.gitbook/assets/image (29) (2).png" alt=""><figcaption></figcaption></figure>

**Customized**: The parameter was modified in the store.

**Inherited**: The parameter is set in the same way in all stores.
