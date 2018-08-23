RM        := rm -rf
BUILDDIR  := ../docs
GITHUBDIR := https://cdnjs.cloudflare.com/ajax/libs/reveal.js/3.6.0

docs:
	$(RM) $(BUILDDIR)
	MKDIR $(BUILDDIR)
	MKDIR $(BUILDDIR)/static
	MKDIR $(BUILDDIR)/images
	$(RM) $(BUILDDIR)/.git
	jupyter nbconvert APIs\ en\ Services.ipynb --to slides --reveal-prefix $(GITHUBDIR)
	MV APIs\ en\ Services.slides.html $(BUILDDIR)/index.html
	CP images/* $(BUILDDIR)/images