# node-sass-watch-import-css-bug
Reduced test case for node-sass bug

1. Clone this repo
2. Run `npm install` from the root of this repo
3. Run `npm run sass`. This should complete without error.
4. Run `npm run watch:sass`. This will error (this is the bug).
5. View package.json for exact command lines for the above 2 commands.

Note: The error occurs in sass-graph when parsing someOtherFile.css (which only happens when node-sass is running in --watch mode -- another issue).
