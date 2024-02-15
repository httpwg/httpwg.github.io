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
xml2rfc ?= "xml2rfc"

specs := $(basename $(wildcard *.xml))
TARGETS := $(addsuffix .html,$(specs))

all: $(TARGETS)

.PHONY: clean
clean:
	rm -f $(TARGETS) lib/rfc2629.xslt

%.html: %.xml $(stylesheet) lib/rfc2629.xslt
	$(saxon) $< $(stylesheet) $(saxparam) pageUrl='https://httpwg.org/specs/$@' > $@

%.xml:
	wget https://rfc-editor.org/rfc/$@
	$(xml2rfc) --unprep -o $@ $@

lib/rfc2629.xslt:
	wget -O $@ https://raw.githubusercontent.com/reschke/xml2rfc/master/rfc2629.xslt