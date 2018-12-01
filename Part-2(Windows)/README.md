# Part 2, Node.js & Gatsby (Windows Instructions)

- Install Node
- Visit https://www.gatsbyjs.org/tutorial/
- Install Gatsby cli `npm install -g gatsby-cli`
- Open a new vscode window
- navigate to websites
- create new gatsby project `gatsby new project-name`
- cd in project
- run `git init`
- delete README.md text and write `project-name`
- run git add .
- `git commit -m "first commit"`
- create new repo on github
- run `git remote add origin https://github.com/anderskitson/website-basics-gatsby.git`
- run `git push -u origin master`
- run gatsby develop
- visit the url
- yay
- Open src folder
- look at index.js and page-2.js
- look at layout .js `children` section
- install prettier, try turning single quotes true/false
- Go to `components/header.js` change header background color
- Go to `gatsby-config.js` change title to `project-name`
- Look at how the title is accessed in the code `<Header siteTitle={data.site.siteMetadata.title} />` in `layout.js` This is using something called `react` and `graphql` React was created by facebook and is a js library for building user interfaces, GraphQl is a querying language it is how you handle data, also create by facebook.
- create a file called `about.js` in the pages folder
- Next Write on the first line `import React from 'react'`
- Now lets create a new function expression called `About` by writing the `=> ()` is called a arrow function
```
const About = () => (

)
```
- Inside of the function expression add the following to look like this

```
const About = () => (
  <div>
    <h1>About Us</h1>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
      tempor incididunt ut labore et dolore magna aliqua. 
    </p>
  </div>
)
```
- Lastly export the expression at the bottom. Final page should look like below

```
import React from 'react'

const About = () => (
  <div>
    ...
  </div>
)

export default About
```
- Now go and visit http://localhost:8000/about you should see your About Us page, yahoo
- 