include_directories( ${PROJECT_BINARY_DIR}/src/libcalamaresui )

calamares_add_plugin( keyboard
    TYPE viewmodule
    EXPORT_MACRO PLUGINDLLEXPORT_PRO
    SOURCES
        KeyboardViewStep.cpp
        KeyboardPage.cpp
        keyboardwidget/keyboardglobal.cpp
        keyboardwidget/keyboardpreview.cpp
    UI
        KeyboardPage.ui
    LINK_LIBRARIES
        calamaresui
    SHARED_LIB
)
