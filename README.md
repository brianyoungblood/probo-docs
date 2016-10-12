# Probo documentation

The docs (will soon) live at https://docs.probo.ci.

## Contributing

Want to contribute to the docs? Have a fancy `.probo.yaml` file you want to show off? See something outdated that we missed? It's as simple as opening a pull request with some changes.

### Contribute documentation

The docs are written in markdown format and live in the `docs` directory. To contribute:

1. Submit your changes in a pull request.
2. Add the **needs review** label.

That's it! We'll take care of wiring any new pages into the menu.

Need a markdown primer? Check out Adam Pritchard's [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

##### To use syntax highlighting with numbers use this format
 ```
 {% highlight ruby linenos %}
 def foo
   puts 'foo'
 end
 {% endhighlight %}
 ```

 ```
 {% highlight css linenos %}
 body {
   background: red;
 }
 {% endhighlight %}
 ```
##### To use syntax highlighting without numbers use this format:
 ```
 {% highlight yaml %}
 var cli = new ArgumentParser({
   prog:     'js-yaml',
   version:  require('../package.json').version,
   addHelp:  true
 });
 {% endhighlight %}
 ```

### Contribute your .probo.yaml recipe

You can share your super slick `.probo.yaml` in just a few steps:

1. Create a markdown file in the `_recipes` directory and paste in the following template.
 ```
 ---
 title:
 category:
 author:
 github:
 ---

 {% highlight yaml %}

  Your yaml goes here!

 {% endhighlight %}
 ```
2. Enter a title and category*. You can optionally add you or your organization's name as you would like it displayed and your GitHub username so we can link to your profile.
3. Paste the contents of your `.probo.yaml` file between the `highlight yaml` tags.
4. Submit a pull request and add the **needs review** label.

*The category will group your `.probo.yaml` file with other files of the same category on https://docs.probo.ci/build/recipes. It should be the most specific need your file addresses (e.g. Drupal, Pantheon). This is an interim solution until we implement a nice filtering system on the page. :simple_smile: