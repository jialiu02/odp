ACLOCAL_AMFLAGS=-I m4
AM_DISTCHECK_CONFIGURE_FLAGS = --enable-user-guides	\
			       --enable-helper-linux	\
			       --with-testdir

if PLATFORM_IS_LINUX_GENERIC
PLATFORM_DIR = platform/linux-generic
PLATFORM_TEST_DIR = platform/linux-generic/test
endif

SUBDIRS = \
	  include \
	  $(PLATFORM_DIR) \
	  helper \
	  helper/test \
	  doc \
	  example . \
	  test \
	  $(PLATFORM_TEST_DIR)

@DX_RULES@

EXTRA_DIST = bootstrap $(DX_CONFIG) CHANGELOG config/README
