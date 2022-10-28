# scala-playground

## Development

First of all, install [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (if necessary).

```bash
conda env create -f environment.yml
```

```bash
conda activate scala-playground
```

```bash
jupyter lab
```

## Notes

- [Install coursier](https://get-coursier.io/docs/cli-installation#macos-brew-based-installation) (macOS):
  - `brew install coursier/formulas/coursier`
  - `cs setup`
- [noether](https://github.com/spotify/noether) package:
  - Model Evaluation package by Spotify
  - [Documentation](https://spotify.github.io/noether/latest/api/com/spotify/noether/index.html)
  - [Maven Central Repository](https://search.maven.org/artifact/com.spotify/noether-core_2.12/0.4.1-M2/jar)
- [almond](https://almond.sh/):
  - Scala kernel for Jupyter
  - [Repo](https://github.com/almond-sh/almond)
  - [Examples](https://github.com/almond-sh/examples)
  - [almond-scalafmt](https://github.com/almond-sh/almond-scalafmt) extension
  - Install ([options](https://almond.sh/docs/install-options)):
    - `cs launch --fork almond:0.13.1 --scala 2.12 -- --install --jupyter-path ~/opt/miniconda3/envs/scala-playground/share/jupyter/kernels` ([launch command](https://get-coursier.io/docs/cli-launch))
  - Uninstall:
    - `jupyter kernelspec list`
    - `jupyter kernelspec remove scala`
