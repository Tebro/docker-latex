# Docker-LaTeX
A container for compiling LaTeX to PDF. Is available on the Docker hub as tebro/latex.


### Usage

To run a one-off compilation do:

```
docker run -it --rm -v $(pwd):/src tebro/latex pdflatex ./hello.tex
```

If you want to keep the container running and watching for changes, and then recompile you can do:

```
docker run -it --rm -v $(pwd):/src tebro/latex latexmk -pvc -pdf ./hello.tex
```

If you need more dependencies you can use a `FROM tebro/latex` statement in your own Dockerfile.
