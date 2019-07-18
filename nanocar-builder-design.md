---
layout: post
title: Nanocar Builder Design
description: UI design for the nanocar builder
nav-menu: true
---

We want to build the most user friendly molecule editor of the web with an emphasis on building nanocars.
Our aim is to apply the familiarity and simple UI design of popular CAD tools to molecular science.
In other words, we want to build an editor that is straight forward to use, doesn't require you to
search through layers of menus and allows you to perform a wide range molecular operations easily.

## User Interface
The user interface has three components, the main window for visualizing molecules, a sidebar
on the left to perform various operations and an axis helper on the top right. You can navigate the view with the left mouse button and zoom in and out with the mouse wheel. The background and the menu is designed to be easy on the eyes but still include the most commonly used functions.
<img src="/assets/images/ui/nanocar-builder-ui.png">

### Expandable menus
The sidebar consists of several expandable menu buttons.
As you click, the menu is expanded to the right to show the options as seen below.
<img src="/assets/images/ui/nanocar-builder-ui-menu.png">

<div class="row">
  <div class="4u 12u$(medium)">
    <h3>File</h3>
    <p>The file menu would be used to load and save molecules
    into a file. Initially simple and commonly used file formats
    such as <code>cjson</code>, <code>xyz</code>, <code>pdb</code>, and <code>cif</code> would be supported.</p>
  </div>
  <div class="4u 12u$(medium)">
    <h3>Build</h3>
    <p>The build menu would consist of custom build operations. Initially these would be functions such as
    adding a chassis molecule, connecting a wheel molecule, and
    building a metal surface. More custom build operations can be
    supported as the editor is developed.</p>
  </div>
  <div class="4u$ 12u$(medium)">
    <h3>Edit</h3>
    <p>The edit menu opens editable options for what is selected. This could be changing elements, resizing, coloring atoms, joining/separating molecules and more.</p>
  </div>
</div>

### Toggle buttons with pop-up windows
The toggle buttons are highlighted as you click on them and they
can open pop-up windows according to their function.
<img src="/assets/images/ui/nanocar-builder-ui-atom-select.png">

<div class="12u 12u$(medium)">
  <h3>Select</h3>
  <p>The select menu allows users to select atom(s), bond(s), or molecule(s). Additionally the box select tool could be used together with these options. For example clicking both atom, and box select would enable selecting all the atoms in the box. As the user selects an atom for example this would  open a pop-up window on the right showing information about the selected atom. This includes element name, which molecule it belongs to, which atoms it's bonded to and its visualization settings such as size and color. Some of these are highlighted in blue meaning that they could be clicked. For example you could click the molecule to select the whole molecule, or click one of the bonded atoms to select it. You could imagine similar menus showing up for different selections. For example, if you would like to select a molecule, you would click the third button from the top in the select menu. This would again open a pop-up windows this time showing information about the whole molecule such as it's composition, molecular weight, and more.</p>
</div>

<div class="row">
  <div class="5u 12u$(medium)">
    <h3>Arrange</h3>
    <p>The arrange menu would be used to perform geometric operations on the atom(s) or molecule(s). These include translation, rotation, and reflection. A small pop-up window would open as you click on the buttons that would let you select parameters. For example when you want to rotate a molecule you would be able to select an axis and an angle of rotation.</p>
  </div>
  <div class="7u$ 12u$(medium)">
    <h3>View</h3>
    <p>The view buttons would be used to adjust the camera view and molecular representions. The user can view the molecule through <code>x, y, z</code> axes by selecting from here or just using keyboard buttons (1, 2, 3). More detailed camera options would be set from the camera icon such as perspective/orthograhic view. The settings button would be used to set the molecular representations such as ball and stick, spacefill, and wireframe. This could be selected for each molecule separately.</p>
  </div>
</div>


## Contributing
We are developing this builder on [GitHub](https://github.com/formulanano/nanocar-builder-web) right now and we appreciate any help. Please check [our GitHub page](https://github.com/formulanano/nanocar-builder-web) and feel free to join the discussion on [our Discord server](https://discord.gg/zAnjADr).
