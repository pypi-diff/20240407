# Comparing `tmp/craftax-1.2.0.tar.gz` & `tmp/craftax-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craftax-1.2.0.tar", last modified: Tue Mar 26 16:30:34 2024, max compression
+gzip compressed data, was "craftax-1.3.0.tar", last modified: Sun Apr  7 21:37:45 2024, max compression
```

## Comparing `craftax-1.2.0.tar` & `craftax-1.3.0.tar`

### file list

```diff
@@ -1,273 +1,262 @@
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.664976 craftax-1.2.0/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1059 2024-03-26 15:44:42.000000 craftax-1.2.0/LICENSE
--rw-rw-r--   0 mikey     (1000) mikey     (1000)       73 2024-03-26 16:11:15.000000 craftax-1.2.0/MANIFEST.in
--rw-r--r--   0 mikey     (1000) mikey     (1000)     8981 2024-03-26 16:30:34.664976 craftax-1.2.0/PKG-INFO
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     8096 2024-03-26 16:27:13.000000 craftax-1.2.0/README.md
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.656977 craftax-1.2.0/craftax/
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.656977 craftax-1.2.0/craftax/craftax/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/__init__.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.660977 craftax-1.2.0/craftax/craftax/assets/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      607 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/0.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1827 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/1.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1501 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/2.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1559 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/3.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1533 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/4.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1518 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/5.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1567 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/6.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1538 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/7.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1506 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/8.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1535 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/9.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1825 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/arrow-down.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1731 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/arrow-left.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1752 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/arrow-right.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1833 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/arrow-up.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      603 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/arrow_fire_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      602 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/arrow_ice_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      652 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/bat.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      719 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/book.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      654 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/boots_fire_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      652 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/boots_ice_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      693 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/bow.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      953 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/chest.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/chestplate_fire_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/chestplate_ice_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      866 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/coal.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1983 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/cow.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      621 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/dagger.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5735 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/debug-2.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5762 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/debug-3.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5761 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/debug.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)       84 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/debug_tile.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      996 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/deep_thing.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      790 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/dexterity.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      839 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/diamond.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      605 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/diamond_boots.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      685 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/diamond_chestplate.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      642 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/diamond_helmet.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      609 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/diamond_pants.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      733 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/diamond_pickaxe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      714 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/diamond_sword.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2492 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/drink.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1087 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/enchantment_table_fire.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1092 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/enchantment_table_ice.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2213 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/energy.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2449 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/fence.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      674 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/fire_elemental.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      710 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/fire_grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      959 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/fire_stone.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1140 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/fire_tree.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/fireball.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2292 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/food.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1141 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/fountain.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      723 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/frost_troll.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      910 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/furnace.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      860 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/gnome_archer.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      847 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/gnome_warrior.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      691 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1099 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/grave.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1210 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/grave2.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1161 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/grave3.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      741 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/gravel.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2721 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/health.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      666 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/helmet_fire_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      666 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/helmet_ice_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      689 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/ice_elemental.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      719 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/ice_grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      994 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/ice_shrub.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      668 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/iceball.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      933 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/intelligence.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1048 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/iron.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      613 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/iron_boots.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      681 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/iron_chestplate.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      642 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/iron_helmet.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      608 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/iron_pants.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2354 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/iron_pickaxe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2390 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/iron_sword.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      839 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/knight.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      889 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/knight_archer.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      737 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/kobold.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/ladder_down.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      855 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/ladder_down_blocked.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      612 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/ladder_up.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2130 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/lava.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      755 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/leaves.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      758 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/lizard.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      745 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/log.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      695 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/mana.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1150 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/necromancer.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1128 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/necromancer_vulnerable.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      769 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/orc_mage.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      777 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/orc_soldier.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      709 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/pants_fire_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      702 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/pants_ice_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     7488 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/path.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      325 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/path_moss.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      809 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/pigman.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2154 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/plant-ripe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2511 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/plant-young.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2080 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/plant.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      219 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/plant_on_grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6186 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/player-down.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6195 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/player-left.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6212 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/player-right.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6590 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/player-sleep.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6144 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/player-up.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      813 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/player.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      715 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/potion_blue.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      723 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/potion_cyan.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      705 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/potion_green.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      715 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/potion_pink.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      708 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/potion_red.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      707 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/potion_yellow.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      245 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/ripe_plant_on_grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1110 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/ruby.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/sand.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1817 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/sapling.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      957 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/sapphire.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5993 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/skeleton.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      673 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/slimeball.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/snail.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      668 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/spider.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1219 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/stalagmite.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     7242 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/stone.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2345 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/stone_pickaxe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2429 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/stone_sword.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/strength.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      613 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/sword_fire_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      620 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/sword_ice_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      885 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/table.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)  1769538 2024-03-26 15:46:49.000000 craftax-1.2.0/craftax/craftax/assets/texture_cache.pbz2
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      615 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/torch_in_inventory.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1197 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/torch_on_path.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     7782 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/tree.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      698 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/troll.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2127 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/unknown.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      126 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/wall.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      163 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/wall2.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      198 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/wall_moss.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2198 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/water.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1577 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/wood.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2045 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/wood_pickaxe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2453 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/wood_sword.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      718 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/xp.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2089 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/assets/zombie.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    34412 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/constants.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2909 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/craftax_state.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.660977 craftax-1.2.0/craftax/craftax/envs/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/envs/__init__.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      484 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/envs/common.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     3079 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/envs/craftax_pixels_env.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     3720 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/envs/craftax_symbolic_env.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)   106092 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/game_logic.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6938 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/play_craftax.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    41178 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/renderer.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.660977 craftax-1.2.0/craftax/craftax/util/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/util/__init__.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    11631 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/util/game_logic_utils.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      813 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/util/maths_utils.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2382 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/util/noise.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.660977 craftax-1.2.0/craftax/craftax/world_gen/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/world_gen/__init__.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    24490 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/world_gen/world_gen.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     9213 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax/world_gen/world_gen_configs.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.660977 craftax-1.2.0/craftax/craftax_classic/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/__init__.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.664976 craftax-1.2.0/craftax/craftax_classic/assets/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1827 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/1.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1501 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/2.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1559 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/3.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1533 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/4.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1518 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/5.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1567 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/6.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1538 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/7.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1506 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/8.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1535 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/9.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1825 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/arrow-down.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1731 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/arrow-left.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1752 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/arrow-right.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1833 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/arrow-up.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      866 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/coal.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1983 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/cow.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5735 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/debug-2.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5762 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/debug-3.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5761 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/debug.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)       84 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/debug_tile.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      839 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/diamond.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2492 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/drink.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2213 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/energy.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2449 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/fence.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2292 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/food.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      910 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/furnace.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      691 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2721 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/health.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1048 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/iron.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2354 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/iron_pickaxe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2390 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/iron_sword.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2130 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/lava.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      755 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/leaves.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      745 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/log.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     7488 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/path.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2154 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/plant-ripe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2511 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/plant-young.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2080 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/plant.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      219 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/plant_on_grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6186 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/player-down.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6195 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/player-left.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6212 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/player-right.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6590 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/player-sleep.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6144 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/player-up.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      813 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/player.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      245 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/ripe_plant_on_grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/sand.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1817 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/sapling.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5993 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/skeleton.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     7242 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/stone.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2345 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/stone_pickaxe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2429 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/stone_sword.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      885 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/table.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)  1262198 2024-03-26 15:51:57.000000 craftax-1.2.0/craftax/craftax_classic/assets/texture_cache_classic.pbz2
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     7782 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/tree.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2127 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/unknown.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2198 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/water.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1577 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/wood.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2045 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/wood_pickaxe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2453 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/wood_sword.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2089 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/assets/zombie.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    13946 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/constants.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.664976 craftax-1.2.0/craftax/craftax_classic/envs/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/envs/__init__.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      505 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/envs/common.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     3171 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/envs/craftax_pixels_env.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2053 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/envs/craftax_state.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     3819 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/envs/craftax_symbolic_env.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    58163 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/game_logic.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     4387 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/play_craftax_classic.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    24401 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/renderer.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.664976 craftax-1.2.0/craftax/craftax_classic/util/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/util/__init__.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2382 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/util/noise.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    10956 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/craftax_classic/world_gen.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.664976 craftax-1.2.0/craftax/environment_base/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/environment_base/__init__.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     3107 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/environment_base/environment_no_auto_reset.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      290 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/environment_base/util.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     7389 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/environment_base/wrappers.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.664976 craftax-1.2.0/craftax/logz/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/logz/__init__.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2744 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/logz/batch_logging.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.664976 craftax-1.2.0/craftax/models/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/models/__init__.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     8066 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/models/actor_critic.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1592 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/models/icm.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      486 2024-03-26 16:11:15.000000 craftax-1.2.0/craftax/models/world_model.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    29307 2024-03-26 16:14:20.000000 craftax-1.2.0/craftax/ppo.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    19555 2024-03-26 16:14:19.000000 craftax-1.2.0/craftax/ppo_rnn.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:30:34.664976 craftax-1.2.0/craftax.egg-info/
--rw-r--r--   0 mikey     (1000) mikey     (1000)     8981 2024-03-26 16:30:34.000000 craftax-1.2.0/craftax.egg-info/PKG-INFO
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     9712 2024-03-26 16:30:34.000000 craftax-1.2.0/craftax.egg-info/SOURCES.txt
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        1 2024-03-26 16:30:34.000000 craftax-1.2.0/craftax.egg-info/dependency_links.txt
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      147 2024-03-26 16:30:34.000000 craftax-1.2.0/craftax.egg-info/entry_points.txt
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      116 2024-03-26 16:30:34.000000 craftax-1.2.0/craftax.egg-info/requires.txt
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        8 2024-03-26 16:30:34.000000 craftax-1.2.0/craftax.egg-info/top_level.txt
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1058 2024-03-26 16:27:13.000000 craftax-1.2.0/pyproject.toml
--rw-rw-r--   0 mikey     (1000) mikey     (1000)       38 2024-03-26 16:30:34.664976 craftax-1.2.0/setup.cfg
+drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.926173 craftax-1.3.0/
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1059 2024-03-06 09:23:28.000000 craftax-1.3.0/LICENSE
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)       73 2024-03-27 11:54:45.000000 craftax-1.3.0/MANIFEST.in
+-rw-r--r--   0 mans4835  (1001) mans4835  (1001)     8674 2024-04-07 21:37:45.926173 craftax-1.3.0/PKG-INFO
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7789 2024-04-07 21:36:12.000000 craftax-1.3.0/README.md
+drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.898172 craftax-1.3.0/craftax/
+drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.898172 craftax-1.3.0/craftax/craftax/
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/__init__.py
+drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.914173 craftax-1.3.0/craftax/craftax/assets/
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      607 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/0.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1827 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/1.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1501 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/2.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1559 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/3.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1533 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/4.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1518 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/5.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1567 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/6.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1538 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/7.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1506 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/8.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1535 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/9.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1825 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/arrow-down.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1731 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/arrow-left.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1752 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/arrow-right.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1833 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/arrow-up.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      603 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/arrow_fire_enchantment.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      602 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/arrow_ice_enchantment.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      652 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/bat.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      719 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/book.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      654 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/boots_fire_enchantment.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      652 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/boots_ice_enchantment.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      693 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/bow.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      953 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/chest.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      670 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/chestplate_fire_enchantment.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      670 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/chestplate_ice_enchantment.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      866 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/coal.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1983 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/cow.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      621 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/dagger.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5735 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/debug-2.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5762 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/debug-3.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5761 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/debug.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)       84 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/debug_tile.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      996 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/deep_thing.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      790 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/dexterity.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      839 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/diamond.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      605 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/diamond_boots.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      685 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/diamond_chestplate.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      642 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/diamond_helmet.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      609 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/diamond_pants.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      733 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/diamond_pickaxe.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      714 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/diamond_sword.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2492 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/drink.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1087 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/enchantment_table_fire.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1092 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/enchantment_table_ice.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2213 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/energy.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2449 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/fence.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      674 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/fire_elemental.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      710 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/fire_grass.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      959 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/fire_stone.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1140 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/fire_tree.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      670 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/fireball.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2292 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/food.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1141 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/fountain.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      723 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/frost_troll.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      910 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/furnace.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      860 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/gnome_archer.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      847 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/gnome_warrior.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      691 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/grass.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1099 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/grave.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1210 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/grave2.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1161 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/grave3.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      741 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/gravel.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2721 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/health.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      666 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/helmet_fire_enchantment.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      666 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/helmet_ice_enchantment.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      689 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ice_elemental.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      719 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ice_grass.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      994 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ice_shrub.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      668 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iceball.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      933 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/intelligence.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1048 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iron.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      613 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iron_boots.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      681 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iron_chestplate.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      642 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iron_helmet.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      608 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iron_pants.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2354 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iron_pickaxe.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2390 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iron_sword.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      839 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/knight.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      889 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/knight_archer.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      737 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/kobold.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      729 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ladder_down.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      855 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ladder_down_blocked.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      612 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ladder_up.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2130 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/lava.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      755 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/leaves.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      758 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/lizard.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      745 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/log.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      695 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/mana.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1150 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/necromancer.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1128 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/necromancer_vulnerable.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      769 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/orc_mage.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      777 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/orc_soldier.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      709 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/pants_fire_enchantment.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      702 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/pants_ice_enchantment.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7488 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/path.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      325 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/path_moss.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      809 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/pigman.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2154 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/plant-ripe.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2511 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/plant-young.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2080 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/plant.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      219 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/plant_on_grass.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6186 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/player-down.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6195 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/player-left.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6212 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/player-right.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6590 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/player-sleep.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6144 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/player-up.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      813 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/player.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      715 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/potion_blue.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      723 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/potion_cyan.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      705 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/potion_green.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      715 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/potion_pink.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      708 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/potion_red.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      707 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/potion_yellow.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      245 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ripe_plant_on_grass.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1110 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ruby.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      729 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/sand.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1817 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/sapling.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      957 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/sapphire.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5993 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/skeleton.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      673 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/slimeball.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      729 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/snail.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      668 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/spider.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1219 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/stalagmite.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7242 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/stone.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2345 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/stone_pickaxe.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2429 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/stone_sword.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      670 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/strength.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      613 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/sword_fire_enchantment.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      620 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/sword_ice_enchantment.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      885 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/table.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)  1769538 2024-03-27 11:45:23.000000 craftax-1.3.0/craftax/craftax/assets/texture_cache.pbz2
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      615 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/torch_in_inventory.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1197 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/torch_on_path.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7782 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/tree.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      698 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/troll.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2127 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/unknown.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      126 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/wall.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      163 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/wall2.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      198 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/wall_moss.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2198 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/water.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1577 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/wood.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2045 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/wood_pickaxe.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2453 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/wood_sword.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      718 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/xp.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2089 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/zombie.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    34412 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/constants.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2909 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/craftax_state.py
+drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.914173 craftax-1.3.0/craftax/craftax/envs/
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/envs/__init__.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      484 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/envs/common.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     3079 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/envs/craftax_pixels_env.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     3720 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/envs/craftax_symbolic_env.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)   106092 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/game_logic.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6938 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/play_craftax.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    41178 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/renderer.py
+drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.914173 craftax-1.3.0/craftax/craftax/util/
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/util/__init__.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    11631 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/util/game_logic_utils.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      813 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/util/maths_utils.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2382 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/util/noise.py
+drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.914173 craftax-1.3.0/craftax/craftax/world_gen/
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/world_gen/__init__.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    24490 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/world_gen/world_gen.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     9213 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/world_gen/world_gen_configs.py
+drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.918172 craftax-1.3.0/craftax/craftax_classic/
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/__init__.py
+drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.922172 craftax-1.3.0/craftax/craftax_classic/assets/
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1827 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/1.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1501 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/2.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1559 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/3.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1533 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/4.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1518 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/5.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1567 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/6.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1538 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/7.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1506 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/8.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1535 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/9.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1825 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/arrow-down.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1731 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/arrow-left.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1752 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/arrow-right.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1833 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/arrow-up.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      866 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/coal.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1983 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/cow.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5735 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/debug-2.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5762 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/debug-3.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5761 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/debug.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)       84 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/debug_tile.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      839 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/diamond.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2492 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/drink.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2213 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/energy.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2449 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/fence.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2292 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/food.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      910 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/furnace.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      691 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/grass.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2721 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/health.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1048 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/iron.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2354 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/iron_pickaxe.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2390 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/iron_sword.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2130 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/lava.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      755 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/leaves.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      745 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/log.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7488 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/path.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2154 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/plant-ripe.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2511 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/plant-young.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2080 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/plant.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      219 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/plant_on_grass.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6186 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/player-down.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6195 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/player-left.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6212 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/player-right.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6590 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/player-sleep.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6144 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/player-up.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      813 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/player.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      245 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/ripe_plant_on_grass.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      729 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/sand.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1817 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/sapling.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5993 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/skeleton.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7242 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/stone.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2345 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/stone_pickaxe.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2429 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/stone_sword.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      885 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/table.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7782 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/tree.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2127 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/unknown.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2198 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/water.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1577 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/wood.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2045 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/wood_pickaxe.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2453 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/wood_sword.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2089 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/zombie.png
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    13946 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax_classic/constants.py
+drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.926173 craftax-1.3.0/craftax/craftax_classic/envs/
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/envs/__init__.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      505 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/envs/common.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     3171 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/envs/craftax_pixels_env.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2053 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/envs/craftax_state.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     3819 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/envs/craftax_symbolic_env.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    58163 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax_classic/game_logic.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     4387 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax_classic/play_craftax_classic.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    24401 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax_classic/renderer.py
+drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.926173 craftax-1.3.0/craftax/craftax_classic/util/
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/util/__init__.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2382 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/util/noise.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    10956 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax_classic/world_gen.py
+drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.926173 craftax-1.3.0/craftax/environment_base/
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/environment_base/__init__.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     3107 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/environment_base/environment_no_auto_reset.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      290 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/environment_base/util.py
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7389 2024-03-27 14:01:47.000000 craftax-1.3.0/craftax/environment_base/wrappers.py
+drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.926173 craftax-1.3.0/craftax.egg-info/
+-rw-r--r--   0 mans4835  (1001) mans4835  (1001)     8674 2024-04-07 21:37:45.000000 craftax-1.3.0/craftax.egg-info/PKG-INFO
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     9455 2024-04-07 21:37:45.000000 craftax-1.3.0/craftax.egg-info/SOURCES.txt
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        1 2024-04-07 21:37:45.000000 craftax-1.3.0/craftax.egg-info/dependency_links.txt
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      147 2024-04-07 21:37:45.000000 craftax-1.3.0/craftax.egg-info/entry_points.txt
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      116 2024-04-07 21:37:45.000000 craftax-1.3.0/craftax.egg-info/requires.txt
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        8 2024-04-07 21:37:45.000000 craftax-1.3.0/craftax.egg-info/top_level.txt
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1058 2024-04-07 21:36:12.000000 craftax-1.3.0/pyproject.toml
+-rw-rw-r--   0 mans4835  (1001) mans4835  (1001)       38 2024-04-07 21:37:45.926173 craftax-1.3.0/setup.cfg
```

### Comparing `craftax-1.2.0/LICENSE` & `craftax-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/PKG-INFO` & `craftax-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craftax
-Version: 1.2.0
+Version: 1.3.0
 Summary: An open-world environment for training RL agents
 Author-email: Michael Matthews <michael.matthews@eng.ox.ac.uk>
 Project-URL: Homepage, https://github.com/MichaelTMatthews/Craftax
 Project-URL: Issues, https://github.com/MichaelTMatthews/Craftax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,15 +31,15 @@
  <img width="80%" src="https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/logo.png" />
 </p>
 
 <p align="center">
         <a href= "https://pypi.org/project/craftax/">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" /></a>
         <a href= "https://pypi.org/project/craftax/">
-        <img src="https://img.shields.io/badge/pypi-1.2.0-green" /></a>
+        <img src="https://img.shields.io/badge/pypi-1.3.0-green" /></a>
        <a href= "https://github.com/MichaelTMatthews/Craftax/blob/main/LICENSE">
         <img src="https://img.shields.io/badge/License-MIT-yellow" /></a>
        <a href= "https://craftaxenv.github.io/">
         <img src="https://img.shields.io/badge/blog-link-purple" /></a>
        <a href= "https://arxiv.org/pdf/2402.16801.pdf">
         <img src="https://img.shields.io/badge/arxiv-2402.16801-b31b1b" /></a>
        <a href= "https://github.com/psf/black">
@@ -117,24 +117,15 @@
 or to play Craftax-Classic run:
 ```
 play_craftax_classic
 ```
 Since Craftax runs entirely in JAX, it will take some time to compile the rendering and step functions - it might take around 30s to render the first frame and then another 20s to take the first action.  After this it should be very quick.  A tutorial for how to beat the game is present in `tutorial.md`.  The controls are printed out at the beginning of play.
 
 # 📈 Experiment
-To run PPO with default hyperparameters run:
-```
-python -m craftax.ppo
-```
-or to run PPO with memory call:
-```
-python -m craftax.ppo_rnn
-```
-To use ICM or E3B with the default parameters use the `--train_icm` and `--use_e3b` flags.
-Use the `env_name` parameter to control which environment is used.  It can be set to  `"Craftax-Symbolic-v1"`, `"Craftax-Pixels-v1"`, `"Craftax-Classic-Symbolic-v1"` or `"Craftax-Classic-Pixels-v1"`
+To run experiments see the [Craftax Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines) repository.
 
 # 🔪 Gotchas
 ### Optimistic Resets
 Craftax provides the option to use optimistic resets to improve performance, which means that (unlike regular gymnax environments) it **does not auto-reset** by default.
 This means that the environment should always be wrapped either in `OptimisticResetVecEnvWrapper` (for efficient resets) or `AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour).  See `ppo.py` for correct usage of both wrappers.
 
 ### Texture Caching
@@ -161,24 +152,24 @@
 |:----------|---------------:|:-------------------------------------------------------------------------:|
 | PPO-RNN   |            2.3 | <a href="https://github.com/luchris429/purejaxrl/tree/main">PureJaxRL</a> |
 | PPO       |            2.2 | <a href="https://github.com/luchris429/purejaxrl/tree/main">PureJaxRL</a> |
 | ICM       |            2.2 |           <a href="https://arxiv.org/abs/1705.05363">ICM</a>              |
 | E3B       |            2.2 |            <a href="https://arxiv.org/abs/2210.05805">E3B</a>             |
 
 
-# See Also
+# 🔎 See Also
 - ⛏️ [Crafter](https://github.com/danijar/crafter) The original Crafter benchmark.
 - ⚔️ [NLE](https://github.com/facebookresearch/nle) NetHack as an RL environment.
 - ⚡ [PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-end RL implementations in Jax.
 - 🌎 [JaxUED](https://github.com/DramaCow/jaxued): CleanRL style UED implementations in Jax.
 - 🌍 [Minimax](https://github.com/facebookresearch/minimax): Modular UED implementations in Jax.
 - 🏋️ [Gymnax](https://github.com/RobertTLange/gymnax): Standard Jax RL interface with classic environments.
 - 🧑‍🤝‍🧑 [JaxMARL](https://github.com/FLAIROx/JaxMARL): Multi-agent RL in Jax.
 
-# Citation
+# 📚 Citation
 If you use Craftax in your work please cite it as follows:
 ```
 @article{matthews2024craftax,
   title={Craftax: A Lightning-Fast Benchmark for Open-Ended Reinforcement Learning},
   author={Michael Matthews and Michael Beukman and Benjamin Ellis and Mikayel Samvelyan and Matthew Jackson and Samuel Coward and Jakob Foerster},
   journal={arXiv preprint},
   year={2024},
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: craftax Version: 1.2.0 Summary: An open-world
+Metadata-Version: 2.1 Name: craftax Version: 1.3.0 Summary: An open-world
 environment for training RL agents Author-email: Michael Matthews
 eng.ox.ac.uk> Project-URL: Homepage, https://github.com/MichaelTMatthews/
 Craftax Project-URL: Issues, https://github.com/MichaelTMatthews/Craftax/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: jax Requires-Dist: distrax Requires-Dist: optax
@@ -10,15 +10,15 @@
 pre-commit Requires-Dist: argparse Requires-Dist: wandb Requires-Dist: orbax-
 checkpoint Requires-Dist: pygame Requires-Dist: gymnax Requires-Dist: chex
 Requires-Dist: matplotlib Requires-Dist: imageio
    [https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/
                                    logo.png]
                      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-
 _3_._9_%_2_0_%_7_C_%_2_0_3_._1_0_%_2_0_%_7_C_%_2_0_3_._1_1_%_2_0_%_7_C_%_2_0_3_._1_2_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-  _p_y_p_i_-_1_._2_._0_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
+  _p_y_p_i_-_1_._3_._0_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_b_l_o_g_-_l_i_n_k_-_p_u_r_p_l_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_r_x_i_v_-
 _2_4_0_2_._1_6_8_0_1_-_b_3_1_b_1_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]
 # âï¸ Craftax Craftax is an RL environment written entirely in _J_A_X. Craftax
 reimplements and significantly extends the game mechanics of _C_r_a_f_t_e_r, taking
 inspiration from roguelike games such as _N_e_t_H_a_c_k. Craftax conforms to the
 _g_y_m_n_a_x interface, allowing easy integration with existing JAX-based frameworks
 like _P_u_r_e_J_a_x_R_L and [JaxUED](https://github.com/DramaCow/jaxued).
@@ -49,48 +49,44 @@
 storage.googleapis.com/jax-releases/jax_cuda_releases.html ``` # ð® Play To
 play Craftax run: ``` play_craftax ``` or to play Craftax-Classic run: ```
 play_craftax_classic ``` Since Craftax runs entirely in JAX, it will take some
 time to compile the rendering and step functions - it might take around 30s to
 render the first frame and then another 20s to take the first action. After
 this it should be very quick. A tutorial for how to beat the game is present in
 `tutorial.md`. The controls are printed out at the beginning of play. # ð
-Experiment To run PPO with default hyperparameters run: ``` python -
-m craftax.ppo ``` or to run PPO with memory call: ``` python -m craftax.ppo_rnn
-``` To use ICM or E3B with the default parameters use the `--train_icm` and `--
-use_e3b` flags. Use the `env_name` parameter to control which environment is
-used. It can be set to `"Craftax-Symbolic-v1"`, `"Craftax-Pixels-v1"`,
-`"Craftax-Classic-Symbolic-v1"` or `"Craftax-Classic-Pixels-v1"` # ðª Gotchas
-### Optimistic Resets Craftax provides the option to use optimistic resets to
-improve performance, which means that (unlike regular gymnax environments) it
-**does not auto-reset** by default. This means that the environment should
-always be wrapped either in `OptimisticResetVecEnvWrapper` (for efficient
-resets) or `AutoResetEnvWrapper` (to recover the default gymnax auto-reset
-behaviour). See `ppo.py` for correct usage of both wrappers. ### Texture
-Caching We use a texture cache to avoid recreating the texture atlas every time
-Craftax is imported. If you are just running Craftax as a benchmark this will
-not affect you. However, if you are editing the game (e.g. adding new blocks,
-entities etc.) then a stale cache could cause errors. You can export the
-following environment variable to force textures to be created from scratch.
-``` export CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like
-to add an algorithm please open a PR and provide a reference to the source of
-the results. We report reward as a % of the maximum (226). ## Craftax-1B |
+Experiment To run experiments see the [Craftax Baselines](https://github.com/
+MichaelTMatthews/Craftax_Baselines) repository. # ðª Gotchas ### Optimistic
+Resets Craftax provides the option to use optimistic resets to improve
+performance, which means that (unlike regular gymnax environments) it **does
+not auto-reset** by default. This means that the environment should always be
+wrapped either in `OptimisticResetVecEnvWrapper` (for efficient resets) or
+`AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour). See
+`ppo.py` for correct usage of both wrappers. ### Texture Caching We use a
+texture cache to avoid recreating the texture atlas every time Craftax is
+imported. If you are just running Craftax as a benchmark this will not affect
+you. However, if you are editing the game (e.g. adding new blocks, entities
+etc.) then a stale cache could cause errors. You can export the following
+environment variable to force textures to be created from scratch. ``` export
+CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like to add an
+algorithm please open a PR and provide a reference to the source of the
+results. We report reward as a % of the maximum (226). ## Craftax-1B |
 Algorithm | Reward (% max) | Source | |:----------|---------------:|:----------
 ---------------------------------------------------------------:| | PPO-RNN |
 15.3 | _P_u_r_e_J_a_x_R_L | | PPO | 11.9 | _P_u_r_e_J_a_x_R_L | | ICM | 11.9 | _I_C_M | | E3B | 11.0
 | _E_3_B | ## Craftax-1M | Algorithm | Reward (% max) | Source | |:----------|----
 -----------:|:-----------------------------------------------------------------
 --------:| | PPO-RNN | 2.3 | _P_u_r_e_J_a_x_R_L | | PPO | 2.2 | _P_u_r_e_J_a_x_R_L | | ICM | 2.2
-| _I_C_M | | E3B | 2.2 | _E_3_B | # See Also - âï¸ [Crafter](https://github.com/
-danijar/crafter) The original Crafter benchmark. - âï¸ [NLE](https://
-github.com/facebookresearch/nle) NetHack as an RL environment. - â¡
+| _I_C_M | | E3B | 2.2 | _E_3_B | # ð See Also - âï¸ [Crafter](https://
+github.com/danijar/crafter) The original Crafter benchmark. - âï¸ [NLE]
+(https://github.com/facebookresearch/nle) NetHack as an RL environment. - â¡
 [PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-end RL
 implementations in Jax. - ð [JaxUED](https://github.com/DramaCow/jaxued):
 CleanRL style UED implementations in Jax. - ð [Minimax](https://github.com/
 facebookresearch/minimax): Modular UED implementations in Jax. - ðï¸
 [Gymnax](https://github.com/RobertTLange/gymnax): Standard Jax RL interface
 with classic environments. - ð§âð¤âð§ [JaxMARL](https://github.com/
-FLAIROx/JaxMARL): Multi-agent RL in Jax. # Citation If you use Craftax in your
-work please cite it as follows: ``` @article{matthews2024craftax, title=
+FLAIROx/JaxMARL): Multi-agent RL in Jax. # ð Citation If you use Craftax in
+your work please cite it as follows: ``` @article{matthews2024craftax, title=
 {Craftax: A Lightning-Fast Benchmark for Open-Ended Reinforcement Learning},
 author={Michael Matthews and Michael Beukman and Benjamin Ellis and Mikayel
 Samvelyan and Matthew Jackson and Samuel Coward and Jakob Foerster}, journal=
 {arXiv preprint}, year={2024}, } ```
```

### Comparing `craftax-1.2.0/README.md` & `craftax-1.3.0/craftax.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,45 @@
+Metadata-Version: 2.1
+Name: craftax
+Version: 1.3.0
+Summary: An open-world environment for training RL agents
+Author-email: Michael Matthews <michael.matthews@eng.ox.ac.uk>
+Project-URL: Homepage, https://github.com/MichaelTMatthews/Craftax
+Project-URL: Issues, https://github.com/MichaelTMatthews/Craftax/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: jax
+Requires-Dist: distrax
+Requires-Dist: optax
+Requires-Dist: flax
+Requires-Dist: numpy
+Requires-Dist: black
+Requires-Dist: pre-commit
+Requires-Dist: argparse
+Requires-Dist: wandb
+Requires-Dist: orbax-checkpoint
+Requires-Dist: pygame
+Requires-Dist: gymnax
+Requires-Dist: chex
+Requires-Dist: matplotlib
+Requires-Dist: imageio
+
 <p align="center">
  <img width="80%" src="https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/logo.png" />
 </p>
 
 <p align="center">
         <a href= "https://pypi.org/project/craftax/">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" /></a>
         <a href= "https://pypi.org/project/craftax/">
-        <img src="https://img.shields.io/badge/pypi-1.2.0-green" /></a>
+        <img src="https://img.shields.io/badge/pypi-1.3.0-green" /></a>
        <a href= "https://github.com/MichaelTMatthews/Craftax/blob/main/LICENSE">
         <img src="https://img.shields.io/badge/License-MIT-yellow" /></a>
        <a href= "https://craftaxenv.github.io/">
         <img src="https://img.shields.io/badge/blog-link-purple" /></a>
        <a href= "https://arxiv.org/pdf/2402.16801.pdf">
         <img src="https://img.shields.io/badge/arxiv-2402.16801-b31b1b" /></a>
        <a href= "https://github.com/psf/black">
@@ -88,24 +117,15 @@
 or to play Craftax-Classic run:
 ```
 play_craftax_classic
 ```
 Since Craftax runs entirely in JAX, it will take some time to compile the rendering and step functions - it might take around 30s to render the first frame and then another 20s to take the first action.  After this it should be very quick.  A tutorial for how to beat the game is present in `tutorial.md`.  The controls are printed out at the beginning of play.
 
 # 📈 Experiment
-To run PPO with default hyperparameters run:
-```
-python -m craftax.ppo
-```
-or to run PPO with memory call:
-```
-python -m craftax.ppo_rnn
-```
-To use ICM or E3B with the default parameters use the `--train_icm` and `--use_e3b` flags.
-Use the `env_name` parameter to control which environment is used.  It can be set to  `"Craftax-Symbolic-v1"`, `"Craftax-Pixels-v1"`, `"Craftax-Classic-Symbolic-v1"` or `"Craftax-Classic-Pixels-v1"`
+To run experiments see the [Craftax Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines) repository.
 
 # 🔪 Gotchas
 ### Optimistic Resets
 Craftax provides the option to use optimistic resets to improve performance, which means that (unlike regular gymnax environments) it **does not auto-reset** by default.
 This means that the environment should always be wrapped either in `OptimisticResetVecEnvWrapper` (for efficient resets) or `AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour).  See `ppo.py` for correct usage of both wrappers.
 
 ### Texture Caching
@@ -132,26 +152,26 @@
 |:----------|---------------:|:-------------------------------------------------------------------------:|
 | PPO-RNN   |            2.3 | <a href="https://github.com/luchris429/purejaxrl/tree/main">PureJaxRL</a> |
 | PPO       |            2.2 | <a href="https://github.com/luchris429/purejaxrl/tree/main">PureJaxRL</a> |
 | ICM       |            2.2 |           <a href="https://arxiv.org/abs/1705.05363">ICM</a>              |
 | E3B       |            2.2 |            <a href="https://arxiv.org/abs/2210.05805">E3B</a>             |
 
 
-# See Also
+# 🔎 See Also
 - ⛏️ [Crafter](https://github.com/danijar/crafter) The original Crafter benchmark.
 - ⚔️ [NLE](https://github.com/facebookresearch/nle) NetHack as an RL environment.
 - ⚡ [PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-end RL implementations in Jax.
 - 🌎 [JaxUED](https://github.com/DramaCow/jaxued): CleanRL style UED implementations in Jax.
 - 🌍 [Minimax](https://github.com/facebookresearch/minimax): Modular UED implementations in Jax.
 - 🏋️ [Gymnax](https://github.com/RobertTLange/gymnax): Standard Jax RL interface with classic environments.
 - 🧑‍🤝‍🧑 [JaxMARL](https://github.com/FLAIROx/JaxMARL): Multi-agent RL in Jax.
 
-# Citation
+# 📚 Citation
 If you use Craftax in your work please cite it as follows:
 ```
 @article{matthews2024craftax,
   title={Craftax: A Lightning-Fast Benchmark for Open-Ended Reinforcement Learning},
   author={Michael Matthews and Michael Beukman and Benjamin Ellis and Mikayel Samvelyan and Matthew Jackson and Samuel Coward and Jakob Foerster},
   journal={arXiv preprint},
   year={2024},
 }
-```
+```
```

#### html2text {}

```diff
@@ -1,12 +1,24 @@
+Metadata-Version: 2.1 Name: craftax Version: 1.3.0 Summary: An open-world
+environment for training RL agents Author-email: Michael Matthews
+eng.ox.ac.uk> Project-URL: Homepage, https://github.com/MichaelTMatthews/
+Craftax Project-URL: Issues, https://github.com/MichaelTMatthews/Craftax/issues
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: jax Requires-Dist: distrax Requires-Dist: optax
+Requires-Dist: flax Requires-Dist: numpy Requires-Dist: black Requires-Dist:
+pre-commit Requires-Dist: argparse Requires-Dist: wandb Requires-Dist: orbax-
+checkpoint Requires-Dist: pygame Requires-Dist: gymnax Requires-Dist: chex
+Requires-Dist: matplotlib Requires-Dist: imageio
    [https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/
                                    logo.png]
                      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-
 _3_._9_%_2_0_%_7_C_%_2_0_3_._1_0_%_2_0_%_7_C_%_2_0_3_._1_1_%_2_0_%_7_C_%_2_0_3_._1_2_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-  _p_y_p_i_-_1_._2_._0_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
+  _p_y_p_i_-_1_._3_._0_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_b_l_o_g_-_l_i_n_k_-_p_u_r_p_l_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_r_x_i_v_-
 _2_4_0_2_._1_6_8_0_1_-_b_3_1_b_1_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]
 # âï¸ Craftax Craftax is an RL environment written entirely in _J_A_X. Craftax
 reimplements and significantly extends the game mechanics of _C_r_a_f_t_e_r, taking
 inspiration from roguelike games such as _N_e_t_H_a_c_k. Craftax conforms to the
 _g_y_m_n_a_x interface, allowing easy integration with existing JAX-based frameworks
 like _P_u_r_e_J_a_x_R_L and [JaxUED](https://github.com/DramaCow/jaxued).
@@ -37,48 +49,44 @@
 storage.googleapis.com/jax-releases/jax_cuda_releases.html ``` # ð® Play To
 play Craftax run: ``` play_craftax ``` or to play Craftax-Classic run: ```
 play_craftax_classic ``` Since Craftax runs entirely in JAX, it will take some
 time to compile the rendering and step functions - it might take around 30s to
 render the first frame and then another 20s to take the first action. After
 this it should be very quick. A tutorial for how to beat the game is present in
 `tutorial.md`. The controls are printed out at the beginning of play. # ð
-Experiment To run PPO with default hyperparameters run: ``` python -
-m craftax.ppo ``` or to run PPO with memory call: ``` python -m craftax.ppo_rnn
-``` To use ICM or E3B with the default parameters use the `--train_icm` and `--
-use_e3b` flags. Use the `env_name` parameter to control which environment is
-used. It can be set to `"Craftax-Symbolic-v1"`, `"Craftax-Pixels-v1"`,
-`"Craftax-Classic-Symbolic-v1"` or `"Craftax-Classic-Pixels-v1"` # ðª Gotchas
-### Optimistic Resets Craftax provides the option to use optimistic resets to
-improve performance, which means that (unlike regular gymnax environments) it
-**does not auto-reset** by default. This means that the environment should
-always be wrapped either in `OptimisticResetVecEnvWrapper` (for efficient
-resets) or `AutoResetEnvWrapper` (to recover the default gymnax auto-reset
-behaviour). See `ppo.py` for correct usage of both wrappers. ### Texture
-Caching We use a texture cache to avoid recreating the texture atlas every time
-Craftax is imported. If you are just running Craftax as a benchmark this will
-not affect you. However, if you are editing the game (e.g. adding new blocks,
-entities etc.) then a stale cache could cause errors. You can export the
-following environment variable to force textures to be created from scratch.
-``` export CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like
-to add an algorithm please open a PR and provide a reference to the source of
-the results. We report reward as a % of the maximum (226). ## Craftax-1B |
+Experiment To run experiments see the [Craftax Baselines](https://github.com/
+MichaelTMatthews/Craftax_Baselines) repository. # ðª Gotchas ### Optimistic
+Resets Craftax provides the option to use optimistic resets to improve
+performance, which means that (unlike regular gymnax environments) it **does
+not auto-reset** by default. This means that the environment should always be
+wrapped either in `OptimisticResetVecEnvWrapper` (for efficient resets) or
+`AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour). See
+`ppo.py` for correct usage of both wrappers. ### Texture Caching We use a
+texture cache to avoid recreating the texture atlas every time Craftax is
+imported. If you are just running Craftax as a benchmark this will not affect
+you. However, if you are editing the game (e.g. adding new blocks, entities
+etc.) then a stale cache could cause errors. You can export the following
+environment variable to force textures to be created from scratch. ``` export
+CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like to add an
+algorithm please open a PR and provide a reference to the source of the
+results. We report reward as a % of the maximum (226). ## Craftax-1B |
 Algorithm | Reward (% max) | Source | |:----------|---------------:|:----------
 ---------------------------------------------------------------:| | PPO-RNN |
 15.3 | _P_u_r_e_J_a_x_R_L | | PPO | 11.9 | _P_u_r_e_J_a_x_R_L | | ICM | 11.9 | _I_C_M | | E3B | 11.0
 | _E_3_B | ## Craftax-1M | Algorithm | Reward (% max) | Source | |:----------|----
 -----------:|:-----------------------------------------------------------------
 --------:| | PPO-RNN | 2.3 | _P_u_r_e_J_a_x_R_L | | PPO | 2.2 | _P_u_r_e_J_a_x_R_L | | ICM | 2.2
-| _I_C_M | | E3B | 2.2 | _E_3_B | # See Also - âï¸ [Crafter](https://github.com/
-danijar/crafter) The original Crafter benchmark. - âï¸ [NLE](https://
-github.com/facebookresearch/nle) NetHack as an RL environment. - â¡
+| _I_C_M | | E3B | 2.2 | _E_3_B | # ð See Also - âï¸ [Crafter](https://
+github.com/danijar/crafter) The original Crafter benchmark. - âï¸ [NLE]
+(https://github.com/facebookresearch/nle) NetHack as an RL environment. - â¡
 [PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-end RL
 implementations in Jax. - ð [JaxUED](https://github.com/DramaCow/jaxued):
 CleanRL style UED implementations in Jax. - ð [Minimax](https://github.com/
 facebookresearch/minimax): Modular UED implementations in Jax. - ðï¸
 [Gymnax](https://github.com/RobertTLange/gymnax): Standard Jax RL interface
 with classic environments. - ð§âð¤âð§ [JaxMARL](https://github.com/
-FLAIROx/JaxMARL): Multi-agent RL in Jax. # Citation If you use Craftax in your
-work please cite it as follows: ``` @article{matthews2024craftax, title=
+FLAIROx/JaxMARL): Multi-agent RL in Jax. # ð Citation If you use Craftax in
+your work please cite it as follows: ``` @article{matthews2024craftax, title=
 {Craftax: A Lightning-Fast Benchmark for Open-Ended Reinforcement Learning},
 author={Michael Matthews and Michael Beukman and Benjamin Ellis and Mikayel
 Samvelyan and Matthew Jackson and Samuel Coward and Jakob Foerster}, journal=
 {arXiv preprint}, year={2024}, } ```
```

### Comparing `craftax-1.2.0/craftax/craftax/assets/0.png` & `craftax-1.3.0/craftax/craftax/assets/0.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/1.png` & `craftax-1.3.0/craftax/craftax/assets/1.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/2.png` & `craftax-1.3.0/craftax/craftax/assets/2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/3.png` & `craftax-1.3.0/craftax/craftax/assets/3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/4.png` & `craftax-1.3.0/craftax/craftax/assets/4.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/5.png` & `craftax-1.3.0/craftax/craftax/assets/5.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/6.png` & `craftax-1.3.0/craftax/craftax/assets/6.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/7.png` & `craftax-1.3.0/craftax/craftax/assets/7.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/8.png` & `craftax-1.3.0/craftax/craftax/assets/8.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/9.png` & `craftax-1.3.0/craftax/craftax/assets/9.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/arrow-down.png` & `craftax-1.3.0/craftax/craftax/assets/arrow-down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/arrow-left.png` & `craftax-1.3.0/craftax/craftax/assets/arrow-left.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/arrow-right.png` & `craftax-1.3.0/craftax/craftax/assets/arrow-right.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/arrow-up.png` & `craftax-1.3.0/craftax/craftax/assets/arrow-up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/arrow_fire_enchantment.png` & `craftax-1.3.0/craftax/craftax/assets/arrow_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/arrow_ice_enchantment.png` & `craftax-1.3.0/craftax/craftax/assets/arrow_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/bat.png` & `craftax-1.3.0/craftax/craftax/assets/bat.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/book.png` & `craftax-1.3.0/craftax/craftax/assets/book.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/boots_fire_enchantment.png` & `craftax-1.3.0/craftax/craftax/assets/boots_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/boots_ice_enchantment.png` & `craftax-1.3.0/craftax/craftax/assets/boots_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/bow.png` & `craftax-1.3.0/craftax/craftax/assets/bow.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/chest.png` & `craftax-1.3.0/craftax/craftax/assets/chest.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/chestplate_fire_enchantment.png` & `craftax-1.3.0/craftax/craftax/assets/chestplate_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/chestplate_ice_enchantment.png` & `craftax-1.3.0/craftax/craftax/assets/chestplate_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/coal.png` & `craftax-1.3.0/craftax/craftax/assets/coal.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/cow.png` & `craftax-1.3.0/craftax/craftax/assets/cow.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/dagger.png` & `craftax-1.3.0/craftax/craftax/assets/dagger.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/debug-2.png` & `craftax-1.3.0/craftax/craftax/assets/debug-2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/debug-3.png` & `craftax-1.3.0/craftax/craftax/assets/debug-3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/debug.png` & `craftax-1.3.0/craftax/craftax/assets/debug.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/deep_thing.png` & `craftax-1.3.0/craftax/craftax/assets/deep_thing.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/dexterity.png` & `craftax-1.3.0/craftax/craftax/assets/dexterity.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/diamond.png` & `craftax-1.3.0/craftax/craftax/assets/diamond.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/diamond_boots.png` & `craftax-1.3.0/craftax/craftax/assets/diamond_boots.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/diamond_chestplate.png` & `craftax-1.3.0/craftax/craftax/assets/diamond_chestplate.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/diamond_helmet.png` & `craftax-1.3.0/craftax/craftax/assets/diamond_helmet.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/diamond_pants.png` & `craftax-1.3.0/craftax/craftax/assets/diamond_pants.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/diamond_pickaxe.png` & `craftax-1.3.0/craftax/craftax/assets/diamond_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/diamond_sword.png` & `craftax-1.3.0/craftax/craftax/assets/diamond_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/drink.png` & `craftax-1.3.0/craftax/craftax/assets/drink.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/enchantment_table_fire.png` & `craftax-1.3.0/craftax/craftax/assets/enchantment_table_fire.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/enchantment_table_ice.png` & `craftax-1.3.0/craftax/craftax/assets/enchantment_table_ice.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/energy.png` & `craftax-1.3.0/craftax/craftax/assets/energy.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/fence.png` & `craftax-1.3.0/craftax/craftax/assets/fence.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/fire_elemental.png` & `craftax-1.3.0/craftax/craftax/assets/fire_elemental.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/fire_grass.png` & `craftax-1.3.0/craftax/craftax/assets/fire_grass.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/fire_stone.png` & `craftax-1.3.0/craftax/craftax/assets/fire_stone.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/fire_tree.png` & `craftax-1.3.0/craftax/craftax/assets/fire_tree.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/fireball.png` & `craftax-1.3.0/craftax/craftax/assets/fireball.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/food.png` & `craftax-1.3.0/craftax/craftax/assets/food.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/fountain.png` & `craftax-1.3.0/craftax/craftax/assets/fountain.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/frost_troll.png` & `craftax-1.3.0/craftax/craftax/assets/frost_troll.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/furnace.png` & `craftax-1.3.0/craftax/craftax/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/gnome_archer.png` & `craftax-1.3.0/craftax/craftax/assets/gnome_archer.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/gnome_warrior.png` & `craftax-1.3.0/craftax/craftax/assets/gnome_warrior.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/grass.png` & `craftax-1.3.0/craftax/craftax/assets/grass.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/grave.png` & `craftax-1.3.0/craftax/craftax/assets/grave.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/grave2.png` & `craftax-1.3.0/craftax/craftax/assets/grave2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/grave3.png` & `craftax-1.3.0/craftax/craftax/assets/grave3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/gravel.png` & `craftax-1.3.0/craftax/craftax/assets/gravel.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/health.png` & `craftax-1.3.0/craftax/craftax/assets/health.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/helmet_fire_enchantment.png` & `craftax-1.3.0/craftax/craftax/assets/helmet_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/helmet_ice_enchantment.png` & `craftax-1.3.0/craftax/craftax/assets/helmet_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/ice_elemental.png` & `craftax-1.3.0/craftax/craftax/assets/ice_elemental.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/ice_grass.png` & `craftax-1.3.0/craftax/craftax/assets/ice_grass.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/ice_shrub.png` & `craftax-1.3.0/craftax/craftax/assets/ice_shrub.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/iceball.png` & `craftax-1.3.0/craftax/craftax/assets/iceball.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/intelligence.png` & `craftax-1.3.0/craftax/craftax/assets/intelligence.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/iron.png` & `craftax-1.3.0/craftax/craftax/assets/iron.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/iron_boots.png` & `craftax-1.3.0/craftax/craftax/assets/iron_boots.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/iron_chestplate.png` & `craftax-1.3.0/craftax/craftax/assets/iron_chestplate.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/iron_helmet.png` & `craftax-1.3.0/craftax/craftax/assets/iron_helmet.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/iron_pants.png` & `craftax-1.3.0/craftax/craftax/assets/iron_pants.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/iron_pickaxe.png` & `craftax-1.3.0/craftax/craftax/assets/iron_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/iron_sword.png` & `craftax-1.3.0/craftax/craftax/assets/iron_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/knight.png` & `craftax-1.3.0/craftax/craftax/assets/knight.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/knight_archer.png` & `craftax-1.3.0/craftax/craftax/assets/knight_archer.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/kobold.png` & `craftax-1.3.0/craftax/craftax/assets/kobold.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/ladder_down.png` & `craftax-1.3.0/craftax/craftax/assets/ladder_down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/ladder_down_blocked.png` & `craftax-1.3.0/craftax/craftax/assets/ladder_down_blocked.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/ladder_up.png` & `craftax-1.3.0/craftax/craftax/assets/ladder_up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/lava.png` & `craftax-1.3.0/craftax/craftax/assets/lava.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/leaves.png` & `craftax-1.3.0/craftax/craftax/assets/leaves.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/lizard.png` & `craftax-1.3.0/craftax/craftax/assets/lizard.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/log.png` & `craftax-1.3.0/craftax/craftax/assets/log.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/mana.png` & `craftax-1.3.0/craftax/craftax/assets/mana.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/necromancer.png` & `craftax-1.3.0/craftax/craftax/assets/necromancer.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/necromancer_vulnerable.png` & `craftax-1.3.0/craftax/craftax/assets/necromancer_vulnerable.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/orc_mage.png` & `craftax-1.3.0/craftax/craftax/assets/orc_mage.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/orc_soldier.png` & `craftax-1.3.0/craftax/craftax/assets/orc_soldier.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/pants_fire_enchantment.png` & `craftax-1.3.0/craftax/craftax/assets/pants_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/pants_ice_enchantment.png` & `craftax-1.3.0/craftax/craftax/assets/pants_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/path.png` & `craftax-1.3.0/craftax/craftax/assets/path.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/pigman.png` & `craftax-1.3.0/craftax/craftax/assets/pigman.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/plant-ripe.png` & `craftax-1.3.0/craftax/craftax/assets/plant-ripe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/plant-young.png` & `craftax-1.3.0/craftax/craftax/assets/plant-young.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/plant.png` & `craftax-1.3.0/craftax/craftax/assets/plant.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/player-down.png` & `craftax-1.3.0/craftax/craftax/assets/player-down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/player-left.png` & `craftax-1.3.0/craftax/craftax/assets/player-left.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/player-right.png` & `craftax-1.3.0/craftax/craftax/assets/player-right.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/player-sleep.png` & `craftax-1.3.0/craftax/craftax/assets/player-sleep.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/player-up.png` & `craftax-1.3.0/craftax/craftax/assets/player-up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/player.png` & `craftax-1.3.0/craftax/craftax/assets/player.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/potion_blue.png` & `craftax-1.3.0/craftax/craftax/assets/potion_blue.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/potion_cyan.png` & `craftax-1.3.0/craftax/craftax/assets/potion_cyan.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/potion_green.png` & `craftax-1.3.0/craftax/craftax/assets/potion_green.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/potion_pink.png` & `craftax-1.3.0/craftax/craftax/assets/potion_pink.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/potion_red.png` & `craftax-1.3.0/craftax/craftax/assets/potion_red.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/potion_yellow.png` & `craftax-1.3.0/craftax/craftax/assets/potion_yellow.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/ruby.png` & `craftax-1.3.0/craftax/craftax/assets/ruby.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/sand.png` & `craftax-1.3.0/craftax/craftax/assets/sand.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/sapling.png` & `craftax-1.3.0/craftax/craftax/assets/sapling.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/sapphire.png` & `craftax-1.3.0/craftax/craftax/assets/sapphire.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/skeleton.png` & `craftax-1.3.0/craftax/craftax/assets/skeleton.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/slimeball.png` & `craftax-1.3.0/craftax/craftax/assets/slimeball.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/snail.png` & `craftax-1.3.0/craftax/craftax/assets/snail.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/spider.png` & `craftax-1.3.0/craftax/craftax/assets/spider.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/stalagmite.png` & `craftax-1.3.0/craftax/craftax/assets/stalagmite.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/stone.png` & `craftax-1.3.0/craftax/craftax/assets/stone.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/stone_pickaxe.png` & `craftax-1.3.0/craftax/craftax/assets/stone_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/stone_sword.png` & `craftax-1.3.0/craftax/craftax/assets/stone_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/strength.png` & `craftax-1.3.0/craftax/craftax/assets/strength.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/sword_fire_enchantment.png` & `craftax-1.3.0/craftax/craftax/assets/sword_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/sword_ice_enchantment.png` & `craftax-1.3.0/craftax/craftax/assets/sword_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/table.png` & `craftax-1.3.0/craftax/craftax/assets/table.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/texture_cache.pbz2` & `craftax-1.3.0/craftax/craftax/assets/texture_cache.pbz2`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/torch_in_inventory.png` & `craftax-1.3.0/craftax/craftax/assets/torch_in_inventory.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/torch_on_path.png` & `craftax-1.3.0/craftax/craftax/assets/torch_on_path.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/tree.png` & `craftax-1.3.0/craftax/craftax/assets/tree.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/troll.png` & `craftax-1.3.0/craftax/craftax/assets/troll.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/unknown.png` & `craftax-1.3.0/craftax/craftax/assets/unknown.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/water.png` & `craftax-1.3.0/craftax/craftax/assets/water.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/wood.png` & `craftax-1.3.0/craftax/craftax/assets/wood.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/wood_pickaxe.png` & `craftax-1.3.0/craftax/craftax/assets/wood_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/wood_sword.png` & `craftax-1.3.0/craftax/craftax/assets/wood_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/xp.png` & `craftax-1.3.0/craftax/craftax/assets/xp.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/assets/zombie.png` & `craftax-1.3.0/craftax/craftax/assets/zombie.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/constants.py` & `craftax-1.3.0/craftax/craftax/constants.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/craftax_state.py` & `craftax-1.3.0/craftax/craftax/craftax_state.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/envs/craftax_pixels_env.py` & `craftax-1.3.0/craftax/craftax/envs/craftax_pixels_env.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/envs/craftax_symbolic_env.py` & `craftax-1.3.0/craftax/craftax/envs/craftax_symbolic_env.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/game_logic.py` & `craftax-1.3.0/craftax/craftax/game_logic.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/play_craftax.py` & `craftax-1.3.0/craftax/craftax/play_craftax.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/renderer.py` & `craftax-1.3.0/craftax/craftax/renderer.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/util/game_logic_utils.py` & `craftax-1.3.0/craftax/craftax/util/game_logic_utils.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/util/maths_utils.py` & `craftax-1.3.0/craftax/craftax/util/maths_utils.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/util/noise.py` & `craftax-1.3.0/craftax/craftax/util/noise.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/world_gen/world_gen.py` & `craftax-1.3.0/craftax/craftax/world_gen/world_gen.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax/world_gen/world_gen_configs.py` & `craftax-1.3.0/craftax/craftax/world_gen/world_gen_configs.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/1.png` & `craftax-1.3.0/craftax/craftax_classic/assets/1.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/2.png` & `craftax-1.3.0/craftax/craftax_classic/assets/2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/3.png` & `craftax-1.3.0/craftax/craftax_classic/assets/3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/4.png` & `craftax-1.3.0/craftax/craftax_classic/assets/4.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/5.png` & `craftax-1.3.0/craftax/craftax_classic/assets/5.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/6.png` & `craftax-1.3.0/craftax/craftax_classic/assets/6.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/7.png` & `craftax-1.3.0/craftax/craftax_classic/assets/7.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/8.png` & `craftax-1.3.0/craftax/craftax_classic/assets/8.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/9.png` & `craftax-1.3.0/craftax/craftax_classic/assets/9.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/arrow-down.png` & `craftax-1.3.0/craftax/craftax_classic/assets/arrow-down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/arrow-left.png` & `craftax-1.3.0/craftax/craftax_classic/assets/arrow-left.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/arrow-right.png` & `craftax-1.3.0/craftax/craftax_classic/assets/arrow-right.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/arrow-up.png` & `craftax-1.3.0/craftax/craftax_classic/assets/arrow-up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/coal.png` & `craftax-1.3.0/craftax/craftax_classic/assets/coal.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/cow.png` & `craftax-1.3.0/craftax/craftax_classic/assets/cow.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/debug-2.png` & `craftax-1.3.0/craftax/craftax_classic/assets/debug-2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/debug-3.png` & `craftax-1.3.0/craftax/craftax_classic/assets/debug-3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/debug.png` & `craftax-1.3.0/craftax/craftax_classic/assets/debug.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/diamond.png` & `craftax-1.3.0/craftax/craftax_classic/assets/diamond.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/drink.png` & `craftax-1.3.0/craftax/craftax_classic/assets/drink.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/energy.png` & `craftax-1.3.0/craftax/craftax_classic/assets/energy.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/fence.png` & `craftax-1.3.0/craftax/craftax_classic/assets/fence.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/food.png` & `craftax-1.3.0/craftax/craftax_classic/assets/food.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/furnace.png` & `craftax-1.3.0/craftax/craftax_classic/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/grass.png` & `craftax-1.3.0/craftax/craftax_classic/assets/grass.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/health.png` & `craftax-1.3.0/craftax/craftax_classic/assets/health.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/iron.png` & `craftax-1.3.0/craftax/craftax_classic/assets/iron.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/iron_pickaxe.png` & `craftax-1.3.0/craftax/craftax_classic/assets/iron_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/iron_sword.png` & `craftax-1.3.0/craftax/craftax_classic/assets/iron_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/lava.png` & `craftax-1.3.0/craftax/craftax_classic/assets/lava.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/leaves.png` & `craftax-1.3.0/craftax/craftax_classic/assets/leaves.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/log.png` & `craftax-1.3.0/craftax/craftax_classic/assets/log.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/path.png` & `craftax-1.3.0/craftax/craftax_classic/assets/path.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/plant-ripe.png` & `craftax-1.3.0/craftax/craftax_classic/assets/plant-ripe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/plant-young.png` & `craftax-1.3.0/craftax/craftax_classic/assets/plant-young.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/plant.png` & `craftax-1.3.0/craftax/craftax_classic/assets/plant.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/player-down.png` & `craftax-1.3.0/craftax/craftax_classic/assets/player-down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/player-left.png` & `craftax-1.3.0/craftax/craftax_classic/assets/player-left.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/player-right.png` & `craftax-1.3.0/craftax/craftax_classic/assets/player-right.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/player-sleep.png` & `craftax-1.3.0/craftax/craftax_classic/assets/player-sleep.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/player-up.png` & `craftax-1.3.0/craftax/craftax_classic/assets/player-up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/player.png` & `craftax-1.3.0/craftax/craftax_classic/assets/player.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/sand.png` & `craftax-1.3.0/craftax/craftax_classic/assets/sand.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/sapling.png` & `craftax-1.3.0/craftax/craftax_classic/assets/sapling.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/skeleton.png` & `craftax-1.3.0/craftax/craftax_classic/assets/skeleton.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/stone.png` & `craftax-1.3.0/craftax/craftax_classic/assets/stone.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/stone_pickaxe.png` & `craftax-1.3.0/craftax/craftax_classic/assets/stone_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/stone_sword.png` & `craftax-1.3.0/craftax/craftax_classic/assets/stone_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/table.png` & `craftax-1.3.0/craftax/craftax_classic/assets/table.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/tree.png` & `craftax-1.3.0/craftax/craftax_classic/assets/tree.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/unknown.png` & `craftax-1.3.0/craftax/craftax_classic/assets/unknown.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/water.png` & `craftax-1.3.0/craftax/craftax_classic/assets/water.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/wood.png` & `craftax-1.3.0/craftax/craftax_classic/assets/wood.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/wood_pickaxe.png` & `craftax-1.3.0/craftax/craftax_classic/assets/wood_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/wood_sword.png` & `craftax-1.3.0/craftax/craftax_classic/assets/wood_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/assets/zombie.png` & `craftax-1.3.0/craftax/craftax_classic/assets/zombie.png`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/constants.py` & `craftax-1.3.0/craftax/craftax_classic/constants.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/envs/craftax_pixels_env.py` & `craftax-1.3.0/craftax/craftax_classic/envs/craftax_pixels_env.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/envs/craftax_state.py` & `craftax-1.3.0/craftax/craftax_classic/envs/craftax_state.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/envs/craftax_symbolic_env.py` & `craftax-1.3.0/craftax/craftax_classic/envs/craftax_symbolic_env.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/game_logic.py` & `craftax-1.3.0/craftax/craftax_classic/game_logic.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/play_craftax_classic.py` & `craftax-1.3.0/craftax/craftax_classic/play_craftax_classic.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/renderer.py` & `craftax-1.3.0/craftax/craftax_classic/renderer.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/util/noise.py` & `craftax-1.3.0/craftax/craftax_classic/util/noise.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/craftax_classic/world_gen.py` & `craftax-1.3.0/craftax/craftax_classic/world_gen.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/environment_base/environment_no_auto_reset.py` & `craftax-1.3.0/craftax/environment_base/environment_no_auto_reset.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax/environment_base/wrappers.py` & `craftax-1.3.0/craftax/environment_base/wrappers.py`

 * *Files identical despite different names*

### Comparing `craftax-1.2.0/craftax.egg-info/PKG-INFO` & `craftax-1.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,16 @@
-Metadata-Version: 2.1
-Name: craftax
-Version: 1.2.0
-Summary: An open-world environment for training RL agents
-Author-email: Michael Matthews <michael.matthews@eng.ox.ac.uk>
-Project-URL: Homepage, https://github.com/MichaelTMatthews/Craftax
-Project-URL: Issues, https://github.com/MichaelTMatthews/Craftax/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: jax
-Requires-Dist: distrax
-Requires-Dist: optax
-Requires-Dist: flax
-Requires-Dist: numpy
-Requires-Dist: black
-Requires-Dist: pre-commit
-Requires-Dist: argparse
-Requires-Dist: wandb
-Requires-Dist: orbax-checkpoint
-Requires-Dist: pygame
-Requires-Dist: gymnax
-Requires-Dist: chex
-Requires-Dist: matplotlib
-Requires-Dist: imageio
-
 <p align="center">
  <img width="80%" src="https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/logo.png" />
 </p>
 
 <p align="center">
         <a href= "https://pypi.org/project/craftax/">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" /></a>
         <a href= "https://pypi.org/project/craftax/">
-        <img src="https://img.shields.io/badge/pypi-1.2.0-green" /></a>
+        <img src="https://img.shields.io/badge/pypi-1.3.0-green" /></a>
        <a href= "https://github.com/MichaelTMatthews/Craftax/blob/main/LICENSE">
         <img src="https://img.shields.io/badge/License-MIT-yellow" /></a>
        <a href= "https://craftaxenv.github.io/">
         <img src="https://img.shields.io/badge/blog-link-purple" /></a>
        <a href= "https://arxiv.org/pdf/2402.16801.pdf">
         <img src="https://img.shields.io/badge/arxiv-2402.16801-b31b1b" /></a>
        <a href= "https://github.com/psf/black">
@@ -117,24 +88,15 @@
 or to play Craftax-Classic run:
 ```
 play_craftax_classic
 ```
 Since Craftax runs entirely in JAX, it will take some time to compile the rendering and step functions - it might take around 30s to render the first frame and then another 20s to take the first action.  After this it should be very quick.  A tutorial for how to beat the game is present in `tutorial.md`.  The controls are printed out at the beginning of play.
 
 # 📈 Experiment
-To run PPO with default hyperparameters run:
-```
-python -m craftax.ppo
-```
-or to run PPO with memory call:
-```
-python -m craftax.ppo_rnn
-```
-To use ICM or E3B with the default parameters use the `--train_icm` and `--use_e3b` flags.
-Use the `env_name` parameter to control which environment is used.  It can be set to  `"Craftax-Symbolic-v1"`, `"Craftax-Pixels-v1"`, `"Craftax-Classic-Symbolic-v1"` or `"Craftax-Classic-Pixels-v1"`
+To run experiments see the [Craftax Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines) repository.
 
 # 🔪 Gotchas
 ### Optimistic Resets
 Craftax provides the option to use optimistic resets to improve performance, which means that (unlike regular gymnax environments) it **does not auto-reset** by default.
 This means that the environment should always be wrapped either in `OptimisticResetVecEnvWrapper` (for efficient resets) or `AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour).  See `ppo.py` for correct usage of both wrappers.
 
 ### Texture Caching
@@ -161,26 +123,26 @@
 |:----------|---------------:|:-------------------------------------------------------------------------:|
 | PPO-RNN   |            2.3 | <a href="https://github.com/luchris429/purejaxrl/tree/main">PureJaxRL</a> |
 | PPO       |            2.2 | <a href="https://github.com/luchris429/purejaxrl/tree/main">PureJaxRL</a> |
 | ICM       |            2.2 |           <a href="https://arxiv.org/abs/1705.05363">ICM</a>              |
 | E3B       |            2.2 |            <a href="https://arxiv.org/abs/2210.05805">E3B</a>             |
 
 
-# See Also
+# 🔎 See Also
 - ⛏️ [Crafter](https://github.com/danijar/crafter) The original Crafter benchmark.
 - ⚔️ [NLE](https://github.com/facebookresearch/nle) NetHack as an RL environment.
 - ⚡ [PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-end RL implementations in Jax.
 - 🌎 [JaxUED](https://github.com/DramaCow/jaxued): CleanRL style UED implementations in Jax.
 - 🌍 [Minimax](https://github.com/facebookresearch/minimax): Modular UED implementations in Jax.
 - 🏋️ [Gymnax](https://github.com/RobertTLange/gymnax): Standard Jax RL interface with classic environments.
 - 🧑‍🤝‍🧑 [JaxMARL](https://github.com/FLAIROx/JaxMARL): Multi-agent RL in Jax.
 
-# Citation
+# 📚 Citation
 If you use Craftax in your work please cite it as follows:
 ```
 @article{matthews2024craftax,
   title={Craftax: A Lightning-Fast Benchmark for Open-Ended Reinforcement Learning},
   author={Michael Matthews and Michael Beukman and Benjamin Ellis and Mikayel Samvelyan and Matthew Jackson and Samuel Coward and Jakob Foerster},
   journal={arXiv preprint},
   year={2024},
 }
-```
+```
```

#### html2text {}

```diff
@@ -1,24 +1,12 @@
-Metadata-Version: 2.1 Name: craftax Version: 1.2.0 Summary: An open-world
-environment for training RL agents Author-email: Michael Matthews
-eng.ox.ac.uk> Project-URL: Homepage, https://github.com/MichaelTMatthews/
-Craftax Project-URL: Issues, https://github.com/MichaelTMatthews/Craftax/issues
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: jax Requires-Dist: distrax Requires-Dist: optax
-Requires-Dist: flax Requires-Dist: numpy Requires-Dist: black Requires-Dist:
-pre-commit Requires-Dist: argparse Requires-Dist: wandb Requires-Dist: orbax-
-checkpoint Requires-Dist: pygame Requires-Dist: gymnax Requires-Dist: chex
-Requires-Dist: matplotlib Requires-Dist: imageio
    [https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/
                                    logo.png]
                      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-
 _3_._9_%_2_0_%_7_C_%_2_0_3_._1_0_%_2_0_%_7_C_%_2_0_3_._1_1_%_2_0_%_7_C_%_2_0_3_._1_2_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-  _p_y_p_i_-_1_._2_._0_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
+  _p_y_p_i_-_1_._3_._0_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_b_l_o_g_-_l_i_n_k_-_p_u_r_p_l_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_r_x_i_v_-
 _2_4_0_2_._1_6_8_0_1_-_b_3_1_b_1_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]
 # âï¸ Craftax Craftax is an RL environment written entirely in _J_A_X. Craftax
 reimplements and significantly extends the game mechanics of _C_r_a_f_t_e_r, taking
 inspiration from roguelike games such as _N_e_t_H_a_c_k. Craftax conforms to the
 _g_y_m_n_a_x interface, allowing easy integration with existing JAX-based frameworks
 like _P_u_r_e_J_a_x_R_L and [JaxUED](https://github.com/DramaCow/jaxued).
@@ -49,48 +37,44 @@
 storage.googleapis.com/jax-releases/jax_cuda_releases.html ``` # ð® Play To
 play Craftax run: ``` play_craftax ``` or to play Craftax-Classic run: ```
 play_craftax_classic ``` Since Craftax runs entirely in JAX, it will take some
 time to compile the rendering and step functions - it might take around 30s to
 render the first frame and then another 20s to take the first action. After
 this it should be very quick. A tutorial for how to beat the game is present in
 `tutorial.md`. The controls are printed out at the beginning of play. # ð
-Experiment To run PPO with default hyperparameters run: ``` python -
-m craftax.ppo ``` or to run PPO with memory call: ``` python -m craftax.ppo_rnn
-``` To use ICM or E3B with the default parameters use the `--train_icm` and `--
-use_e3b` flags. Use the `env_name` parameter to control which environment is
-used. It can be set to `"Craftax-Symbolic-v1"`, `"Craftax-Pixels-v1"`,
-`"Craftax-Classic-Symbolic-v1"` or `"Craftax-Classic-Pixels-v1"` # ðª Gotchas
-### Optimistic Resets Craftax provides the option to use optimistic resets to
-improve performance, which means that (unlike regular gymnax environments) it
-**does not auto-reset** by default. This means that the environment should
-always be wrapped either in `OptimisticResetVecEnvWrapper` (for efficient
-resets) or `AutoResetEnvWrapper` (to recover the default gymnax auto-reset
-behaviour). See `ppo.py` for correct usage of both wrappers. ### Texture
-Caching We use a texture cache to avoid recreating the texture atlas every time
-Craftax is imported. If you are just running Craftax as a benchmark this will
-not affect you. However, if you are editing the game (e.g. adding new blocks,
-entities etc.) then a stale cache could cause errors. You can export the
-following environment variable to force textures to be created from scratch.
-``` export CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like
-to add an algorithm please open a PR and provide a reference to the source of
-the results. We report reward as a % of the maximum (226). ## Craftax-1B |
+Experiment To run experiments see the [Craftax Baselines](https://github.com/
+MichaelTMatthews/Craftax_Baselines) repository. # ðª Gotchas ### Optimistic
+Resets Craftax provides the option to use optimistic resets to improve
+performance, which means that (unlike regular gymnax environments) it **does
+not auto-reset** by default. This means that the environment should always be
+wrapped either in `OptimisticResetVecEnvWrapper` (for efficient resets) or
+`AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour). See
+`ppo.py` for correct usage of both wrappers. ### Texture Caching We use a
+texture cache to avoid recreating the texture atlas every time Craftax is
+imported. If you are just running Craftax as a benchmark this will not affect
+you. However, if you are editing the game (e.g. adding new blocks, entities
+etc.) then a stale cache could cause errors. You can export the following
+environment variable to force textures to be created from scratch. ``` export
+CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like to add an
+algorithm please open a PR and provide a reference to the source of the
+results. We report reward as a % of the maximum (226). ## Craftax-1B |
 Algorithm | Reward (% max) | Source | |:----------|---------------:|:----------
 ---------------------------------------------------------------:| | PPO-RNN |
 15.3 | _P_u_r_e_J_a_x_R_L | | PPO | 11.9 | _P_u_r_e_J_a_x_R_L | | ICM | 11.9 | _I_C_M | | E3B | 11.0
 | _E_3_B | ## Craftax-1M | Algorithm | Reward (% max) | Source | |:----------|----
 -----------:|:-----------------------------------------------------------------
 --------:| | PPO-RNN | 2.3 | _P_u_r_e_J_a_x_R_L | | PPO | 2.2 | _P_u_r_e_J_a_x_R_L | | ICM | 2.2
-| _I_C_M | | E3B | 2.2 | _E_3_B | # See Also - âï¸ [Crafter](https://github.com/
-danijar/crafter) The original Crafter benchmark. - âï¸ [NLE](https://
-github.com/facebookresearch/nle) NetHack as an RL environment. - â¡
+| _I_C_M | | E3B | 2.2 | _E_3_B | # ð See Also - âï¸ [Crafter](https://
+github.com/danijar/crafter) The original Crafter benchmark. - âï¸ [NLE]
+(https://github.com/facebookresearch/nle) NetHack as an RL environment. - â¡
 [PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-end RL
 implementations in Jax. - ð [JaxUED](https://github.com/DramaCow/jaxued):
 CleanRL style UED implementations in Jax. - ð [Minimax](https://github.com/
 facebookresearch/minimax): Modular UED implementations in Jax. - ðï¸
 [Gymnax](https://github.com/RobertTLange/gymnax): Standard Jax RL interface
 with classic environments. - ð§âð¤âð§ [JaxMARL](https://github.com/
-FLAIROx/JaxMARL): Multi-agent RL in Jax. # Citation If you use Craftax in your
-work please cite it as follows: ``` @article{matthews2024craftax, title=
+FLAIROx/JaxMARL): Multi-agent RL in Jax. # ð Citation If you use Craftax in
+your work please cite it as follows: ``` @article{matthews2024craftax, title=
 {Craftax: A Lightning-Fast Benchmark for Open-Ended Reinforcement Learning},
 author={Michael Matthews and Michael Beukman and Benjamin Ellis and Mikayel
 Samvelyan and Matthew Jackson and Samuel Coward and Jakob Foerster}, journal=
 {arXiv preprint}, year={2024}, } ```
```

### Comparing `craftax-1.2.0/craftax.egg-info/SOURCES.txt` & `craftax-1.3.0/craftax.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-craftax/ppo.py
-craftax/ppo_rnn.py
 craftax.egg-info/PKG-INFO
 craftax.egg-info/SOURCES.txt
 craftax.egg-info/dependency_links.txt
 craftax.egg-info/entry_points.txt
 craftax.egg-info/requires.txt
 craftax.egg-info/top_level.txt
 craftax/craftax/__init__.py
@@ -225,15 +223,14 @@
 craftax/craftax_classic/assets/sand.png
 craftax/craftax_classic/assets/sapling.png
 craftax/craftax_classic/assets/skeleton.png
 craftax/craftax_classic/assets/stone.png
 craftax/craftax_classic/assets/stone_pickaxe.png
 craftax/craftax_classic/assets/stone_sword.png
 craftax/craftax_classic/assets/table.png
-craftax/craftax_classic/assets/texture_cache_classic.pbz2
 craftax/craftax_classic/assets/tree.png
 craftax/craftax_classic/assets/unknown.png
 craftax/craftax_classic/assets/water.png
 craftax/craftax_classic/assets/wood.png
 craftax/craftax_classic/assets/wood_pickaxe.png
 craftax/craftax_classic/assets/wood_sword.png
 craftax/craftax_classic/assets/zombie.png
@@ -243,14 +240,8 @@
 craftax/craftax_classic/envs/craftax_state.py
 craftax/craftax_classic/envs/craftax_symbolic_env.py
 craftax/craftax_classic/util/__init__.py
 craftax/craftax_classic/util/noise.py
 craftax/environment_base/__init__.py
 craftax/environment_base/environment_no_auto_reset.py
 craftax/environment_base/util.py
-craftax/environment_base/wrappers.py
-craftax/logz/__init__.py
-craftax/logz/batch_logging.py
-craftax/models/__init__.py
-craftax/models/actor_critic.py
-craftax/models/icm.py
-craftax/models/world_model.py
+craftax/environment_base/wrappers.py
```

### Comparing `craftax-1.2.0/pyproject.toml` & `craftax-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "craftax"
-version = "1.2.0"
+version = "1.3.0"
 authors = [
   { name="Michael Matthews", email="michael.matthews@eng.ox.ac.uk" },
 ]
 description = "An open-world environment for training RL agents"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

