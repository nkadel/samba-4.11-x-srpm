samba-4.13.x-srpm
================

SRPM building tools for Samba 4.12 on Fedora and RHEL. Samba 4.12.x
with domain controller is enabled with the experimental MIT kerberos.
dc is only enabled on Fedora.

These are built from Fedora rawhide releases, and need to be built and
installed in the following order.

	libtalloc-2.3.x-srpm
	libtdb-1.4.x-srpm
	libldb-2.2.x-srpm
	libtevent-0.10.x-srpm

	samba-4.13.x-srpm

The "make" command will do these steps.

	make build	# Build the package on the local OS
	make all	# Use "mock" to build the packages with the local
			# samba4repo-8-x96_64 configuration, which needs.
	make install	# Actually install the RPM's in the repo

		Nico Kadel-Garcia <nkadel@gmail.com>
