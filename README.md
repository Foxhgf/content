# Welcome to MDN Web Docs

![github-profile](https://user-images.githubusercontent.com/10350960/166113119-629295f6-c282-42c9-9379-af2de5ad4338.png)

[MDN Web Docs][] is an open-source, collaborative project that documents web technologies including CSS, HTML, JavaScript, and Web APIs.
Alongside detailed reference documentation, we provide extensive learning resources for students and beginners getting started with web development.
LICENSE.md
## MDN's mission

MDN's mission is to provide a blueprint for a better internet and empower a new generation of developers and content creators to build it.

The strength of MDN Web Docs lies in its vast community of active readers and contributors.
Since 2005, approximately 45,000 contributors have created the documentation we know and love.
Together, contributors have created over 45,000 documents that make up an up-to-date, comprehensive, and free resource for web developers worldwide.

In addition to English-language articles, over 35 volunteers lead translation and localization efforts for Chinese, French, Japanese, Korean, Portuguese, Russian, and Spanish.

## Build the site

To set up the site locally, you need to have [Node.js](https://nodejs.org/) and [Yarn](https://yarnpkg.com/) installed.
You can check if these are installed by running the following commands:

```bash
node -v
yarn -v
```

After you have installed Node.js and Yarn, you can install the dependencies using `yarn` and start the local preview:

```bash
yarn
yarn start
```

Once started, a live preview is available at `http://localhost:5042/`.

## Contribute to MDN Web Docs

You can contribute to MDN Web Docs and be a part of our community through content contributions, engineering, or translation work.
The MDN Web Docs project welcomes contributions from everyone who shares our goals and wants to contribute constructively and respectfully within our community.

To find out how to get started, see the [CONTRIBUTING.md](CONTRIBUTING.md) document in this repository.
By participating in and contributing to our projects and discussions, you acknowledge that you have read and agree to our [Code of Conduct](CODE_OF_CONDUCT.md).

## Get in touch

You can communicate with the MDN Web Docs team and community using the [communication channels][].
https://github.com/Foxhgf/Foxhgf/pull/8/files
[communication channels]: https://developer.mozilla.org/en-US/docs/MDN/Community/Communication_channels
[MDN Web Docs]: https://
developer.mozilla.org/
    # This is a basic workflow to help you get started with Actions

name: CI

# Controls when the workflow will run
on:
  # Triggers the workflow on push or pull request events but only for the "main" branch
  push:
    branches: [ "main" ]
  pull_request:
    branches: [ "main" ]

  # Allows you to run this workflow manually from the Actions tab
  workflow_dispatch:

# A workflow run is made up of one or more jobs that can run sequentially or in parallel
jobs:
  # This workflow contains a single job called "build"
  build:
    # The type of runner that the job will run on
    runs-on: ubuntu-latest

    # Steps represent a sequence of tasks that will be executed as part of the job
    steps:
      # Checks-out your repository under $GITHUB_WORKSPACE, so your job can access it
      - uses: actions/checkout@v3

      # Runs a single command using the runners shell
      - name: Run a one-line script
        run: echo Hello, world!

      # Runs a set of commands using the runners shell
      - name: Run a multi-line script
        run: |
          echo Add other actions to build,
          echo test, and deploy your project.
