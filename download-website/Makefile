all : linux.html mac.html windows.html prior.html contents.html changelog.html

%.html : %.markdown
	pandoc --from=markdown --to=html \
		--standalone \
		--css=style.css \
        --include-in-header header.txt\
	    --include-after-body analytics.js \
		--output=$@ $<
