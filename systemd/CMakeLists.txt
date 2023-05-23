# SPDX-License-Identifier: GPL-2.0-or-later

include(FindPkgConfig)
pkg_check_modules(SYSTEMD REQUIRED "systemd")
pkg_get_variable(SYSTEMD_SYSTEMUNITDIR "systemd" "systemdsystemunitdir")

install(FILES revpi-bthelper@.service revpi-hciuart@.service
	DESTINATION ${SYSTEMD_SYSTEMUNITDIR}
)
