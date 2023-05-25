# SPDX-FileCopyrightText: 2021-2023 KUNBUS GmbH
#
# SPDX-License-Identifier: GPL-2.0-or-later

install(PROGRAMS revpi-btuart
  DESTINATION ${CMAKE_INSTALL_BINDIR}/
)
install(PROGRAMS revpi-bthelper
  DESTINATION ${CMAKE_INSTALL_SBINDIR}/
)
