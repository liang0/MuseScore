#=============================================================================
#  MuseScore
#  Music Composition & Notation
#
#  Copyright (C) 2020 MuseScore BVBA and others
#
#  This program is free software; you can redistribute it and/or modify
#  it under the terms of the GNU General Public License version 2.
#
#  This program is distributed in the hope that it will be useful,
#  but WITHOUT ANY WARRANTY; without even the implied warranty of
#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
#  GNU General Public License for more details.
#
#  You should have received a copy of the GNU General Public License
#  along with this program; if not, write to the Free Software
#  Foundation, Inc., 675 Mass Ave, Cambridge, MA 02139, USA.
#=============================================================================

set(MODULE audio)

set(MODULE_QRC audio.qrc)

set(MODULE_QML_IMPORT ${CMAKE_CURRENT_LIST_DIR}/qml)

set(MODULE_SRC
    ${CMAKE_CURRENT_LIST_DIR}/audiostubmodule.cpp
    ${CMAKE_CURRENT_LIST_DIR}/audiostubmodule.h
    ${CMAKE_CURRENT_LIST_DIR}/audioconfigurationstub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/audioconfigurationstub.h
    ${CMAKE_CURRENT_LIST_DIR}/sequencerstub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/sequencerstub.h
    ${CMAKE_CURRENT_LIST_DIR}/synthesizerstub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/synthesizerstub.h
    ${CMAKE_CURRENT_LIST_DIR}/synthesizersregisterstub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/synthesizersregisterstub.h
    ${CMAKE_CURRENT_LIST_DIR}/soundfontsproviderstub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/soundfontsproviderstub.h
    ${CMAKE_CURRENT_LIST_DIR}/audiodriverstub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/audiodriverstub.h
    ${CMAKE_CURRENT_LIST_DIR}/internal/rpc/rpcchannelstub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/internal/rpc/rpcchannelstub.h
    )                           

include(${PROJECT_SOURCE_DIR}/build/module.cmake)
