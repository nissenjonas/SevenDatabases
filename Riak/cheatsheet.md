# Cheatsheed for using Riak and cUrl

## Basic cUrl commands
	curl http://host.com/path			# standard is a Get request output to sdout
	curl -o <filename> http://host.com/path		# Get request with repsonse output to a file
	curl -X PUT http://host.com/pat
		-H "<headerKey>: <headerValue>" \		# -H adds header information
		-d "<body text>"				# -d adds body text
		-v						# verbose
