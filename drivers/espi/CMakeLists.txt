# SPDX-License-Identifier: Apache-2.0

zephyr_library()

zephyr_library_sources_ifdef(CONFIG_ESPI_XEC		espi_mchp_xec.c)
zephyr_library_sources_ifdef(CONFIG_ESPI_NPCX		espi_npcx.c)
zephyr_library_sources_ifdef(CONFIG_ESPI_NPCX		host_subs_npcx.c)
zephyr_library_sources_ifdef(CONFIG_USERSPACE		espi_handlers.c)
zephyr_library_sources_ifdef(CONFIG_ESPI_EMUL		espi_emul.c)
zephyr_library_sources_ifdef(CONFIG_ESPI_SAF		espi_saf_mchp_xec.c)
zephyr_library_sources_ifdef(CONFIG_ESPI_XEC_V2		espi_mchp_xec_v2.c)
zephyr_library_sources_ifdef(CONFIG_ESPI_XEC_V2		espi_mchp_xec_host_v2.c)
