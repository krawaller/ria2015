<img class="toprightimg" src="http://jshint.com/res/jshint-dark.png"/>

###What JSHint is

JSHint is a "code linting library", that is, it parses your JavaScript code and warns you when something seems off. It is primarily used to catch syntax errors, but it can also enforce stylistic choices. The former, catching syntax errors, is a real time saver, and no JS developer worth his salt would ever want to work without JSHint or an equivalent library.

The latter, enforcing certain coding styles, becomes important in a collaborative project where many chefs are stirring the same soup, all having their individual styles and preferences.

JSHint can be configured using a special comment block at the top of the file to be parsed, but more commonly the settings are store in a separate file named `.jshintrc` which is stored at the root of the project. Most modern editors will then automatically find the file and apply it to all JavaScript files in the project.

###An example

Here's an example of a `.jshintrc`-file. As you can see it is a simple JSON object where the keys are the different JSHint options. Most of them are simply set to true, while a few take a number value.

It is not necessary to include a setting just to set it to false, as is the case for some settings below. The reason to do that is probably to make it easier to turn the setting back on should the user later on wish to do so.

<pre><code>{
    "<span class="hljs-attribute">maxparams</span>": <span class="hljs-value"><span class="hljs-number">5</span></span>,
    "<span class="hljs-attribute">maxdepth</span>": <span class="hljs-value"><span class="hljs-number">5</span></span>,
    "<span class="hljs-attribute">maxstatements</span>": <span class="hljs-value"><span class="hljs-number">25</span></span>,
    "<span class="hljs-attribute">maxcomplexity</span>": <span class="hljs-value"><span class="hljs-number">10</span></span>,
    "<span class="hljs-attribute">node</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">browser</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">boss</span>": <span class="hljs-value"><span class="hljs-literal">false</span></span>,
    "<span class="hljs-attribute">curly</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">debug</span>": <span class="hljs-value"><span class="hljs-literal">false</span></span>,
    "<span class="hljs-attribute">devel</span>": <span class="hljs-value"><span class="hljs-literal">false</span></span>,
    "<span class="hljs-attribute">eqeqeq</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">evil</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">forin</span>": <span class="hljs-value"><span class="hljs-literal">false</span></span>,
    "<span class="hljs-attribute">immed</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">laxbreak</span>": <span class="hljs-value"><span class="hljs-literal">false</span></span>,
    "<span class="hljs-attribute">newcap</span>": <span class="hljs-value"><span class="hljs-literal">false</span></span>,
    "<span class="hljs-attribute">noarg</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">noempty</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">nomen</span>": <span class="hljs-value"><span class="hljs-literal">false</span></span>,
    "<span class="hljs-attribute">onevar</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">plusplus</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">regexp</span>": <span class="hljs-value"><span class="hljs-literal">false</span></span>,
    "<span class="hljs-attribute">undef</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">sub</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">strict</span>": <span class="hljs-value"><span class="hljs-literal">false</span></span>,
    "<span class="hljs-attribute">white</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">unused</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">nonew</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">bitwise</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">latedef</span>": <span class="hljs-value"><span class="hljs-literal">true</span></span>,
    "<span class="hljs-attribute">nonbsp</span>": <span class="hljs-value"><span class="hljs-literal">true</span>
</span>}
</code></pre>


###Using JSHint in the course

Unlike in previous iterations of the course, using JSHint is **not** mandatory. If you do use it, please present the contents of your `.jshintrc`-file in a blog post and explain your choices.

And even if you don't "officially" use JSHint you are **strongly** recommended to make sure you have some kind of syntax checker in your editor, especially if you are somewhat new to coding with JavaScript. This will save you lots and lots of time.



###What style rules should I use?

This is entirely up to you! However, we'd like to make two recommendations:

*    The `newcap` setting (which makes you have to use `new` when invoking a function starting with a capital letter) should be `false`, or JSHint might choke on the JSX-compiled code.
*    It is a very good idea to use the complexity dampening settings `maxparams`, `maxdepth`, `maxstatements` and `maxcomplexity`! You can read up on them [here](http://www.elijahmanor.com/control-the-complexity-of-your-javascript-functions-with-jshint/).


###Other options

There are other linting solutions out there. The most viable alternatives are perhaps [ESLint](http://eslint.org/) and the original [JSLint](http://www.jslint.com/).