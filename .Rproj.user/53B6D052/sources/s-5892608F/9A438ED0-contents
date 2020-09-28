#' The application server-side
#' 
#' @param input,output,session Internal parameters for {shiny}. 
#'     DO NOT REMOVE.
#' @import shiny
#' @noRd
app_server <- function( input, output, session ) {
  # List the first level callModules here

  output$param <- renderPrint({
    paste("parametre p2 = ",get_golem_options("p2"))
  
  })
  output$param3 <- renderPrint({
    paste("parametre p3 = ",get_golem_options("name"))
  
  })
  
  
}
