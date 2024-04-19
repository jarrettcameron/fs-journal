# Single Page Applications with Vue
01. What is the entrypoint of an application?

  > The entrypoint of an application is the first-most component of an application, this entrypoint usually loads other pages, components, etc that branch off and make an application whole. In the vue-starter the entrypoint would be either the index.html or App.vue depending on how you define it.

02. What is the difference between a vue `component` and `page`?

  > From a technical view, nothing. From a structural view, a lot. Components and pages are differentiated to give your application more organization and structure. A page is a basic container for your components and your components are (usually) blocks of code that are injected into your page (which is technically injected into the App.vue). Components are typically done this way

03. What is ***Component-Based Architecture***?

  > Component-based architecture was *roughly* described in my previous answer, instead of separating things by how they interact with the backend and user (like MVC does), CBA divides your application into smaller chunks usually pieces that need to be consistent and repeated throughout an application. Of course, CBA can still be integrated with MVC to keep the interaction more organized.

04. What are the three tags that make up a Vue component?

  > There are three tags that make up a vue component and they all relate back to everything we've worked with in the past. The first tag is the script tag which allows JS to be written for a specific component, the second tag is the template tag which is the HTML of the component and finally (and my favorite to be honest) the style tag which is the CSS for the component. The ability to have scoped styles is so insanely helpful.

05. What are ***lifecycle hooks***? What are lifecycle hooks used for?

  > Lifecycle Hooks are pretty similar to event listeners in the sense that they hook into Vue to allow us to access events. Some of the ones we've used so far are onMounted and onUnmounted which make running code when a component/page is loaded/unloaded possible.

06. Which component in Vue does the vue-router use to mount pages onto?

  > Question is worded a bit weird but I'll try my best. If the question is asking how are pages mounted, they are mounted to App.vue.

07. What is the difference between the `AppState` and the state object within a component?

  > AppState is globally scoped for all components to use and interact with, state objects within components are local to that component and cannot be interacted with outside the component (unless passed through).

08. What is the responsibility of `Services` in our Vue projects?

  > Same as before. The only thing that Vue has really changed is our controller system has been broken down into CBA, the service is still responsible for communicating with the AppState & external APIs. Now our components are responsible for communicating user interaction to the service instead of a dedicated controller.

09. What are ***props*** and how are they used? Provide an example

  > Props are used to move data (reference and primative types) between Vue pages or components. A great example of this is loading objects from a page and trying to draw them using components. Props can be attached using data-bound fields (:prop="dataObject") and they can be read from a component by defining the property and it's type ( defineProp({ prop: DataType }) ).

10. What is the Vue method used to create watchable objects such as `state` or `AppState`?

  > Still a unsure of what state is referring to here but pretty sure the answer being looked for is computed(() => obj).
