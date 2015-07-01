# Docker-LaTeX
A container for compiling LaTeX to PDF. Is available on the Docker hub as tebro/latex.


### Usage

```
docker run -it --rm -v $(pwd):/src tebro/latex
```

Hit enter, it then asks which file to use, enter the name and hit enter.


If you need more dependencies you can use a `FROM tebro/latex` statement in your own Dockerfile.
