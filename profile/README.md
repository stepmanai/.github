<!-- PROJECT LOGO -->
![GitHub-Mark-Light](https://user-images.githubusercontent.com/3369400/139447912-e0f43f33-6d9f-45f8-be46-2df5bbc91289.png#gh-dark-mode-only)![GitHub-Mark-Dark](https://user-images.githubusercontent.com/3369400/139448065-39a229ba-4b06-434b-bc67-616e2ed80c8f.png#gh-light-mode-only)

![GitHub-Mark-Light](assets/logo/stepman.ai/dark-mode/stepmanai.png#gh-dark-mode-only)![GitHub-Mark-Dark](assets/logo/stepman.ai/no-dark-mode/stepmanai.png#gh-light-mode-only)

<br />
<div align="center">
    <picture>
        <source srcset="assets/logo/stepman.ai/dark-mode/stepmanai.png"  media="(prefers-color-scheme: dark)">
        <img src="assets/logo/stepman.ai/no-dark-mode/stepmanai.png" alt="Logo" width="200px" height=auto>
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
        <source srcset="assets/logo/ffr/dark-mode.svg" media="(prefers-color-scheme: dark)">
        <img src="assets/logo/ffr/no-dark-mode.svg" alt="Logo" width="50px" height=auto>
    </picture></a>ㅤ
    <a href="https://osu.ppy.sh/"><picture>
        <source srcset="assets/logo/osumania/dark-mode.svg" media="(prefers-color-scheme: dark)">
        <img src="assets/logo/osumania/no-dark-mode.svg" alt="Logo" width="50px" height=auto opacity=0.3>
    </picture></a>ㅤ
    <a href="https://quavergame.com/"><picture>
        <source srcset="assets/logo/quaver/dark-mode.svg" media="(prefers-color-scheme: dark)">
        <img src="assets/logo/quaver/no-dark-mode.svg" alt="Logo" width="50px" height=auto opacity=0.3>
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
    <a href="https://www.docker.com/"><picture>
        <source srcset="https://cdn.simpleicons.org/docker/000/fff"  media="(prefers-color-scheme: dark)">
        <img src="https://cdn.simpleicons.org/docker/000/000" alt="Logo" width="50px" height=auto></a>
    </picture></a>ㅤ
    <a href="https://supabase.com/"><picture>
        <source srcset="https://cdn.simpleicons.org/supabase/000/fff"  media="(prefers-color-scheme: dark)">
        <img src="https://cdn.simpleicons.org/supabase/000/000" alt="Logo" width="50px" height=auto></a>
    </picture></a>ㅤ
    <a href="https://duckdb.org/"><picture>
        <source srcset="https://cdn.simpleicons.org/duckdb/000/fff"  media="(prefers-color-scheme: dark)">
        <img src="https://cdn.simpleicons.org/duckdb/000/000" alt="Logo" width="50px" height=auto></a>
    </picture></a>ㅤ
    <a href="https://www.dotenv.org/"><picture>
        <source srcset="https://cdn.simpleicons.org/dotenv/000/fff"  media="(prefers-color-scheme: dark)">
        <img src="https://cdn.simpleicons.org/dotenv/000/000" alt="Logo" width="50px" height=auto></a>
    </picture></a>ㅤ
    <a href="https://www.getdbt.com/"><picture>
        <source srcset="https://cdn.simpleicons.org/dbt/000/fff"  media="(prefers-color-scheme: dark)">
        <img src="https://cdn.simpleicons.org/dbt/000/000" alt="Logo" width="50px" height=auto></a>
    </picture></a>
</p>

and operates under the overall `stepman.ai` ecosystem depicted in the following technical diagram:

```mermaid
%%{
  init: {
    'themeVariables': {
      'fontFamily': 'courier',
      'fontSize': '12px'
    }
  }
}%%

flowchart LR

D1 ---|Player's
Score from
Stepfile| R@{shape: sm-circ} ---|Player's
High
Scores| D

D3["..."] -.-|Player's
Scores from
Other Stepfiles| R;

F2 -.-> H@{shape: braces, label: "Other
Players"} -.- D2["..."]

D@{ label: "stepman.rating" } --> G@{shape: braces, label: "Overall
Leaderboards"};
C@{ label: "acubed.features" }---|"Stepfile
Features"|F2@{shape: sm-circ} -->F;
B ---|Stepfile| P@{shape: sm-circ} --> C;
P --> C1@{ label: "acubed.difficulty" }---|"Stepfile
Difficulty"|F2@{shape: sm-circ}

C---|"Stepfile
Features"|D1

A4[ ]---|"In-Game
APIs"|B;
A1[ ]---|"External
Files"|B@{label: "trancecode" };

B -.-|Other
Stepfiles| D4["..."];

F@{shape: braces, label: "Player"} -->|Playing
Performance|D1@{ label: "stepman.score" };

D2-.-|Other 
Players'
High
Scores|D;

click B "https://github.com/stepmanai/trancecode";
click C "https://github.com/stepmanai/acubed";
click C1 "https://github.com/stepmanai/acubed";
click D1 "https://github.com/stepmanai/stepman";
click D "https://github.com/stepmanai/stepman";
style A1 height:0px;
style A4 height:0px;
style D2 height:0px;
style D3 height:0px;
style D4 height:0px;

``` 
