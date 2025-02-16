<!-- PROJECT LOGO -->
<br />
<div align="center">
    <picture>
        <source srcset="assets/logo/stepman.ai/dark-mode/stepmanai.png"  media="(prefers-color-scheme: dark)">
        <img src="assets/logo/acubed/no-dark-mode/stepmanai.png" alt="Logo" width="200px" height=auto>
    </picture>
  <br />
  <br />
  <p align="center">
    A suite of machine learning algorithms to support the development of community-driven open source vertical scroll rhythm games.
  </p>
  <br />
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

And operates under the overall `stepman.ai` ecosystem depicted in the following technical diagram:

```mermaid
flowchart LR;
    A-->B["B#dagger; (internal link)"];
    B-->C;
    C-->D["D#ddagger; (external link)"];
    click B "https://gist.github.com/ChristopherA/bffddfdf7b1502215e44cec9fb766dfd/#flowchart-with-hyperlinks"
    click D "https://gist.github.com/ChristopherA/"
``` 