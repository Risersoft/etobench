---
title: Toolbar Commands
keywords: Toolbar Commands
sidebar: viscir_sidebar
permalink: visual-circuit/toolbar-commands.html
folder: VisualCircuit
hide_sidebar: false
comments: false
---

# Toolbar Commands

![](/images/toolbar-command.png)

VisualCircuit maintains a history of what you have viewed and allows you to navigate backwards and forwards using the **Back** and **Forward** commands.

You can click on the **Home** button to go to the starting screen which is the work orders screen.

You can click on the **Refresh** button to get the results again from the database server. In such case VisualCircuit remembers your custom sorting of columns and selected row and tries to maintain that as far as possible.

![](/images/toolbar-command-new.png)

The New menu allows you to create entities. Information on each entity can be found in the respective sections.

The Alter menu presents altering options for the currently selected row. Generally, the commands contained inside this menu are same as the ones contained inside the context menu obtained by right clicking on the selected row.

The Delete menu allows you to delete the selected row. On pressing the delete command contained inside this menu, a screen like following is presented –

![](/images/toolbar-command-delete.png)

The first tab on the right lists what needs to be deleted before deleting the selected row. The second tab lists what will also be deleted when the selected row is deleted.

If there is data in the first tab, the Delete Button on the lower right will be disabled and you need to first take care of the concerns listed on this tab. This button will be enabled and allow you to delete the selected row only when the first tab has no data.

This design helps to alert user of the consequences and also helps to maintain data integrity.
