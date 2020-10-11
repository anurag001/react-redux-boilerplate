# react-redux-boilerplate
https://codeburst.io/its-easy-setting-up-react-and-webpack-eb9ecaef5094

https://medium.com/swlh/a-complete-webpack-setup-for-react-e56a2edf78ae

https://medium.com/@dv19196/creating-a-react-js-app-with-babel-webpack-9837033c1e56 <- Follow this

These versions are supporting

{
    "webpack": "^4.41.2",
    "webpack-cli": "^3.3.10",
    "webpack-dev-server": "^3.11.0"
}

GO for

npm uninstall webpack-dev-server --save

npm uninstall webpack-cli --save

npm uninstall webpack --save

npm install --save-dev webpack@4.41.2 webpack-cli@3.3.10 webpack-dev-server@3.11.0

---------------------------------------------------------------------------------------------------
Jest and Enzyme
https://medium.com/codeclan/testing-react-with-jest-and-enzyme-20505fec4675

If not using CRA install Jest:

npm install --save-dev jest babel-jest

Install Enzyme:

npm install --save-dev enzyme enzyme-adapter-react-16 enzyme-to-json

Update your package.json :

"jest": {
  "snapshotSerializers": ["enzyme-to-json/serializer"]
}

enzyme-to-json provides a better component format for snapshot comparison than Enzyme’s internal component representation. snapshotSerializers allows you to minimise code duplication when working with snapshots. Without the serializer each time a component is created in a test it must have the enzyme-to-json method .toJson() used individually before it can be passed to Jest’s snapshot matcher, with the serializer you never use it individually.


