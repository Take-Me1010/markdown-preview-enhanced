Markdown Preview Enhanced
===
**By Yiyi Wang (shd101wyy)**   
Still Beta Version!  
This package was named `atom-markdown-katex` before.

Post [here](https://github.com/shd101wyy/markdown-preview-enhanced/issues) if you request new features or you want to report bugs ;)

(TOC below was generated by this package)
<!-- toc -->

- [Markdown Preview Enhanced](#markdown-preview-enhanced)
	- [Features](#features)
	- [How it works](#how-it-works)
	- [Usages](#usages)
	- [Preview Context Menu](#preview-context-menu)
	- [Settings Panel](#settings-panel)
	- [Extra](#extra)
	- [For Developer](#for-developer)
	- [Thanks](#thanks)
	- [TODO](#todo)

<!-- tocstop -->
---

![main](https://cloud.githubusercontent.com/assets/1908863/15383014/14ad19d0-1dc2-11e6-9385-acd90f53a831.gif)

## Features
- **2-way scroll sync**  
- markdown preview with math rendering support   
You can choose [MathJax](https://github.com/mathjax/MathJax) or [KaTeX](https://github.com/Khan/KaTeX) to render math expressions  
- export PDF    
- export beautiful HTML (mobile device supported)  
- customize Markdown Preview css  
- settings panel  
- [TOC] generation **(beta)**  
- Flowchart / Sequence Diagram **(beta)**  
- Task List *(Github Flavored)* **(beta)**  
- Image Helper **(beta)**
- [Footnotes](https://github.com/shd101wyy/markdown-preview-enhanced/issues/35)  
- And many more...

## How it works
- [remarkable](https://github.com/jonschlinkert/remarkable) to convert markdown to html
- [MathJax](https://github.com/mathjax/MathJax) or [KaTeX](https://github.com/Khan/KaTeX) to render math expressions. ([KaTeX Supported functions/symbols](https://github.com/Khan/KaTeX/wiki/Function-Support-in-KaTeX))
  - expression within `$...$` will be rendered normally.  
  - expression within `$$...$$` will be rendered in displayMode.   
  - You can choose your math rendering method from [settings panel](#settings-panel).   
		**MathJax** supports more symbols, but it has slower rendering speed compared to **KaTeX**.
  - <img src="https://cloud.githubusercontent.com/assets/1908863/14398210/0e408954-fda8-11e5-9eb4-562d7c0ca431.gif">
- [mermaid](https://github.com/knsv/mermaid) to render flowchart and sequence diagram  
	- code block within `mermaid` notation will be rendered by [mermaid](https://github.com/knsv/mermaid)  
	- check [mermaid doc](http://knsv.github.io/mermaid/#flowcharts-basic-syntax) for more information about how to create flowchart and sequence diagram   
	- <img src="https://cloud.githubusercontent.com/assets/1908863/15132962/468c0dd0-1624-11e6-868c-cf3033ce3b5d.gif">

## Usages
To use this package, press <strong> cmd + shift + p </strong> in atom editor first to toggle <strong> Command Palette </strong>. Then choose the commands below:
- <strong>Markdown Preview Enhanced: Toggle</strong>
  - Toggle Markdown file preview with KaTeX support.   
	You can also use the keymap `ctrl+shift+m` to toggle preview. (To use keymap, you have to disable the default [markdown preview](https://atom.io/packages/markdown-preview) package, otherwise there would be keymap conflict)
- <strong>Markdown Preview Enhanced: Customize CSS</strong>
  - Customize preview page css. You can edit styles inside `markdown-preview-enhanced-custom` section in `style.less` file.
- <strong>Markdown Preview Enhanced: Toc Create </strong>
  - Generate TOC
	 or simply insert ` <!-- toc -->` in editor (need preview toggled).
- <strong>Markdown Preview Enhanced: Toggle Scroll Sync </strong>
  - Enable/Disable scroll sync for preview.
- <strong>Markdown Preview Enhanced: Insert Table </strong>
  - Insert a markdown table.    
- <strong>Markdown Preview Enhanced: Image Helper</strong>  
	- With **Image Helper**(still beta), you can quickly insert image url and upload image to [imgur](http://imgur.com/) using imgur API.   
	Keymap `ctrl+shift+i`

## Preview Context Menu
**Right click at preview to see the menu**

![context menu](https://cloud.githubusercontent.com/assets/1908863/14586062/18852988-0451-11e6-9cc0-578d54384926.gif)

- <strong> Save as PDF </strong>
  - Create PDF in the same directory
- <strong> Save as HTML </strong>
  - Create HTML in the same directory
- <strong> Save as HTML (CDN) </strong>  
	- Create HTML in the same directory.
	- Require network connection to render correctly.
	- This method is different from **Save as HTML** as it will load javascript and css dependencies from `cdn.js` instead of doing so locally.
- <strong> Open in Browser </strong>
  - Open HTML in browser

## Settings Panel  
![settings_panel](https://cloud.githubusercontent.com/assets/1908863/15383036/44f79cb4-1dc2-11e6-80b3-3b3bdd9ab7d3.gif)

## Extra
* **Task List**  
	This package supports *Github Flavored* task list.  
	More information about how to create **task list** can be found [here](https://github.com/blog/1375-task-lists-in-gfm-issues-pulls-comments)
* **Smart Navigation**    
	You can quickly open another markdown file by clicking its link in preview.  
	![smart_navigation](https://cloud.githubusercontent.com/assets/1908863/15382175/e5f0a66e-1db9-11e6-9581-3f3ee8dc45dd.gif)  
* **Preview Auto Open**  
	Open preview pane automatically when you open a markdown file. You can disable this functionality from settings panel.
* **Image Helper**  
	Image Helper supports image url quick insertion, image paste, and image upload powered by [imgur](http://imgur.com/).
	![image_helper](https://cloud.githubusercontent.com/assets/1908863/15414603/c40b6556-1e6e-11e6-956c-090b5996ec87.gif)

## For Developer
Manual installation instruction can be found [here](./DEVELOPER.md)

## Thanks
Thanks for everyone that supports this package!   


## TODO
- [ ] fix bugs
- [ ] modify css to make preview look nice
- [ ] epub output
- [ ] support more image upload methods other than imgur (as imgur is blocked in some countries)
- [ ] image paste [#30](https://github.com/shd101wyy/markdown-preview-enhanced/issues/30)

Thanks for using and supporting this package ;)

> MIT License
