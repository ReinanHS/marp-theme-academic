<div align="center">
   <img src="https://marp.app/assets/marp.svg" alt="Marp Logo" width="40%">
</div><br>

# ReinanHS/marp-theme-academic

> This template is forked from [yunzinan/marp-theme-academic](https://github.com/yunzinan/marp-theme-academic), modified by [@ReinanHS](https://github.com/ReinanHS).

This is a custom template for the Marp plugin in Visual Studio Code (VSCode). The primary purpose of this repository is to provide a clear and clean structure for creating academic presentations.

Within this repository, you will find an example of an academic presentation related to the field of programming. This example discusses the concept of recursion in programming and is available in Brazilian Portuguese.

## Features ✨

- Changed the colorscheme, using [IFS](http://www.ifs.edu.br/) base colors.
- Changed the font, using the [Public Sans](https://fonts.google.com/specimen/Public+Sans?query=Public+Sans).

## Preview 🎨

This project uses CI/CD automation to automatically process information whenever there are changes to the `main` branch. This means that, when pushing changes to the main branch, the system will automatically export the presentation to HTML format.

![Google Chrome - Light](https://github.com/ReinanHS/marp-theme-academic/assets/28494067/de5d8f73-f57b-4059-815a-5e82cfc7aa7a)
![Slide 4](https://github.com/ReinanHS/marp-theme-academic/assets/28494067/fb94803c-5f6a-425c-9a70-028b926cbece)

📌 To view the presentation in your browser, [click this link](https://reinanhs.github.io/marp-theme-academic/).

## How to use 🎈

1. Clone this repository to your local machine using the command below:

```bash
git clone https://github.com/reinanhs/marp-theme-academic.git
```

1. Open the `slide-deck.md` file in Visual Studio Code.

To make these settings work in Visual Studio Code (VS Code), it is necessary to install the Marp plugin in VS Code. You can find this plugin in the VS Code extensions marketplace.

It's worth noting that after you install this plugin and open this template project, the settings will be applied automatically to your editor. This happens due to specific configurations in a file `.vscode/settings.json`, located within the project's directory.

Here is the content of that file:

```json
{
    "markdown.marp.themes": [
        "https://raw.githubusercontent.com/reinanhs/marp-theme-academic/main/themes/academic.css"
    ],
    "markdown.marp.enableHtml": true
}
```

These configurations ensure the proper functioning of the Marp environment in your VS Code, enabling an optimized editing and presentation experience.

2. Customize the presentation content according to your needs. You can use Markdown to format your slides.
3. After customizing your presentation, you can generate the slides in PDF format.
4. Run the command below to generate the slides in PDF format:

```bash
docker run --rm --init -v "${PWD}:/home/marp/app/" -e LANG="pt_BR.UTF-8" marpteam/marp-cli slide-deck.md --theme themes/academic.css --pdf
```

6. At the end of execution, the `slide-deck.pdf` file will be generated in the root of your project.


## Software stack

Esse projeto roda nos seguintes softwares:

- Marp 2.7.0
- Docker

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information about what has changed recently.

## Contributors

Feel free to contribute improvements, bug fixes or add features to this repository. Just create a fork of the project, make your changes and submit a pull request. Your contributions are welcome!

Do you want to be part of this project? read [how to contribute](CONTRIBUTING.md).

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
