SHELL := bash
.DEFAULT_GOAL := all

INSTALL=install
PREFIX=/usr/local
BINDIR=$(PREFIX)/bin

dest_bindir := $(DESTDIR)$(BINDIR)

all:
	@echo "Available target: 'install'"

install:
	$(INSTALL) -d $(dest_bindir)
	$(INSTALL) -pm 0755 osinstancectl.sh $(dest_bindir)/osinstancectl
	$(INSTALL) -pm 0755 openslides-docker-pg-dump.sh \
	  $(dest_bindir)/openslides-docker-pg-dump
	$(INSTALL) -pm 0755 openslides-instance-sync.sh \
	  $(dest_bindir)/openslides-instance-sync
	$(INSTALL) -pm 0755 openslides-logwatch.sh $(dest_bindir)/openslides-logwatch
	$(INSTALL) -pm 644 bash-completion.sh /etc/bash_completion.d/osinstancectl
