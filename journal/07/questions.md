# Managing the Fullstack Application

1. Describe the two ways to bind Data in Vue?

  > The first way (standard data binding) can be done by using :prop="value", the other way (double data binding) can be done through the v-model property.

2. The `SPA` acronym stands for what?

  > SPA stands for Single Page Application.

3. What are some of the advantages/uses of a `SPA` over a traditional one?

  > Single-page applications have a huge benefit of improved loading speeds and responsiveness. Apart from this, they are also useful because they avoid page refreshes when switching between views.

4. What does the `onMounted` method in Vue do?

  > The onMounted method is a lifecycle hook that allows code to be ran when Vue loads or 'mounts' a component or page.

5. What is the `v-model` attribute in Vue for, and when might you use it?

  > The 'v-model' attribute is used for two way data binding, it's primary use is for forms. It allows a local variable to be updated when an input element is changed and an input element to be changed if the local variable changes. This makes is extremely useful for forms because you can use an object to automatically construct post data/objects for a post request.

6. What is the package.json file used for?

  > The primary purpose of package.json is to define script shortcuts and identify the entry point of/for an application. It can also be used to show metadata about a project's dependencies.

7. Which Vue attributes(directives) could you use to conditionally render elements on a page?

  > There are a few but honestly conditions could be used in any data-bound attribute to apply certain attributes or styles. In the case of enabled and disabling rendering specifically the attributes 'v-if' and 'v-else' are the best example.

8. What is the purpose of the `key` attribute when using `v-for` on an element?

  > The key attribute is used by Vue to keep track of iterations on the page.

9. What is the `<slot>` element and what is it used for?

  > The slot element is used within vue components to allow HTML to be embedded within a component from the calling page/component. A prime example of this being used this week was with modals. A modal component was created to create the basic template of it and within the component tag the content was placed which loads into the component's slot element.
