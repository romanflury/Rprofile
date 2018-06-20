
# set default device to X11
hook <- function() { options(device = "X11"); graphics.off() }
setHook("before.plot.new", hook)

# force R to never use scientific notation to express very small or large numbers.
options(scipen=10)

# allows to tab-complete package names for use in “library()” or “require()” calls.
utils::rc.settings(ipck=TRUE)

# set default CRAN repository mirror
local({
  r <- getOption("repos")
  r["CRAN"] <- "https://stat.ethz.ch/CRAN/"
  options(repos = r)
})
