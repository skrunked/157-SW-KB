Follow this guide to contribute pages to the site! 

Your options are:
1. Make your documentation changes directly to the codebase, and create a Pull Request to be reviewed. 
	- Allows you to see your changes as you make them on the website, giving you full control over the outcome, and eliminates future review headaches
2. Write your documentation externally (ie Google doc), and create an Issue for your changes to be integrated
	- More convenient, less setup, but less control over the product, and more work for Software to integrate your changes.

:::info
This guide assumes you are using a Windows, Mac, or Linux-based PC. You can write your docs on mobile and export them later, if you wish.
::: 

## Method 1: Make changes directly, create Pull Request
### What You'll Need
- a [GitHub](https://github.com) account and membership to the [Aztechs157](https://github.com/Aztechs157) organization
	- Allows you to push your edits to the site (or rather have them review before being pushed to the site).
- [Node.js](https://nodejs.org) of no particular version
	- Allows you to run the website locally and see your changes as you make them
- [Visual Studio Code](https://code.visualstudio.com), or another editor of your choice. This guide will use VSCode.
	- To clone the codebase and document files locally and utilize version control
- Optional: [Obsidian](https://obsidian.md) for more intuitive markdown editing
### Getting Started: Base Package Installation
1. Create a GitHub account, if you have not already, and join the Aztechs157 organization. This will allow you to contribute pages to the knowledge base.
2. Install [Visual Studio Code (VSCode)](https://code.visualstudio.com/Download). There *is* a web version of VSCode, but you won't be able to launch the site from it.
3. Install [Node.js](https://nodejs.org/en/download) with a **prebuilt installer**. Beneath the codeblock, it should automatically present the best installer for your platform.
### Setting Up Your Workspace
1. Sign into your GitHub account in VSCode.
2. Inside the 'Source Control' tab, clone the repository Aztechs157/157-Knowledge-Base
3. Open a Terminal to access the folder you cloned the repository into. For this part, you can either:
	1. cd from your starting directory to the folder you cloned the repo into
		1. Probably only makes sense to Avid Computer Touchers
	2. Navigate to your folder in your filesystem (File Explorer, Finder, etc) and open a terminal at the folder.
4. Run the following command in your terminal:
```bash
npm install docusaurus
```

This will install all the necessary packages you need to run the site locally.

5. Run the following command in the same terminal:
```bash
npm run start
```
This will start up the local version of the site, then open it in your browser. If it doesn't open automatically, you can find it at http://localhost:3000.

6. Enjoy! Whenever you save a file with this server running, the site will automatically update.
### Writing Your Docs
1. In the bottom left of the VSCode UI, there should be an icon that says 'main'. Click on it, then click 'Create New Branch' in the popup that appears. Name it in the format `department/topic`, i.e. `software/led-control` or `engineering/bambu-studio`.
2. Determine which folder meets your needs. If an existing folder, say `java-basics` or `robot-code`, is an adequate home for your docs, you'll start there. If not, make a new folder in either the `Software` or `Engineering` folder.
3. Once you've chosen a folder, create a new markdown file, ending with .md.
4. Write your content using Markdown for formatting. You'll know this if you've used teh Markdown editor on Chief Delphi before. Docusaurus has a nifty guide [here](https://docusaurus.io/docs/markdown-features) on the syntax.
5. Under the Source Control tab in VSCode, feel free to stage your changes (with the little + button next to each file when you hover) and commit them as often as you'd like, and push them once you're done working.
### Integrating Your Changes
1. On GitHub, create a Pull Request to merge your branch into `main`.
2. Add a description summarizing the documentation that you added.
3. Publish your pull request, and assign an appropriate user as a reviewer (Eng. lead or mentor for Engineering, SW lead or mentor for Software)

## Method 2: Make changes externally, create Issue
:::warning
While this method is a *lot* more convenient for non-Software team members, it creates more work for your Software team, taking time they could use for Literally Anything Else. Please use Method 1 if you're able to; a Software member can walk you through, if necessary.
:::

### Writing your Docs
1. Create a Google Doc and write as you typically would.
2. On the Github Repository for our documentation, Aztechs157/157-Knowledge-Base, create a new Issue.
	1. Include a link to your Google Doc.
	2. Summarize what your documentation covers.
	3. Detail what category/folder the doc should fall under (Software, Engineering, a specific subcategory of that team, a new category, et cetera)
	4. Create your issue! Software will be notified once it is published.
3. Software will handle integrating your new doc into the knowledge base, and present the changes to you before integration.
