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
- Playing performance evaluations based on accuracy and precision to objectively reward players with `pa-scoring`
- Cross-platform ranked leaderboards to measure and compare player’s skill under a modified ELO rating system with `stepman-rating`

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

flowchart TD

subgraph Z["<div style="width:25em; display:flex;">stepman.ai</div>"]
direction LR
B@{ label: "trancecode" } --> C@{ label: "acubed" }; 
C --> D1@{ label: "pa-scoring" };
D1 --> D@{ label: "stepman-rating" };
end

A1[ ]---|"External Files"|B;
A4[ ]---|"In-Game APIs"|B;
C---|"Stepfile
Difficulty"|C1[ ];
E1[ ]---|Player's Score|D1;
D---|Player's Rating|E2[ ];
click B "https://github.com/stepmanai";
click C "https://github.com/stepmanai";
click D1 "https://github.com/stepmanai";
click D "https://github.com/stepmanai";
style A1 height:0px;
style A4 height:0px;
style C1 height:0px;
style E1 height:0px;
style E2 height:0px;

``` 
