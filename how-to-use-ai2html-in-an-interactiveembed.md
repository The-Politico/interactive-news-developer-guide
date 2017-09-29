# **How to use AI2HTML in the politico-interactive-generator:**

Repo w/ artboards and key elements: [https://github.com/The-Politico/tool\_ai2html](https://github.com/The-Politico/tool_ai2html)

### Steps:

1. When creating a new interactive, in your `templates` directory, create a folder called `ai`
2. Place `ai2html-resizer-html` \([https://github.com/The-Politico/tool\_ai2html/blob/master/ai2html-resizer.html](https://github.com/The-Politico/tool_ai2html/blob/master/ai2html-resizer.html)\) into your `ai` directory.
3. Add `{% include "ai2html-resizer.html" %}` at the bottom of your `_base.html` file.![](/assets/Screen Shot 2017-09-29 at 4.17.34 PM.png)

### Exporting artboards:

1. When creating assets in AI, you have a number of different art board sizes at your disposal. You can see the different sizes available to you here: [https://github.com/The-Politico/tool\_ai2html/blob/master/politico-graphics.ait](https://github.com/The-Politico/tool_ai2html/blob/master/politico-graphics.ait)
2. The artboard sizes that are essential for a project are **270px \(width\) for mobile **and then **400px or 600px** \(for iPad\). Our content well on an interactive page is 600px, so unless you are breaking outside of the well, you won't need larger artboards at 7**20px, 945px **or** 1050px.**
   1. A good example of using a larger artboard is when it needs to be lede art like here:  [http://www.politico.com/interactives/2017/trump-travel-ban-muslim-visa-decline/](http://www.politico.com/interactives/2017/trump-travel-ban-muslim-visa-decline/)
3. You need to **delete any unused artboards**, b/c AI2HTML will export them all.
4. Then save your ai file in the `ai` folder and run `ai2html` within illustrator \(Under `File` &gt; `Scripts` &gt; `ai2html`\)
   1. This generates your artboards and a partial \(with the name of your ai project\) in the root of `src`. Your partial is also generated, which you then include as a partial in your `index.html` file.
   2. You can make changes directly in CSS, but Jeremy’s work flow is to make the changes in AI and run the script again, as this will overwrite preexisting files \(including any custom CSS style changes you made\).



