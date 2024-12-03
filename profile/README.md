<!-- PROJECT LOGO -->
<br />
<div align="center">
    <picture>
        <source srcset="assets/logo/acubed/dark-mode/acubed-logo.png"  media="(prefers-color-scheme: dark)">
        <img src="assets/logo/acubed/no-dark-mode/acubed-logo.png" alt="Logo" width="200px" height=auto>
    </picture>
  <br />
  <br />
  <p align="center">
    A machine learning framework designed to standardize skill measurement in community-based vertical scroll rhythm games.
  </p>
  <br />
</div>

## Motivation

Establishing a consistent method for measuring skill in vertical scroll rhythm games is crucial for ensuring fairness and competitiveness in tournaments. In the absence of a unified system, players from different rhythm game communities are often mismatched within divisions, resulting in unsatisfactory experiences. Each game utilizes distinct difficulty scales and mechanics to assess player performance, complicating the accurate comparison of skill levels across games and leading to divisions that fail to reflect comparable abilities. A more integrated approach to skill measurement would promote greater balance and enhance the overall tournament experience for all participants.

## Introduction
ACubed is a model framework developed to standardize skill measurement across vertical scroll rhythm games. By leveraging machine learning, it constructs game-independent models that evaluate player performance, taking into account the unique mechanics and difficulty scales of each game to enable more accurate skill comparisons. Currently, ACubed supports the following games:
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

and addresses several key challenges by:
- Standardizing map file formats to facilitate model integration
- Refining the definition of stepfile difficulty through comprehensive chart analysis
- Evaluating player performance on individual stepfiles
- Aggregating player scores to derive a comprehensive overall rating

