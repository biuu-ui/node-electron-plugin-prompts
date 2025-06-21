# Node Electron Plugin Prompts 🎨

![GitHub Release](https://img.shields.io/github/release/biuu-ui/node-electron-plugin-prompts.svg) ![NPM Version](https://img.shields.io/npm/v/node-electron-plugin-prompts.svg)

Welcome to the **Node Electron Plugin Prompts** repository! This project allows you to create custom dialogs, prompts, or forms for your Electron applications using simple HTML and CSS templates. Whether you need a dropdown menu, input fields, or other UI elements, this plugin provides an easy way to enhance your Electron app's user experience.

## Table of Contents

1. [Features](#features)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Examples](#examples)
5. [Contributing](#contributing)
6. [License](#license)
7. [Releases](#releases)

## Features

- **Customizable Dialogs**: Easily create dialogs that match your app's design.
- **HTML & CSS Templates**: Use straightforward HTML and CSS to style your prompts.
- **Multiple Input Types**: Support for various input types like text, dropdowns, and checkboxes.
- **Easy Integration**: Simple setup and integration into your existing Electron app.

## Installation

To get started with the Node Electron Plugin Prompts, follow these steps:

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/biuu-ui/node-electron-plugin-prompts.git
   cd node-electron-plugin-prompts
   ```

2. **Install Dependencies**:

   Run the following command to install the required packages:

   ```bash
   npm install
   ```

3. **Build the Plugin**:

   After installation, build the plugin using:

   ```bash
   npm run build
   ```

## Usage

To use the Node Electron Plugin Prompts in your Electron app, follow these steps:

1. **Import the Plugin**:

   In your main JavaScript file, import the plugin:

   ```javascript
   const prompts = require('node-electron-plugin-prompts');
   ```

2. **Create a Prompt**:

   Use the following code to create a simple prompt:

   ```javascript
   prompts.createPrompt({
       title: 'Sample Prompt',
       message: 'Please enter your name:',
       inputType: 'text'
   }).then(response => {
       console.log('User response:', response);
   });
   ```

3. **Customize the Prompt**:

   You can customize the prompt further by adding more options. For example:

   ```javascript
   prompts.createPrompt({
       title: 'Choose an Option',
       message: 'Select your favorite fruit:',
       inputType: 'dropdown',
       options: ['Apple', 'Banana', 'Cherry']
   }).then(response => {
       console.log('Selected fruit:', response);
   });
   ```

## Examples

### Basic Text Input

```javascript
prompts.createPrompt({
    title: 'Enter Your Email',
    message: 'Please provide your email address:',
    inputType: 'text'
}).then(response => {
    console.log('Email entered:', response);
});
```

### Dropdown Selection

```javascript
prompts.createPrompt({
    title: 'Select Your Language',
    message: 'Choose your preferred programming language:',
    inputType: 'dropdown',
    options: ['JavaScript', 'Python', 'Java', 'C#']
}).then(response => {
    console.log('Language selected:', response);
});
```

### Checkbox Input

```javascript
prompts.createPrompt({
    title: 'Select Your Hobbies',
    message: 'Choose your hobbies:',
    inputType: 'checkbox',
    options: ['Reading', 'Gaming', 'Traveling', 'Cooking']
}).then(response => {
    console.log('Hobbies selected:', response);
});
```

## Contributing

We welcome contributions to the Node Electron Plugin Prompts project! If you have suggestions for improvements or want to report a bug, please follow these steps:

1. **Fork the Repository**: Click on the "Fork" button in the top right corner of the repository page.
2. **Create a New Branch**: Create a new branch for your feature or bug fix.

   ```bash
   git checkout -b feature-name
   ```

3. **Make Your Changes**: Implement your changes and commit them.

   ```bash
   git commit -m "Add feature or fix bug"
   ```

4. **Push Your Changes**: Push your changes to your forked repository.

   ```bash
   git push origin feature-name
   ```

5. **Create a Pull Request**: Go to the original repository and click on "New Pull Request."

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Releases

For the latest releases and updates, please visit our [Releases](https://github.com/biuu-ui/node-electron-plugin-prompts/releases) section. Here, you can download the latest version of the plugin and view the change log.

Feel free to check the **Releases** section for updates and new features as they become available.

---

Thank you for checking out the Node Electron Plugin Prompts! We hope this tool enhances your Electron applications and makes your development process smoother. If you have any questions or need assistance, don't hesitate to reach out.