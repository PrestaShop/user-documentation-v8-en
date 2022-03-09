# Positions

* [Front office Positions](positions.md#Positions-FrontofficePositions)
  * [Moving a module within a hook](positions.md#Positions-Movingamodulewithinahook)
  * [Attaching a module to a hook: Transplanting](positions.md#Positions-Attachingamoduletoahook:Transplanting)
  * [Editing an attached module](positions.md#Positions-Editinganattachedmodule)
  * [Removing a module from a hook](positions.md#Positions-Removingamodulefromahook)
  * [Transplanting a module by modifying its code](positions.md#Positions-Transplantingamodulebymodifyingitscode)
  * [Widgets](positions.md#Positions-Widgets)

A module can have two views: one on the back office (its options, or even a configuration screen), and one on the front office. The front office view is how and where the module is displayed within your shop's theme.

The position of a module in your theme can be changed, because you might want one module's block to be placed much higher (or lower) in the page that others. In PrestaShop's parlance, this is called "transplanting", and is done using the tool available in the "Positions" page, under the "Design" menu. In effect, this enables you to attach a module to one of the many available hooks in the current theme, without writing any code.

The "Positions" page displays all the available hooks and their attached modules. Many are empty by default, but some of the most useful ones can have a dozen of modules.

![](<../../../.gitbook/assets/64225563 (6).png>)

At the top of the page, a drop-down menu enables you to only display the module in which you are interested. Alternatively, you can also search for a specific hook. By default, this page only displays the hooks on which you can position functions. Checking the "Display non-positionable hooks" box below displays all the hooks, even the invisible ones, that are linked to an action for an instance.

The header of the table for each hook displays the hook's name, a quick description (when available), and its number of attached modules. The table lists the modules that are attached to that hook. The modules are displayed in the order in which they appear in the hook.

## Moving a module within a hook <a href="#positions-movingamodulewithinahook" id="positions-movingamodulewithinahook"></a>

You have two ways of changing a module's position within a hook:

* Click the up or down arrow. The page will reload and display the new order.
* Drag and drop the module's row itself:
  1. Place the mouse cursor on the position number to have it change into a "move item" cursor.
  2. Click and hold while moving the cursor over the row/position where you want the module to be: the module's row changes position accordingly.
  3. Release the mouse button: the current position for the module is saved.

For most modules, transplantation can easily be done directly via the back office. Some modules require you to alter their code in order to transplant them.

## Attaching a module to a hook: Transplanting <a href="#positions-attachingamoduletoahook-transplanting" id="positions-attachingamoduletoahook-transplanting"></a>

In PrestaShop, "transplanting" is the action of attaching a module to a hook. You can add a module to more than one hook.

Two things to know before transplanting a module:

* Some modules are written to only be attached to a given set of hooks.
* Some hooks are written to not accept some specific kinds of modules.

Therefore, be aware that you cannot always transplant any module to any hook.

Make sure to disable the cache when testing the effect of a new module on the front-end. You can do this in the "Performance" page, under the "Advanced Parameters" menu.

The transplanting process has its own interface:

1. Go to the "Design" menu, and its "Positions" page.
2. Click the "Transplant a module" button at the top right. The transplanting interface appears.
3. In the "Module" drop-down list, select the module you want to transplant.
4. In the "Transplant to" drop-down list, select where you want to transplant the module to. There are many hooks available. You can change your settings later if needed.
5. In the "Exceptions" field, type the name of the file(s) of the pages in which you do not want the module to appear.\
   You can perform multiple selections simply by clicking on the file names while keeping the Ctrl key pressed. You can deselect files in the same manner: Ctrl+click.
6. Do not forget to save your changes.\
   \


![](<../../../.gitbook/assets/51839907 (4) (3).png>)

The "Transplant to" drop-down menu gives you a good idea where modules can be placed.

Even though the "Transplant to" drop-down list gives a comprehensive overview of the available hooks, it might not always be clear which is the one to which you want to attach your module. Do not hesitate to try another hook if the result of your selection if not what you expect. The list gives some details: some hook have a description after the hook's name, for instance, "Add fields to the form 'attribute value'" for `displayAttributeForm`. Peruse them all in order to choose your hook correctly.

## Editing an attached module <a href="#positions-editinganattachedmodule" id="positions-editinganattachedmodule"></a>

Each module has an action button on the right side of its row, with two possible options: one to edit its settings, the other one to delete the module.

Editing a module's setting uses the same interface as the one used for transplanting a module. The only difference is that you cannot change the "Module" field, as it is disabled, and thus grayed out. You can edit both the "Transplant to" setting and the exceptions, which works just as described in the "Attaching a module to a hook" method above.

![](<../../../.gitbook/assets/64225504 (4) (5) (7).png>)

Always check your front office to make sure the module is indeed where you intended it to be.

## Removing a module from a hook <a href="#positions-removingamodulefromahook" id="positions-removingamodulefromahook"></a>

There are two ways to remove a module from a hook:

* Removing a single module: click the trashcan icon on the right of the module's row.
* Removing a batch of modules: select the modules by checking the box on the left of their row, and then click the "Unhook the selection" button, found at the top and the bottom of the list of hooks.

## Transplanting a module by modifying its code <a href="#positions-transplantingamodulebymodifyingitscode" id="positions-transplantingamodulebymodifyingitscode"></a>

This is for experts only: you must have a good knowledge of PHP and HTML before attempting anything with the code of a module.

Some modules cannot be transplanted into other sections of the front office simply because they lack the necessary code. For example, some modules contains templates for both column display and header display, whereas others have one template file which only works with the header section.&#x20;

If you want to display simple modules in a position for which it was not built, you will have to edit its template files. More complex modules can also be made to be displayed in other sections of the page, but they might have to be partly rewritten in order to have their design work with that new location.

To customize the transplantation ability of a module, you must give it the correct PHP function for the new target hook. For example, for a module that has this function:

```
function hookTop($params) { ... } 
```

In order to transplant its block into the right column, for instance, you need to add the `hookRightColumn()` function:

```
function hookRightColumn($params) { ... } 
```

Afterward, you must write the code that displays the content on the front page. At best, that means copy/pasting the content of the `hookTop()` function; at worst, you need to rework the content of `hookTop()` function into something that will work for the new location.

## Widgets <a href="#positions-widgets" id="positions-widgets"></a>

PrestaShop 1.7 has introduced a new system to hook modules: widgets. Thanks to widgets, a module can be used and transplanted to any display hook.

Widgets work with 1.7 modules only (for PrestaShop modules, their technical names start with "ps\_"), and cannot be used on all the modules. Read more about widgets here: [https://devdocs.prestashop.com/1.7/modules/concepts/widgets](https://devdocs.prestashop.com/1.7/modules/concepts/widgets/)
