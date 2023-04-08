<h1 align="center">
  <br>
    <img align="center" src="img/logo.png" width="200">
  <br>
	<br>
  Humane JS Snippets
  <br>
  <br>
</h1>
<h4 align="center">Descriptive, easy to find JavaScript snippets.</h4>
<br/>
<p align="center">
<img src="https://img.shields.io/static/v1?logo=visual-studio-code&label=made%20for&message=VS%20Code&color=0000ff" alt="Made for VSCode">
<img src="https://img.shields.io/visual-studio-marketplace/v/robole.javascript-snippets?logo=visual-studio-code&color=ffa500" alt="Visual Studio Marketplace Version">
<img src="https://img.shields.io/static/v1?logo=visual-studio-code&label=size&message=20KB&color=008000"
alt="Extension file size in bytes">
<img src="https://img.shields.io/visual-studio-marketplace/r/robole.javascript-snippets?logo=visual-studio-code&color=yellow" alt="Visual Studio Marketplace Rating">
<img src="https://img.shields.io/visual-studio-marketplace/d/robole.javascript-snippets?logo=visual-studio-code&color=blue" alt="downloads"/>
<img src="https://img.shields.io/visual-studio-marketplace/i/robole.javascript-snippets?logo=visual-studio-code&color=blue" alt="installs"/>
<img src="https://img.shields.io/static/v1?label=built%20with&message=good%20vibrations&color=purple" alt="Built with"/>
<a href="https://ko-fi.com/roboleary"><img src="https://img.shields.io/badge/Buy%20me%20a%20coffee-$4-orange?logo=buy-me-a-coffee" alt="Buy me a coffee"></a>
</p>

> This extension is **published for education purposes**, in support of the article - [VS Code - How to write great snippets that anyone can use](https://www.roboleary.net/2021/08/23/vscode-snippets-are-not-aliases.html). It is not open for changes.

Most snippet collections resemble bash aliases. You have a list of nonsense abbreviations such as: "imp", "clg", "fre". You must learn these to use them. 🤕

There is a better way!

Snippets are not confined to using a single word as the trigger (prefix), quick suggestions offered by VS Code are produced from a fuzzy substring search on the prefix. This means we can use spaces in prefixes, and be more descriptive to make our snippets easier to discover.

For example, you want to find an array function, but you're not sure which to use. Just type "arr" and you get a list of array functions with descriptions:

![example with suggested array functions](img/array-functions.gif)

In future, you know you want to use the `filter` function, just type "filt" or some variation, and you will get that as the first suggestion. 🔥

## Activation

These snippets are available for the follow [language identifiers](https://code.visualstudio.com/docs/languages/identifiers):
- `javascript`
- `javascriptreact`
- `typescript`
- `vue`
- `svelte`

## Snippets

You can install the [Snippets Ranger extension](https://marketplace.visualstudio.com/items?itemName=robole.snippets-ranger) to view the full list of snippets inside VS Code.

I didn't repeat any of the builtin JavaScript snippets (see FAQ section for more info on builtin snippets).

<table>
<thead>
  <tr>
    <th>Prefix</th>
    <th>Description</th>
    <th>Body</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>array concat</td>
    <td>Joins two or more arrays, and returns a copy of the joined arrays</td>
    <td>let ${1:newArray} = ${2:array1}.concat(${3:array2});<br>$0<br></td>
  </tr>
  <tr>
    <td>array copyWithin</td>
    <td>Copies array elements within the array, to and from specified positions. Syntax: array.copyWithin(target, start, end).</td>
    <td>${1:array}.copyWithin(${2:target}, ${3:start}, ${4:end});<br>$0<br></td>
  </tr>
  <tr>
    <td>array every</td>
    <td>Checks if every element in an array pass a test.</td>
    <td>let ${1:boolean} = ${2:array}.every((${3:item}) =&gt; {<br> $4<br>});<br>$0<br></td>
  </tr>
  <tr>
    <td>array fill</td>
    <td>Fill the elements in an array with a static value.</td>
    <td>${1:array}.fill(${2:target}, ${3:start}, ${4:end});<br>$0<br></td>
  </tr>
  <tr>
    <td>array filter</td>
    <td>Creates a new array with every element in an array that pass a test</td>
    <td>let ${1:newArray} = ${2:array}.filter((${3:item}) =&gt; {<br> $4<br>});<br>$0<br></td>
  </tr>
  <tr>
    <td>array find</td>
    <td>Returns the value of the first element in an array that pass a test.</td>
    <td>let ${1:result} = ${2:array}.find((${3:item}) =&gt; {<br> $4<br>});<br>$0<br></td>
  </tr>
  <tr>
    <td>array findIndex</td>
    <td>Returns the index of the first element in an array that pass a test</td>
    <td>let ${1:result} = ${2:array}.findIndex((${3:item}) =&gt; {<br> $4<br>});<br>$0<br></td>
  </tr>
  <tr>
    <td>array includes</td>
    <td>Check if an array contains the specified element. It is case sensitive.</td>
    <td>let ${1:boolean} = ${2:array}.includes(${3:element}, ${4:start});<br>$0<br></td>
  </tr>
  <tr>
    <td>array indexOf</td>
    <td>Search the array for an element and return its position.</td>
    <td>let ${1:index} = ${2:array}.indexOf(${3:item}, ${4:start});<br>$0<br></td>
  </tr>
  <tr>
    <td>array map</td>
    <td>Creates a new array populated with the results of calling the provided function on every element in the array.</td>
    <td>let ${1:newArray} = ${2:array}.map((${3:item}) =&gt; {<br> $4<br>});<br>$0<br></td>
  </tr>
  <tr>
    <td>array push</td>
    <td>Add new items to the end of an array.</td>
    <td>${1:array}.push(${2:items});<br>$0<br></td>
  </tr>
  <tr>
    <td>array reduce</td>
    <td>Reduce the values of an array to a single value (going left-to-right).</td>
    <td>let ${1:newValue} = ${2:array}.reduce((sum, currentValue) =&gt; {<br> $4<br>});<br>$0<br></td>
  </tr>
  <tr>
    <td>array reduceRight</td>
    <td>Reduce the values of an array to a single value (going left-to-right).</td>
    <td>let ${1:newValue} = ${2:array}.reduceRight((sum, currentValue) =&gt; {<br> $4<br>});<br>$0<br></td>
  </tr>
  <tr>
    <td>array slice</td>
    <td>Selects a part of an array, and returns the new array.</td>
    <td>let ${1:newArray} = ${2:array}.slice(${3:start}, ${4:end});<br>${0}<br></td>
  </tr>
  <tr>
    <td>array some</td>
    <td>Checks if any of the elements in an array pass a test.</td>
    <td>let ${1:result} = ${2:array}.some((${3:item}) =&gt; {<br> $4<br>});<br>${0}<br></td>
  </tr>
  <tr>
    <td>array splice</td>
    <td>Adds/Removes elements from an array.</td>
    <td>${1:array}.splice(${3:index}, ${4:howManyToRemove}, ${5:newItems});<br>${0}<br></td>
  </tr>
  <tr>
    <td>array unshift</td>
    <td>Adds new elements to the beginning of an array, and returns the new length.</td>
    <td>${1:array}.unshift(${3:items});<br>${0}<br></td>
  </tr>
  <tr>
    <td>array destructure</td>
    <td>Assign values from array elements to new variables using destructuring.</td>
    <td>const [${1:variables}] = ${2:arrayName};<br>$0<br></td>
  </tr>
  <tr>
    <td>json parse</td>
    <td>Parses a JSON string and returns a JavaScript object</td>
    <td>let ${1:obj} = JSON.parse(${2:string});<br>$0<br></td>
  </tr>
  <tr>
    <td>json stringify</td>
    <td>Convert a JavaScript object to a JSON string.</td>
    <td>let ${1:string} = JSON.stringify(${2:obj});<br>$0<br></td>
  </tr>
</tbody>
</table>

## FAQ

### 1) Where are the builtin JavaScripts?

There is a set of snippets for the JavaScript installed with VS Code as part of the built-in JavaScript extension. [This is the source file](https://raw.githubusercontent.com/microsoft/vscode/94c9ea46838a9a619aeafb7e8afd1170c967bb55/extensions/javascript/snippets/javascript.code-snippets).

You can see these inside VS Code by:
1. By opening a JavaScript file and running the commmand `Insert Snippet`, which gives a list of the snippets in the dropdown.
1. The [Snippets Ranger extension](https://marketplace.visualstudio.com/items?itemName=robole.snippets-ranger) will show you the built-in snippets organised into groups in a good-looking webview.

### 2) How do you get snippets to be shown at the top of the suggetion list?

Snippets are mixed in with other suggestions, and by default they are placed towards the end of the list. To promote suggestions to the top of the list, you can set `editor.snippetSuggestions": "top"` in your `settings.json`.

### 3) How do I use the snippets?

To insert a snippet, you can just type one of the prefixes in a JavaScript file, and you will be offered a completion suggestion. The setting `Editor: Snippet Suggestions` controls whether snippets are shown with other suggestions and how they are sorted. By default, they are shown inline.

Alternatively, you can open the Command Palette (`Ctrl+Shift+P`) and run the command "Insert Snippet", which presents you with a list to choose from.

### 4) How do I add shortcuts for the snippets?

Run the command `Preferences: Open Settings (UI)` to open the keyboard shortcuts config. Add an new object to the array such as this:

```JSON
[

	{
		"key": "ctrl+t",
		"mac": "cmd+t",
		"command": "editor.action.insertSnippet",
		"when": "!editorReadonly && editorLangId == javascript",
		"args": {
			"langId": "javascript",
			"name": "arrow function"
		}
	}
]
```

The `args.name` property <u>must exactly match</u> the snippet name.

### 5) Where can I learn more about snippets?

You can read my comprehensive guide on Snippets on FreeCodeCamp: [Visual Studio Code Snippets – the Definitive VS Code Snippet Guide for Beginners](https://www.freecodecamp.org/news/definitive-guide-to-snippets-visual-studio-code/). It's not just for beginners! 😉

## Image Attribution

Logo inspired by [Brain by Nithinan Tatah from the Noun Project](https://thenounproject.com/search/?q=brain&i=2452319).
