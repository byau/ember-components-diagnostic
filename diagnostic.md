# Ember Components Diagnostic

Record your responses inside the fenced code blocks below each question.

1.  Give an example of a visual hierarchy that could be modeled with components.

    ```md
    <!-- your response here -->
    hiding and showing div ?
    ```

1.  What is the command to generate a new component called '`my-map`'?

    ```sh
    # your response here
    ember generate component my-map
    ```

1.  What files are edited to produce a component, and what are their
    responsibilities?

    ```md
    <!-- your response here -->
    component.js - use to define the component, can incorporate classes, tags, actions them.
    template.hbs - template on how to display data
    ```

1.  Suppose you have a component '`my-contact`', which is loaded from
    '`app/contacts/template.hbs`' when visiting the `/contacts` path. What is
    the syntax for loading this component inside that template?

    ```html
    <!-- your response here -->
    {{contacts/my-contact}}
    ```

    Each contact has multiple phone numbers. Suppose you also have '`my-phone`'
    nested under '`my-contact`'. What is the code you would write in
    '`app/components/my-contact/template.hbs`' to load the nested component and
    pass it data?

    ```html
    <!-- your response here -->
    {{#each my-phone.phoneNum as |phoneNum|}}
      {{contacts/my-contact/my-phone phoneNum=phoneNum}}
    {{/each}}

    ```
