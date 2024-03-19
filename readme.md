# Blazor with TailwindCSS Integration

This project demonstrates the integration of TailwindCSS into a Blazor application, combining the power of Microsoft's Blazor framework with the utility-first styling approach of TailwindCSS.

## Overview

TailwindCSS has emerged as a popular choice for frontend development due to its flexible utility classes and efficient workflow. Integrating TailwindCSS into a Blazor project allows developers to leverage its extensive set of styles while building interactive web applications with C# and .NET.

This repository provides a step-by-step guide and sample code for integrating TailwindCSS into a Blazor project, enabling developers to enhance the visual aesthetics and user experience of their web applications.

For a detailed tutorial on this integration, check out the accompanying [WordPress post](https://michaeltrinh7.wordpress.com/2024/03/19/integrating-tailwindcss-into-your-blazor-project/).

## Features

- Seamless integration of TailwindCSS into a Blazor project.
- Utilization of TailwindCSS utility classes within Blazor components.
- Watch mode for automatic generation of TailwindCSS styles.

## Getting Started

To get started with this project, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/michaeltrinh7/blazor-with-tailwindcss.git
   ```

2. **Navigate to the project directory:**

   ```bash
   cd blazor-with-tailwindcss
   ```

3. **Download Tailwind's CLI:**

   If you don't have npm installed, download the TailwindCSS CLI from the [release page](https://github.com/tailwindlabs/tailwindcss/releases) and place it in a folder named "Tailwind" within the project directory.

4. **Initialize Tailwind configuration:**

   Run the following command from the project directory to generate the Tailwind configuration file:

   ```bash
   ./../Tailwind/tailwindcss-windows-x64.exe init
   ```

5. **Create Tailwind CSS file:**

   Inside the "Styles" folder, create a file named "tailwind.css" with the following content:

   ```css
   @tailwind base;
   @tailwind components;
   @tailwind utilities;
   ```

6. **Adapt App.razor:**

   Add the following line to the App.razor file to include the Tailwind CSS file:

   ```html
   <link rel="stylesheet" href="tailwind.css" />
   ```

7. **Watch for changes:**

   Execute the following command to enable Tailwind to watch for changes and generate styles:

   ```bash
   ./../Tailwind/tailwindcss-windows-x64.exe -i ./Styles/tailwind.css -o ./wwwroot/tailwind.css --watch
   ```

8. **Run the project:**

   Run the Blazor application and navigate to the Home page to see the integration of TailwindCSS in action.

## Sample Code

Check out the sample Blazor components within this repository to see how TailwindCSS utility classes are utilized:

- **Home.razor:** Demonstrates the usage of TailwindCSS styles within a Blazor component.

## Contributing

Contributions to this project are welcome! If you find any issues or have suggestions for improvement, feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).