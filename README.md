# Sigil Icon Themes

Regrettably, the free and multi-platform ebook editor **[Sigil](https://github.com/Sigil-Ebook/Sigil)** offers a limited selection of just three user interface icon themes. Recognizing the diverse preferences of users, this repository is designed to expand those choices, providing additional icon theme options to enhance the user experience.

This repository features an array of icon themes for **Sigil**, beginning with the three standard sets and expanding to include six color variants from the Material icons. Additionally, it offers a diverse collection of custom icon themes, broadening the spectrum of visual customization.

To enhance user convenience, this repository provides clear guidelines for installing any icon theme, ensuring a smooth setup process. Furthermore, a detailed guide that assists users in crafting and compiling their own personalized icon set is included, making customization accessible for all.

## Standard Icons

Sigil users have the liberty to select from three main icon themes included with Sigil:


- **[Main](https://github.com/Sigil-Ebook/Sigil/tree/master/src/Resource_Files/main)**: The standard icon set introduced in Sigil version 1.0 and onwards.
     - ![Main Icon Theme Light](./img/Main.png)
     - ![Main Icon Theme Dark](./img/Main_dark.png)
- **[Fluent](https://github.com/microsoft/fluentui-system-icons)**: A collection of icons inspired by Microsoft's Fluent Design System.
     - ![Fluent Icon Theme Light](./img/Fluent.png)
     - ![Fluent Icon Theme Dark](./img/Fluent_dark.png)
- **[Material](https://github.com/google/material-design-icons)**: A set of icons based on Google's Material Design guidelines.
     - ![Material Icon Theme Light](./img/Material.png)
     - ![Material Icon Theme Dark](./img/Material_dark.png)

Beyond the primary themes, Sigil also accommodates the integration of custom icon themes. Users can compile their own themes using Qt's Resource Compiler to produce .rcc files.

## Material Icons Derivatives

For those seeking alternative custom themes, this repository offers several additional icon sets derived from Sigil's original designs:

- **Legacy Theme**: SVG-based icons reminiscent of Sigil's style prior to version 0.9.7.
     - ![Legacy Icon Theme](./img/legacy.png)
- **Material Derivative Themes**: A spectrum of color-based themes (blue, gray, lilac, orange, pink, red) designed to complement both light and dark user interfaces.
     - ![Material Red Icon Theme](./img/material-red.png)
     - ![Material Orange Icon Theme](./img/material-orange.png)
     - ![Material Pink Icon Theme](./img/material-pink.png)
     - ![Material Gray Icon Theme](./img/material-gray.png)
     - ![Material Lilac Icon Theme](./img/material-lilac.png)
     - ![Material Blue Icon Theme](./img/material-blue.png)

To obtain any of these custom themes, visit the repository's Releases section and download the desired .rcc icon theme file.

## Custom Icon Themes

## How to Install a Custom Icon Theme in Sigil

To install a custom icon theme:

1. Acquire the .rcc file from the Releases section.
2. Rename the file to "custom_icon_theme.rcc."
3. Place the renamed file into the Sigil preferences directory specific to your operating system.

Download one of the .rcc files from Releases
Rename it to "custom_icon_theme.rcc"
Copy that file to your Sigil user preferences Folder:
On macOS: "~/Library/Application Support/sigil-ebook/sigil/"
On Windows: "%localappdata%\sigil-ebook\sigil\
On Linux: "~/.local/share/sigil-ebook/sigil"

For quick access to the Sigil preferences directory, open Sigil, head to the Preferences menu, and use the "Open Preferences Location" button found in the Preferences dialog's lower-left corner.

After installation, launch Sigil, navigate to Preferences > Appearance, select the Icon Themes tab, choose your new theme, and restart Sigil to apply the changes.

## Crafting Your Personal Icon Theme

Tech-savvy users with a knack for SVG editing and Qt's resource compiler (rcc) can design a unique set of icons. Follow the naming conventions outlined in the src/main/folder and use the rcc command line tool to compile your theme:

```bash
rcc -binary -o YOUR_OUTPUT_FILE.RCC YOUR_QRC_FILE
```

For detailed instructions on using rcc, refer to the Qt documentation for your specific Qt version.

---

This reworded README maintains the original content's intent while offering a fresh structure and phrasing. If you need further assistance or modifications, feel free to ask!

Source: Conversation with Bing, 3/17/2024
(1) undefined. https://github.com/JedWag/dotfiles.git.

---
Installing a .rcc icon Theme into Sigil
Download one of the .rcc files from Releases
Rename it to "custom_icon_theme.rcc"
Copy that file to your Sigil user preferences Folder:
On macOS: "~/Library/Application Support/sigil-ebook/sigil/"
On Windows: "%localappdata%\sigil-ebook\sigil\
On Linux: "~/.local/share/sigil-ebook/sigil"
An easier way to find your Sigil user preferences folder is to launch Sigil and navigate to the Preferences menu item. Once Preferences opens, you will see a button to "Open Preferences Location" in the bottom left corner of the Preferences dialog.

Clicking this button should open a Window showing this folder. Drag and drop the .rcc file here.

Once installed. Fire Up Sigil and go to Preferences->Appearance and select the Icon Themes tab. Make your selection and restart Sigil.

Creating Your Own Icon Theme
More advanced users who are familiar with svg editing (Inkscape, etc) and have Qt installed (for its resource compiler, rcc) can create a complete set of icons matching the names provided in the src/main/folder here.

You can use the command line to run rcc: rcc -binary -o PATH_TO_OUTPUT_FILE.RCC PATH_TO_QRC_FILE

See the Qt docs on rcc for your version of Qt: https://doc.qt.io/qt-5/rcc.html