
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]

# Simulation of N-of-One Trials (SiNOT)

<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
  * [Built With](#built-with)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
* [Usage](#usage)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#contact)
* [Acknowledgements](#acknowledgements)



<!-- ABOUT THE PROJECT -->
## About The Project
The project started with a master thesis on analysing causal effects in N of 1 studies. Unfortunately there was no library available, which meets the needs. Hence, this package was created. Within this package, data of N-of-1 studies could be created though a DAG file and a configuration file. A preprint of the related publication could be found on [medRxiv](https://www.medrxiv.org/content/10.1101/2022.07.21.22277832v1).

### Built With
This project is build on `python 3.8` and is using following libraries: 
* Numpy
* Pandas
* (Matplotlib)

For detailed description you can have a look into `requirements.txt`.


<!-- GETTING STARTED -->
## Getting Started
Here you can see, how to use the library.

### Prerequisites

Python is required for this package. For that, I used anaconda and created my own environment with in it. 
Afterwards I installed all requirements within this environment with:

```shell
pip install -r requirements.txt
```

### Installation

1. Clone the repo
```shell
git clone https://github.com/thogaertner/n-of-1-simulation
```
2. Use the python functions within python or shell


<!-- USAGE EXAMPLES -->
## Usage

### Create Study Parameters
This project consists of 2 functions. The first oen is `creat_study_parameters.py`. It transforms a DAGitty text file into the parameter file.
A DAGitty text file could be found at `./example/dagitty_example.txt`. 

A study parameter file `out.json` could be created by using:
```shell
python create_study_params.py ./example/dagitty_example.txt example/out.json
```

If you need help, you can simply use the option `--help`:
```shell 
python create_study_params.py --help
```

### Simulate Data

To simulate data, you use functions from `simulation.py` to create a cohort based on a parameters file.

```python
sim = Simulation(study_params)
pat_complete, pat_drop = sim.gen_patient(study_design, days_per_period, drop_out=drop_out)
```

A complete example of simulation data could be found in `Simulate_Example.ipynb`.


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

Thomas Gärtner - [Linked In][linkedin-url] - [thomas.gaertner[at]hpi.de](mailto:thomas.gaertner@hpi.de)

Project Link: [https://www.github.com/HIAlab/sinot](https://www.github.com/HIAlab/sinot)



<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/thogaertner/sinot.svg?style=flat-square
[contributors-url]: https://github.com/thogaertner/sinot/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/thogaertner/sinot.svg?style=flat-square
[forks-url]: https://github.com/thogaertner/sinot/network/members
[stars-shield]: https://img.shields.io/github/stars/thogaertner/sinot.svg?style=flat-square
[stars-url]: vhttps://github.com/thogaertner/sinot/stargazers
[issues-shield]: https://img.shields.io/github/issues/thogaertner/sinot.svg?style=flat-square
[issues-url]: https://github.com/thogaertner/sinot/issues
[license-shield]: https://img.shields.io/github/license/thogaertner/sinot.svg?style=flat-square
[license-url]: https://github.com/thogaertner/sinot/blob/master/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/thomas-g%C3%A4rtner-490658143/
