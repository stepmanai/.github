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
- Objective stepfile feature extraction and unbiased difficulty measurement with `acubed`
- Cross-platform ranked leaderboards to measure playing performance and compare player skill with `stepman`

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

and operates under the overall `stepman.ai` ecosystem depicted in the following technical diagram for $M$ players and $N$ stepfiles:

```mermaid
%%{
  init: {
    'theme': 'dark',
    'themeVariables': {
      'fontFamily': 'courier',
      'fontSize': '12px',
      'secondaryColor': '#006100'
    }
  }
}%%

flowchart LR

A1[ ]---|"External
Files"|B@{label: "trancecode" };
A4[ ]---|"In-Game
APIs"|B;

B ---|"Stepfile 1"| C@{ label: "acubed" };
C---|"Stepfile
Features"|D1@{ label: "stepman" };
C---|"Stepfile
Difficulty"|F@{ shape: braces, label: "Player 1" };
F -->|Player 1's
Score|D1;
D1 ---|Player 1's
Rating| D@{ label: "stepman" };
D --> G@{shape: braces, label: "Stepfile 1
Leaderboards"};

C ~~~ F3@{ label: "⋮" } ~~~ |⋮| D3["⋮"] ~~~ |⋮| D@{ label: "stepman" };

C---|"Stepfile
Difficulty"|F2@{ shape: braces, label: "Player M" };
F2 -->|Player M's
Score|D2;
C---|"Stepfile
Features"|D2@{ label: "stepman" };
D2 ---|Player M's
Rating| D@{ label: "stepman" };

B ~~~|⋮| C33["⋮"]

B ---|"Stepfile N"| C11@{ label: "acubed" };
C11---|"Stepfile
Features"|D111@{ label: "stepman" };
C11---|"Stepfile
Difficulty"|F11@{ shape: braces, label: "Player 1" };
F11 -->|Player 1's
Score|D111;
D111 ---|Player 1's
Rating| D11@{ label: "stepman" };
D11 --> G11@{shape: braces, label: "Stepfile N
Leaderboards"};

C11 ~~~ F311@{ label: "⋮" } ~~~ |⋮| D311["⋮"] ~~~ |⋮| D11@{ label: "stepman" };

C11---|"Stepfile
Difficulty"|F211@{ shape: braces, label: "Player M" };
F211 -->|Player M's
Score|D211;
C11---|"Stepfile
Features"|D211@{ label: "stepman" };
D211 ---|Player M's
Rating| D11@{ label: "stepman" };

G--> H1@{ label: "stepman" }--> H@{ shape: braces, label: "Overall
Leaderboards" }
Q["⋮"]~~~P["⋮"]~~~H1
G11--> H1

click B "https://github.com/stepmanai/trancecode";
click C "https://github.com/stepmanai/acubed";
click D1 "https://github.com/stepmanai/stepman";
click D2 "https://github.com/stepmanai/stepman";
click D "https://github.com/stepmanai/stepman";
click C11 "https://github.com/stepmanai/acubed";
click D111 "https://github.com/stepmanai/stepman";
click D211 "https://github.com/stepmanai/stepman";
click D11 "https://github.com/stepmanai/stepman";
click H1 "https://github.com/stepmanai/stepman";
style A1 height:0px;
style A4 height:0px;
style D3 height:0px;
style F3 height:0px;
style Q height:0px;
style P height:0px;
classDef test font-size:24px
class F3 test
class D3 test
class C33 test
class Q test
class P test
style D311 height:0px;
style F311 height:0px;
linkStyle 9 font-size:24px
linkStyle 10 font-size:24px
class F311 test
class D311 test
linkStyle 23 font-size:24px
linkStyle 24 font-size:24px
style C33 height:0px;
linkStyle 15 font-size:24px

``` 
