# Quarto TUM output format

## Create a new project

```bash
quarto use template alpkaanaksu/tum
```

This will install the extension and create an example qmd file that you can use as a starting place for your thesis.

## Using

You can write your chaters under 'chapters/' and include them in your document by using quarto shorcodes: `{{< include chatpters/chapter_name.qmd >}}`

## Rendering

Make sure you have the following in your main .qmd file:

```yaml
format:
  tum-pdf: default
```

Then, simply run:
```{bash}
quarto render <filename>.qmd
```

## Format Options

| option | explanation |
| --- | --- |
| `university` | Name of the university, default: Technical University of Munich |
| `faculty` | Name of the faculty, default: School of Computation, Information and Technology - Informatics |
| `author` | Name of the author |
| `supervisor` | Name of the supervisor |
| `advisor` | Name of the advisor |
| `date` | Submission date |
| `location` | Submission location, default: Munich |
| `abstract` | Abstract |
| `acknowledgements` | Acknowledgements |


## License

[![Creative Commons License][license-image]][license]

This Quarto template builds upon the work of [Florian Walch and other contributors][template-authors]. The original template can be found [here][template-url].

This template is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License][license], meaning that:

* You can share (copy, redistribute) and adapt (remix, transform, build upon) this template for any purpose, even commercially.
* If you share the template or a modified (derived) version of it, you must attribute the template to the original authors.
* Any derived template has to use the [same][license] or a [compatible license][license-compatible].


 The license **applies only to the template**; there are no restrictions on the resulting PDF file or the contents of your thesis.


[license-compatible]: https://creativecommons.org/compatiblelicenses
[license-image]: https://i.creativecommons.org/l/by-sa/4.0/88x31.png
[license]: https://creativecommons.org/licenses/by-sa/4.0/

[template-authors]: https://github.com/TUM-Dev/tum-thesis-latex/graphs/contributors
[template-download]: https://github.com/TUM-Dev/tum-thesis-latex/archive/master.zip
[template-url]: https://github.com/TUM-Dev/tum-thesis-latex
