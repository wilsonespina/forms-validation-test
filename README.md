# Springload test

https://forms-validation-test.netlify.app/

<img src="./src/assets/form-validation-test.png" width="400px"/>

## Running the app

Requirements

`node version 18.16.0`

```bash
npm run start
```

## Running tests

```bash
# all tests
npm run test

# unit tests
npm run test:unit

# e2e tests
npm run test:e2e
```

## Technologies used

* [Netlify](https://www.netlify.com/) for hosting the site.
* [nx](https://nx.dev/) to scaffold project as Standalone React project.
* [Tailwind](https://tailwindcss.com/) css for styling
* Testing:
    * e2e test [Cypress](https://docs.cypress.io/guides/overview/why-cypress).
    * [React Testing Library](https://testing-library.com/) for unit tests.
* Browser Support - Tailwind css takes care of vendor prefixes.

## Validation:

* Password - Length has to be between 8 - 20 characters.
* Email - A valid email address with `@` etc.

## Future Refactoring

* Improve the UX of the validation by running validation on change rather than on blur. This would be better for users who see the error message, re-type a password and it passes on the second attempt while typing.
* Server-side render the application using a tool like [Next.js](https://nextjs.org/) to ensure users can view the page when javascript is disabled.
* Make the `Form` component more reusable by making it more generic and not just the Contact Form. This could be done by passing through form fields as props to the component.
* Remove placeholders for form submit.
* Add more integration tests on more parts of the form.
