samba-4.9.x-srpm
================

SRPM building tools for Samba 4.9 on Fedora. Samba 4.x compatibilies
are no longer with RHEL or CentOS, due to gnutls and other updates.

These are built from Fedora rawhide releases, and need to be built and
installed in the following order.

	libtalloc-srpm
	libtdb-srpm
	libldb-srpm
	libtevent-srpm

	samba-4.9.x-srpm

The "make" command will do these steps.

	make build	# Build the package on the local OS
	make all	# Use "mock" to build the packages with the local
			# smbrepo-6-x96_64 configuration, which needs.
	make install	# Actually install the RPM's in the designated
			# location for smbrepo-6-x86_64


		Nico Kadel-Garcia <nkadel@gmail.com>
