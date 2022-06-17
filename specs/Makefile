saxpath ?= "lib/saxon9.jar"
saxon ?= java -classpath $(saxpath) net.sf.saxon.Transform -l
themedir ?= ../../../httpwg-theme
saxparam ?= bootstrapJsUrl='/assets/node_modules/bootstrap/dist/js/bootstrap.min.js' \
					  bootstrapCssUrl='/assets/node_modules/bootstrap/dist/css/bootstrap.min.css' \
						jqueryJsUrl='/assets/node_modules/jquery/dist/jquery.min.js' \
						siteCssUrl='/assets/site.css' \
						navbar='$(themedir)/_includes/navbar.html' \
						siteName='IETF HTTP Working Group Specifications' \
						pageImageUrl='https://httpwg.org/assets/favicon/apple-icon-180x180.png'
stylesheet := lib/rfcbootstrap.xslt

specs := rfc2818 rfc5789 rfc5861 rfc5988 rfc6265 rfc6266 rfc6585 rfc7230 rfc7231 rfc7232 rfc7233 rfc7234 rfc7235 rfc7236 rfc7237 rfc7240 rfc7538 rfc7540 rfc7541 rfc7615 rfc7616 rfc7617 rfc7639 rfc7694 rfc7725 rfc7838 rfc8164 rfc8188 rfc8246 rfc8288 rfc8297 rfc8336 rfc8441 rfc8470 rfc8586 rfc8740 rfc8941 rfc9110 rfc9111 rfc9112 rfc9113 rfc9114 rfc9204 rfc9205 rfc9211 rfc9209  rfc9213 rfc9218 rfc9220 
TARGETS := $(addsuffix .html,$(specs))

.PHONY: all clean

all: $(TARGETS)

clean:
	rm -f $(TARGETS)

%.html: %.xml $(stylesheet) lib/rfc2629.xslt
	$(saxon) $< $(stylesheet) $(saxparam) pageUrl='https://httpwg.org/specs/$@' > $@

%.xml:
	wget https://rfc-editor.org/rfc/$@
	xml2rfc --unprep -o $@ $@

.PHONY: lib/rfc2629.xslt
lib/rfc2629.xslt:
	wget -O $@ https://raw.githubusercontent.com/reschke/xml2rfc/master/rfc2629.xslt