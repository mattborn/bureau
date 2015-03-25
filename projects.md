# Projects

## Proficiency Paths

- [Install prerequisites](prerequisites.md)
- Deploy a static site to Github Pages
- Build a hybrid document + application stack
- Build a login with Firebase
- Build a contact form with Firebase
- Build a sortable list with Firebase
- Contribute to an open source project (find something you care about … if you don’t care about anything, create opportunities)

## Simple Schemas

> Everything is a list.

### Food Menu
Item name, description + price.


# Work in progress below

### New repo in Github

![](https://dl.dropboxusercontent.com/s/zw0us7hkw7ipr3s/github-new-repo.png)

```
~/Code && git clone git@github.com:mattborn/bureau.git && bureau
```
*Note: `~/Code` should be wherever you keep all your repos. Also, this step is an example + you should be creating a new repo since this one will already include all the upcoming steps (unless that’s what you want).*

### Initialize as node project

`npm init`, then just keep hitting Enter for all the questions since you can always change this stuff later in your `package.json` file if it starts to matter.

### Install dependencies

```
npm install --save-dev assemble grunt grunt-gh-pages
```

### Directory structure

`mkdir src && mkdir src/partials && mkdir src/pages && mkdir src/posts`
