# See the build system documentation in IDF programming guide
# for more information about component CMakeLists.txt files.

idf_component_register(
    SRCS main.c         # list the source files of this component
    HAL\\LL_PORTS.c
    HAL\\LL_TIMERS.c
    HAL\\LL_ISR.c
    APP\\APP_MOT_CTRL.c
    INCLUDE_DIRS        # optional, add here public include directories
    C:/Espressif/frameworks/esp-idf-v5.0.2/components/driver/include/driver
    C:/Espressif/frameworks/esp-idf-v5.0.2/components/esp_hw_support/include
    C:/Espressif/frameworks/esp-idf-v5.0.2/components/hal/include/hal
    CFG/
    HAL/
    APP/
    PRIV_INCLUDE_DIRS   # optional, add here private include directories
    REQUIRES            # optional, list the public requirements (component names)
    PRIV_REQUIRES       # optional, list the private requirements
)
