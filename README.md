# angular-review

## Angular (v9): Some Introductory Notes

- angular-cli: "batteries included"
  -- Significant difference vs. React - think of Django's CLI, or Laravel's or RoR.

- Nrwl workspace
- Angular Material

-- on top of setting up dev server etc., you can create schematics that let people auto-generate projects based on a schematic.

## Getting started

```
npm i -g @angular/cli@
npm i -g @nrwl/nx
npm i -g @nrwl/cli
npm i -g @nrwl/schematics
npx create-nx-workspace angular-core-workshop
```

It splits into applications and reusable component libraries. We can create an Angular app called `angular-core-workshop`

`cd angular-core-workshop/`

- Then add angular material UI component library:
  `ng add @angular/material`

then `ng g lib material`

`npm start`

To create a module (something that would have its own route) -
`ng g m [module-name] --routing`

then `ng g c [component-name (same as module name)]`

### General notes:

Best to have very light front-end components, with state management abstracted away in libs folder.
