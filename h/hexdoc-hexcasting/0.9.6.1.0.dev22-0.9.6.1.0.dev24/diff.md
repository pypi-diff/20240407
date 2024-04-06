# Comparing `tmp/hexdoc_hexcasting-0.9.6.1.0.dev22.tar.gz` & `tmp/hexdoc_hexcasting-0.9.6.1.0.dev24.tar.gz`

## Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22.tar` & `hexdoc_hexcasting-0.9.6.1.0.dev24.tar`

### file list

```diff
@@ -1,724 +1,725 @@
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/gradle.properties
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/__gradle_version__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/__init__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/__version__.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_hooks.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/__init__.py
--rw-r--r--   0        0        0   164412 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/hexcasting.hexdoc.json
--rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/hexcasting.patterns.hexdoc.json
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/emi/models/item/tag/hexcasting/akashic_logs.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/emi/models/item/tag/hexcasting/akashic_planks.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/emi/models/item/tag/hexcasting/phial_base.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/emi/models/item/tag/hexcasting/wands.json
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/blockstates/skillet.json
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/lang/en_us.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/lang/zh_cn.json
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/models/block/skillet.json
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/models/item/skillet.json
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/textures/block/skillet_bottom.png
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/textures/block/skillet_side.png
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/textures/block/skillet_top.png
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_bookshelf.json
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_button.json
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_connector.json
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_door.json
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_leaves1.json
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_leaves2.json
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_leaves3.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_log.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_log_stripped.json
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_panel.json
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_planks.json
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_pressure_plate.json
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_record.json
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_slab.json
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_stairs.json
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_tile.json
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_trapdoor.json
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_wood.json
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_wood_stripped.json
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/amethyst_dust_block.json
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/amethyst_sconce.json
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/amethyst_tiles.json
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/ancient_scroll_paper.json
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/ancient_scroll_paper_lantern.json
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/conjured.json
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/conjured_block.json
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/directrix_redstone.json
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/empty_directrix.json
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/empty_impetus.json
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/impetus_look.json
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/impetus_rightclick.json
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/impetus_storedplayer.json
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/scroll_paper.json
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/scroll_paper_lantern.json
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/slate.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/slate_block.json
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
--rw-r--r--   0        0        0   139392 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/en_us.json
--rw-r--r--   0        0        0   225345 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/ru_ru.json
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/zh_cn.flatten.json5
--rw-r--r--   0        0        0   205391 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/zh_cn.json
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_bookshelf_empty0.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_button.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_connector.json
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_leaves1.json
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_leaves2.json
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_leaves3.json
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_log.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_log_stripped.json
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_panel.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_planks1.json
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_pressure_plate.json
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_record.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_slab.json
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_stairs.json
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_tile.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_trapdoor_bottom.json
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_wood.json
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_wood_stripped.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/amethyst_dust_block.json
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/amethyst_sconce.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/amethyst_tiles.json
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/ancient_scroll_paper.json
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/ancient_scroll_paper_lantern.json
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/cube_half_mirrored.json
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/empty_directrix_dim_z.json
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/empty_impetus_dim_east.json
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/impetus_look_dim_east.json
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/impetus_rightclick_dim_east.json
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/impetus_storedplayer_dim_east.json
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/redstone_directrix_unpowered_dim_north.json
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/scroll_paper.json
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/scroll_paper_lantern.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/slate_block.json
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/abacus.json
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_bookshelf.json
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_button.json
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_connector.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_door.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_leaves1.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_leaves2.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_leaves3.json
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_log.json
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_log_stripped.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_panel.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_planks.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_pressure_plate.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_record.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_slab.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_stairs.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_tile.json
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_trapdoor.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_wood.json
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_wood_stripped.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/amethyst_dust.json
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/amethyst_dust_block.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/amethyst_sconce.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/amethyst_tiles.json
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/ancient_scroll_paper.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/ancient_scroll_paper_lantern.json
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/artifact.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/artifact_filled.json
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/battery.json
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/charged_amethyst.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/conjured.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/conjured_block.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/creative_unlocker.json
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/cypher.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/cypher_filled.json
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/directrix_redstone.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_black.json
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_blue.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_brown.json
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_cyan.json
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_gray.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_green.json
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_light_blue.json
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_light_gray.json
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_lime.json
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_magenta.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_orange.json
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_pink.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_purple.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_red.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_white.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_yellow.json
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/empty_directrix.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/empty_impetus.json
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_double.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_double_sealed.json
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_empty.json
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_empty_sealed.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_entity.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_entity_sealed.json
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_list.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_list_sealed.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_pattern.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_pattern_sealed.json
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_vec3.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_vec3_sealed.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_widget.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_widget_sealed.json
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/impetus_look.json
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/impetus_rightclick.json
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/impetus_storedplayer.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/jeweler_hammer.json
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/lens.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/patchouli_book.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_large_0.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_large_1.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_large_2.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_large_3.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_large_4.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_medium_0.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_medium_1.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_medium_2.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_medium_3.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_medium_4.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_small_0.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_small_1.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_small_2.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_small_3.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_small_4.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_agender.json
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_aroace.json
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_aromantic.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_asexual.json
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_bisexual.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_demiboy.json
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_demigirl.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_gay.json
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_genderfluid.json
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_genderqueer.json
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_intersex.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_lesbian.json
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_nonbinary.json
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_pansexual.json
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_plural.json
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_transgender.json
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_ancient_large.json
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_ancient_medium.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_ancient_small.json
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_medium.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_paper.json
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_paper_lantern.json
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_pristine_large.json
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_pristine_medium.json
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_pristine_small.json
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_small.json
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/slate.json
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/slate_blank.json
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/slate_block.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/slate_written.json
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook.json
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_double.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_double_sealed.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_empty.json
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_empty_sealed.json
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_entity.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_entity_sealed.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_list.json
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_list_sealed.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_pattern.json
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_pattern_sealed.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_vec3.json
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_vec3_sealed.json
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_widget.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_widget_sealed.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/sub_sandwich.json
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/trinket.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/trinket_filled.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/uuid_colorizer.json
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_acacia.json
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_akashic.json
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_birch.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_bosnia.json
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_crimson.json
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_dark_oak.json
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_jungle.json
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_oak.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_old.json
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_spruce.json
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_warped.json
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_bricks.png
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_bricks_small.png
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_chiseled.png
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_dust_block.png
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_polished.png
--rw-r--r--   0        0        0    18846 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_sconce.png
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_tiles.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/ancient_scroll_paper.png
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/ancient_scroll_paper_lantern.png
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/ancient_scroll_paper_lantern_bottom.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/ancient_scroll_paper_lantern_side.png
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/ancient_scroll_paper_lantern_top.png
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/cracked_calcite.png
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_button.png
--rw-r--r--   0        0        0    16742 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_pressure_plate.png
--rw-r--r--   0        0        0    26881 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_slab.png
--rw-r--r--   0        0        0    31222 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_stairs.png
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/scroll_paper.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/scroll_paper_lantern.png
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/scroll_paper_lantern_bottom.png
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/scroll_paper_lantern_side.png
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/scroll_paper_lantern_top.png
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/slate.png
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/slate_directional.png
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/smooth_amethyst.png
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/connector.png
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/door_lower.png
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/door_upper.png
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/leaves1.png
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/leaves2.png
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/leaves3.png
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/log.png
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/log_alt_end.png
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/log_alt_end_stripped.png
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/log_end.png
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/log_end_stripped.png
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/log_stripped.png
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/panel.png
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/planks1.png
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/planks2.png
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/planks3.png
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/record.png
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/record_inner.png
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/tile.png
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/trapdoor.png
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/double1.png
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/double2.png
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/double3.png
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/double4.png
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/empty.png
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/end.png
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/entity1.png
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/entity2.png
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/entity3.png
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/entity4.png
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/list1.png
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/list2.png
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/list3.png
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/list4.png
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/other1.png
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/other2.png
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/other3.png
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/other4.png
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/pattern1.png
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/pattern2.png
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/pattern3.png
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/pattern4.png
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/side.png
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/vec1.png
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/vec2.png
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/vec3.png
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/vec4.png
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget1.png
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget2.png
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget3.png
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget4.png
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/end_dim.png
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/end_lit.png
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/horiz_dim.png
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/horiz_lit.png
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/vert_dim.png
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/vert_lit.png
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/back_powered.png
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/back_unpowered.png
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_powered_dim.png
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_powered_lit.png
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_unpowered_dim.png
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_unpowered_lit.png
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/front_dim.png
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/front_lit.png
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_powered_dim.png
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_powered_lit.png
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_unpowered_dim.png
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_unpowered_lit.png
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_powered_dim.png
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_powered_lit.png
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_unpowered_dim.png
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_unpowered_lit.png
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_powered_dim.png
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_powered_lit.png
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_unpowered_dim.png
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_unpowered_lit.png
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/atlas.png
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/back_dim.png
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/back_empty_dim.png
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/back_empty_lit.png
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/back_lit.png
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/down_dim.png
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/down_empty_dim.png
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/down_empty_lit.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/down_lit.png
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/front_empty_dim.png
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/front_empty_lit.png
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_dim.png
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_empty_dim.png
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_empty_lit.png
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_lit.png
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/look_dim.png
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/look_lit.png
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/right_dim.png
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/right_empty_dim.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/right_empty_lit.png
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/right_lit.png
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/rightclick_dim.png
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/rightclick_lit.png
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/something.png
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/storedplayer_dim.png
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/storedplayer_lit.png
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/up_dim.png
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/up_empty_dim.png
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/up_empty_lit.png
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/up_lit.png
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/scroll_ancient_large.png
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/scroll_ancient_medium.png
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/scroll_large.png
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/scroll_medium.png
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/sentinel.png
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/white.png
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/brainsweep.png
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/brainsweep_emi.png
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/brainsweep_jei.png
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/edify.png
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/edify_emi.png
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/edify_jei.png
--rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/patchi_filler.png
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/phial.png
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/phial_emi.png
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/phial_jei.png
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/scroll.png
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/scroll_ancient.png
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/slate.png
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/villager_leveling.png
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/villager_profession.png
--rw-r--r--   0        0        0    35018 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/entries/spell_circle.png
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/hexdoc/brainsweep.png
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/abacus.png
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/akashic_door.png
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/amethyst_dust.png
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/artifact.png
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/artifact_filled.png
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/charged_amethyst.png
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/creative_unlocker.png
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/cypher.png
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/cypher_filled.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/jeweler_hammer.png
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/lens.png
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/patchouli_book.png
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/scroll_ancient_large.png
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/scroll_ancient_medium.png
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/scroll_ancient_small.png
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/scroll_pristine_large.png
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/scroll_pristine_medium.png
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/scroll_pristine_small.png
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/slate_blank.png
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/slate_written.png
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/sub_sandwich.png
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/trinket.png
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/trinket_filled.png
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_black.png
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_blue.png
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_brown.png
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_cyan.png
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_gray.png
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_green.png
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_light_blue.png
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_light_gray.png
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_lime.png
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_magenta.png
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_orange.png
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_pink.png
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_purple.png
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_red.png
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_white.png
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_yellow.png
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_agender.png
--rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_aroace.png
--rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_aromantic.png
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_asexual.png
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_bisexual.png
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_demiboy.png
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_demigirl.png
--rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_gay.png
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_genderfluid.png
--rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_genderqueer.png
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_intersex.png
--rw-r--r--   0        0        0     6871 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_lesbian.png
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_nonbinary.png
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_pansexual.png
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_plural.png
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_transgender.png
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/uuid.png
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/double.png
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/double_sealed.png
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/empty.png
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/empty_sealed.png
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/entity.png
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/entity_sealed.png
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/list.png
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/list_sealed.png
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/pattern.png
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/pattern_sealed.png
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/vec3.png
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/vec3_sealed.png
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/widget.png
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/widget_sealed.png
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_large_0.png
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_large_1.png
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_large_2.png
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_large_3.png
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_large_4.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_medium_0.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_medium_1.png
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_medium_2.png
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_medium_3.png
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_medium_4.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_small_0.png
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_small_1.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_small_2.png
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_small_3.png
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_small_4.png
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/double.png
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/double_sealed.png
--rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/empty.png
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/empty_sealed.png
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/entity.png
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/entity_sealed.png
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/list.png
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/list_sealed.png
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/pattern.png
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/pattern_sealed.png
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/vec3.png
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/vec3_sealed.png
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/widget.png
--rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/widget_sealed.png
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/acacia.png
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/akashic.png
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/birch.png
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/bosnia.png
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/crimson.png
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/dark_oak.png
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/jungle.png
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/oak.png
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/old.png
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/spruce.png
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/warped.png
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/cloud.png
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_1.png
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_2.png
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_3.png
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_4.png
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_5.png
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_6.png
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_7.png
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_8.png
--rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/allay.png
--rw-r--r--   0        0        0    48613 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/armorer.png
--rw-r--r--   0        0        0    17388 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/butcher.png
--rw-r--r--   0        0        0    16563 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/cartographer.png
--rw-r--r--   0        0        0    16752 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/cleric.png
--rw-r--r--   0        0        0    23744 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/farmer.png
--rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/fisherman.png
--rw-r--r--   0        0        0    16906 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/fletcher.png
--rw-r--r--   0        0        0    16807 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/leatherworker.png
--rw-r--r--   0        0        0    17118 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/librarian.png
--rw-r--r--   0        0        0    16898 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/mason.png
--rw-r--r--   0        0        0    15451 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/nitwit.png
--rw-r--r--   0        0        0    27110 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/none.png
--rw-r--r--   0        0        0    18911 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/sphepherd.png
--rw-r--r--   0        0        0    16436 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/toolsmith.png
--rw-r--r--   0        0        0    16968 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/weaponsmith.png
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/book.json
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/basics.json
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/casting.json
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/greatwork.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/interop.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/items.json
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/patterns.json
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/patterns/great_spells.json
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/patterns/spells.json
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/basics/couldnt_cast.json
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/basics/geodes.json
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/basics/media.json
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/basics/start_to_see.json
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/101.json
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/influences.json
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/mishaps.json
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/mishaps2.json
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/naming.json
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/stack.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/vectors.json
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/akashiclib.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/brainsweeping.json
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/directrix.json
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/impetus.json
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/spellcircles.json
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/the_work.json
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/interop/gravity.json
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/interop/interop.json
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/interop/pehkui.json
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/abacus.json
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/amethyst.json
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/decoration.json
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/edified.json
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/focus.json
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/hexcasting.json
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/jeweler_hammer.json
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/lens.json
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/phials.json
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/pigments.json
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/scroll.json
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/slate.json
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/spellbook.json
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/staff.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/advanced_math.json
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/akashic_patterns.json
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/basics.json
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/circle.json
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/consts.json
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/entities.json
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/lists.json
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/logic.json
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/math.json
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/meta.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/numbers.json
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/patterns_as_iotas.json
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/readers_guide.json
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/readwrite.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/sets.json
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/stackmanip.json
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/brainsweep.json
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/create_lava.json
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/flight.json
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/greater_sentinel.json
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/make_battery.json
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/teleport.json
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/weather_manip.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/zeniths.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/basic.json
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/blockworks.json
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/colorize.json
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/hexcasting.json
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/itempicking.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/nadirs.json
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/sentinels.json
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/abacus.json
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/ageing_scroll_paper_lantern.json
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_bookshelf.json
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_button.json
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_connector.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_door.json
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_panel.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_planks.json
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_pressure_plate.json
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_slab.json
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_stairs.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_tile.json
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_trapdoor.json
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_wood.json
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/amethyst_dust_packing.json
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/amethyst_dust_unpacking.json
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/amethyst_sconce.json
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/amethyst_tiles.json
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/ancient_scroll_paper.json
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/ancient_scroll_paper_lantern.json
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/artifact.json
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/cypher.json
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_blue.json
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_brown.json
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_cyan.json
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_gray.json
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_green.json
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_light_blue.json
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_light_gray.json
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_lime.json
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_magenta.json
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_orange.json
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_pink.json
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_purple.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_red.json
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_white.json
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_yellow.json
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/empty_directrix.json
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/empty_impetus.json
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/focus.json
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/jeweler_hammer.json
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/lens.json
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_agender.json
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_aroace.json
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_aromantic.json
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_asexual.json
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_bisexual.json
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_demiboy.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_demigirl.json
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_gay.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_genderfluid.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_genderqueer.json
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_intersex.json
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_lesbian.json
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_nonbinary.json
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_pansexual.json
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_plural.json
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_transgender.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/scroll.json
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/scroll_medium.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/scroll_paper.json
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/scroll_paper_lantern.json
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/scroll_small.json
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/slate.json
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/slate_block.json
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/slate_block_from_slates.json
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/spellbook.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/trinket.json
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/uuid_colorizer.json
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_acacia.json
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_akashic.json
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_birch.json
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_crimson.json
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_dark_oak.json
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_jungle.json
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_oak.json
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_spruce.json
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_warped.json
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/brainsweep/akashic_record.json
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/brainsweep/budding_amethyst.json
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/brainsweep/directrix_redstone.json
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/brainsweep/impetus_look.json
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/brainsweep/impetus_rightclick.json
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/brainsweep/impetus_storedplayer.json
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/tags/items/akashic_logs.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/tags/items/akashic_planks.json
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexdoc/tags/advancements/spoilered.json
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexdoc/tags/items/gaslighting.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/minecraft/tags/items/planks.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/__init__.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/hexcasting.js.jinja
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/index.css.jinja
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/index.html.jinja
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/ingredients/hexcasting/brainsweepee/entity_tag.html.jinja
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/ingredients/hexcasting/brainsweepee/entity_type.html.jinja
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/ingredients/hexcasting/brainsweepee/villager.html.jinja
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/pages/hexcasting/brainsweep.html.jinja
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/pages/hexcasting/crafting_multi.html.jinja
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/pages/hexcasting/manual_pattern.html.jinja
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/pages/hexcasting/pattern.html.jinja
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/recipes/hexcasting/brainsweep.html.jinja
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/book/recipes.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/book/page/__init__.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/book/page/abstract_pages.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/book/page/pages.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/utils/__init__.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/utils/pattern.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/LICENSE.txt
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/pyproject.toml
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/doc/README.md
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev22/PKG-INFO
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/gradle.properties
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/__gradle_version__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/__version__.py
+-rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_hooks.py
+-rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/__init__.py
+-rw-r--r--   0        0        0   164412 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/hexcasting.hexdoc.json
+-rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/hexcasting.patterns.hexdoc.json
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/emi/models/item/tag/hexcasting/akashic_logs.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/emi/models/item/tag/hexcasting/akashic_planks.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/emi/models/item/tag/hexcasting/phial_base.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/emi/models/item/tag/hexcasting/wands.json
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/blockstates/skillet.json
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/lang/en_us.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/lang/zh_cn.json
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/models/block/skillet.json
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/models/item/skillet.json
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/textures/block/skillet_bottom.png
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/textures/block/skillet_side.png
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/textures/block/skillet_top.png
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_bookshelf.json
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_button.json
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_connector.json
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_door.json
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_leaves1.json
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_leaves2.json
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_leaves3.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_log.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_log_stripped.json
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_panel.json
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_planks.json
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_pressure_plate.json
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_record.json
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_slab.json
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_stairs.json
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_tile.json
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_trapdoor.json
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_wood.json
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_wood_stripped.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/amethyst_dust_block.json
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/amethyst_sconce.json
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/amethyst_tiles.json
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/ancient_scroll_paper.json
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/ancient_scroll_paper_lantern.json
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/conjured.json
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/conjured_block.json
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/directrix_redstone.json
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/empty_directrix.json
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/empty_impetus.json
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/impetus_look.json
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/impetus_rightclick.json
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/impetus_storedplayer.json
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/scroll_paper.json
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/scroll_paper_lantern.json
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/slate.json
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/slate_block.json
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
+-rw-r--r--   0        0        0   139392 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/en_us.json
+-rw-r--r--   0        0        0   225345 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/ru_ru.json
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/zh_cn.flatten.json5
+-rw-r--r--   0        0        0   205391 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/zh_cn.json
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_bookshelf_empty0.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_button.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_connector.json
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_leaves1.json
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_leaves2.json
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_leaves3.json
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_log.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_log_stripped.json
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_panel.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_planks1.json
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_pressure_plate.json
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_record.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_slab.json
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_stairs.json
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_tile.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_trapdoor_bottom.json
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_wood.json
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_wood_stripped.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/amethyst_dust_block.json
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/amethyst_sconce.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/amethyst_tiles.json
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/ancient_scroll_paper.json
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/ancient_scroll_paper_lantern.json
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/cube_half_mirrored.json
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/empty_directrix_dim_z.json
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/empty_impetus_dim_east.json
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/impetus_look_dim_east.json
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/impetus_rightclick_dim_east.json
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/impetus_storedplayer_dim_east.json
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/redstone_directrix_unpowered_dim_north.json
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/scroll_paper.json
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/scroll_paper_lantern.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/slate_block.json
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/abacus.json
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_bookshelf.json
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_button.json
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_connector.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_door.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_leaves1.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_leaves2.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_leaves3.json
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_log.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_log_stripped.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_panel.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_planks.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_pressure_plate.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_record.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_slab.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_stairs.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_tile.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_trapdoor.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_wood.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/akashic_wood_stripped.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/amethyst_dust.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/amethyst_dust_block.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/amethyst_sconce.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/amethyst_tiles.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/ancient_scroll_paper.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/ancient_scroll_paper_lantern.json
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/artifact.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/artifact_filled.json
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/battery.json
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/charged_amethyst.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/conjured.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/conjured_block.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/creative_unlocker.json
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/cypher.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/cypher_filled.json
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/directrix_redstone.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_black.json
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_blue.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_brown.json
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_cyan.json
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_gray.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_green.json
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_light_blue.json
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_light_gray.json
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_lime.json
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_magenta.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_orange.json
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_pink.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_purple.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_red.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_white.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/dye_colorizer_yellow.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/empty_directrix.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/empty_impetus.json
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_double.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_double_sealed.json
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_empty.json
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_empty_sealed.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_entity.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_entity_sealed.json
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_list.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_list_sealed.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_pattern.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_pattern_sealed.json
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_vec3.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_vec3_sealed.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_widget.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus_widget_sealed.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/impetus_look.json
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/impetus_rightclick.json
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/impetus_storedplayer.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/jeweler_hammer.json
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/lens.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/patchouli_book.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_large_0.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_large_1.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_large_2.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_large_3.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_large_4.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_medium_0.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_medium_1.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_medium_2.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_medium_3.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_medium_4.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_small_0.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_small_1.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_small_2.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_small_3.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/phial_small_4.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_agender.json
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_aroace.json
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_aromantic.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_asexual.json
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_bisexual.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_demiboy.json
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_demigirl.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_gay.json
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_genderfluid.json
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_genderqueer.json
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_intersex.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_lesbian.json
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_nonbinary.json
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_pansexual.json
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_plural.json
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/pride_colorizer_transgender.json
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_ancient_large.json
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_ancient_medium.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_ancient_small.json
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_medium.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_paper.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_paper_lantern.json
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_pristine_large.json
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_pristine_medium.json
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_pristine_small.json
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/scroll_small.json
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/slate.json
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/slate_blank.json
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/slate_block.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/slate_written.json
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook.json
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_double.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_double_sealed.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_empty.json
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_empty_sealed.json
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_entity.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_entity_sealed.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_list.json
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_list_sealed.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_pattern.json
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_pattern_sealed.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_vec3.json
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_vec3_sealed.json
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_widget.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook_widget_sealed.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/sub_sandwich.json
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/trinket.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/trinket_filled.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/uuid_colorizer.json
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_acacia.json
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_akashic.json
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_birch.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_bosnia.json
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_crimson.json
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_dark_oak.json
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_jungle.json
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_oak.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_old.json
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_spruce.json
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/wand_warped.json
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_bricks.png
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_bricks_small.png
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_chiseled.png
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_dust_block.png
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_polished.png
+-rw-r--r--   0        0        0    18846 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_sconce.png
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_tiles.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/ancient_scroll_paper.png
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/ancient_scroll_paper_lantern.png
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/ancient_scroll_paper_lantern_bottom.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/ancient_scroll_paper_lantern_side.png
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/ancient_scroll_paper_lantern_top.png
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/cracked_calcite.png
+-rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_button.png
+-rw-r--r--   0        0        0    16742 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_pressure_plate.png
+-rw-r--r--   0        0        0    26881 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_slab.png
+-rw-r--r--   0        0        0    31222 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_stairs.png
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/scroll_paper.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/scroll_paper_lantern.png
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/scroll_paper_lantern_bottom.png
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/scroll_paper_lantern_side.png
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/scroll_paper_lantern_top.png
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/slate.png
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/slate_directional.png
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/smooth_amethyst.png
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/connector.png
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/door_lower.png
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/door_upper.png
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/leaves1.png
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/leaves2.png
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/leaves3.png
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/log.png
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/log_alt_end.png
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/log_alt_end_stripped.png
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/log_end.png
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/log_end_stripped.png
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/log_stripped.png
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/panel.png
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/planks1.png
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/planks2.png
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/planks3.png
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/record.png
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/record_inner.png
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/tile.png
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/trapdoor.png
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/double1.png
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/double2.png
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/double3.png
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/double4.png
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/empty.png
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/end.png
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/entity1.png
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/entity2.png
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/entity3.png
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/entity4.png
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/list1.png
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/list2.png
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/list3.png
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/list4.png
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/other1.png
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/other2.png
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/other3.png
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/other4.png
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/pattern1.png
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/pattern2.png
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/pattern3.png
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/pattern4.png
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/side.png
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/vec1.png
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/vec2.png
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/vec3.png
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/vec4.png
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget1.png
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget2.png
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget3.png
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget4.png
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/end_dim.png
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/end_lit.png
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/horiz_dim.png
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/horiz_lit.png
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/vert_dim.png
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/vert_lit.png
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/back_powered.png
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/back_unpowered.png
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_powered_dim.png
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_powered_lit.png
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_unpowered_dim.png
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_unpowered_lit.png
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/front_dim.png
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/front_lit.png
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_powered_dim.png
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_powered_lit.png
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_unpowered_dim.png
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_unpowered_lit.png
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_powered_dim.png
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_powered_lit.png
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_unpowered_dim.png
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_unpowered_lit.png
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_powered_dim.png
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_powered_lit.png
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_unpowered_dim.png
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_unpowered_lit.png
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/atlas.png
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/back_dim.png
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/back_empty_dim.png
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/back_empty_lit.png
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/back_lit.png
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/down_dim.png
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/down_empty_dim.png
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/down_empty_lit.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/down_lit.png
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/front_empty_dim.png
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/front_empty_lit.png
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_dim.png
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_empty_dim.png
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_empty_lit.png
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_lit.png
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/look_dim.png
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/look_lit.png
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/right_dim.png
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/right_empty_dim.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/right_empty_lit.png
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/right_lit.png
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/rightclick_dim.png
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/rightclick_lit.png
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/something.png
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/storedplayer_dim.png
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/storedplayer_lit.png
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/up_dim.png
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/up_empty_dim.png
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/up_empty_lit.png
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/up_lit.png
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/scroll_ancient_large.png
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/scroll_ancient_medium.png
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/scroll_large.png
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/scroll_medium.png
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/sentinel.png
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/white.png
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/brainsweep.png
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/brainsweep_emi.png
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/brainsweep_jei.png
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/edify.png
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/edify_emi.png
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/edify_jei.png
+-rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/patchi_filler.png
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/phial.png
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/phial_emi.png
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/phial_jei.png
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/scroll.png
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/scroll_ancient.png
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/slate.png
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/villager_leveling.png
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/villager_profession.png
+-rw-r--r--   0        0        0    35018 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/entries/spell_circle.png
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/hexdoc/brainsweep.png
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/abacus.png
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/akashic_door.png
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/amethyst_dust.png
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/artifact.png
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/artifact_filled.png
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/charged_amethyst.png
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/creative_unlocker.png
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/cypher.png
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/cypher_filled.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/jeweler_hammer.png
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/lens.png
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/patchouli_book.png
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/scroll_ancient_large.png
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/scroll_ancient_medium.png
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/scroll_ancient_small.png
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/scroll_pristine_large.png
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/scroll_pristine_medium.png
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/scroll_pristine_small.png
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/slate_blank.png
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/slate_written.png
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/sub_sandwich.png
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/trinket.png
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/trinket_filled.png
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_black.png
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_blue.png
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_brown.png
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_cyan.png
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_gray.png
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_green.png
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_light_blue.png
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_light_gray.png
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_lime.png
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_magenta.png
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_orange.png
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_pink.png
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_purple.png
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_red.png
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_white.png
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_yellow.png
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_agender.png
+-rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_aroace.png
+-rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_aromantic.png
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_asexual.png
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_bisexual.png
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_demiboy.png
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_demigirl.png
+-rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_gay.png
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_genderfluid.png
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_genderqueer.png
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_intersex.png
+-rw-r--r--   0        0        0     6871 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_lesbian.png
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_nonbinary.png
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_pansexual.png
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_plural.png
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_transgender.png
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/uuid.png
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/double.png
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/double_sealed.png
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/empty.png
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/empty_sealed.png
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/entity.png
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/entity_sealed.png
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/list.png
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/list_sealed.png
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/pattern.png
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/pattern_sealed.png
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/vec3.png
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/vec3_sealed.png
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/widget.png
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/widget_sealed.png
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_large_0.png
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_large_1.png
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_large_2.png
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_large_3.png
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_large_4.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_medium_0.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_medium_1.png
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_medium_2.png
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_medium_3.png
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_medium_4.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_small_0.png
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_small_1.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_small_2.png
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_small_3.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/phial/phial_small_4.png
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/double.png
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/double_sealed.png
+-rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/empty.png
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/empty_sealed.png
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/entity.png
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/entity_sealed.png
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/list.png
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/list_sealed.png
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/pattern.png
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/pattern_sealed.png
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/vec3.png
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/vec3_sealed.png
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/widget.png
+-rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/widget_sealed.png
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/acacia.png
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/akashic.png
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/birch.png
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/bosnia.png
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/crimson.png
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/dark_oak.png
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/jungle.png
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/oak.png
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/old.png
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/spruce.png
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/warped.png
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/cloud.png
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_1.png
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_2.png
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_3.png
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_4.png
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_5.png
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_6.png
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_7.png
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/spin_cube_8.png
+-rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/allay.png
+-rw-r--r--   0        0        0    48613 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/armorer.png
+-rw-r--r--   0        0        0    17388 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/butcher.png
+-rw-r--r--   0        0        0    16563 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/cartographer.png
+-rw-r--r--   0        0        0    16752 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/cleric.png
+-rw-r--r--   0        0        0    23744 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/farmer.png
+-rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/fisherman.png
+-rw-r--r--   0        0        0    16906 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/fletcher.png
+-rw-r--r--   0        0        0    16807 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/leatherworker.png
+-rw-r--r--   0        0        0    17118 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/librarian.png
+-rw-r--r--   0        0        0    16898 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/mason.png
+-rw-r--r--   0        0        0    15451 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/nitwit.png
+-rw-r--r--   0        0        0    27110 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/none.png
+-rw-r--r--   0        0        0    18911 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/sphepherd.png
+-rw-r--r--   0        0        0    16436 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/toolsmith.png
+-rw-r--r--   0        0        0    16968 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/weaponsmith.png
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/book.json
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/basics.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/casting.json
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/greatwork.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/interop.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/items.json
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/patterns.json
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/patterns/great_spells.json
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/categories/patterns/spells.json
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/basics/couldnt_cast.json
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/basics/geodes.json
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/basics/media.json
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/basics/start_to_see.json
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/101.json
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/influences.json
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/mishaps.json
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/mishaps2.json
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/naming.json
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/stack.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/vectors.json
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/akashiclib.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/brainsweeping.json
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/directrix.json
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/impetus.json
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/spellcircles.json
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/the_work.json
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/interop/gravity.json
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/interop/interop.json
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/interop/pehkui.json
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/abacus.json
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/amethyst.json
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/decoration.json
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/edified.json
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/focus.json
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/hexcasting.json
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/jeweler_hammer.json
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/lens.json
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/phials.json
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/pigments.json
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/scroll.json
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/slate.json
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/spellbook.json
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/staff.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/advanced_math.json
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/akashic_patterns.json
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/basics.json
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/circle.json
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/consts.json
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/entities.json
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/lists.json
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/logic.json
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/math.json
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/meta.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/numbers.json
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/patterns_as_iotas.json
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/readers_guide.json
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/readwrite.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/sets.json
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/stackmanip.json
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/brainsweep.json
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/create_lava.json
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/flight.json
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/greater_sentinel.json
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/make_battery.json
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/teleport.json
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/weather_manip.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/zeniths.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/basic.json
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/blockworks.json
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/colorize.json
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/hexcasting.json
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/itempicking.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/nadirs.json
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/sentinels.json
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/abacus.json
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/ageing_scroll_paper_lantern.json
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_bookshelf.json
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_button.json
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_connector.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_door.json
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_panel.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_planks.json
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_pressure_plate.json
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_slab.json
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_stairs.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_tile.json
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_trapdoor.json
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/akashic_wood.json
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/amethyst_dust_packing.json
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/amethyst_dust_unpacking.json
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/amethyst_sconce.json
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/amethyst_tiles.json
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/ancient_scroll_paper.json
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/ancient_scroll_paper_lantern.json
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/artifact.json
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/cypher.json
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_blue.json
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_brown.json
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_cyan.json
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_gray.json
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_green.json
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_light_blue.json
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_light_gray.json
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_lime.json
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_magenta.json
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_orange.json
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_pink.json
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_purple.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_red.json
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_white.json
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/dye_colorizer_yellow.json
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/empty_directrix.json
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/empty_impetus.json
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/focus.json
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/jeweler_hammer.json
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/lens.json
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_agender.json
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_aroace.json
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_aromantic.json
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_asexual.json
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_bisexual.json
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_demiboy.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_demigirl.json
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_gay.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_genderfluid.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_genderqueer.json
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_intersex.json
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_lesbian.json
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_nonbinary.json
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_pansexual.json
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_plural.json
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/pride_colorizer_transgender.json
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/scroll.json
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/scroll_medium.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/scroll_paper.json
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/scroll_paper_lantern.json
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/scroll_small.json
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/slate.json
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/slate_block.json
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/slate_block_from_slates.json
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/spellbook.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/trinket.json
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/uuid_colorizer.json
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_acacia.json
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_akashic.json
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_birch.json
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_crimson.json
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_dark_oak.json
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_jungle.json
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_oak.json
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_spruce.json
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/wand_warped.json
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/brainsweep/akashic_record.json
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/brainsweep/budding_amethyst.json
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/brainsweep/directrix_redstone.json
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/brainsweep/impetus_look.json
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/brainsweep/impetus_rightclick.json
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/brainsweep/impetus_storedplayer.json
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/tags/items/akashic_logs.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/tags/items/akashic_planks.json
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexdoc/tags/advancements/spoilered.json
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexdoc/tags/items/gaslighting.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/minecraft/tags/items/planks.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/__init__.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/hexcasting.js.jinja
+-rw-r--r--   0        0        0    10267 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/hexcasting_render.js.jinja
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/index.css.jinja
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/index.html.jinja
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/ingredients/hexcasting/brainsweepee/entity_tag.html.jinja
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/ingredients/hexcasting/brainsweepee/entity_type.html.jinja
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/ingredients/hexcasting/brainsweepee/villager.html.jinja
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/pages/hexcasting/brainsweep.html.jinja
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/pages/hexcasting/crafting_multi.html.jinja
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/pages/hexcasting/manual_pattern.html.jinja
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/pages/hexcasting/pattern.html.jinja
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/recipes/hexcasting/brainsweep.html.jinja
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/book/recipes.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/book/page/__init__.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/book/page/abstract_pages.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/book/page/pages.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/utils/__init__.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/utils/pattern.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/LICENSE.txt
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/pyproject.toml
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/doc/README.md
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 hexdoc_hexcasting-0.9.6.1.0.dev24/PKG-INFO
```

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_hooks.py` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,8 +143,9 @@
     def jinja_template_root(self) -> tuple[Package, str]:
         return hexdoc_hexcasting, "_templates"
 
     @override
     def default_rendered_templates(self) -> dict[str | Path, str]:
         return {
             "hexcasting.js": "hexcasting.js.jinja",
+            "hexcasting_render.js": "hexcasting_render.js.jinja",
         }
```

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/metadata.py` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         return Path(f"{modid}.patterns.hexdoc.json")
 
 
 class PatternStubProps(StripHiddenModel):
     path: RelativePath
     regex: re.Pattern[str]
     per_world_value: str | None = "true"
+    required: bool = True
+    """If `True` (the default), raise an error if no patterns were loaded from here."""
 
 
 class HexProperties(StripHiddenModel):
     pattern_stubs: list[PatternStubProps]
 
 
 # conthext, perhaps
@@ -112,22 +114,36 @@
         stub: PatternStubProps,
         per_world_tag: Tag | None,
     ):
         # TODO: add Gradle task to generate json with this data. this is dumb and fragile.
         logger.debug(f"Load pattern stub from {stub.path}")
         stub_text = stub.path.read_text("utf-8")
 
+        patterns = list[PatternInfo]()
+
         for match in stub.regex.finditer(stub_text):
             groups = match.groupdict()
             id = props.mod_loc(groups["name"])
 
             if per_world_tag is not None:
                 is_per_world = id in per_world_tag.values
             else:
                 is_per_world = groups.get("is_per_world") == stub.per_world_value
 
-            yield PatternInfo(
-                id=id,
-                startdir=Direction[groups["startdir"]],
-                signature=groups["signature"],
-                is_per_world=is_per_world,
+            patterns.append(
+                PatternInfo(
+                    id=id,
+                    startdir=Direction[groups["startdir"]],
+                    signature=groups["signature"],
+                    is_per_world=is_per_world,
+                )
             )
+
+        pretty_path = stub.path.resolve().relative_to(Path.cwd())
+
+        if stub.required and not patterns:
+            raise ValueError(
+                f"No patterns found in {pretty_path} (check the pattern regex)"
+            )
+
+        logger.info(f"Loaded {len(patterns)} patterns from {pretty_path}")
+        return patterns
```

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/hexcasting.hexdoc.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/hexcasting.hexdoc.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6599726228632479%*

 * *Differences: {"'asset_url'": "'https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9'",*

 * * "'book_url'": "'https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/en_us'",*

 * * "'textures'": "{'PNGTexture': {'hexcasting:textures/gui/scroll.png': {'url': "*

 * *               "'https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/scroll.png'}, "*

 * *               "'hexcasting:textures/gui/edify_jei.png […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "asset_url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769",
-    "book_url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/en_us",
+    "asset_url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9",
+    "book_url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/en_us",
     "textures": {
         "AnimatedTexture": {
             "hexcasting:textures/item/colorizer/dye_black.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_black-png",
                 "meta": {
                     "animation": {
                         "frames": [
@@ -129,15 +129,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_black.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_black.png"
             },
             "hexcasting:textures/item/colorizer/dye_blue.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_blue-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -261,15 +261,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_blue.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_blue.png"
             },
             "hexcasting:textures/item/colorizer/dye_brown.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_brown-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -393,15 +393,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_brown.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_brown.png"
             },
             "hexcasting:textures/item/colorizer/dye_cyan.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_cyan-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -525,15 +525,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_cyan.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_cyan.png"
             },
             "hexcasting:textures/item/colorizer/dye_gray.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_gray-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -657,15 +657,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_gray.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_gray.png"
             },
             "hexcasting:textures/item/colorizer/dye_green.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_green-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -789,15 +789,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_green.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_green.png"
             },
             "hexcasting:textures/item/colorizer/dye_light_blue.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_light_blue-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -921,15 +921,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_light_blue.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_light_blue.png"
             },
             "hexcasting:textures/item/colorizer/dye_light_gray.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_light_gray-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -1053,15 +1053,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_light_gray.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_light_gray.png"
             },
             "hexcasting:textures/item/colorizer/dye_lime.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_lime-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -1185,15 +1185,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_lime.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_lime.png"
             },
             "hexcasting:textures/item/colorizer/dye_magenta.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_magenta-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -1317,15 +1317,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_magenta.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_magenta.png"
             },
             "hexcasting:textures/item/colorizer/dye_orange.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_orange-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -1449,15 +1449,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_orange.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_orange.png"
             },
             "hexcasting:textures/item/colorizer/dye_pink.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_pink-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -1581,15 +1581,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_pink.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_pink.png"
             },
             "hexcasting:textures/item/colorizer/dye_purple.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_purple-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -1713,15 +1713,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_purple.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_purple.png"
             },
             "hexcasting:textures/item/colorizer/dye_red.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_red-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -1845,15 +1845,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_red.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_red.png"
             },
             "hexcasting:textures/item/colorizer/dye_white.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_white-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -1977,15 +1977,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_white.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_white.png"
             },
             "hexcasting:textures/item/colorizer/dye_yellow.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-dye_yellow-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -2109,15 +2109,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_yellow.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_yellow.png"
             },
             "hexcasting:textures/item/colorizer/pride_agender.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_agender-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -2249,15 +2249,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_agender.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_agender.png"
             },
             "hexcasting:textures/item/colorizer/pride_aroace.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_aroace-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -2389,15 +2389,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_aroace.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_aroace.png"
             },
             "hexcasting:textures/item/colorizer/pride_aromantic.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_aromantic-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -2529,15 +2529,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_aromantic.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_aromantic.png"
             },
             "hexcasting:textures/item/colorizer/pride_asexual.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_asexual-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -2669,15 +2669,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_asexual.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_asexual.png"
             },
             "hexcasting:textures/item/colorizer/pride_bisexual.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_bisexual-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -2825,15 +2825,15 @@
                                 "time": 10
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_bisexual.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_bisexual.png"
             },
             "hexcasting:textures/item/colorizer/pride_demiboy.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_demiboy-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -2981,15 +2981,15 @@
                                 "time": 10
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_demiboy.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_demiboy.png"
             },
             "hexcasting:textures/item/colorizer/pride_demigirl.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_demigirl-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -3137,15 +3137,15 @@
                                 "time": 10
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_demigirl.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_demigirl.png"
             },
             "hexcasting:textures/item/colorizer/pride_gay.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_gay-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -3277,15 +3277,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_gay.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_gay.png"
             },
             "hexcasting:textures/item/colorizer/pride_genderfluid.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_genderfluid-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -3417,15 +3417,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_genderfluid.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_genderfluid.png"
             },
             "hexcasting:textures/item/colorizer/pride_genderqueer.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_genderqueer-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -3573,15 +3573,15 @@
                                 "time": 10
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_genderqueer.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_genderqueer.png"
             },
             "hexcasting:textures/item/colorizer/pride_intersex.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_intersex-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -3705,15 +3705,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_intersex.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_intersex.png"
             },
             "hexcasting:textures/item/colorizer/pride_lesbian.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_lesbian-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -3845,15 +3845,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_lesbian.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_lesbian.png"
             },
             "hexcasting:textures/item/colorizer/pride_nonbinary.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_nonbinary-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -3985,15 +3985,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_nonbinary.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_nonbinary.png"
             },
             "hexcasting:textures/item/colorizer/pride_pansexual.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_pansexual-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -4141,15 +4141,15 @@
                                 "time": 10
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_pansexual.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_pansexual.png"
             },
             "hexcasting:textures/item/colorizer/pride_plural.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_plural-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -4281,15 +4281,15 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_plural.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_plural.png"
             },
             "hexcasting:textures/item/colorizer/pride_transgender.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-pride_transgender-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -4437,15 +4437,15 @@
                                 "time": 10
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_transgender.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_transgender.png"
             },
             "hexcasting:textures/item/colorizer/uuid.png": {
                 "css_class": "texture-hexcasting-textures-item-colorizer-uuid-png",
                 "meta": {
                     "animation": {
                         "frames": [
                             {
@@ -4529,1057 +4529,1057 @@
                                 "time": 1
                             }
                         ],
                         "interpolate": false
                     }
                 },
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/uuid.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/uuid.png"
             }
         },
         "PNGTexture": {
             "farmersdelight:textures/block/skillet_bottom.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/farmersdelight/textures/block/skillet_bottom.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/farmersdelight/textures/block/skillet_bottom.png"
             },
             "farmersdelight:textures/block/skillet_side.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/farmersdelight/textures/block/skillet_side.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/farmersdelight/textures/block/skillet_side.png"
             },
             "farmersdelight:textures/block/skillet_top.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/farmersdelight/textures/block/skillet_top.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/farmersdelight/textures/block/skillet_top.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/double1.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/double1.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/double1.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/double2.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/double2.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/double2.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/double3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/double3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/double3.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/double4.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/double4.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/double4.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/empty.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/empty.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/empty.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/end.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/end.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/end.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/entity1.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/entity1.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/entity1.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/entity2.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/entity2.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/entity2.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/entity3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/entity3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/entity3.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/entity4.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/entity4.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/entity4.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/list1.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/list1.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/list1.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/list2.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/list2.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/list2.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/list3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/list3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/list3.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/list4.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/list4.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/list4.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/other1.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/other1.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/other1.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/other2.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/other2.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/other2.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/other3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/other3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/other3.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/other4.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/other4.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/other4.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/pattern1.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/pattern1.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/pattern1.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/pattern2.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/pattern2.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/pattern2.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/pattern3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/pattern3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/pattern3.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/pattern4.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/pattern4.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/pattern4.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/side.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/side.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/side.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/vec1.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/vec1.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/vec1.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/vec2.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/vec2.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/vec2.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/vec3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/vec3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/vec3.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/vec4.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/vec4.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/vec4.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/widget1.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/widget1.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/widget1.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/widget2.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/widget2.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/widget2.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/widget3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/widget3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/widget3.png"
             },
             "hexcasting:textures/block/akashic/bookshelf/widget4.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/widget4.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/bookshelf/widget4.png"
             },
             "hexcasting:textures/block/akashic/connector.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/connector.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/connector.png"
             },
             "hexcasting:textures/block/akashic/door_lower.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/door_lower.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/door_lower.png"
             },
             "hexcasting:textures/block/akashic/door_upper.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/door_upper.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/door_upper.png"
             },
             "hexcasting:textures/block/akashic/leaves1.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/leaves1.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/leaves1.png"
             },
             "hexcasting:textures/block/akashic/leaves2.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/leaves2.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/leaves2.png"
             },
             "hexcasting:textures/block/akashic/leaves3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/leaves3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/leaves3.png"
             },
             "hexcasting:textures/block/akashic/log.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/log.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/log.png"
             },
             "hexcasting:textures/block/akashic/log_alt_end.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/log_alt_end.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/log_alt_end.png"
             },
             "hexcasting:textures/block/akashic/log_alt_end_stripped.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/log_alt_end_stripped.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/log_alt_end_stripped.png"
             },
             "hexcasting:textures/block/akashic/log_end.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/log_end.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/log_end.png"
             },
             "hexcasting:textures/block/akashic/log_end_stripped.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/log_end_stripped.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/log_end_stripped.png"
             },
             "hexcasting:textures/block/akashic/log_stripped.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/log_stripped.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/log_stripped.png"
             },
             "hexcasting:textures/block/akashic/panel.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/panel.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/panel.png"
             },
             "hexcasting:textures/block/akashic/planks1.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/planks1.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/planks1.png"
             },
             "hexcasting:textures/block/akashic/planks2.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/planks2.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/planks2.png"
             },
             "hexcasting:textures/block/akashic/planks3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/planks3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/planks3.png"
             },
             "hexcasting:textures/block/akashic/record.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/record.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/record.png"
             },
             "hexcasting:textures/block/akashic/record_inner.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/record_inner.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/record_inner.png"
             },
             "hexcasting:textures/block/akashic/tile.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/tile.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/tile.png"
             },
             "hexcasting:textures/block/akashic/trapdoor.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/akashic/trapdoor.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/akashic/trapdoor.png"
             },
             "hexcasting:textures/block/amethyst_bricks.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/amethyst_bricks.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/amethyst_bricks.png"
             },
             "hexcasting:textures/block/amethyst_bricks_small.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/amethyst_bricks_small.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/amethyst_bricks_small.png"
             },
             "hexcasting:textures/block/amethyst_chiseled.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/amethyst_chiseled.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/amethyst_chiseled.png"
             },
             "hexcasting:textures/block/amethyst_dust_block.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/amethyst_dust_block.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/amethyst_dust_block.png"
             },
             "hexcasting:textures/block/amethyst_polished.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/amethyst_polished.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/amethyst_polished.png"
             },
             "hexcasting:textures/block/amethyst_sconce.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/hexcasting/textures/block/amethyst_sconce.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/hexcasting/textures/block/amethyst_sconce.png"
             },
             "hexcasting:textures/block/amethyst_tiles.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/amethyst_tiles.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/amethyst_tiles.png"
             },
             "hexcasting:textures/block/ancient_scroll_paper.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/ancient_scroll_paper.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/ancient_scroll_paper.png"
             },
             "hexcasting:textures/block/ancient_scroll_paper_lantern.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/ancient_scroll_paper_lantern.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/ancient_scroll_paper_lantern.png"
             },
             "hexcasting:textures/block/ancient_scroll_paper_lantern_bottom.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/ancient_scroll_paper_lantern_bottom.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/ancient_scroll_paper_lantern_bottom.png"
             },
             "hexcasting:textures/block/ancient_scroll_paper_lantern_side.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/ancient_scroll_paper_lantern_side.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/ancient_scroll_paper_lantern_side.png"
             },
             "hexcasting:textures/block/ancient_scroll_paper_lantern_top.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/ancient_scroll_paper_lantern_top.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/ancient_scroll_paper_lantern_top.png"
             },
             "hexcasting:textures/block/cracked_calcite.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/cracked_calcite.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/cracked_calcite.png"
             },
             "hexcasting:textures/block/directrix/empty/end_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/empty/end_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/empty/end_dim.png"
             },
             "hexcasting:textures/block/directrix/empty/end_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/empty/end_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/empty/end_lit.png"
             },
             "hexcasting:textures/block/directrix/empty/horiz_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/empty/horiz_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/empty/horiz_dim.png"
             },
             "hexcasting:textures/block/directrix/empty/horiz_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/empty/horiz_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/empty/horiz_lit.png"
             },
             "hexcasting:textures/block/directrix/empty/vert_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/empty/vert_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/empty/vert_dim.png"
             },
             "hexcasting:textures/block/directrix/empty/vert_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/empty/vert_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/empty/vert_lit.png"
             },
             "hexcasting:textures/block/directrix/redstone/back_powered.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/back_powered.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/back_powered.png"
             },
             "hexcasting:textures/block/directrix/redstone/back_unpowered.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/back_unpowered.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/back_unpowered.png"
             },
             "hexcasting:textures/block/directrix/redstone/down_powered_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/down_powered_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/down_powered_dim.png"
             },
             "hexcasting:textures/block/directrix/redstone/down_powered_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/down_powered_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/down_powered_lit.png"
             },
             "hexcasting:textures/block/directrix/redstone/down_unpowered_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/down_unpowered_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/down_unpowered_dim.png"
             },
             "hexcasting:textures/block/directrix/redstone/down_unpowered_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/down_unpowered_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/down_unpowered_lit.png"
             },
             "hexcasting:textures/block/directrix/redstone/front_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/front_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/front_dim.png"
             },
             "hexcasting:textures/block/directrix/redstone/front_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/front_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/front_lit.png"
             },
             "hexcasting:textures/block/directrix/redstone/left_powered_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/left_powered_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/left_powered_dim.png"
             },
             "hexcasting:textures/block/directrix/redstone/left_powered_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/left_powered_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/left_powered_lit.png"
             },
             "hexcasting:textures/block/directrix/redstone/left_unpowered_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/left_unpowered_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/left_unpowered_dim.png"
             },
             "hexcasting:textures/block/directrix/redstone/left_unpowered_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/left_unpowered_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/left_unpowered_lit.png"
             },
             "hexcasting:textures/block/directrix/redstone/right_powered_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/right_powered_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/right_powered_dim.png"
             },
             "hexcasting:textures/block/directrix/redstone/right_powered_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/right_powered_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/right_powered_lit.png"
             },
             "hexcasting:textures/block/directrix/redstone/right_unpowered_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/right_unpowered_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/right_unpowered_dim.png"
             },
             "hexcasting:textures/block/directrix/redstone/right_unpowered_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/right_unpowered_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/right_unpowered_lit.png"
             },
             "hexcasting:textures/block/directrix/redstone/up_powered_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/up_powered_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/up_powered_dim.png"
             },
             "hexcasting:textures/block/directrix/redstone/up_powered_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/up_powered_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/up_powered_lit.png"
             },
             "hexcasting:textures/block/directrix/redstone/up_unpowered_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/up_unpowered_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/up_unpowered_dim.png"
             },
             "hexcasting:textures/block/directrix/redstone/up_unpowered_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/up_unpowered_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/directrix/redstone/up_unpowered_lit.png"
             },
             "hexcasting:textures/block/edified_button.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/hexcasting/textures/block/edified_button.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/hexcasting/textures/block/edified_button.png"
             },
             "hexcasting:textures/block/edified_pressure_plate.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/hexcasting/textures/block/edified_pressure_plate.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/hexcasting/textures/block/edified_pressure_plate.png"
             },
             "hexcasting:textures/block/edified_slab.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/hexcasting/textures/block/edified_slab.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/hexcasting/textures/block/edified_slab.png"
             },
             "hexcasting:textures/block/edified_stairs.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/hexcasting/textures/block/edified_stairs.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/hexcasting/textures/block/edified_stairs.png"
             },
             "hexcasting:textures/block/impetus/atlas.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/atlas.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/atlas.png"
             },
             "hexcasting:textures/block/impetus/back_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/back_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/back_dim.png"
             },
             "hexcasting:textures/block/impetus/back_empty_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/back_empty_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/back_empty_dim.png"
             },
             "hexcasting:textures/block/impetus/back_empty_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/back_empty_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/back_empty_lit.png"
             },
             "hexcasting:textures/block/impetus/back_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/back_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/back_lit.png"
             },
             "hexcasting:textures/block/impetus/down_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/down_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/down_dim.png"
             },
             "hexcasting:textures/block/impetus/down_empty_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/down_empty_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/down_empty_dim.png"
             },
             "hexcasting:textures/block/impetus/down_empty_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/down_empty_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/down_empty_lit.png"
             },
             "hexcasting:textures/block/impetus/down_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/down_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/down_lit.png"
             },
             "hexcasting:textures/block/impetus/front_empty_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/front_empty_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/front_empty_dim.png"
             },
             "hexcasting:textures/block/impetus/front_empty_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/front_empty_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/front_empty_lit.png"
             },
             "hexcasting:textures/block/impetus/left_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/left_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/left_dim.png"
             },
             "hexcasting:textures/block/impetus/left_empty_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/left_empty_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/left_empty_dim.png"
             },
             "hexcasting:textures/block/impetus/left_empty_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/left_empty_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/left_empty_lit.png"
             },
             "hexcasting:textures/block/impetus/left_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/left_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/left_lit.png"
             },
             "hexcasting:textures/block/impetus/look_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/look_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/look_dim.png"
             },
             "hexcasting:textures/block/impetus/look_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/look_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/look_lit.png"
             },
             "hexcasting:textures/block/impetus/right_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/right_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/right_dim.png"
             },
             "hexcasting:textures/block/impetus/right_empty_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/right_empty_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/right_empty_dim.png"
             },
             "hexcasting:textures/block/impetus/right_empty_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/right_empty_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/right_empty_lit.png"
             },
             "hexcasting:textures/block/impetus/right_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/right_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/right_lit.png"
             },
             "hexcasting:textures/block/impetus/rightclick_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/rightclick_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/rightclick_dim.png"
             },
             "hexcasting:textures/block/impetus/rightclick_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/rightclick_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/rightclick_lit.png"
             },
             "hexcasting:textures/block/impetus/something.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/something.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/something.png"
             },
             "hexcasting:textures/block/impetus/storedplayer_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/storedplayer_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/storedplayer_dim.png"
             },
             "hexcasting:textures/block/impetus/storedplayer_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/storedplayer_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/storedplayer_lit.png"
             },
             "hexcasting:textures/block/impetus/up_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/up_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/up_dim.png"
             },
             "hexcasting:textures/block/impetus/up_empty_dim.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/up_empty_dim.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/up_empty_dim.png"
             },
             "hexcasting:textures/block/impetus/up_empty_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/up_empty_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/up_empty_lit.png"
             },
             "hexcasting:textures/block/impetus/up_lit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/impetus/up_lit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/impetus/up_lit.png"
             },
             "hexcasting:textures/block/scroll_paper.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/scroll_paper.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/scroll_paper.png"
             },
             "hexcasting:textures/block/scroll_paper_lantern.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/scroll_paper_lantern.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/scroll_paper_lantern.png"
             },
             "hexcasting:textures/block/scroll_paper_lantern_bottom.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/scroll_paper_lantern_bottom.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/scroll_paper_lantern_bottom.png"
             },
             "hexcasting:textures/block/scroll_paper_lantern_side.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/scroll_paper_lantern_side.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/scroll_paper_lantern_side.png"
             },
             "hexcasting:textures/block/scroll_paper_lantern_top.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/scroll_paper_lantern_top.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/scroll_paper_lantern_top.png"
             },
             "hexcasting:textures/block/slate.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/slate.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/slate.png"
             },
             "hexcasting:textures/block/slate_directional.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/slate_directional.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/slate_directional.png"
             },
             "hexcasting:textures/block/smooth_amethyst.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/block/smooth_amethyst.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/block/smooth_amethyst.png"
             },
             "hexcasting:textures/entity/scroll_ancient_large.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/entity/scroll_ancient_large.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/entity/scroll_ancient_large.png"
             },
             "hexcasting:textures/entity/scroll_ancient_medium.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/entity/scroll_ancient_medium.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/entity/scroll_ancient_medium.png"
             },
             "hexcasting:textures/entity/scroll_large.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/entity/scroll_large.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/entity/scroll_large.png"
             },
             "hexcasting:textures/entity/scroll_medium.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/entity/scroll_medium.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/entity/scroll_medium.png"
             },
             "hexcasting:textures/entity/sentinel.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/entity/sentinel.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/entity/sentinel.png"
             },
             "hexcasting:textures/entity/white.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/entity/white.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/entity/white.png"
             },
             "hexcasting:textures/gui/brainsweep.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/brainsweep.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/brainsweep.png"
             },
             "hexcasting:textures/gui/brainsweep_emi.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/brainsweep_emi.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/brainsweep_emi.png"
             },
             "hexcasting:textures/gui/brainsweep_jei.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/brainsweep_jei.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/brainsweep_jei.png"
             },
             "hexcasting:textures/gui/edify.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/edify.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/edify.png"
             },
             "hexcasting:textures/gui/edify_emi.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/edify_emi.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/edify_emi.png"
             },
             "hexcasting:textures/gui/edify_jei.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/edify_jei.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/edify_jei.png"
             },
             "hexcasting:textures/gui/entries/spell_circle.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/entries/spell_circle.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/entries/spell_circle.png"
             },
             "hexcasting:textures/gui/hexdoc/brainsweep.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/hexcasting/textures/gui/hexdoc/brainsweep.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/hexcasting/textures/gui/hexdoc/brainsweep.png"
             },
             "hexcasting:textures/gui/patchi_filler.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/patchi_filler.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/patchi_filler.png"
             },
             "hexcasting:textures/gui/phial.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/phial.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/phial.png"
             },
             "hexcasting:textures/gui/phial_emi.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/phial_emi.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/phial_emi.png"
             },
             "hexcasting:textures/gui/phial_jei.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/phial_jei.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/phial_jei.png"
             },
             "hexcasting:textures/gui/scroll.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/scroll.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/scroll.png"
             },
             "hexcasting:textures/gui/scroll_ancient.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/scroll_ancient.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/scroll_ancient.png"
             },
             "hexcasting:textures/gui/slate.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/slate.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/slate.png"
             },
             "hexcasting:textures/gui/villager_leveling.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/villager_leveling.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/villager_leveling.png"
             },
             "hexcasting:textures/gui/villager_profession.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/gui/villager_profession.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/gui/villager_profession.png"
             },
             "hexcasting:textures/item/abacus.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/abacus.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/abacus.png"
             },
             "hexcasting:textures/item/akashic_door.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/akashic_door.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/akashic_door.png"
             },
             "hexcasting:textures/item/amethyst_dust.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/amethyst_dust.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/amethyst_dust.png"
             },
             "hexcasting:textures/item/artifact.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/artifact.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/artifact.png"
             },
             "hexcasting:textures/item/artifact_filled.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/artifact_filled.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/artifact_filled.png"
             },
             "hexcasting:textures/item/charged_amethyst.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/charged_amethyst.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/charged_amethyst.png"
             },
             "hexcasting:textures/item/creative_unlocker.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/creative_unlocker.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/creative_unlocker.png"
             },
             "hexcasting:textures/item/cypher.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/cypher.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/cypher.png"
             },
             "hexcasting:textures/item/cypher_filled.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/cypher_filled.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/cypher_filled.png"
             },
             "hexcasting:textures/item/focus/double.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/double.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/double.png"
             },
             "hexcasting:textures/item/focus/double_sealed.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/double_sealed.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/double_sealed.png"
             },
             "hexcasting:textures/item/focus/empty.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/empty.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/empty.png"
             },
             "hexcasting:textures/item/focus/empty_sealed.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/empty_sealed.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/empty_sealed.png"
             },
             "hexcasting:textures/item/focus/entity.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/entity.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/entity.png"
             },
             "hexcasting:textures/item/focus/entity_sealed.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/entity_sealed.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/entity_sealed.png"
             },
             "hexcasting:textures/item/focus/list.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/list.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/list.png"
             },
             "hexcasting:textures/item/focus/list_sealed.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/list_sealed.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/list_sealed.png"
             },
             "hexcasting:textures/item/focus/pattern.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/pattern.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/pattern.png"
             },
             "hexcasting:textures/item/focus/pattern_sealed.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/pattern_sealed.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/pattern_sealed.png"
             },
             "hexcasting:textures/item/focus/vec3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/vec3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/vec3.png"
             },
             "hexcasting:textures/item/focus/vec3_sealed.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/vec3_sealed.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/vec3_sealed.png"
             },
             "hexcasting:textures/item/focus/widget.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/widget.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/widget.png"
             },
             "hexcasting:textures/item/focus/widget_sealed.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/widget_sealed.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/widget_sealed.png"
             },
             "hexcasting:textures/item/jeweler_hammer.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/jeweler_hammer.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/jeweler_hammer.png"
             },
             "hexcasting:textures/item/lens.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/lens.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/lens.png"
             },
             "hexcasting:textures/item/patchouli_book.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/patchouli_book.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/patchouli_book.png"
             },
             "hexcasting:textures/item/phial/phial_large_0.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_0.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_0.png"
             },
             "hexcasting:textures/item/phial/phial_large_1.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_1.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_1.png"
             },
             "hexcasting:textures/item/phial/phial_large_2.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_2.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_2.png"
             },
             "hexcasting:textures/item/phial/phial_large_3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_3.png"
             },
             "hexcasting:textures/item/phial/phial_large_4.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_4.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_4.png"
             },
             "hexcasting:textures/item/phial/phial_medium_0.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_0.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_0.png"
             },
             "hexcasting:textures/item/phial/phial_medium_1.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_1.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_1.png"
             },
             "hexcasting:textures/item/phial/phial_medium_2.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_2.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_2.png"
             },
             "hexcasting:textures/item/phial/phial_medium_3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_3.png"
             },
             "hexcasting:textures/item/phial/phial_medium_4.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_4.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_4.png"
             },
             "hexcasting:textures/item/phial/phial_small_0.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_0.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_0.png"
             },
             "hexcasting:textures/item/phial/phial_small_1.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_1.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_1.png"
             },
             "hexcasting:textures/item/phial/phial_small_2.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_2.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_2.png"
             },
             "hexcasting:textures/item/phial/phial_small_3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_3.png"
             },
             "hexcasting:textures/item/phial/phial_small_4.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_4.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_4.png"
             },
             "hexcasting:textures/item/scroll_ancient_large.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_ancient_large.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_ancient_large.png"
             },
             "hexcasting:textures/item/scroll_ancient_medium.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_ancient_medium.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_ancient_medium.png"
             },
             "hexcasting:textures/item/scroll_ancient_small.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_ancient_small.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_ancient_small.png"
             },
             "hexcasting:textures/item/scroll_pristine_large.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_large.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_large.png"
             },
             "hexcasting:textures/item/scroll_pristine_medium.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_medium.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_medium.png"
             },
             "hexcasting:textures/item/scroll_pristine_small.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_small.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_small.png"
             },
             "hexcasting:textures/item/slate_blank.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/slate_blank.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/slate_blank.png"
             },
             "hexcasting:textures/item/slate_written.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/slate_written.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/slate_written.png"
             },
             "hexcasting:textures/item/spellbook/double.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/double.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/double.png"
             },
             "hexcasting:textures/item/spellbook/double_sealed.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/double_sealed.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/double_sealed.png"
             },
             "hexcasting:textures/item/spellbook/empty.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/empty.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/empty.png"
             },
             "hexcasting:textures/item/spellbook/empty_sealed.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/empty_sealed.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/empty_sealed.png"
             },
             "hexcasting:textures/item/spellbook/entity.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/entity.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/entity.png"
             },
             "hexcasting:textures/item/spellbook/entity_sealed.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/entity_sealed.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/entity_sealed.png"
             },
             "hexcasting:textures/item/spellbook/list.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/list.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/list.png"
             },
             "hexcasting:textures/item/spellbook/list_sealed.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/list_sealed.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/list_sealed.png"
             },
             "hexcasting:textures/item/spellbook/pattern.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/pattern.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/pattern.png"
             },
             "hexcasting:textures/item/spellbook/pattern_sealed.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/pattern_sealed.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/pattern_sealed.png"
             },
             "hexcasting:textures/item/spellbook/vec3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/vec3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/vec3.png"
             },
             "hexcasting:textures/item/spellbook/vec3_sealed.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/vec3_sealed.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/vec3_sealed.png"
             },
             "hexcasting:textures/item/spellbook/widget.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/widget.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/widget.png"
             },
             "hexcasting:textures/item/spellbook/widget_sealed.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/widget_sealed.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/widget_sealed.png"
             },
             "hexcasting:textures/item/sub_sandwich.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/sub_sandwich.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/sub_sandwich.png"
             },
             "hexcasting:textures/item/trinket.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/trinket.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/trinket.png"
             },
             "hexcasting:textures/item/trinket_filled.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/trinket_filled.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/trinket_filled.png"
             },
             "hexcasting:textures/item/wands/acacia.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/acacia.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/acacia.png"
             },
             "hexcasting:textures/item/wands/akashic.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/akashic.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/akashic.png"
             },
             "hexcasting:textures/item/wands/birch.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/birch.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/birch.png"
             },
             "hexcasting:textures/item/wands/bosnia.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/bosnia.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/bosnia.png"
             },
             "hexcasting:textures/item/wands/crimson.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/crimson.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/crimson.png"
             },
             "hexcasting:textures/item/wands/dark_oak.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/dark_oak.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/dark_oak.png"
             },
             "hexcasting:textures/item/wands/jungle.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/jungle.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/jungle.png"
             },
             "hexcasting:textures/item/wands/oak.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/oak.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/oak.png"
             },
             "hexcasting:textures/item/wands/old.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/old.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/old.png"
             },
             "hexcasting:textures/item/wands/spruce.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/spruce.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/spruce.png"
             },
             "hexcasting:textures/item/wands/warped.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/warped.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/warped.png"
             },
             "hexcasting:textures/particle/cloud.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/particle/cloud.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/particle/cloud.png"
             },
             "hexcasting:textures/particle/spin_cube_1.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_1.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_1.png"
             },
             "hexcasting:textures/particle/spin_cube_2.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_2.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_2.png"
             },
             "hexcasting:textures/particle/spin_cube_3.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_3.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_3.png"
             },
             "hexcasting:textures/particle/spin_cube_4.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_4.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_4.png"
             },
             "hexcasting:textures/particle/spin_cube_5.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_5.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_5.png"
             },
             "hexcasting:textures/particle/spin_cube_6.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_6.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_6.png"
             },
             "hexcasting:textures/particle/spin_cube_7.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_7.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_7.png"
             },
             "hexcasting:textures/particle/spin_cube_8.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_8.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/particle/spin_cube_8.png"
             },
             "minecraft:textures/entities/allay.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/allay.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/allay.png"
             },
             "minecraft:textures/entities/villagers/armorer.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/armorer.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/armorer.png"
             },
             "minecraft:textures/entities/villagers/butcher.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/butcher.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/butcher.png"
             },
             "minecraft:textures/entities/villagers/cartographer.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/cartographer.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/cartographer.png"
             },
             "minecraft:textures/entities/villagers/cleric.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/cleric.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/cleric.png"
             },
             "minecraft:textures/entities/villagers/farmer.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/farmer.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/farmer.png"
             },
             "minecraft:textures/entities/villagers/fisherman.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/fisherman.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/fisherman.png"
             },
             "minecraft:textures/entities/villagers/fletcher.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/fletcher.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/fletcher.png"
             },
             "minecraft:textures/entities/villagers/leatherworker.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/leatherworker.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/leatherworker.png"
             },
             "minecraft:textures/entities/villagers/librarian.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/librarian.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/librarian.png"
             },
             "minecraft:textures/entities/villagers/mason.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/mason.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/mason.png"
             },
             "minecraft:textures/entities/villagers/nitwit.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/nitwit.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/nitwit.png"
             },
             "minecraft:textures/entities/villagers/none.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/none.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/none.png"
             },
             "minecraft:textures/entities/villagers/sphepherd.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/sphepherd.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/sphepherd.png"
             },
             "minecraft:textures/entities/villagers/toolsmith.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/toolsmith.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/toolsmith.png"
             },
             "minecraft:textures/entities/villagers/weaponsmith.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/doc/resources/assets/minecraft/textures/entities/villagers/weaponsmith.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/doc/resources/assets/minecraft/textures/entities/villagers/weaponsmith.png"
             }
         },
         "SingleItemTexture": {
             "emi:tag/hexcasting/akashic_logs": {
                 "inner": {
                     "pixelated": true,
                     "url": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAAACXBIWXMAAC4jAAAuIwF4pT92AAAAJElEQVQoz2NkwAF+MPzAKs7EQCIY1UAMYMQV3hwMHKOhRD8NAPogBA/DVsDEAAAAAElFTkSuQmCC"
@@ -5602,195 +5602,195 @@
                     "pixelated": true,
                     "url": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAAACXBIWXMAAC4jAAAuIwF4pT92AAAAJElEQVQoz2NkwAF+MPzAKs7EQCIY1UAMYMQV3hwMHKOhRD8NAPogBA/DVsDEAAAAAElFTkSuQmCC"
                 }
             },
             "farmersdelight:skillet": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/farmersdelight/textures/block/skillet.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/farmersdelight/textures/block/skillet.png"
                 }
             },
             "hexcasting:abacus": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/abacus.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/abacus.png"
                 }
             },
             "hexcasting:akashic_bookshelf": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_bookshelf_empty0.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_bookshelf_empty0.png"
                 }
             },
             "hexcasting:akashic_button": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_button.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_button.png"
                 }
             },
             "hexcasting:akashic_connector": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_connector.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_connector.png"
                 }
             },
             "hexcasting:akashic_door": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/akashic_door.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/akashic_door.png"
                 }
             },
             "hexcasting:akashic_leaves1": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_leaves1.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_leaves1.png"
                 }
             },
             "hexcasting:akashic_leaves2": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_leaves2.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_leaves2.png"
                 }
             },
             "hexcasting:akashic_leaves3": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_leaves3.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_leaves3.png"
                 }
             },
             "hexcasting:akashic_log": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_log.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_log.png"
                 }
             },
             "hexcasting:akashic_log_stripped": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_log_stripped.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_log_stripped.png"
                 }
             },
             "hexcasting:akashic_panel": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_panel.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_panel.png"
                 }
             },
             "hexcasting:akashic_planks": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_planks1.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_planks1.png"
                 }
             },
             "hexcasting:akashic_pressure_plate": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_pressure_plate.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_pressure_plate.png"
                 }
             },
             "hexcasting:akashic_record": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_record.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_record.png"
                 }
             },
             "hexcasting:akashic_slab": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_slab.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_slab.png"
                 }
             },
             "hexcasting:akashic_stairs": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_stairs.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_stairs.png"
                 }
             },
             "hexcasting:akashic_tile": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_tile.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_tile.png"
                 }
             },
             "hexcasting:akashic_trapdoor": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_trapdoor_bottom.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_trapdoor_bottom.png"
                 }
             },
             "hexcasting:akashic_wood": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_wood.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_wood.png"
                 }
             },
             "hexcasting:akashic_wood_stripped": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/akashic_wood_stripped.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/akashic_wood_stripped.png"
                 }
             },
             "hexcasting:amethyst_dust": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/amethyst_dust.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/amethyst_dust.png"
                 }
             },
             "hexcasting:amethyst_dust_block": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/amethyst_dust_block.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/amethyst_dust_block.png"
                 }
             },
             "hexcasting:amethyst_sconce": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/amethyst_sconce.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/amethyst_sconce.png"
                 }
             },
             "hexcasting:amethyst_tiles": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/amethyst_tiles.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/amethyst_tiles.png"
                 }
             },
             "hexcasting:ancient_scroll_paper": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/ancient_scroll_paper.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/ancient_scroll_paper.png"
                 }
             },
             "hexcasting:ancient_scroll_paper_lantern": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/ancient_scroll_paper_lantern.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/ancient_scroll_paper_lantern.png"
                 }
             },
             "hexcasting:artifact": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/artifact.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/artifact.png"
                 }
             },
             "hexcasting:artifact_filled": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/artifact_filled.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/artifact_filled.png"
                 }
             },
             "hexcasting:battery": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_0.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_0.png"
                 }
             },
             "hexcasting:charged_amethyst": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/charged_amethyst.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/charged_amethyst.png"
                 }
             },
             "hexcasting:conjured": {
                 "inner": {
                     "pixelated": true,
                     "url": "https://raw.githubusercontent.com/PrismarineJS/minecraft-assets/a14c64362abe4a12c2dfd87f8d1673af9d1b09f4/data/1.18.1/items/amethyst_shard.png"
                 }
@@ -5800,33 +5800,33 @@
                     "pixelated": true,
                     "url": "https://raw.githubusercontent.com/PrismarineJS/minecraft-assets/a14c64362abe4a12c2dfd87f8d1673af9d1b09f4/data/1.18.1/items/amethyst_shard.png"
                 }
             },
             "hexcasting:creative_unlocker": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/creative_unlocker.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/creative_unlocker.png"
                 }
             },
             "hexcasting:cypher": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/cypher.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/cypher.png"
                 }
             },
             "hexcasting:cypher_filled": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/cypher_filled.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/cypher_filled.png"
                 }
             },
             "hexcasting:directrix_redstone": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/redstone_directrix_unpowered_dim_north.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/redstone_directrix_unpowered_dim_north.png"
                 }
             },
             "hexcasting:dye_colorizer_black": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_black-png",
                     "meta": {
                         "animation": {
@@ -5952,15 +5952,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_black.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_black.png"
                 }
             },
             "hexcasting:dye_colorizer_blue": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_blue-png",
                     "meta": {
                         "animation": {
@@ -6086,15 +6086,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_blue.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_blue.png"
                 }
             },
             "hexcasting:dye_colorizer_brown": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_brown-png",
                     "meta": {
                         "animation": {
@@ -6220,15 +6220,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_brown.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_brown.png"
                 }
             },
             "hexcasting:dye_colorizer_cyan": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_cyan-png",
                     "meta": {
                         "animation": {
@@ -6354,15 +6354,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_cyan.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_cyan.png"
                 }
             },
             "hexcasting:dye_colorizer_gray": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_gray-png",
                     "meta": {
                         "animation": {
@@ -6488,15 +6488,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_gray.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_gray.png"
                 }
             },
             "hexcasting:dye_colorizer_green": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_green-png",
                     "meta": {
                         "animation": {
@@ -6622,15 +6622,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_green.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_green.png"
                 }
             },
             "hexcasting:dye_colorizer_light_blue": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_light_blue-png",
                     "meta": {
                         "animation": {
@@ -6756,15 +6756,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_light_blue.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_light_blue.png"
                 }
             },
             "hexcasting:dye_colorizer_light_gray": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_light_gray-png",
                     "meta": {
                         "animation": {
@@ -6890,15 +6890,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_light_gray.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_light_gray.png"
                 }
             },
             "hexcasting:dye_colorizer_lime": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_lime-png",
                     "meta": {
                         "animation": {
@@ -7024,15 +7024,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_lime.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_lime.png"
                 }
             },
             "hexcasting:dye_colorizer_magenta": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_magenta-png",
                     "meta": {
                         "animation": {
@@ -7158,15 +7158,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_magenta.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_magenta.png"
                 }
             },
             "hexcasting:dye_colorizer_orange": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_orange-png",
                     "meta": {
                         "animation": {
@@ -7292,15 +7292,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_orange.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_orange.png"
                 }
             },
             "hexcasting:dye_colorizer_pink": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_pink-png",
                     "meta": {
                         "animation": {
@@ -7426,15 +7426,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_pink.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_pink.png"
                 }
             },
             "hexcasting:dye_colorizer_purple": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_purple-png",
                     "meta": {
                         "animation": {
@@ -7560,15 +7560,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_purple.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_purple.png"
                 }
             },
             "hexcasting:dye_colorizer_red": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_red-png",
                     "meta": {
                         "animation": {
@@ -7694,15 +7694,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_red.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_red.png"
                 }
             },
             "hexcasting:dye_colorizer_white": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_white-png",
                     "meta": {
                         "animation": {
@@ -7828,15 +7828,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_white.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_white.png"
                 }
             },
             "hexcasting:dye_colorizer_yellow": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-dye_yellow-png",
                     "meta": {
                         "animation": {
@@ -7962,243 +7962,243 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_yellow.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/dye_yellow.png"
                 }
             },
             "hexcasting:empty_directrix": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/empty_directrix_dim_z.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/empty_directrix_dim_z.png"
                 }
             },
             "hexcasting:empty_impetus": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/empty_impetus_dim_east.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/empty_impetus_dim_east.png"
                 }
             },
             "hexcasting:focus": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/empty.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/empty.png"
                 }
             },
             "hexcasting:focus_double": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/double.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/double.png"
                 }
             },
             "hexcasting:focus_double_sealed": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/double_sealed.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/double_sealed.png"
                 }
             },
             "hexcasting:focus_empty": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/empty.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/empty.png"
                 }
             },
             "hexcasting:focus_empty_sealed": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/empty_sealed.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/empty_sealed.png"
                 }
             },
             "hexcasting:focus_entity": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/entity.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/entity.png"
                 }
             },
             "hexcasting:focus_entity_sealed": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/entity_sealed.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/entity_sealed.png"
                 }
             },
             "hexcasting:focus_list": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/list.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/list.png"
                 }
             },
             "hexcasting:focus_list_sealed": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/list_sealed.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/list_sealed.png"
                 }
             },
             "hexcasting:focus_pattern": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/pattern.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/pattern.png"
                 }
             },
             "hexcasting:focus_pattern_sealed": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/pattern_sealed.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/pattern_sealed.png"
                 }
             },
             "hexcasting:focus_vec3": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/vec3.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/vec3.png"
                 }
             },
             "hexcasting:focus_vec3_sealed": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/vec3_sealed.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/vec3_sealed.png"
                 }
             },
             "hexcasting:focus_widget": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/widget.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/widget.png"
                 }
             },
             "hexcasting:focus_widget_sealed": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/focus/widget_sealed.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/focus/widget_sealed.png"
                 }
             },
             "hexcasting:impetus_look": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/impetus_look_dim_east.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/impetus_look_dim_east.png"
                 }
             },
             "hexcasting:impetus_rightclick": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/impetus_rightclick_dim_east.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/impetus_rightclick_dim_east.png"
                 }
             },
             "hexcasting:impetus_storedplayer": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/impetus_storedplayer_dim_east.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/impetus_storedplayer_dim_east.png"
                 }
             },
             "hexcasting:jeweler_hammer": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/jeweler_hammer.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/jeweler_hammer.png"
                 }
             },
             "hexcasting:lens": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/lens.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/lens.png"
                 }
             },
             "hexcasting:patchouli_book": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/patchouli_book.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/patchouli_book.png"
                 }
             },
             "hexcasting:phial_large_0": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_0.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_0.png"
                 }
             },
             "hexcasting:phial_large_1": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_1.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_1.png"
                 }
             },
             "hexcasting:phial_large_2": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_2.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_2.png"
                 }
             },
             "hexcasting:phial_large_3": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_3.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_3.png"
                 }
             },
             "hexcasting:phial_large_4": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_4.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_large_4.png"
                 }
             },
             "hexcasting:phial_medium_0": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_0.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_0.png"
                 }
             },
             "hexcasting:phial_medium_1": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_1.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_1.png"
                 }
             },
             "hexcasting:phial_medium_2": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_2.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_2.png"
                 }
             },
             "hexcasting:phial_medium_3": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_3.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_3.png"
                 }
             },
             "hexcasting:phial_medium_4": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_4.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_medium_4.png"
                 }
             },
             "hexcasting:phial_small_0": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_0.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_0.png"
                 }
             },
             "hexcasting:phial_small_1": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_1.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_1.png"
                 }
             },
             "hexcasting:phial_small_2": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_2.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_2.png"
                 }
             },
             "hexcasting:phial_small_3": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_3.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_3.png"
                 }
             },
             "hexcasting:phial_small_4": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_4.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/phial/phial_small_4.png"
                 }
             },
             "hexcasting:pride_colorizer_agender": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_agender-png",
                     "meta": {
                         "animation": {
@@ -8332,15 +8332,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_agender.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_agender.png"
                 }
             },
             "hexcasting:pride_colorizer_aroace": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_aroace-png",
                     "meta": {
                         "animation": {
@@ -8474,15 +8474,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_aroace.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_aroace.png"
                 }
             },
             "hexcasting:pride_colorizer_aromantic": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_aromantic-png",
                     "meta": {
                         "animation": {
@@ -8616,15 +8616,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_aromantic.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_aromantic.png"
                 }
             },
             "hexcasting:pride_colorizer_asexual": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_asexual-png",
                     "meta": {
                         "animation": {
@@ -8758,15 +8758,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_asexual.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_asexual.png"
                 }
             },
             "hexcasting:pride_colorizer_bisexual": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_bisexual-png",
                     "meta": {
                         "animation": {
@@ -8916,15 +8916,15 @@
                                     "time": 10
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_bisexual.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_bisexual.png"
                 }
             },
             "hexcasting:pride_colorizer_demiboy": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_demiboy-png",
                     "meta": {
                         "animation": {
@@ -9074,15 +9074,15 @@
                                     "time": 10
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_demiboy.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_demiboy.png"
                 }
             },
             "hexcasting:pride_colorizer_demigirl": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_demigirl-png",
                     "meta": {
                         "animation": {
@@ -9232,15 +9232,15 @@
                                     "time": 10
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_demigirl.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_demigirl.png"
                 }
             },
             "hexcasting:pride_colorizer_gay": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_gay-png",
                     "meta": {
                         "animation": {
@@ -9374,15 +9374,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_gay.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_gay.png"
                 }
             },
             "hexcasting:pride_colorizer_genderfluid": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_genderfluid-png",
                     "meta": {
                         "animation": {
@@ -9516,15 +9516,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_genderfluid.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_genderfluid.png"
                 }
             },
             "hexcasting:pride_colorizer_genderqueer": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_genderqueer-png",
                     "meta": {
                         "animation": {
@@ -9674,15 +9674,15 @@
                                     "time": 10
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_genderqueer.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_genderqueer.png"
                 }
             },
             "hexcasting:pride_colorizer_intersex": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_intersex-png",
                     "meta": {
                         "animation": {
@@ -9808,15 +9808,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_intersex.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_intersex.png"
                 }
             },
             "hexcasting:pride_colorizer_lesbian": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_lesbian-png",
                     "meta": {
                         "animation": {
@@ -9950,15 +9950,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_lesbian.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_lesbian.png"
                 }
             },
             "hexcasting:pride_colorizer_nonbinary": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_nonbinary-png",
                     "meta": {
                         "animation": {
@@ -10092,15 +10092,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_nonbinary.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_nonbinary.png"
                 }
             },
             "hexcasting:pride_colorizer_pansexual": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_pansexual-png",
                     "meta": {
                         "animation": {
@@ -10250,15 +10250,15 @@
                                     "time": 10
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_pansexual.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_pansexual.png"
                 }
             },
             "hexcasting:pride_colorizer_plural": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_plural-png",
                     "meta": {
                         "animation": {
@@ -10392,15 +10392,15 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_plural.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_plural.png"
                 }
             },
             "hexcasting:pride_colorizer_transgender": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-pride_transgender-png",
                     "meta": {
                         "animation": {
@@ -10550,213 +10550,213 @@
                                     "time": 10
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_transgender.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/pride_transgender.png"
                 }
             },
             "hexcasting:scroll": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_large.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_large.png"
                 }
             },
             "hexcasting:scroll_ancient_large": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_ancient_large.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_ancient_large.png"
                 }
             },
             "hexcasting:scroll_ancient_medium": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_ancient_medium.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_ancient_medium.png"
                 }
             },
             "hexcasting:scroll_ancient_small": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_ancient_small.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_ancient_small.png"
                 }
             },
             "hexcasting:scroll_medium": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_medium.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_medium.png"
                 }
             },
             "hexcasting:scroll_paper": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/scroll_paper.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/scroll_paper.png"
                 }
             },
             "hexcasting:scroll_paper_lantern": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/scroll_paper_lantern.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/scroll_paper_lantern.png"
                 }
             },
             "hexcasting:scroll_pristine_large": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_large.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_large.png"
                 }
             },
             "hexcasting:scroll_pristine_medium": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_medium.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_medium.png"
                 }
             },
             "hexcasting:scroll_pristine_small": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_small.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_small.png"
                 }
             },
             "hexcasting:scroll_small": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_small.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/scroll_pristine_small.png"
                 }
             },
             "hexcasting:slate": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/slate_blank.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/slate_blank.png"
                 }
             },
             "hexcasting:slate_blank": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/slate_blank.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/slate_blank.png"
                 }
             },
             "hexcasting:slate_block": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev22/assets/hexcasting/textures/block/slate_block.png"
+                    "url": "https://hexcasting.hexxy.media/v/0.9.6/1.0.dev24/assets/hexcasting/textures/block/slate_block.png"
                 }
             },
             "hexcasting:slate_written": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/slate_written.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/slate_written.png"
                 }
             },
             "hexcasting:spellbook": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/empty.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/empty.png"
                 }
             },
             "hexcasting:spellbook_double": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/double.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/double.png"
                 }
             },
             "hexcasting:spellbook_double_sealed": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/double_sealed.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/double_sealed.png"
                 }
             },
             "hexcasting:spellbook_empty": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/empty.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/empty.png"
                 }
             },
             "hexcasting:spellbook_empty_sealed": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/empty_sealed.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/empty_sealed.png"
                 }
             },
             "hexcasting:spellbook_entity": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/entity.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/entity.png"
                 }
             },
             "hexcasting:spellbook_entity_sealed": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/entity_sealed.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/entity_sealed.png"
                 }
             },
             "hexcasting:spellbook_list": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/list.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/list.png"
                 }
             },
             "hexcasting:spellbook_list_sealed": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/list_sealed.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/list_sealed.png"
                 }
             },
             "hexcasting:spellbook_pattern": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/pattern.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/pattern.png"
                 }
             },
             "hexcasting:spellbook_pattern_sealed": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/pattern_sealed.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/pattern_sealed.png"
                 }
             },
             "hexcasting:spellbook_vec3": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/vec3.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/vec3.png"
                 }
             },
             "hexcasting:spellbook_vec3_sealed": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/vec3_sealed.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/vec3_sealed.png"
                 }
             },
             "hexcasting:spellbook_widget": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/widget.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/widget.png"
                 }
             },
             "hexcasting:spellbook_widget_sealed": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/widget_sealed.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/spellbook/widget_sealed.png"
                 }
             },
             "hexcasting:sub_sandwich": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/sub_sandwich.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/sub_sandwich.png"
                 }
             },
             "hexcasting:trinket": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/trinket.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/trinket.png"
                 }
             },
             "hexcasting:trinket_filled": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/trinket_filled.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/trinket_filled.png"
                 }
             },
             "hexcasting:uuid_colorizer": {
                 "inner": {
                     "css_class": "texture-hexcasting-textures-item-colorizer-uuid-png",
                     "meta": {
                         "animation": {
@@ -10842,79 +10842,79 @@
                                     "time": 1
                                 }
                             ],
                             "interpolate": false
                         }
                     },
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/uuid.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/colorizer/uuid.png"
                 }
             },
             "hexcasting:wand_acacia": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/acacia.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/acacia.png"
                 }
             },
             "hexcasting:wand_akashic": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/akashic.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/akashic.png"
                 }
             },
             "hexcasting:wand_birch": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/birch.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/birch.png"
                 }
             },
             "hexcasting:wand_bosnia": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/bosnia.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/bosnia.png"
                 }
             },
             "hexcasting:wand_crimson": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/crimson.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/crimson.png"
                 }
             },
             "hexcasting:wand_dark_oak": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/dark_oak.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/dark_oak.png"
                 }
             },
             "hexcasting:wand_jungle": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/jungle.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/jungle.png"
                 }
             },
             "hexcasting:wand_oak": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/oak.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/oak.png"
                 }
             },
             "hexcasting:wand_old": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/old.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/old.png"
                 }
             },
             "hexcasting:wand_spruce": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/spruce.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/spruce.png"
                 }
             },
             "hexcasting:wand_warped": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/87f3e3156d11efa2c076aff8fdd4c9ee68936769/Common/src/main/resources/assets/hexcasting/textures/item/wands/warped.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexMod/f604a19b9b246638f62931a3c9502249d64223a9/Common/src/main/resources/assets/hexcasting/textures/item/wands/warped.png"
                 }
             }
         }
     }
 }
```

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/hexcasting.patterns.hexdoc.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/hexcasting.patterns.hexdoc.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/blockstates/skillet.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/blockstates/skillet.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/models/block/skillet.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/models/block/skillet.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/models/item/skillet.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/farmersdelight/models/item/skillet.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_bookshelf.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_bookshelf.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_button.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_button.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_door.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_door.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_stairs.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_stairs.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_trapdoor.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/akashic_trapdoor.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/directrix_redstone.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/directrix_redstone.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/empty_directrix.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/empty_directrix.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/empty_impetus.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/empty_impetus.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/impetus_look.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/impetus_look.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/impetus_rightclick.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/impetus_rightclick.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/impetus_storedplayer.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/impetus_storedplayer.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/slate.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/blockstates/slate.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/en_us.flatten.json5` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/zh_cn.flatten.json5`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2727272727272727%*

 * *Differences: {"'block.hexcasting.slate'": "'空白石板'",*

 * * "'hexdoc.hexcasting.description'": "'咒术之书，辑录合一。'",*

 * * "'hexdoc.hexcasting.title'": "'咒术之书'",*

 * * "'hexdoc.pages.hexcasting.brainsweep.description'": "'书中显示如下事物的意识剥离配方：'",*

 * * "'hexdoc.pages.hexcasting.crafting_multi.description'": "'书中显示如下事物的合成配方：'",*

 * * "'hexdoc.pages.hexcasting.crafting_multi.separator'": "'、'",*

 * * "'hexdoc.pattern.hide'": "'点击以隐藏图案'",*

 * * "'hexdoc.pattern.not_supported'": "'浏览器不支持图案的可视化。图案代码见此：{}'",*

 * * "'hexdoc.pattern.paused'": "'暂停'",*

 * * "'hexdoc.pattern.show'": "'点 […]*

```diff
@@ -1,17 +1,19 @@
 {
-    "block.hexcasting.slate": "Blank Slate",
-    "hexdoc.hexcasting.description": "The Hex Book, all in one place.",
-    "hexdoc.hexcasting.title": "Hex Book",
-    "hexdoc.pages.hexcasting.brainsweep.description": "Depicted in the book: A mind-flaying recipe producing the",
+    "block.hexcasting.slate": "\u7a7a\u767d\u77f3\u677f",
+    "hexdoc.hexcasting.description": "\u5492\u672f\u4e4b\u4e66\uff0c\u8f91\u5f55\u5408\u4e00\u3002",
+    "hexdoc.hexcasting.title": "\u5492\u672f\u4e4b\u4e66",
+    "hexdoc.pages.hexcasting.brainsweep.description": "\u4e66\u4e2d\u663e\u793a\u5982\u4e0b\u4e8b\u7269\u7684\u610f\u8bc6\u5265\u79bb\u914d\u65b9\uff1a",
     "hexdoc.pages.hexcasting.brainsweep.separator": "",
-    "hexdoc.pattern.hide": "Click to hide spell",
+    "hexdoc.pages.hexcasting.crafting_multi.description": "\u4e66\u4e2d\u663e\u793a\u5982\u4e0b\u4e8b\u7269\u7684\u5408\u6210\u914d\u65b9\uff1a",
+    "hexdoc.pages.hexcasting.crafting_multi.separator": "\u3001",
+    "hexdoc.pattern.hide": "\u70b9\u51fb\u4ee5\u9690\u85cf\u56fe\u6848",
     "hexdoc.pattern.multiplier": "${speedScale()}x",
-    "hexdoc.pattern.not_supported": "Your browser does not support visualizing patterns. Pattern code: {}",
-    "hexdoc.pattern.paused": "Paused",
-    "hexdoc.pattern.show": "Click to show spell",
-    "hexdoc.villager_requirements.any": "Villager must be a {level} or higher",
-    "hexdoc.villager_requirements.professional": "Villager must be a {level} {profession} or higher",
-    "tag.item.c.brown_dye": "Brown Dyes",
-    "tag.item.c.glowstone_dusts": "Glowstone Dusts",
-    "tag.item.c.wood_sticks": "Wood Sticks"
+    "hexdoc.pattern.not_supported": "\u6d4f\u89c8\u5668\u4e0d\u652f\u6301\u56fe\u6848\u7684\u53ef\u89c6\u5316\u3002\u56fe\u6848\u4ee3\u7801\u89c1\u6b64\uff1a{}",
+    "hexdoc.pattern.paused": "\u6682\u505c",
+    "hexdoc.pattern.show": "\u70b9\u51fb\u4ee5\u663e\u793a\u56fe\u6848",
+    "item.minecraft.amethyst_shard": "\u7d2b\u6c34\u6676\u788e\u7247",
+    "item.minecraft.budding_amethyst": "\u7d2b\u6c34\u6676\u6bcd\u5ca9",
+    "key.jump": "\u7a7a\u683c",
+    "key.sneak": "\u5de6Shift",
+    "key.use": "\u53f3\u952e"
 }
```

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/en_us.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/en_us.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/ru_ru.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/ru_ru.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/zh_cn.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/lang/zh_cn.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_record.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/akashic_record.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/amethyst_sconce.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/amethyst_sconce.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/cube_half_mirrored.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/block/cube_half_mirrored.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/battery.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/battery.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/focus.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/models/item/spellbook.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_sconce.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/amethyst_sconce.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/cracked_calcite.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/cracked_calcite.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_button.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_button.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_pressure_plate.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_pressure_plate.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_slab.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_slab.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_stairs.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/edified_stairs.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/other3.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/other3.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/vec3.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/vec3.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget1.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget1.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget2.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget2.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget3.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget3.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget4.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/akashic/bookshelf/widget4.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/horiz_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/horiz_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/vert_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/empty/vert_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_powered_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_powered_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_powered_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_powered_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_unpowered_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_unpowered_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_unpowered_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/down_unpowered_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_powered_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_powered_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_powered_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_powered_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_unpowered_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_unpowered_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_unpowered_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/left_unpowered_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_powered_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_powered_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_powered_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_powered_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_unpowered_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_unpowered_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_unpowered_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/right_unpowered_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_powered_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_powered_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_powered_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_powered_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_unpowered_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_unpowered_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_unpowered_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/directrix/redstone/up_unpowered_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/atlas.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/atlas.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/down_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/down_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/down_empty_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/down_empty_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/down_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/down_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/front_empty_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/front_empty_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_empty_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_empty_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_empty_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_empty_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/left_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/look_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/look_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/look_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/look_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/right_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/right_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/right_empty_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/right_empty_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/right_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/right_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/rightclick_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/rightclick_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/rightclick_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/rightclick_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/something.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/something.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/storedplayer_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/storedplayer_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/storedplayer_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/storedplayer_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/up_dim.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/up_dim.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/up_empty_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/up_empty_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/up_lit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/block/impetus/up_lit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/scroll_ancient_large.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/scroll_ancient_large.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/scroll_ancient_medium.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/scroll_ancient_medium.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/scroll_large.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/entity/scroll_large.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/brainsweep.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/brainsweep.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/brainsweep_jei.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/brainsweep_jei.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/edify.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/edify.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/edify_jei.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/edify_jei.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/patchi_filler.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/patchi_filler.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/phial.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/phial.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/phial_jei.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/phial_jei.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/scroll.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/scroll.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/scroll_ancient.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/scroll_ancient.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/slate.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/slate.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/entries/spell_circle.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/entries/spell_circle.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/hexdoc/brainsweep.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/gui/hexdoc/brainsweep.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/artifact.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/artifact.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/artifact_filled.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/artifact_filled.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/lens.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/lens.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/sub_sandwich.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/sub_sandwich.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_black.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_black.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_blue.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_blue.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_brown.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_brown.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_cyan.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_cyan.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_gray.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_gray.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_green.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_green.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_light_blue.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_light_blue.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_light_gray.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_light_gray.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_lime.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_lime.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_magenta.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_magenta.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_orange.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_orange.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_pink.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_pink.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_purple.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_purple.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_red.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_red.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_white.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_white.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_yellow.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/dye_yellow.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_agender.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_agender.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_aroace.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_aroace.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_aromantic.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_aromantic.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_asexual.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_asexual.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_bisexual.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_bisexual.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_demiboy.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_demiboy.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_demigirl.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_demigirl.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_gay.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_gay.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_genderfluid.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_genderfluid.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_genderqueer.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_genderqueer.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_intersex.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_intersex.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_lesbian.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_lesbian.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_nonbinary.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_nonbinary.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_pansexual.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_pansexual.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_plural.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_plural.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_transgender.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/pride_transgender.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/uuid.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/colorizer/uuid.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/widget.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/widget.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/widget_sealed.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/focus/widget_sealed.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/double.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/double.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/double_sealed.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/double_sealed.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/empty.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/empty.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/empty_sealed.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/empty_sealed.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/entity.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/entity.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/entity_sealed.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/entity_sealed.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/list.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/list.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/list_sealed.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/list_sealed.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/pattern.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/pattern.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/pattern_sealed.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/pattern_sealed.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/vec3.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/vec3.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/vec3_sealed.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/vec3_sealed.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/widget.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/widget.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/widget_sealed.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/spellbook/widget_sealed.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/crimson.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/crimson.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/warped.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/item/wands/warped.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/cloud.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/hexcasting/textures/particle/cloud.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/allay.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/allay.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/armorer.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/armorer.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/butcher.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/butcher.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/cartographer.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/cartographer.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/cleric.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/cleric.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/farmer.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/farmer.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/fisherman.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/fisherman.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/fletcher.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/fletcher.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/leatherworker.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/leatherworker.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/librarian.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/librarian.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/mason.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/mason.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/nitwit.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/nitwit.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/none.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/none.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/sphepherd.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/sphepherd.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/toolsmith.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/toolsmith.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/weaponsmith.png` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/assets/minecraft/textures/entities/villagers/weaponsmith.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/book.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/book.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/basics/couldnt_cast.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/basics/couldnt_cast.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/basics/start_to_see.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/basics/start_to_see.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/101.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/101.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/mishaps.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/mishaps.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/mishaps2.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/mishaps2.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/stack.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/stack.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/vectors.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/casting/vectors.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/akashiclib.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/akashiclib.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/brainsweeping.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/brainsweeping.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/directrix.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/directrix.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/impetus.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/impetus.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/spellcircles.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/greatwork/spellcircles.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/interop/gravity.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/interop/gravity.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/interop/pehkui.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/interop/pehkui.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/amethyst.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/amethyst.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/decoration.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/decoration.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/edified.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/edified.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/focus.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/focus.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/hexcasting.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/hexcasting.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/phials.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/phials.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/pigments.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/pigments.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/scroll.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/scroll.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/slate.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/slate.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/staff.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/items/staff.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/advanced_math.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/advanced_math.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/akashic_patterns.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/akashic_patterns.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/basics.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/basics.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/circle.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/circle.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/consts.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/consts.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/entities.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/entities.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/lists.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/lists.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/logic.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/logic.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/math.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/math.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/meta.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/meta.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/numbers.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/numbers.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/patterns_as_iotas.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/patterns_as_iotas.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/readers_guide.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/readers_guide.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/readwrite.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/readwrite.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/sets.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/sets.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/stackmanip.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/stackmanip.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/create_lava.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/create_lava.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/flight.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/flight.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/greater_sentinel.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/greater_sentinel.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/make_battery.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/make_battery.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/teleport.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/teleport.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/weather_manip.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/weather_manip.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/zeniths.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/great_spells/zeniths.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/basic.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/basic.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/blockworks.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/blockworks.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/hexcasting.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/hexcasting.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/nadirs.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/nadirs.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/sentinels.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/spells/sentinels.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/ageing_scroll_paper_lantern.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/ageing_scroll_paper_lantern.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/ancient_scroll_paper.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/ancient_scroll_paper.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/jeweler_hammer.json` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_export/generated/data/hexcasting/recipes/jeweler_hammer.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/hexcasting.js.jinja` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/hexcasting.js.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     case "e":
       return 5;
     default:
       return -1;
   }
 }
 
-function initializeElem(canvas) {
+export function initializeElem(canvas) {
   const str = canvas.dataset.string;
   let angle = startAngle(canvas.dataset.start);
   const perWorld = canvas.dataset.perWorld === "True";
 
   // build geometry
   const points = [[0, 0]];
   let lastPoint = points[0];
@@ -237,23 +237,23 @@
       }
       ev.preventDefault();
     });
   }
 }
 
 
-function hookLoad(elem) {
+export function hookLoad(elem) {
   let init = false;
   const canvases = elem.querySelectorAll("canvas");
-  elem.addEventListener("toggle", () => {
+  elem.addEventListener("toggle", (a) => {
     if (!init) {
       canvases.forEach(initializeElem);
       init = true;
     }
-  });
+  }, {once: true});
 }
 
 document.addEventListener("DOMContentLoaded", () => {
   document.querySelectorAll(".details-collapsible").forEach(hookLoad);
 
   function tick(prevTime, time) {
     const dt = time - prevTime;
```

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/ingredients/hexcasting/brainsweepee/villager.html.jinja` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/ingredients/hexcasting/brainsweepee/villager.html.jinja`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/_templates/recipes/hexcasting/brainsweep.html.jinja` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/_templates/recipes/hexcasting/brainsweep.html.jinja`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/book/recipes.py` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/book/recipes.py`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/book/page/abstract_pages.py` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/book/page/abstract_pages.py`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/book/page/pages.py` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/book/page/pages.py`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/src/hexdoc_hexcasting/utils/pattern.py` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/src/hexdoc_hexcasting/utils/pattern.py`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/.gitignore` & `hexdoc_hexcasting-0.9.6.1.0.dev24/.gitignore`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/LICENSE.txt` & `hexdoc_hexcasting-0.9.6.1.0.dev24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/pyproject.toml` & `hexdoc_hexcasting-0.9.6.1.0.dev24/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 [tool.hatch.version]
 scheme = "gradle"
 source = "gradle-properties"
 py-path = "doc/src/hexdoc_hexcasting/__version__.py"
 
 [tool.hatch.metadata.hooks.gradle-properties]
 dependencies = [
-    "hexdoc~=1!0.1.0a5",
+    "hexdoc~=1!0.1.0a10",
     { package="hexdoc-minecraft", op="~=", py-version="1.0.dev", key="minecraftVersion" },
 ]
 
 [tool.hatch.metadata.hooks.gradle-properties.optional-dependencies]
 dev = [
     "ruff~=0.1.4",
 ]
```

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/doc/README.md` & `hexdoc_hexcasting-0.9.6.1.0.dev24/doc/README.md`

 * *Files identical despite different names*

### Comparing `hexdoc_hexcasting-0.9.6.1.0.dev22/PKG-INFO` & `hexdoc_hexcasting-0.9.6.1.0.dev24/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hexdoc-hexcasting
-Version: 0.9.6.1.0.dev22
+Version: 0.9.6.1.0.dev24
 Summary: Hex Casting web book.
 Project-URL: Homepage, https://gamma-delta.github.io/HexMod/
 Project-URL: Source, https://github.com/gamma-delta/HexMod/
 Author: object-Object, Alwinfy
 License: MIT License
         
         Copyright (c) 2023 object-Object, gamma-delta
@@ -26,15 +26,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE.txt
 Keywords: hexdoc
 Requires-Python: >=3.11
 Requires-Dist: hexdoc-minecraft~=1.18.2.1.0.dev0
-Requires-Dist: hexdoc~=1!0.1.0a5
+Requires-Dist: hexdoc~=1!0.1.0a10
 Provides-Extra: dev
 Requires-Dist: ruff~=0.1.4; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # hexdoc-hexcasting
 
 Python web book docgen and [hexdoc](https://pypi.org/project/hexdoc) plugin for Hex Casting.
```

