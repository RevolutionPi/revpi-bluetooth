# SPDX-License-Identifier: GPL-2.0-or-later

include(FindPkgConfig)
pkg_check_modules(UDEV REQUIRED "udev")
pkg_get_variable(UDEV_UDEVDIR "udev" "udevdir")

install(FILES 90-revpi-bluetooth.rules
	DESTINATION ${UDEV_UDEVDIR}/rules.d
)
