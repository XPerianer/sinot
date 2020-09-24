
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



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
During my master thesis, I am focussing on causal effects in N of 1 studies. Unfortunately there was no library available, which meets my needs. Hence, I created my own library for simulating data in this context to test different methods on it.  

### Built With
This project is build on `python 3.8` and is using following libraries: 
* Numpy
* Pandas

For detailed description you can have a look into `requirements.txt`.


<!-- GETTING STARTED -->
## Getting Started
Here you can see, how to use the library.

### Prerequisites

Python is required for this package. For that, I used anaconda and created my own environment with in it. 
Afterwards I installed all requirements within this environment with:

```sh
pip install -r requirements.txt
```

### Installation

1. Clone the repo
```sh
git clone https://github.com/your_username_/Project-Name.git
```
2. Use the python functions within python or shell


<!-- USAGE EXAMPLES -->
## Usage

### Create Study Parameters
This project consists of 2 important files. The first oen is `creaty_study_parameters.py`. It transforms a DAGitty text file into the parameter file.
A DAGitty text file could be found at `./example/dagitty_example.txt`. 

A study parameter file `out.json` could be created by using:
```sh 
python create_study_params.py ./example/dagitty_example.txt example/out.json
```

If you need help, you can simply use the option `--help`:
```sh 
python create_study_params.py --help
```

### Simulate Data


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

Thomas Gärtner - [![LinkedIn][linkedin-shield]][linkedin-url] - thomas.gaertner@student.hpi.de

Project Link: [https://github.com/tommysft/n-of-1-simulation](https://github.com/tommysft/n-of-1-simulation)



<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/tommysft/n-of-1-simulation.svg?style=flat-square
[contributors-url]: https://github.com/tommysft/n-of-1-simulation/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/tommysft/n-of-1-simulation.svg?style=flat-square
[forks-url]: https://github.com/tommysft/n-of-1-simulation/network/members
[stars-shield]: https://img.shields.io/github/stars/tommysft/n-of-1-simulation.svg?style=flat-square
[stars-url]: vhttps://github.com/tommysft/n-of-1-simulation/stargazers
[issues-shield]: https://img.shields.io/github/issues/tommysft/n-of-1-simulation.svg?style=flat-square
[issues-url]: https://github.com/tommysft/n-of-1-simulation/issues
[license-shield]: https://img.shields.io/github/license/tommysft/n-of-1-simulation.svg?style=flat-square
[license-url]: XXX
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/thomas-g%C3%A4rtner-490658143/