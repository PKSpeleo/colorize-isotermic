
# Colorize Isotermic

Online: [Colorize Isotermic Demo](https://github.com/PKSpeleo/colorize-isotermic)

**Colorize Isotermic** is a simple web application that allows users to customize the colors of various parts of thermal clothing for spelunkers (or other outdoor enthusiasts). The application enables users to adjust hues in real-time and share their personalized configurations using a shareable link.

## Table of Contents

- [Demo](#demo)
- [Features](#features)
- [How It Works](#how-it-works)
- [Usage](#usage)
- [Development](#development)
- [License](#license)
- [Contributing](#contributing)

## Demo

Check out the live demo: [Colorize Isotermic Demo](https://github.com/PKSpeleo/colorize-isotermic)

## Features

- **Customizable Hues**: Modify the colors of thermal clothing parts (body, hands, legs, plates) using sliders or numerical inputs.
- **Live Preview**: View changes in real-time as hues are adjusted.
- **Reset and Randomize**: Reset hues to default values or generate random configurations with a single click.
- **Shareable Links**: Easily share customized configurations by copying the URL, which encodes all settings.
- **Responsive Design**: Optimized for both desktop and mobile devices.

## How It Works

1. Hue Adjustment: Each clothing layer (body, hands, legs, plates) has its own slider and numerical input. Users can adjust the hue values from 0 to 360 degrees, which updates the layer's color in real-time.

2. URL Encoding: The current hue settings for each layer are encoded into the URL's query parameters. For example: `?Body=120&Hands=60&Legs=300&Plates=45`.

3. State Restoration: When the application is opened with a custom URL, the hue values are automatically applied, restoring the saved configuration.

4. Buttons:
    - **Reset**: Reverts all hues to their default value (0 degrees).
    - **Randomize**: Assigns random hue values to all layers.
    - **Copy URL**: Copies the current URL with the encoded hue values to the clipboard.

## Usage

1. Open the Application: Visit the [Colorize Isotermic Demo](https://github.com/PKSpeleo/colorize-isotermic).
2. Adjust the Hues: Use the sliders or input fields to set the hue values for each clothing layer. The preview updates in real-time to reflect your changes.
3. Reset or Randomize: Click **Reset** to restore default settings. Click **Randomize** to apply random hues to all layers.
4. Share Your Configuration: Click the **Copy URL** button to copy a shareable link. Share the link with others, and they will see the same colors and settings when they open it.

## Development

To run or modify the application locally:

1. Clone the Repository:
   ```bash
   git clone https://github.com/PKSpeleo/colorize-isotermic.git
   ```

2. Navigate to the Directory:
   ```bash
   cd colorize-isotermic
   ```

3. Serve the Application:
   Since the application uses URLs to store state, you should serve it via a local web server:

   - Using Python 3:
     ```bash
     python -m http.server
     ```
     Navigate to `http://localhost:8000`.

   - Using Node.js:
     ```bash
     npm install -g http-server
     http-server
     ```
     Navigate to the provided local address.

   - Using Live Server (VS Code):
     - Install the **Live Server** extension in Visual Studio Code.
     - Open the project folder in VS Code.
     - Right-click `index.html` and select **Open with Live Server**.

4. Make Changes: Edit the `index.html`, `CSS`, or JavaScript as needed. Refresh your browser to see the updates.

5. Contribute: Report bugs or suggest features via GitHub Issues. Fork the repository, make changes, and open a Pull Request.

## License

This project is licensed under the [MIT License](LICENSE).

## Contributing

Contributions are welcome! Please fork the repository, create a new branch for your changes, and submit a pull request.

---

© 2024 **Colorize Isotermic**. All rights reserved.
