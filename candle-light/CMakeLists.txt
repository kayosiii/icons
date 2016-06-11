########### install files ###############

set( candle_light_icon_dirs  actions applets apps categories devices emblems emotes mimetypes places status)

set(CANDLE_LIGHT_INSTALL_DIR ${KDE_INSTALL_FULL_ICONDIR}/candle_light)
install( DIRECTORY ${candle_light_icon_dirs} DESTINATION ${CANDLE_LIGHT_INSTALL_DIR} )
install( FILES index.theme DESTINATION ${CANDLE_LIGHT_INSTALL_DIR})

gtk_update_icon_cache(${CANDLE_LIGHT_INSTALL_DIR})
