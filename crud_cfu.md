## Questions
1. Define CRUD.

2. Why do we use set method_override: true?

3. Explain the difference between value and name in this line: `<input type='text' name='task[title]' value="<%= @task.title %>"/>.`

4. What are params? Where do they come from?

5. Check out your routes. Why do we need two routes each for creating a new Task and editing an existing Task?

## My Answers
1. CRUD is a abbreviation for Create, Read, Update, Destory. It describes the actions that can be taken on an object in the MVC paradigm.

2. To use the secret form input `_method` we added that allows us to bypass restrictions put in place by HTML.

3. `value` is the default value for the input field on the page. `name` is the internal name of the input field on the DOM.

4. Params come from `<form>` tags where any `<input>` fields that have a `name` attribute.

5. We need two routes because they are different HTTP commands trying to do different things. `GET` is for retrieving a URL form the server and `POST` is for sending data to the server
