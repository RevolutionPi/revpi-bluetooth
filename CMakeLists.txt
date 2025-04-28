# SPDX-FileCopyrightText: 2021-2023 KUNBUS GmbH
#
# SPDX-License-Identifier: GPL-2.0-or-later

cmake_minimum_required(VERSION 3.13)

project(revpi-bluetooth LANGUAGES NONE)

include(GNUInstallDirs)

add_subdirectory(scripts)
add_subdirectory(systemd)
add_subdirectory(udev)
add_subdirectory(firmware)
