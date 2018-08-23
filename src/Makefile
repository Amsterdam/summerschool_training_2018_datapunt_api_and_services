RM        := rm -rf
BUILDDIR  := ../docs

docs:
	$(RM) $(BUILDDIR)
	MKDIR $(BUILDDIR)
	MKDIR $(BUILDDIR)/images
	git clone https://github.com/hakimel/reveal.js.git $(BUILDDIR)/reveal.js
	jupyter nbconvert APIs\ en\ Services.ipynb --to slides --reveal-prefix reveal.js
	MV APIs\ en\ Services.slides.html $(BUILDDIR)/index.html
	CP images/* $(BUILDDIR)/images