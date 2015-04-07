saxpath ?= "lib/saxon9.jar"
saxon ?= java -classpath $(saxpath) net.sf.saxon.Transform -novw -l
saxparam ?= bootstrapJsUrl='/bower_components/bootstrap/dist/js/bootstrap.min.js' \
					  bootstrapCssUrl='/bower_components/bootstrap/dist/css/bootstrap.min.css' \
						jqueryJsUrl='/bower_components/jquery/dist/jquery.min.js' \
						siteCssUrl='/asset/site.css' \
						navbar='../../_includes/navbar.html'
stylesheet := lib/rfcbootstrap.xslt

specs := rfc6265 rfc6585 rfc7230 rfc7231 rfc7232 rfc7233 rfc7234 rfc7235 rfc7236 rfc7237 rfc7538
TARGETS := $(addsuffix .html,$(specs))

.PHONY: all clean

all: $(TARGETS)

clean:
	rm -f $(TARGETS)

%.html: %.xml $(stylesheet)
	$(saxon) $< $(stylesheet) $(saxparam) > $@
