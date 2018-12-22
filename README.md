samba-4.9.x-srpm
================

SRPM building tools for Samba 4.9 on Fedora and RHEL. Samba 4.9.x
with domain controller enabled is is not possible on current RHEL, so
dc is only enabled on Fedora. Fedora now *has* 4.9.3, so it's not as
necessary there anymore.

These are built from Fedora rawhide releases, and need to be built and
installed in the following order.

	libtalloc-2.1.x-srpm
	libtdb-1.3.x-srpm
	libldb-1.4.x-srpm
	libtevent-0.9.x-srpm

	samba-4.9.x-srpm

The "make" command will do these steps.

	make build	# Build the package on the local OS
	make all	# Use "mock" to build the packages with the local
			# smbrepo-6-x96_64 configuration, which needs.
	make install	# Actually install the RPM's in the designated
			# location for smbrepo-6-x86_64


		Nico Kadel-Garcia <nkadel@gmail.com>
