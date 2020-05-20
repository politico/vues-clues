# Vue's Clues

Snippets of more obscure Vue.js experiences @ POLITICO, captured in quick code demos & explanations

## [Compile Vue.js templates on the Fly](https://codepen.io/ivan-shtyrliaev/pen/NWGdLYx)

**Note! Only available in the full build.**  
Sometimes you may end up needing to compile a template on the fly. For example, you get HTML code from your back-end server with inner links and you don't want your site to reload clicking on that links. Normally, you would have router-link component. But here it's just tag link "a"

    <a href="/some/inner/path">SomeLink</a>
Using v-html does not allow you to do this. In this case, you need to change links to router-link components and compile HTML string