# GAD - Local Deployment:

## Requirements:

- Installed `Node.js` on your system.

- Tested with `Node.js` versions 18 and 20.

- Installed `Git` on your system.

## First Usage:

1. Open the main project directory in the command prompt or terminal.

2. Clone the repository using the command `git clone <repository address>`. This is the preferred way to use this application.

3. Run `npm i` to install the modules (avoid using global Node.js packages!).

4. Run `npm run start` to launch the `GAD` application.

5. The application will be accessible at `http://localhost:3000`.

## Version Update:

1. If you're using a ZIP package:

   - Download the zipped repository.
   - Unzip it and replace your local `GAD` instance.
   - Run `npm i` in the main directory to install new modules.
   - Run `npm run start` to restart `GAD`.

2. If you're using a cloned repository:

   - Open the main project directory in the command prompt or terminal.
   - Execute `git pull` to fetch the latest changes.
   - Run `npm i` to install new modules.
   - Run `npm run start` to restart `GAD`.

3. Version update for changes (e.g., database updates):

   - One option is to reset all local changes and fetch the new version. However, be aware that this will discard all local changes and data!
   - Open the main project directory in the command prompt or terminal.
   - Execute the following commands:
     ```
     git reset --hard HEAD
     git pull
     ```
   - Run `npm i` to install new modules.
   - Run `npm run start` to restart `GAD`.

Based on the [GAD instructions](https://github.com/jaktestowac/gad-gui-api-demo/blob/main/README.md)
