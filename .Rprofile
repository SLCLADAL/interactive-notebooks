source("renv/activate.R")
setwd('notebooks')
setHook(
	'rstudio.sessionInit', function(newSession) {
		if (newSession)
		rstudioapi::filesPaneNavigate('notebooks')
	},
	action = 'append'
)
