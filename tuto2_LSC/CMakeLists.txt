SET(LIST2EXOS
      tuto2_LSC
  )

FOREACH(FILE ${LIST2EXOS})
  add_executable(${FILE} ${FILE})
  target_link_libraries (${FILE} ${DGTAL_LIBRARIES} ${TutoDependencies})
ENDFOREACH(FILE)

