
<table align = 'left' >
<tr>
<td>

[« What does an **Addon** even do?][Page-Addon]

</td>
</tr>
</table>

<table align = 'right' >
<tr>
<td>

[How to use the **Template** repo »][Page-Template]

</td>
</tr>
</table>

<br/>
<br/>

# 2. Structure

In the following we will cover a modern way of  
structuring your addon, there are other ways  
to do this, but this is what we recommend.

You can find a bare bones example of the structure  
described below in our [Template] repository, don't  
worry about it yet, we will cover the setup later.

<br/>

## 📂 Overview

We have structured our template to use the latest  
features of FreeCAD while also keeping things tidy.

```
<Repository>
│
├─ Source
│  └─ freecad
│     └─ <Addon>
│        ├─ Resources
│        │  └─ Icons
│        │     └─ Addon.svg
│        ├─ __init__.py
│        └─ init_gui.py
│
├─ Assets
│  ├─ Documents
│  │  └─ Overview.md
│  └─ Images
│
├─ LICENSE-CODE
├─ LICENSE-ICON
├─ package.xml
└─ README.md
```

<br/>

## 📑 Files & Folders

Below you can find descriptions for each  
of the items listed in the above file tree.

<details>
<summary>
    
### `<Repository>`

This is the root of your repository.
    
</summary>

#### `.editorconfig`
Config that tells editors to use the same line endings,  
charset, indentation, etc. to keep things consistent.

#### `.gitignore`
Config that prevents certain files from being committed to  
git, like Python cache or files generated from editing UIs.

#### `LICENSE-CODE`
This is the license file for the code of your project.

#### `LICENSE-ICON`
This is the license file for the icons of your project.

#### `package.xml`
Config that tells FreeCAD about your addon, for example  
where it can find your files, your dependencies, links, etc.

#### `pyproject.toml`
Config to tell tools like [`uv`][UV] what dependencies we need  
while developing, like the Python stubs package for FreeCAD.

### `README.md`
The overview of your repository, in our template this is  
only for contributors, not for the users of your addon.

</details>

<details>
<summary>
    
### `Source`

Extra folder to make it easy for people  
to know which files are the source files.

</summary>

#### `freecad`
Folder with a set name needed to load your addon.

#### `<Addon>`
Folder with the name of your addon, for example `MagicTools`

#### `<Resources>`
Here you want to store the assets you package with  
your addon like icons, locales or data files you load.

#### `__init__.py`
This is the entry point to your code that is called when  
running FreeCAD from either the terminal or with a GUI.

#### `init_gui.py`
This is the entrypoint to your code that is called  
only when FreeCAD is ran as a GUI application.

</details>

### `Assets`
    
Media, Documents, etc. that aren't packaged with the  
addon like a cheatsheet PDF, header images or the like.

<br/>

[Page-Template]: ./Template.md
[Page-Addon]: ./Addon.md

[Template]: https://github.com/Wazzards/Template
[UV]: https://docs.astral.sh/uv/
