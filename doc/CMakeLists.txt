ADD_CUSTOM_TARGET (doc-html
		  sphinx-build -b html
		  ${CMAKE_CURRENT_SOURCE_DIR} ${CMAKE_CURRENT_BINARY_DIR}
		  COMMENT "Building html documentation")
ADD_CUSTOM_TARGET (doc)
ADD_DEPENDENCIES (doc doc-html)
