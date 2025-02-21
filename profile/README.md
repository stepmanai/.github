<!-- PROJECT LOGO -->
<br />
<div align="center">
    <picture>
        <source srcset="assets/logo/stepman.ai/dark-mode/stepmanai.png"  media="(prefers-color-scheme: dark)">
        <img src="assets/logo/acubed/no-dark-mode/stepmanai.png" alt="Logo" width="200px" height=auto>
    </picture>
</div>

## Introduction
Welcome to `stepman.ai`, an organization devoted to support community-driven open source vertical scroll rhythm games through machine learning and artificial intelligence. Currently, `stepman.ai` supports the following games:
  <p align="center">
    <a href="https://etternaonline.com/"><picture>
        <source srcset="assets/logo/etterna/dark-mode.svg"  media="(prefers-color-scheme: dark)">
        <img src="assets/logo/etterna/no-dark-mode.svg" alt="Logo" width="50px" height=auto></a>
    </picture></a>ㅤ
    <a href="https://www.flashflashrevolution.com/"><picture>
        <source srcset="assets/logo/ffr/dark-mode.svg"  media="(prefers-color-scheme: dark)">
        <img src="assets/logo/ffr/no-dark-mode.svg" alt="Logo" width="50px" height=auto>
    </picture></a>ㅤ
    <a href="https://osu.ppy.sh/"><picture>
        <source srcset="assets/logo/osumania/dark-mode.svg"  media="(prefers-color-scheme: dark)">
        <img src="assets/logo/osumania/no-dark-mode.svg" alt="Logo" width="50px" height=auto>
    </picture></a>ㅤ
    <a href="https://quavergame.com/"><picture>
        <source srcset="assets/logo/quaver/dark-mode.svg"  media="(prefers-color-scheme: dark)">
        <img src="assets/logo/quaver/no-dark-mode.svg" alt="Logo" width="50px" height=auto>
    </picture></a>
  </p>

and offers modules to address several key challenges including:
- File format standardization to facilitate framework integration with `trancecode`
- Scalability of the definition of difficulty to minimize inherent biases and subjectivity with `acubed`
- Playing performance evaluations rewarded to players based on standard metrics in confusion matrices (e.g. accuracy, precision, etc.) with `psyduck`
- Cross-platform ranked leaderboards to measure and compare player’s skill under a modified ELO rating system with `stepman`

Each module is developed using the following technological stack:
<p align="center">
    <a href="https://www.python.org/"><picture>
        <source srcset="https://cdn.simpleicons.org/python/000/fff"  media="(prefers-color-scheme: dark)">
        <img src="https://cdn.simpleicons.org/python/000/000" alt="Logo" width="50px" height=auto></a>
    </picture></a>ㅤ
    <a href="https://github.com/features/actions"><picture>
        <source srcset="https://cdn.simpleicons.org/githubactions/000/fff"  media="(prefers-color-scheme: dark)">
        <img src="https://cdn.simpleicons.org/githubactions/000/000" alt="Logo" width="50px" height=auto></a>
    </picture></a>ㅤ
    <a href="https://ubuntu.com/"><picture>
        <source srcset="https://cdn.simpleicons.org/ubuntu/000/fff"  media="(prefers-color-scheme: dark)">
        <img src="https://cdn.simpleicons.org/ubuntu/000/000" alt="Logo" width="50px" height=auto></a>
    </picture></a>ㅤ
    <a href="https://pypi.org/"><picture>
        <source srcset="https://cdn.simpleicons.org/pypi/000/fff"  media="(prefers-color-scheme: dark)">
        <img src="https://cdn.simpleicons.org/pypi/000/000" alt="Logo" width="50px" height=auto></a>
    </picture></a>ㅤ
    <a href="https://www.mongodb.com/"><picture>
        <source srcset="https://cdn.simpleicons.org/mongodb/000/fff"  media="(prefers-color-scheme: dark)">
        <img src="https://cdn.simpleicons.org/mongodb/000/000" alt="Logo" width="50px" height=auto></a>
    </picture></a>
</p>

and operates under the overall `stepman.ai` ecosystem depicted in the following technical diagram:

```mermaid
%%{
  init: {
    'theme': 'dark',
    'themeVariables': {
      'fontFamily': 'courier',
      'fontSize': '12px'
    }
  }
}%%

flowchart LR

A1[ ]---|"External
Files"|B@{label: "trancecode" };
A4[ ]---|"In-Game
APIs"|B;
B ---|Standardized
File Format| C@{ label: "acubed" };
C---|"Stepfile
Features"|D1@{ label: "psyduck" };
C---|"Stepfile
Difficulty"|F@{ label: "Player 1" };
F -->|Player 1's
Score|D1;
D1 ---|Player 1's
Rating| D@{ label: "stepman" };
D --> G@{shape: braces, label: "Leaderboards"};

C ~~~ F3["..."] ~~~ |...| D3["..."] ~~~ |...| D@{ label: "stepman" };

C---|"Stepfile
Difficulty"|F2@{ label: "Player N" };
F2 -->|Player N's
Score|D2;
C---|"Stepfile
Features"|D2@{ label: "psyduck" };
D2 ---|Player N's
Rating| D@{ label: "stepman" };


click B "https://github.com/stepmanai/trancecode";
click C "https://github.com/stepmanai/acubed";
click D1 "https://github.com/stepmanai/psyduck";
click D2 "https://github.com/stepmanai/psyduck";
click D "https://github.com/stepmanai/stepman";
style A1 height:0px;
style A4 height:0px;
style D3 height:0px;
style F3 height:0px;
style F height:0px;
style F2 height:0px;


``` 
