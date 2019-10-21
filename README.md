# Uzu Demo Site

The `master` branch contains the HTML files for the website rendered
using the static site generator
[Uzu](https://github.com/scmorrison/uzu#getting-started). The resulting 
website is located at https://uzluisf.github.io/uzu-demo-site/.

The content files and theme used to generate the HTML are on the
`source` branch.

### Requirements

- Perl 6 (see https://perl6.org/downloads/ for installation instructions)
- Uzu
    - Using zef: `zef install Uzu`
    - From source:
    ```
    git clone https://github.com/scmorrison/uzu.git
    cd uzu && zef install .
    ```

### Rendering the website

After everything is properly setup:

1. Clone the `source` branch and `cd` into `uzu-demo-site`

```
$ git clone --single-branch --branch source https://github.com/uzluisf/uzu-demo-site.git
$ cd uzu-demo-site
```

2. Render all templates and content files

```
$ uzu build
```

A `build` directory will be created. You can either open it with a browser 
and navigate to each HTML file to view it. Or else...

3. Start a local web server

```
$ uzu webserver
```

By default, the site will be served at http://0.0.0.0:3000/.
