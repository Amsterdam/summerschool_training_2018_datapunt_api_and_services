RM        := rm -rf
BUILDDIR  := ../docs
GITHUBDIR := summerschool_training_2018_datapunt_api_and_services

docs:
	$(RM) $(BUILDDIR)
	MKDIR $(BUILDDIR)
	MKDIR $(BUILDDIR)/static
	MKDIR $(BUILDDIR)/images
	git clone https://github.com/hakimel/reveal.js.git $(BUILDDIR)/static
	$(RM) $(BUILDDIR)/static/.git
	jupyter nbconvert APIs\ en\ Services.ipynb --to slides --reveal-prefix $(GITHUBDIR)/static
	MV APIs\ en\ Services.slides.html $(BUILDDIR)/index.html
	CP images/* $(BUILDDIR)/images

dev:
	$(RM) $(BUILDDIR)
	MKDIR $(BUILDDIR)
	MKDIR $(BUILDDIR)/static
	MKDIR $(BUILDDIR)/images
	git clone https://github.com/hakimel/reveal.js.git $(BUILDDIR)/static
	$(RM) $(BUILDDIR)/static/.git
	jupyter nbconvert APIs\ en\ Services.ipynb --to slides --reveal-prefix static
	MV APIs\ en\ Services.slides.html $(BUILDDIR)/index.html
	CP images/* $(BUILDDIR)/images