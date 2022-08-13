# Model Template

[![GitHub](https://img.shields.io/github/license/Theia-Scientific/model-template)](https://github.com/Theia-Scientific/model-template/blob/main/LICENSE)
[![DOI](https://zenodo.org/badge/522758267.svg)](https://zenodo.org/badge/latestdoi/522758267)
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/Theia-Scientific/model-template)](https://github.com/Theia-Scientific/model-template/releases)

## Introduction

An example GitHub-hosted repository for a Machine Learning (ML) model using best
practices for model deployment. This repository can be used as a template for
hosting a ML model on GitHub for publishing to other "hubs" and to easily share
a model with anyone.

## Getting Started

1. Ensure [Python] >= v3.7.0 is installed on the computer.
2. Start a terminal. This can be [Windows Terminal], [Terminal.app], [Gnome
   Terminal], or similar application running a [shell], like [bash], [zsh],
   [PowerShell], etc.
3. Clone this repository.

   ```sh
   git clone https://github.com/Theia-Scientific/model-template.git
   ```

4. Navigate into the project's root folder, i.e. the same folder as this README
   file.

   ```sh
   cd model-template
   ```

5. Create a virtual environment to safely install the Python dependencies. This
   step only has to be done once. If a virtual environment already exists, then
   this step can be skipped.

   ```sh
   python3 -m venv .venv
   ```

   The `python3` command is used to ensure that the correct version of Python is
   used. Some system will have Python v2 and v3 installed and the `python`
   command will use Python v2.

6. Activate the virtual environment.

   ```sh
   source .venv/bin/activate
   ```

   The prompt in your terminal may change appearance to indicate you are in the
   virtual environment and are safe to install dependencies without clobbering
   the dependencies for other models installed on your computer.

7. Install the Python dependencies, i.e. requirements, into the virtual
   environment created in the previous step.

   ```sh
   python3 -m pip install -r requirements.txt
   ```

8. Run the inference.

   ```sh
   python3 detect.py --weights ./weights/cat-detector_v1.0.0.pt ./images/cats.jpg
   ```

## Citation

Please use the following BibTeX citation for including in bibliographies and
references:

```bibtex
@software{theia_scientific_model_template,
  author    = {Christopher Field and
               Kevin Field and
  title     = {{Theia-Scientific/model-template - A template repository
                for sharing Machine Learning models for the Nuclear Materials
                community}},
  month     = aug,
  year      = 2022,
  publisher = {zenodo},
  version   = {v1.0.0},
  doi       = {10.5281/zenodo.6977690},
  url       = {https://doi.org/10.5281/zenodo.6977690}
}
```

## Acknowledgments

This material is based upon work supported by the U.S. Department of Energy,
Office of Science, Office of Basic Energy Sciences under Award Number
DE-SC0021529.

## License

The model-template project is licensed under Apache-2.0 license. See the
[LICENSE] file for information.

[bash]: https://www.gnu.org/software/bash/
[gnome terminal]: https://help.gnome.org/users/gnome-terminal/stable/
[license]: https://github.com/Theia-Scientific/model-template/blob/main/LICENSE
[powershell]: https://docs.microsoft.com/en-us/powershell/
[python]: https://www.python.org/
[shell]: https://en.wikipedia.org/wiki/Shell_%28computing%29
[terminal.app]: https://support.apple.com/guide/terminal/welcome/mac
[windows terminal]: https://github.com/Microsoft/Terminal
[zsh]: https://www.zsh.org/
