add_definitions(-std=gnu99)

add_executable(bot-wavefront-viewer
    main.c
    renderer_wavefront.c)

pods_use_pkg_config_packages(bot-wavefront-viewer bot2-vis)  # need headers as well as target link libraries

pods_install_executables(bot-wavefront-viewer)
