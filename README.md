# Converting a streamlit app to exe

### Stlite Approach
Stlite is a WebAssembly port of Streamlit that runs on Pyodide runtime. Pyodide is an experimental project from Mozilla to create a full Python data science stack that runs entirely in the browser. A Streamlit application can be converted to an exe using Stlite desktop. This approach does not require you to deploy the Streamlit application to Streamlit share.

Install packages as follows:

```
npm install
```
Then create a directory to contain the application files, e.g., streamlit_app. So the path of the main app file looks like streamlit_app/streamlit_app.py

Run the dump command to create the ./build folder.

```
npm run dump app
```
The dist command bundles the ./build directory created in the step above into application files (.app, .exe, .dmg etc.) in the ./dist directory.

```
npm run dist
```
