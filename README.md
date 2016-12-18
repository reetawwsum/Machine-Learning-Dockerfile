# Machine-Learning-Dockerfile
Dockerfile for Machine Learning

## Features

1. CentOS 7
2. Python 2.7.12
3. pip
4. IPython
5. jupyter
6. matplotlib
7. nltk
8. NumPy
9. pandas
10. scikit-learn
11. SciPy
12. virtualenv

## Usage

To launch Jupyter Notebook

	$ docker run --rm -t -i --name ml -p 8888:8888 machine-learning --ip=0.0.0.0

To launch Jupyter Notebook on current directory

	$ docker run --rm -t -i --name ml -p 8888:8888 -v $PWD:/usr/local/src/notebooks machine-learning --ip=0.0.0.0

To run shell after launching Jupyter Notebook

	$ docker exec -t -i ml /bin/bash

To run Python REPL after launching Jupyter Notebook

	$ docker exec -t -i ml python2.7

To build image from Dockerfile

	$ git clone https://github.com/reetawwsum/Machine-Learning-Dockerfile.git
	$ cd Machine-Learning-Dockerfile
	$ docker build -t machine-learning .

## License
[The MIT License (MIT)](LICENSE)
