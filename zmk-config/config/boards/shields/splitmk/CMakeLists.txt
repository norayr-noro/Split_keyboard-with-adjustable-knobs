if (CONFIG_SHIELD_SPLITMK_LEFT)
  target_sources(app PRIVATE splitmk_left.c)
endif()

if (CONFIG_SHIELD_SPLITMK_RIGHT)
  target_sources(app PRIVATE splitmk_right.c)
endif()
