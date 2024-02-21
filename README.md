# quarto-reprex
examples are stored in subdirectories

## Render the example

Using quarto 1.4.550 on Ubuntu linux, render the example

    quarto render presentation/presentation.qmd

this should open a browser tab

    head --bytes=80 presentation/presentation_files/libs/revealjs/dist/theme/quarto.css

shows that the combined css is wrong, it should not be using the Montserrat font.
When rendering with quarto 1.4.550 on macOS, the combined css is correct.

This problem only shows up in the reprex after adding the theme setting.
