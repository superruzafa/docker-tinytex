# My TinyTeX Docker image

A Docker image that contains a basic installation of [TinyTex] along with several
utilities like [pdf2svg].

## Usage

Create a Dockerfile using this image as base and then install all TeX
packages you want.

```
FROM superruzafa/tinytex

# Install TeX packages

RUN tlmgr install standalone
RUN tlmgr install pgf
...
```

[TinyTeX]: https://yihui.org/tinytex/
[pdf2svg]: https://github.com/dawbarton/pdf2svg