# Meteor todo
[![npm version](https://badge.fury.io/js/meteor-todo.svg)](https://badge.fury.io/js/meteor-todo)
[![Generic badge](https://img.shields.io/badge/github-sylhare-blue.svg)](https://github.com/Sylhare/meteor-todo)

This is a basic todo app with the [meteor platform](https://www.meteor.com/) and [React](https://reactjs.org/).

![https://raw.githubusercontent.com/Sylhare/meteor-todo/security/meteor-todo.png](https://raw.githubusercontent.com/Sylhare/meteor-todo/security/meteor-todo.png)

## Installation

### Meteor

Following the meteor [installation procedure](https://www.meteor.com/install).

On OSX / Linux:

```bash
curl https://install.meteor.com/ | sh
```

### React

The app is running with react, sometime it is not installed automatically.

After installing meteor, go into the `todo-app/` folder and make sure you have the react dependencies installed using:

```bash
meteor npm install --save react react-dom
```

## Getting Started

### Basic use

Then start the app with:

```bash
meteor
```

The the app should be running at [localhost:3000/](http://localhost:3000/).

### Database manipulation

Once the app is started, you can open a new terminal and manually add a todo item with this command:

```bash
meteor mongo
```

A mongo DB is created automatically with meteor, add a new task that will be store in this database with:

```bash
db.tasks.insert({ text: "Hello world!", createdAt: new Date() });
```