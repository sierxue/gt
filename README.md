[![Build
Status](https://travis-ci.org/drvinceknight/gt.svg?branch=master)](https://travis-ci.org/drvinceknight/gt)

# Game Theory

## Description

This is a course on Game theory. It covers 3 main topics:

1. Equilibrium computation and Repeated games;
2. Evolutionary game theory;
3. Current research topics

The course is taught in an active learning framework with class time being used
for activities and demonstrations whilst the content is made available to the
students at the start of the course.

Throughout this course concepts are illustrated/demonstrated using
Python. In particular the following libraries are used:

- [Nashpy](https://github.com/drvinceknight/Nashpy): computation of
  equilibria.
- [Axelrod](http://axelrod.readthedocs.io/en/stable/): study of the Iterated
  Prisoner's Dilemma.
- [Sympy](http://www.sympy.org/en/index.html): used to verify and carry out
  symbolic computations.
- [Numpy](http://www.numpy.org): used for various linear algebraic calculations.

## Syllabus

- Normal Form Games
- Nash equilibrium
- Repeated games
- Evolutionary game theory
- Contemporary research

## Notes

Teaching notes are available here http://vkgt.readthedocs.io/en/latest/

## Contents of this repository

```
|--- README.md
|--- environment.yml  # A conda environment file
|--- render.py  # A file to serve the static content
|--- nbtests.py  # A file to test the notebooks
|--- doctests.py  # A file to test the code in the docs
|--- docs  # documentation (notes for the class leader)
|--- nbs  # nbs representing content for the site
     |--- chapters  # Chapters for the course
|--- index.html  # A landing webpage automatically generated by static.py
|--- chapters  # Served content
     |--- 00  # Content directories automatically generated by static.py
     |--- 01
     |--- ...
```

## Serving the content

All the content of the site is written in [Jupyter](http://jupyter.org/)
notebooks in the `nbs` directory. These are used to create `.html`
versions of the content. To generate all the files:

```
$ python render.py
```

This requires python 3+. An anaconda virtual environment file `environment.yml`
is available.
