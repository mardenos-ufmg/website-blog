atualizar =
  ( file.info("posts")$mtime > as.POSIXct(readLines("timestamp.txt")) ) |>
  {\(.) ifelse(is.na(.), T, .)}()

if (atualizar) {
  cat(as.character(Sys.time()), "\n", file = "timestamp.txt")
}
