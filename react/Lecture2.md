# How to push code to github
<!-- Create a repo on github then run following commands on the terminal -->
1. git init
2. git branch -M main
3. git add .
4. git commit -m "Initializing"
5. echo "# reactProject" >> README.md
6. git add README.md
7. git commit -m "readme.md added"
8. git branch -M main
9. git remote add origin https://github.com/1Alisha/reactProject.git
10. git push -u origin main

# NPM REACT
1. npm does not stands for node package manager as on the npm website it is nowhere mentioned .(npm full form is not node package manager)
2. It is a package mananger .
3. It is a standard repository for all the packages.

# How to add npm mamager to ur project
1. npm init or npm init -v (to skip some steps)
It will create a package.json file which is configuration for node
(configuration refers to the arrangement or settings of a system or application. It involves specifying how different components or modules should behave or interact with each other. )

sometimes packages are also known as dependencies.

# Most important tools in our project is BUNDLER
 Bundlers are tools that combine and optimize code and assets (such as JavaScript, CSS, and images) to improve the performance of web applications.

 Examples of popular bundlers include 
1. Webpack
2. Parcel 
3. Rollup.

When we use create-react-app behind the scenes it use WEBPACK as default bundler.

There are two types of dependencies in web
1. dev depenencies (Generally required for the developement phase)
2. Production dependencies (Required in production and execution of application.)

# To install parcel
npm  install   -D     parcel 
              |___|  |_______|
               dev    dependency name
            dependency

# What is the difference between tilde (~) and caret (^)
1. Tilde (~):
   Example: "~1.2.3"
   For example, if your dependency is at version 1.2.3, running npm update would install 1.2.4 (a patch-level change) but not 1.3.0 (a minor-level change).

2. Caret (^):
   Example: "^1.2.3"
   For example, if your dependency is at version 1.2.3, running npm update would install 1.2.4 or 1.3.0 but not 2.0.0 (a major-level change).

# What is the difference between package.json and package-lock.json
package-lock.json file ensures that every person working on a project, as well as every environment where the project runs, uses the exact same versions of dependencies.
It contain the exact version of the dependency

package.json contains the range of version of dependency

# NODE MODULES
It is a database for all our dependencies.
This folder is very heavy
It  fetches all the code of all the dependencies into our system.

# Transitive dependencies
When you include a package as a dependency in your package.json file, that package may, in turn, have its own dependencies. These dependencies of dependencies are called transitive dependencies.

The relationship between direct dependencies and their transitive dependencies forms a tree structure known as the dependency tree.

# Every package will have its own package.json file and its own dependencies

# Should we push node modules to the github
No as it's a very huge in size
Moreover, Package managers are designed to handle dependency management efficiently. By relying on package.json and the lock file (package-lock.json for npm or yarn.lock for yarn), you allow the package manager to install the correct versions of dependencies based on the specified ranges or exact versions.

So it's a common practice to include a .gitignore file in your project that excludes the node_modules directory. 

This will ensure that node_modules is ignored when you commit changes.

# To install node modules
npm install

# npx parcel index.html ->to execute 

# To install react 
npm install react
npm i react
npm install react-dom (i/install both are same thing)
This command installs the latest version of React and adds it to your project's node_modules directory.

as using cdn links is not a good option.

# Parcel
1. dev build
2. Local server
3. HMR=Hot Module Replacement
4. File matching algorithms
5. Caching-Faster builds
6. Minification
7. Bundling
8. Compress

