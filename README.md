# vscode-config

These are some of my favorite add-ons and extensions for VS Code.

&nbsp;

## Getting Started

&nbsp;

### What You Will Need

**Install [VS Code](https://code.visualstudio.com/)**. VS Code is a light weight IDE for doing just about any type of development given you have the right extensions installed. 

&nbsp;

### Clone the repo:

You can optionally choose to download the repo as a zip but cloning will make sure you can get latest updates when I make them.

```sh
$ git clone https://github.com/dallen2525/vscode-config.git
```

&nbsp;

### Copy the desire config to the root of your project
1. Pick a preferred color mode (see section below for assistance). Copy the respective .vscode directory into the root of your project.

VS Code detects suggested add-ons and local configurations based on the existence of a .vscode file in the root of the project. Simply copy the .vscode folder and it's contents to the root of your project and if you have the extensions installed; the theme should just take over.

If you don't have the extensions installed then you should...
1. Close the VS Code IDE
2. Re-Open the project where you just added the .vscode folder in the root
3. After opening a notification will pop up in the bottom right corner suggesting that you install project recommended addons. Hit "Install All Recommended"
4. Wait for the installs to finish. If the theme doesnt take effect then another simple restart of the IDE should force the change.

&nbsp;

2. (optional) If you would also like to use my editor configuration you can copy the .editorconfig file from the root of this project to the root of your own project. Make sure to install the Editor Config extension.

&nbsp;

## Decide which config best suites you

I have provided 3 different configurations. They are more or less just different themes. 

&nbsp;

#### Light Mode

I used to default to dark mode for development. It almost evokes this sensation of being a hacker (I know; lame). However, I watched a [YouTube video](https://www.youtube.com/watch?v=bCaFRN3aaP8) that talked about whether dark mode is really better for us. 

In summary: When you are doing tasks that require a lot of focus on text; It is actually better to use light mode themes. Using dark mode makes it more straining for our eyes to focus on text. After a long day of coding this can result it fatigue. I decided to find a good light mode setup which had good color contrast. The result is my light mode setup which is now my default configuration for projects that I work in the most.

**Theme**: Winter Is Coming (Light)
**Icons**: Material Icon Theme

&nbsp;

#### Color Mode

As a UX designer; going full dark mode or full light mode can sometimes get boring. In my hunt for some of the best themes I stumbled across a purple theme that I really enjoyed. While I likely wouldnt want to spend my entire day coding in this environment; It is a nice change of pace to spice things up. I like to use this for Node API projects. That way I can have my web projects (where I spend most of my time) in light mode while having the associated API projects in color mode. The stark difference ensures that I am never confused about which project I am making changes in.

**Theme**: Shades of Purple
**Icons**: Material Icon Theme

&nbsp;

#### Dark Mode

Likely the chosen path for most folks out there. Dark mode is still a favorite despite research showing that is can cause fatigue. If this is your cup of tea then I always suggest the tride and true Dracula Official theme. No other dark mode provides the perfect balance of contrast that you get with Dracula. Out of the box is is great and it stylizes the code in such a way that it is easy to follow. 

**Theme**: Dracula Official
**Icons**: Material Icon Theme

&nbsp;

### Other theme elements used across all modes

&nbsp;

### Bracket Coloring

Brackets make it easy to track where something opens and closes in code. Specifically helpful for HTML and JSX. While VS Code has built in brackets highlighting; they are sometimes difficult to distinguish still. Bracket Colorizer is a great way to bring some color into your code while providing meaningful value. You can tell which items are tied together based on their color which is driven by a configured series of colors. I chose the colors in this config because they contrasted well with all of the color modes above. 

&nbsp;

### Guides

Guides are the vertical lines that provide further clarity to where something opens/closes. It pairs nicely with Bracket colorizer. I used to get this from Power Tools for Visual Studio back in the day. This is the best for getting a similar feature in VS Code. This needs to be explicitly turned on. A notification should prompt you in the bottom right corner. Just say Yes!

&nbsp;

## Understand what these add-ons are doing

(In alphabetical order. Not order of how awesome they are)

- **Auto Import** *must have*: This is great because it automatically imports dependencies to files without you having to scroll to the top and add it manually. Combined with intellisense; auto import makes it easy to code faster with fewer import errors.

- **Babel ES6/ES7 + Babel Javascript**: Not a lot to say here. They are 2 of the most installed and for those of you writing javascript they will come in handy. I myself have gone full on TypeScript and the usefulness of these extensions has somewhat been lost. 

- **Bracket Pair Colorizer 2** *must  have*: I explain the benefits of this plugin in the section below titled "Other theme elements used across all modes". It is just a personal preference. Take it or leave it. It is included in the config whether you use it or not.

- **Debugger for Chrome** *must have*: We all need to troubleshoot and debug. Assuming that you use Chrome as your primary development browser; This is a must have.

- **DotENV** *must have for me. maybe not for you*: How you manage local development variables is up to you or your team. If you are not using environment variables then you certainly should be. Hard coding environment values is bad practice. If you are using environment variables then DotENV is just one of many ways to implement it into your code. I find DotENV to be easy to use and a common practice across projects that I follow. Having the extension doesnt add much value beyond just syntax highlighting.

- **Dracula Official** *used for dark mode*: See the theme section regarding Dark Mode.

- **EditorConfig for VS Code** *must have for me. maybe not for you*: How you manage code preferences is likely ip to your or your team. This is just one way of standardizing it across all of my projects because I can move the config around. Your team may have their own preferences which would trump your own. 

- **ESLint** *must have for javascript writers*: If you are writing javascript then you should be linting it to ensure best practice and consistency.

- **GitLens** *must have*: We likely all use git considering that you got to this project via Github. GitLens is a great way to get greater insights into changes in the code. Invaluable when working on a team.

- **Guides** *must have*: I explain the benefits of this plugin in the section below titled "Other theme elements used across all modes". It is just a personal preference. Take it or leave it. 

- **HTML CSS Support + HTML Snippets**: If you write a lot of HTML and are doing CSS styling then this syntax highlighting and code snippet extension could prove to be useful. I still install it for the off chance that I work on a simple HTML file.

- **Material Icon Theme** *must have*: The best in class icon extension chances from time to time. This is the current flavor of the week. It works great for my project naming conventions and the recognition of third party files is second to none. I use it across all of my theme modes.

- **Path Intellisense** *must have*: This pairs perfectly with Auto Import. Auto Import handles it 90% of the time but when you do need to manually type the path to a file this tool is extremely helpful. No guessing at the path anymore.

- **Prettier - Code Formatter** *must have for me. maybe not for you*: As the title states; this is a code formatter. This is also the most opinionated item on the list most likely. There are basicall 2 popular choices in this category. Beautify and Prettier. Beautify is *less opionated* with *more extensive configuration*. Prettier is *more opinionated* with *less configuration*. This comes down to personal preference and team. I like and agree with the out of the box Prettier opinions. Combined with my very light editor config I have struck the perfect balance of readability and function (IMO). Having this extension installed allows me to exclude it from my transpiler and instead only execute code cleanup if I explicitly turn it on via my IDE. The configs provided in this repo all expect you to use Prettier and your code will format automatically on file save. At the end of the day I want the easiest option to propogate across my team. Consistency across team members is the most important thing. Not what the formatting rules are but rather that all team members are consistent. Prettier, with it's opinions, makes it easier to propogate without configuration. Instead of arguing about who is right; we all just agree that Prettier is right and blame the extension when we don't like something!

- **Shades of Purple** *used for color mode*: See the theme section regarding Color Mode.

- **TSLint** *must have*: TypeScript is great and if you are writing it then you should be linting it. 

- **Version Lens** *nice to have**: When working on personal projects I like to keep all dependencies up-to-date. This helps visualize that and add context right inside of your package.json. For enterprise projects this is less of a concern since you likely wont be updating your dependencies constantly. 

- **Visual Studio IntelliCode**: Honestly, I saw this recently. Thought it looked and sounded good. Take it or leave it.

- **Winter is Coming Theme** *used for light mode*: See the theme section regarding Light Mode.

&nbsp;

## Closing Remarks

Add-ons are very personal to the individual. These are just my preferences. I keep an open mind to alternatives and I am always happy to try something new. Years of micro decisions have resulted in this outcome and I hope that by compiling these configurations; You will benefit from my time spent.

Enjoy and Happy Coding!
