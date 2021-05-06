## Bookdown installation 

To use Bookdown we first you need to install:
* [R](https://www.r-project.org/) programming language. 
* The development environment [RStudio](https://www.rstudio.com/).
* Add the R packages [Bookdown](https://github.com/rstudio/bookdown) and [JuliaCall]( https://github.com/Non-Contradiction/JuliaCall)
    NOTE: For the time being, JuliaCall is having an [issue](https://github.com/Non-Contradiction/JuliaCall/issues/164) with the Julia 1.6 version. So you will need to set Julia version v1.5.4 or older as the default one

## Workflow

1. Make all the modifications of the chapter you are working on in the .Rmd file

2. Once you finish making all the modifications, run all the code cells to make sure you you don't get any error

3. Since Data Science in Julia for Hackers has chapters that involve a lot of computation we render each chapter separately.

    We do this by running `bookdown::preview_chapter(“{Rmd_file}”)`in the RStudio console.

4. If the .Rmd file run without errors the console will tell you that the html file is created with the console message

    `Output created: docs/{title}.html`

5. If you open the html file, you will notice that in the left index the sections dividers are missing. 

    So we will need to add them manually in the .html file. To do it you will need to copy the summary code from another chapter and replace it: 

    ```
    <ul class="summary">
    ...
    </ul>
    ```

    You can open the html file and see that the seccion divider is now displayed in the left-side index of the book.



