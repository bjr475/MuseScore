#=============================================================================
#  MuseScore
#  Music Composition & Notation
#  $Id:$
#
#  Copyright (C) 2011 Werner Schweer
#
#  This program is free software; you can redistribute it and/or modify
#  it under the terms of the GNU General Public License version 2
#  as published by the Free Software Foundation and appearing in
#  the file LICENSE.GPL
#=============================================================================

set(TARGET tst_sfzcomments)

include(${PROJECT_SOURCE_DIR}/mtest/cmake.inc)

include_directories(
      ${SNDFILE_INCDIR}
      )

target_link_libraries(tst_sfzcomments zerberus synthesizer audiofile ${SNDFILE_LIB})
