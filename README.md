HART Avionics - EECS Documentation
======
![CI/CD](https://github.com/Anatrax/HART-Avionics-docs/workflows/CI/CD/badge.svg?branch=develop)

<img src="https://images.squarespace-cdn.com/content/v1/5a19a459e5dd5b3614fc8595/1518733757123-JZ5199GBQVQOEJBC9VKR/ke17ZwdGBToddI8pDm48kOx9thYkxoPEJMHoJ7vUPbh7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z5QHyNOqBUUEtDDsRWrJLTmS0k9nmfOWkBD2X4dgpGrpWVYQT8AbCbINUUJycgJH0K3YOIy-qewO29_jEB_UvA_/HARTlogo.jpg" width="200px" height="auto"/>

Table of Contents
---------------------
- [About the Project](#about-the-project)
  - [Built with](#about-the-project-built-with)
- [Getting Started](#getting-started)
  - [Prerequisites](#getting-started-prerequisites)
  - [Installing](#getting-started-installing)
- [Usage](#usage)
<!-- - [FAQ](#faq) -->
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Contacts](#contacts)
- [Support the Project](#donate)

<a name="about-the-project"></a>
About the Project
---------------------
This is the documentation repo for the Oregon State Univerity AIAA High Altitude Rocket Team's ECE & CS avionics sub-team. This covers any system-wide and user-level documentation for the project. For more detailed documentation on project internals and developer documentation, see the corresponding project's repository.

<a name="about-the-project-built-with"></a>
### Built with
<!--This section should list any major frameworks that you built your project using. Leave any add-ons/plugins for the acknowledgements section.-->

- [Sphinx](https://www.sphinx-doc.org/en/master/usage/installation.html) documentation generator
- [TexLive](https://www.tug.org/texlive/)

<a name="getting-started"></a>
Getting Started
---------------------
<a name="getting-started-prerequisites"></a>
### Prerequisites

- [pip](https://pip.pypa.io/en/stable/installing/)
  ```bash
  $ sudo apt-get install python3-pip
  ```
- [Sphinx](https://www.sphinx-doc.org/en/master/usage/installation.html) documentation generator
  ```bash
  $ pip3 install -U sphinx
  ```
  > Make sure `~/.local/bin` is added to PATH
- [GNU make](https://www.gnu.org/software/make/manual/make.html)
  ```bash
  $ sudo apt-get install build-essential
  ```
- [recommonmark](https://github.com/readthedocs/recommonmark)
  ```bash
  $ pip3 install recommonmark
  ```

If you plan on building LaTeX PDF documentation, you'll also need the following packages:
```bash
$ sudo apt-get install texlive-latex-recommended texlive-fonts-recommended texlive-latex-extra latexmk
```

<a name="getting-started-installing"></a>
### Installing
1. Clone the repo
    ```bash
    $ git clone https://github.com/HART-Avionics/docs.git
    ```

<a name="usage"></a>
Usage
--------
The manual documentation is written mostly in Markdown, but Sphinx also has it's own default markup format called reStructuredText which can be used for generating documentation from code. Once you're finished making changes, you can build the documentation.

```bash
$ make build
```

Sphinx will try to generate both HTML & LaTeX PDF documentation in a build directory. The PDF (if generated successfully) is copied into the root directory and renamed *ProjectCharter.pdf*. These options can be configured in the project Makefile.

*For more examples, please refer to the official [Sphinx documentation](https://www.sphinx-doc.org/en/master/index.html)*

<!--
<a name="faq"></a>
FAQ
----
-->

<a name="roadmap"></a>
Roadmap
----------
See the [open issues](https://github.com/HART-Avionics/docs/issues) for a list of proposed features (and known issues).

<a name="contributing"></a>
Contributing
---------------
Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<a name="license"></a>
License
-----------
Distributed under the GNU GPLv3 License. See `LICENSE` for more information.

<a name="contacts"></a>
Contacts
-----------
<!-- Your Name - @your_twitter - example@example.com -->
**Maintainer:** Samuel D. Villegas - villegsa@oregonstate.edu

<a name="donate"></a>
Support the Project
--------------------
[Donate to HART](https://osuaiaa.com/donate)
