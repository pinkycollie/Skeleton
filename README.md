<h1 align="center">👋 Sign Translate - Skeleton Fork</h1>

<p align="center">
  <i>
    Revolutionizing Sign Language Communication with Cutting-Edge Real-Time Translation Models.
    <br>
    Enjoy seamless Sign Language Translation on desktop and mobile.
  </i>
</p>

<p align="center">
  <strong>Forked from <a href="https://sign.mt/">sign.mt</a></strong>
  <br>
</p>

<p align="center">
  <a href="https://github.com/pinkycollie/Skeleton/issues">Submit an Issue</a>
</p>

<p align="center">
  <a href="https://github.com/pinkycollie/Skeleton/blob/master/LICENSE.md">
    <img src="https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg" alt="License: CC BY-NC-SA 4.0 Badge" />
  </a>
</p>

<p align="center">
  <a href="https://github.com/pinkycollie/Skeleton/stargazers" target="_blank">
    <img src="https://img.shields.io/github/stars/pinkycollie/Skeleton" alt="GitHub Stars for pinkycollie/Skeleton" />
  </a>
  <a href="https://github.com/pinkycollie/Skeleton/network/members" target="_blank">
    <img src="https://img.shields.io/github/forks/pinkycollie/Skeleton" alt="GitHub Forks for pinkycollie/Skeleton" />
  </a>
  <a href="https://github.com/pinkycollie/Skeleton/stargazers" target="_blank">
    <img src="https://img.shields.io/github/contributors/pinkycollie/Skeleton" alt="GitHub Contributors for pinkycollie/Skeleton" />
  </a>
  <a href="https://github.com/pinkycollie/Skeleton/issues" target="_blank">
    <img src="https://img.shields.io/github/issues/pinkycollie/Skeleton" alt="GitHub Issues for pinkycollie/Skeleton" />
  </a>
</p>

<p align="center">
  <a href="https://sign.mt" target="_blank">
    <img src="src/assets/promotional/about/hero.webp" alt="Sign Language Translation Demo Image" />
  </a>
</p>

<hr>

## Key Features

### Sign Language Production

```
┌─────────────────────┐
│Spoken Language Audio│                                                              ┌─────────┐
└─────────┬───────────┘                                                  ┌──────────►│Human GAN│
          │                                                              │           └─────────┘
          ▼                                                              │
┌────────────────────┐     ┌───────────────┐     ┌───────────┐    ┌──────┴──────┐    ┌───────────────┐
│Spoken Language Text├────►│Normalized Text├────►│SignWriting├───►│Pose Sequence├───►│Skeleton Viewer│
└─────────┬──────────┘     └───────────────┘     └───────────┘    └──────┬──────┘    └───────────────┘
          │                        ▲                   ▲                 │
          ▼                        │                   │                 │           ┌─────────┐
┌───────────────────────┐          │                   │                 └──────────►│3D Avatar│
│Language Identification├──────────┘───────────────────┘                             └─────────┘
└───────────────────────┘
```

### Sign Language Translation

```
┌──────────────────────────┐                                ┌────────────────────┐
│Upload Sign Language Video│                      ┌────────►│Spoken Language Text│
└──────────┬───────────────┘                      │         └──────────┬─────────┘
           │                                      │                    │
           │          ┌────────────┐       ┌──────┴────┐               │
           ├─────────►│Segmentation├──────►│SignWriting│               │
           │          └────────────┘       └───────────┘               │
           │                                                           ▼
┌──────────┴────────────────┐                               ┌─────────────────────┐
│Camera Sign Language Video │                               │Spoken Language Audio│
└───────────────────────────┘                               └─────────────────────┘
```

### Want to Help?

Join us on the journey to revolutionize sign language communication.

Wish to report a bug, contribute some code, or enhance documentation? Fantastic!
Explore our issues and contribute to the project.

**Find this useful? Give our repo a star :star: :arrow_up:.**

### Original Project

This is a fork of the original [sign.mt](https://sign.mt/) project by [sign/translate](https://github.com/sign/translate).
For the original project documentation and contributing guidelines, please visit the [original repository](https://github.com/sign/translate).

## Development

### Prerequisites

- Install [Node.js] which includes [Node Package Manager][npm]

### Setting Up the Project

Install dependencies locally:

```bash
npm install
```

Run the application:

```bash
npm start
```

Test the application:

```bash
npm test
```

Run the application on iOS:

```bash
npm run build:full && \
npx cap sync ios && \
npx cap run ios
```

[node.js]: https://nodejs.org/
[npm]: https://www.npmjs.com/get-npm

### Cite

```bibtex
@misc{moryossef2023signmt,
    title={sign.mt: Effortless Real-Time Sign Language Translation},
    author={Moryossef, Amit},
    howpublished={\url{https://sign.mt/}},
    year={2023}
}
```
