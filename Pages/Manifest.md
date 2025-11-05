
# Manifest

The package manifest is a config that tells FreeCAD  
about your addon, where to find specific resources,  
what to link and what to display when presenting  
your addon in for example - the addon manager.

<br/>

## Format

The manifest is unfortunately an XML file so be careful  
with what you put where, you cannot for example move  
the top ( `<?xml` ) around much without breaking it.

The template includes a recommendation for an XML  
extension for VSCode that should help to avoid errors.

Currently the linked schema ( the `xmlns` attribute )  
does not offer any autocompletion or type hinting.

<br/>

## Fields

To give you a first impression of what data is included,  
here is a summary of the fields that are available for use.

<kbd> conflict </kbd> <kbd> replace </kbd> <kbd> name </kbd> <kbd> description </kbd> <kbd> maintainer </kbd> <kbd> author </kbd> <kbd> license </kbd>  
<kbd> icon </kbd> <kbd> content </kbd> <kbd> pythonmin </kbd> <kbd> file </kbd> <kbd> preferencepack </kbd> <kbd> subdirectory </kbd> <kbd> tag </kbd>  
<kbd> macro </kbd> <kbd> freecadmin </kbd> <kbd> freecadmax </kbd> <kbd> version </kbd> <kbd> bundle </kbd> <kbd> other </kbd> <kbd> workbench </kbd>  
<kbd> classname </kbd> <kbd> date </kbd> <kbd> depend </kbd>

<br/>

