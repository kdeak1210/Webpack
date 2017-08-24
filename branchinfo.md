# Before Webpack

## This branch shows the project before the use of Webpack

- Although the application is trivial, the imports (<link>, <script>) in the index.html file must be done in a specific order due to the source code's organization.
- The use of Webpack would allow us to 'bundle' our source code files so that we only need to link one (possibly more) of these bundled files for the production code.
  - This improvement becomes especially helpful as the complexity and size of our project scales, Webpack aims to keep source code management as simple as possible
