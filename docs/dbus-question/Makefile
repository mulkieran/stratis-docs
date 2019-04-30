dbus.pdf: dbus.lyx
	lyx -batch --export pdf $<

clean:
	-rm dbus.pdf

check-closed-insets:
	@grep --quiet "^status open$$" dbus.lyx ; if [ $$? -ne "1" ] ; then exit 1 ; fi

check: check-closed-insets

.PHONY:
	check
	check-closed-insets
