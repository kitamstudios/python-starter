[![Continuos Deployment](https://github.com/kitamstudios/python-starter/workflows/Continuos%20Deployment/badge.svg)](https://github.com/kitamstudios/python-starter/actions?query=workflow%3A%22Continuous+Integration%22)

# Kitam Studios - Template for Python Applications

## Getting started

```sh
conda env create -f .environment.yml
pip install -r requirements.txt
```

## Available out of the box

- Core
  - [x] editorconfig, prospector, black
  - [x] Unit tests: pytest
  - [ ] pre-commit integration
- VSCode
  - [x] pytest
  - [x] editorconfig, prospector, black
  - [x] configure settings
  - [x] recommended extensions
  - [x] F5 debugging from VSCode
- CI/CD
  - [x] lint, black, unit test github workflow

## Useful documents

- [Getting Started with Python in VS Code](https://code.visualstudio.com/docs/python/)

## Available Scripts

In the project directory, you can run:

- Style check: ```black . --check --color --diff --target-version py37```
- Lint: ```prospector```
- Unit tests: ```pytest```

## Other Miscellaneous

### Environment setup

- Create new environment
  - Setup conda
    ```sh
    conda deactivate
    conda env remove --name my.py.proj.1
    conda create --name my.py.proj.1 python=3.7
    conda activate my.py.proj.1
    ```
  - Install dependencies
    ```
    # conda install numpy
    ```
- Export environment
  ```sh
  conda env export --name my.py.proj.1 >.environment.yml
  ```

- Import environment
  ```sh
  conda env create -f .environment.yml
  ```

- Load anaconda:
  ```sh
  & 'C:\Users\partho\Anaconda3\shell\condabin\conda-hook.ps1' ; conda activate 'C:\Users\partho\Anaconda3' ; cd d:\src\c
  ```
