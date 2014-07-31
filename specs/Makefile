saxpath ?= "lib/saxon9.jar"
saxon ?= java -classpath $(saxpath) net.sf.saxon.Transform -novw -l
saxparam ?= bootstrapJsUrl='/components/bootstrap/dist/js/bootstrap.min.js' \
					  bootstrapCssUrl='/components/bootstrap/dist/css/bootstrap.min.css' \
						jqueryJsUrl='/components/jquery/dist/jquery.min.js' \
						siteCssUrl='/asset/site.css' \
						navbar='../../_includes/navbar.html'
stylesheet := lib/rfcbootstrap.xslt

specs := rfc7230 rfc7231 rfc7232 rfc7233 rfc7234 rfc7235 rfc7236 rfc7237
TARGETS := $(addsuffix .html,$(specs))

.PHONY: all 

all: $(TARGETS)

%.html: %.xml $(stylesheet)
	$(saxon) $< $(stylesheet) $(saxparam) > $@
