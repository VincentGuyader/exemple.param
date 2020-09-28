
<!-- README.md is generated from README.Rmd. Please edit that file -->

# How to use get\_golem\_options

1.  Pass parameters to `run_app`

<!-- end list -->

``` r
run_app(p1 = "param1", p2 = "param2")
```

2.  Use get\_golem\_options()

in UI…

``` r
h1(get_golem_options("p1"))
```

…or in server

``` r
  output$param <- renderPrint({
    paste("param p2 = ",get_golem_options("p2"))
    })
```

Et voila.

## You can set default value

``` r
run_app <- function(
  ...,name="default p3"
) {
  with_golem_options(
    app = shinyApp(
      ui = app_ui, 
      server = app_server
    ), 
    golem_opts = list(..., name=name)
  )
}
```
