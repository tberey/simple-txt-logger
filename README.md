<!--
*** Using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

<!-- PROJECT SHIELDS/BADGES -->
[![Workflow][workflow-shield]][workflow-url]
[![Issues][issues-shield]][issues-url]
[![Version][version-shield]][version-url]
[![Stargazers][stars-shield]][stars-url]
[![Forks][forks-shield]][forks-url]
[![Contributors][contributors-shield]][contributors-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO & TITLE -->
<br>
<div align="center">
  <a href="https://github.com/tberey">
    <img src="public/assets/logo.png" alt="Logo" width="200" height="100">
  </a><br><br>
  <div align="center"><h1>SimpleTxtLogger</h1>A simple and lightweight logging module,<br>by TomCo (Technology & Online Media Company)</div>
  <div align="right">
    <br>
    <a href="https://github.com/tberey/simple-txt-logger/blob/master/README.md"><strong>Documentation »</strong></a>
    <br>
    <a href="#usage">View Demo</a>
    ·
    <a href="https://github.com/tberey/simple-txt-logger/issues">Report Bug</a>
    ·
    <a href="https://github.com/tberey/simple-txt-logger/issues">Request Feature</a>
  </div>
</div>



<!-- TABLE OF CONTENTS -->
<details open="open" style="padding:4px;display:inline;border-width:1px;border-style:solid;">
  <summary><b style="display: inline-block"><u>Contents</u></b></summary>
    <ol>
        <li>
        <a href="#about-this-project">About</a>
        <ul>
            <li><a href="#tech-stack">Tech Stack</a></li>
        </ul>
        </li>
        <li><a href="#installation">Installation</a></li>
        <li>
          <a href="#usage">Usage</a>
          <ul>
            <li><a href="#screenshots">Screenshots</a></li>
        </ul>
        </li>
        <li><a href="#complete-setup-instructions">Complete Setup Instructions</a></li>
        <li><a href="#changelog">Changelog</a></li>
        <li><a href="#contributing">Contributing</a></li>
        <li><a href="#contact">Contact</a></li>
        <li><a href="#acknowledgements">Acknowledgements</a></li>
    </ol>
</details><hr><br>



<!-- ABOUT THis PROJECT -->
## About This Project
This is a simple and easy to use logging tool, that is also light-weight. It streams dynamically into a concise and pretty format, into .txt file, with all .txt files under one root directory (all done automatically). Simply add the module to your project,create a new instance for each logger you want, and away you go. For example you could create a new logger each for client-side or server-side logging separately, outputted to two txt files. See [Usage](#usage) and [Screenshots](#screenshots) for more information.

<br>

### Tech Stack
* [TypeScript](https://www.typescriptlang.org/) - Write in TypeScript (or JS), Compiles down to JavaScript.
* [Nodejs](https://nodejs.org/en/) - Node Runtime Environment.
* [fs](https://nodejs.org/api/fs.html) - Asynchronous File Sytem methods.
* [ESLint](https://eslint.org/) - Code Parsing, Styling & Error Checking.
* [Mocha-Chai](https://mochajs.org/) - Testing with Mocha Framework, using the Chai Library.

<br><hr><br>



<!-- Setup -->
## Installation
  ```sh
  npm install simple-txt-logger
  ```

<br><hr><br>



<!-- USAGE EXAMPLES -->
## Usage
By default, all .txt log files are placed in a 'logs' folder/directory, which is automatically created in the root folder of the app.

1. Create a new logger & log file, and continuously stream items or events to it:<br>*(Arguments are optional)*
  ```sh
  const logger = new SimpleTxtLogger('<FileName?>', '<Env?>', '<AppName?>');    //Create a logger instance.
  ```
  ```sh
  logger.writeToLogFile(<ItemToLog>);    //Logs an item to the loggers current .txt log file.

  logger.getPath();                      //Output: '<path>/logs/*.txt'.

  logger.close();                        //Closes stream to the loggers .txt log file.
  ```

2. Create a single data log dump, to log an item or event into a single txt file, one time only:<br>*('Directory' Argument is optional)*
  ```sh
  logger.dumpToNewTxtFile('<ItemToLog>', '<FileName>', '<Directory?>');    //Create a single item log file.
  ```


<br><br>

### Screenshots

Logging Sample<br>
![Screenshot#1](https://github.com/tberey/simple-txt-logger/blob/master/screenshots/local-logs-sample.png?raw=true)

Logging Sample#2<br>
![Screenshot#2](https://github.com/tberey/simple-txt-logger/blob/master/screenshots/local-logs-sample-two.png?raw=true)

<br><hr><br>



<!-- ROADMAP -->
## Roadmap
Below is the refined and confirmed roadmap, that has been planned for completion. See [open issues][issues-url] and also the [project board][project-url], for any other proposed features or known issues, which may not be listed below.

| Feature/Task/Bugfix | Details | Version <i>(if released)</i> | Notes |
|:---|:---|:---|:---|
| <i>Bug#1</i> | <i>Bug details...</i> | <i>0.0.1</i> | <i>example#1</i> |
| <i>Feature#4</i> | <i>Feature details...</i> |   | <i>example#2</i> |

<br><hr><br>



<!-- CHANGELOG -->
## Changelog

| Version | Date | Changes |
|:---|:---|:---|
| 1.0.0 | 2021-07-09 | <ul><li>Initial Commit - Release Day!</li><li>Add inital directory structure and files.</li><li>Add Screenshots directory, and images.</li><li>Create and format README.md</li></ul> |
| 1.0.1 | 2021-07-14 | <ul><li>NPM Package Release Day!</li><li>Update all dependancies.</li><li>Remove old test commands from package.json and codeql.yml.</li><li>Update README.md.</li></ul> |

<br><hr><br>



<!-- CONTRIBUTING -->
## Contributing
Contributions are welcomed and, of course, **greatly appreciated**.

1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/Feature`)
3. Commit your Changes (`git commit -m 'Add some Feature'`)
4. Push to the Branch (`git push origin feature/Feature`)
5. Open a Pull Request.

<br><hr><br>



<!-- CONTACT -->
### Contact

<b>Tom Berey</b>; <i>Project Manager, Lead Developer, Principal Tester & Customer Services;</i><br>tomberey1@gmail.com;

* [Issues & Requests.][issues-url]
* [My Other Projects.](https://github.com/tberey?tab=repositories)
* [Personal Website.](https://tberey.github.io/)
* [Linked In.](https://uk.linkedin.com/in/thomas-berey-2a1860129)

<br>

<!-- ACKNOWLEDGEMENTS -->
### Acknowledgements

* [Me](https://github.com/tberey)


<br><br><hr><div align="center">TomCo&trade; (Technology & Online Media Company &copy;)</div>


<!-- SPECIFIC URLS - NEED CHANGING PER PROJECT -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[workflow-shield]: https://github.com/tberey/simple-txt-logger/actions/workflows/codeql-analysis.yml/badge.svg
[workflow-url]: https://github.com/tberey/simple-txt-logger/actions
[version-shield]: https://img.shields.io/github/v/release/tberey/simple-txt-logger
[version-url]: https://github.com/tberey/simple-txt-logger/releases/
[stars-shield]: https://img.shields.io/github/stars/tberey/simple-txt-logger.svg
[stars-url]: https://github.com/tberey/simple-txt-logger/stargazers
[contributors-shield]: https://img.shields.io/github/contributors/tberey/simple-txt-logger.svg
[contributors-url]: https://github.com/tberey/simple-txt-logger/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/tberey/simple-txt-logger.svg
[forks-url]: https://github.com/tberey/simple-txt-logger/network/members
[issues-shield]: https://img.shields.io/github/issues/tberey/simple-txt-logger.svg
[issues-url]: https://github.com/tberey/simple-txt-logger/issues
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?logo=linkedin&colorB=555
[linkedin-url]: https://uk.linkedin.com/in/thomas-berey-2a1860129
[project-url]: https://github.com/tberey/simple-txt-logger/projects