dir = usr/share/graphics

files = \
	logo_debian.png \
	logo_debian_dark.png \
	note_icon.png \
	warning_icon.png

build-local:: $(files)

clean-local::
	rm -f logo_debian.png logo_debian_dark.png

install-local:: $(outdir)
	ln -fs logo_debian.png $(outdir)/logo_installer.png
	ln -fs logo_debian_dark.png $(outdir)/logo_installer_dark.png

logo_debian.png: logo_debian_softwaves.svg
	cp logo_pardus.png logo_debian.png

logo_debian_dark.png: logo_debian_softwaves_dark.svg
	cp logo_pardus.png logo_debian_dark.png

include ../../../../Makefile.inc
