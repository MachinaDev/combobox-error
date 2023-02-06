# Combobox Error Reproduction

## Where is the problem

I tried to add the Combobox into my project with NextJS 12.1.4. I have created a custom component named _CommandPalette.js_.
The problem is located in the _components/CommandPalette.js_ component and seems to come from the `Combobox.Options static` property.
No problem in development mode but crash app after building the app.

### Install Web Application
- Install this project: `yarn install`

### Launch the App: No Error

- Start development mode: `yarn dev`
- Go to localhost:3000 -> No problem at all

### Build the App: Error

- Build and serve the app: `yarn build && yarn serve`
- - Go to localhost:3000 -> App craches when clicking or keyboard call the command palette component.

***error*** : _TypeError: Cannot read properties of null (reading 'isSelected')_