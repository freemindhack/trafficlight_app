file(GLOB COMPONENTS_QML_JS_FILES *.qml *.js)

# make the files visible in the qtcreator tree
add_custom_target(trafficlight_components_QMlFiles ALL SOURCES ${COMPONENTS_QML_JS_FILES})

install(FILES ${COMPONENTS_QML_JS_FILES} DESTINATION ${TRAFFICLIGHT_DIR}/components)

