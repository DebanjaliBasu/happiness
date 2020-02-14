# Imports the data to be analyzed into a Dataframe (DF)
#' @title Import Happiness report 2019 Data
#'
#' @description This function reads the data from a csv-file and returns it as a DataFrame-object.
#' @usage To use this function by itself, store the DF in a variable.
#' @examples
#' df = get_data()

#' @export
get_data <- function() {
  df <- read.csv(system.file("extdata", "happinessreport2019.csv", package="happiness"))

  #changing the column names
  colnames(df)<- c("rank","country","score","gdp","social","lifexp","freedom","generosity","corruption")

  #since there is no missing data I can directly use it without handling for na values.

  usethis::use_data(df, overwrite = TRUE)
  return(df)
}
