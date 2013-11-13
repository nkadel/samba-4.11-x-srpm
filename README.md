samba-4.0.x-srpm
================

SRPM building tools for Samba 4 on RHEL 6.

These are built from Fedora rawhide releases, and need to be built and
installed in the following order.

	krb5-srpm
	iniparser-srpm

	libtalloc-srpm
	libtdb-srpm
	libldb-srpm
	libtevent-srpm

	samba-4.0.x-srpm

The "make" command will do these steps.

	make build	# Build the package on the local OS
	make all	# Use "mock" to build the packages with the local
			# smbrepo-6-x96_64 configuration, which needs.
	make install	# Actually install the RPM's in the designated
			# location for smbrepo-6-x86_64


		Nico Kadel-Garcia <nkadel@gmail.com>
