# cheatsheet

### To set up env
- install ruby jekyll bundler gems: `gem install jekyll bundler`
- create a new template blog: `jekyll new myblog`
- compile and run on localhost:4000 : `bundle exec jekyll serve`

Gemfile is similar to package.json
It has dependencies, plugins and itself a gem.

Bundler installs and serves your jekyll site with version dependencies from gemfile.

- compiles the static site and places contents in _site directory: `jekyll build`
- watches your directory and compiles and runs when changes are made: `jekyll serve`

### Liquid is a templating language similar to hugo.

- Objects output content as {{page.title}}
- tags are denoted by {% comment %} `{% wwdwd %}` {% endcomment %}  and they control flow and logic
- filters are similar to pipes in angular: They modify outputs: `{{ "hi" | capitalize }}`

- front matter is used to set varibales for a page:
    Represented as 
    ```yaml
    ---
    my_number: 5
    ---```
- front matter properties are accessible under page object acessed with dot notation.

### Layout
- Layouts are under _layout folder

Additional jekyll gems
