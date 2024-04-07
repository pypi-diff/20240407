# Comparing `tmp/pandalibs-0.1.2-py3-none-any.whl.zip` & `tmp/pandalibs-0.1.3.tar.gz`

 * *Command `'zipinfo {}'` failed with exit code 9. Standard output:*

 * *    Archive:  tmp/pandalibs-0.1.3.tar.gz*

 * *    […]*

 * *Archive contents identical but files differ, possibly due to different compression levels. Falling back to binary comparison.*

```diff
@@ -1,139 +1,132 @@
-00000000: 504b 0304 1400 0000 0800 1c70 8758 0000  PK.........p.X..
-00000010: 0000 0200 0000 0000 0000 1500 0000 7061  ..............pa
-00000020: 6e64 616c 6962 732f 5f5f 696e 6974 5f5f  ndalibs/__init__
-00000030: 2e70 7903 0050 4b03 0414 0000 0008 00ad  .py..PK.........
-00000040: 7c87 5858 f167 9446 0300 00e2 0800 001a  |.XX.g.F........
-00000050: 0000 0070 616e 6461 6c69 6273 2f79 616d  ...pandalibs/yam
-00000060: 6c5f 696d 706f 7274 6572 2e70 79ad 56c1  l_importer.py.V.
-00000070: 8adb 3010 bd2f ec3f 0cee 611d 08a6 e785  ..0../.?..a.....
-00000080: 1c96 3429 4b97 16da eda1 9462 147b 9c55  ..4)K......b.{.U
-00000090: ab48 6624 6f9b 2efb ef9d b11d 5bf6 e650  .Hf$o.......[..P
-000000a0: 4a9d 4314 49f3 de1b cd1b c5fa 503b 0ae0  J.C.I.......P;..
-000000b0: fce5 85ee 86fe 388e 8fea 602e 2fe4 f30a  ......8...`./...
-000000c0: d68d 0fee 00f8 abc0 3a68 67a1 7204 85b3  ........:hg.r...
-000000d0: 95de 37a4 da19 2472 c4d1 8551 dec3 3a5e  ..7...$r...Q..:^
-000000e0: dbc8 52ba 3905 2fae 2f2f 809f 9a37 0e04  ..R.9././/...7..
-000000f0: cefa a06c e089 379b edcd e7bb fb7c fde1  ...l..7......|..
-00000100: fdf6 f66d bebd bddb c00a 928e 2d13 55c9  ...m........-.U.
-00000110: 29ea 2d06 4609 0fe0 2aa0 c65a 6df7 a0ea  ).-.F...*..Zm...
-00000120: dae8 a2e5 bdbc 28b1 823d 863c 9acc 2520  ......(..=.<..% 
-00000130: ddbb bca9 7367 3137 f888 66b5 55c6 e349  ....sg17..f.U..I
-00000140: 5892 24dd e023 8686 ac87 f080 316e cf49  X.$..#......1n.I
-00000150: a083 e731 a10d 506a c222 383a c24e 792c  ...1..Pj."8:.Ny,
-00000160: 8177 b551 b46f 0ebc 9e89 6081 bca1 bdef  .w.Q.o....`.....
-00000170: 69e4 99e9 8074 e79c 5982 6b0f 4a99 c535  i....t..Y.k.J..5
-00000180: dc56 704f 0d2e 8122 3173 d20c de60 a51a  .VpO..."1s...`..
-00000190: c37a 8283 3699 81b1 4f22 22f5 81ae e1be  .z..6...O"".....
-000001a0: 85e1 3c38 609e df98 cc24 c96c 763c ba3d  ..<8`....$.lv<.=
-000001b0: 5c15 02a5 6c9c 2524 15b9 df68 9325 4c8e  \...l.%$...h.%L.
-000001c0: 539e 57b0 6dd7 d842 5834 41ed 0c67 d4d2  S.W.m..BX4A..g..
-000001d0: 1f94 d575 63fa 829d f6b7 4b2b b666 26a3  ...uc.....K+.f&.
-000001e0: 8c05 5975 40a1 c946 84c5 b8bf 3b9c 2e8c  ..Yu@..F....;...
-000001f0: 6559 175e 1c2d b2a4 1780 f2a3 8791 f589  eY.^.-..........
-00000200: e28f b867 5d04 be20 5d87 7f91 7bfa ad76  ...g].. ]...{..v
-00000210: be75 9dc8 6747 3c7e 7dfd 6df1 ffc4 8fbd  .u..gG<~}.m.....
-00000220: 30ed c852 0505 ca83 e27a 16ad 9fe8 38b6  0..R.....z....8.
-00000230: c464 6f2e 7b53 6654 713f 2ca1 d206 73e1  .do.{SfTq?,...s.
-00000240: 5a9d e9ca 25f8 6657 3953 22ad faf6 4ca2  Z...%.fW9S"...L.
-00000250: 16ba 73aa 0465 4b51 f588 3457 27d0 a02d  ..s..eKQ..4W'..-
-00000260: bb8f 9d47 ae26 ad02 b69a 7b9b dd14 725f  ...G.&....{...r_
-00000270: f8a1 17da 08d1 d282 0ed4 4b49 f127 1a23  ..........KI.'.#
-00000280: dfdd 5eb1 f4de 4153 73ea 6d3a 3d62 dc23  ..^...ASs.m:=b.#
-00000290: d175 023f 7578 d0b6 9f1a 91e7 760f 748c  .u.?ux......v.t.
-000002a0: fcc1 36cc b910 5cf5 b317 cc78 9651 a1b9  ..6...\....x.Q..
-000002b0: b803 7a04 254f 479e cf8c f4dd 699b f64c  ..z.%OG.....i..L
-000002c0: cb38 e7a1 3011 facc c07f 8b1a 434d a48a  .8..0.......CM..
-000002d0: 0f4f 21f8 4bfb e0d3 086f 31a3 22a5 d9a2  .O!.K....o1."...
-000002e0: 67ee fd2a 59bf 2cfc d5d3 40fb 7cd5 3255  g..*Y.,...@.|.2U
-000002f0: aee1 b2aa c04b 11cb f355 3291 25a5 e22a  .....K...U2.%..*
-00000300: a38d a5f0 cd43 c942 ea5f cd44 351e 49db  .....C.B._.D5.I.
-00000310: ca71 f252 e9cc ab8a 3b8a 8d99 5613 5869  .q.R....;...V.Xi
-00000320: 1f8b 240e ec0d fe6e f3e5 1394 4716 c865  ..$....n....G..e
-00000330: 35e6 087c b71d e007 1ef9 3224 f472 fbea  5..|......2$.r..
-00000340: ee8a 7f69 eb11 3706 5b81 e133 4c4f 9232  ...i..7.[..3LO.2
-00000350: c14a 1733 196b 4211 11b7 acb8 95ff 7d69  .J.3.kB.......}i
-00000360: ce24 ad32 86f6 c721 61cc f4f4 3cae c85f  .$.2...!a...<.._
-00000370: 3573 89dc 48ce 79a3 48f8 57de fc8d 3106  5s..H.y.H.W...1.
-00000380: a1ec ef94 e726 4afb 2b2b 0a3b ad76 ef08  .....&J.++.;.v..
-00000390: 678c 20f5 89fd d919 0667 71c3 5bc2 f9ed  g. ......gq.[...
-000003a0: 67fd 75d3 bf7d 802b 8a86 08cb 6b78 c267  g.u..}.+....kx.g
-000003b0: 31ce 1f50 4b03 0414 0000 0008 0006 7d87  1..PK.........}.
-000003c0: 5860 0789 3d77 0000 0088 0000 0022 0000  X`..=w......."..
-000003d0: 0070 616e 6461 6c69 6273 2d30 2e31 2e32  .pandalibs-0.1.2
-000003e0: 2e64 6973 742d 696e 666f 2f4d 4554 4144  .dist-info/METAD
-000003f0: 4154 413d 8d3b 0ac3 3010 05fb 85bd c35e  ATA=.;..0......^
-00000400: c0c2 5215 d405 d23a 450c e9d7 58c4 027d  ..R....:E...X..}
-00000410: 1c69 55e8 f611 29dc ce0c ef2d 4e78 67e1  .iU...)....-Nxg.
-00000420: e9ed 4af5 3959 324a 233c 393a 4b27 a79d  ..J.9Y2J#<9:K'..
-00000430: 83df 2ac2 a567 a595 4158 5b8c 5cba a5a5  ..*..g..AX[.\...
-00000440: d339 5c4e 1c68 a465 4085 706f 72e4 6229  .9\N.h.e@.por.b)
-00000450: f9cf 21ff 1973 d333 c2cb 7d9b 2fae 4e0f  ..!..s.3..}./.N.
-00000460: 5f65 1cf4 ce31 2020 fc00 504b 0304 1400  _e...1  ..PK....
-00000470: 0000 0800 067d 8758 fc0e 7b4b 5c00 0000  .....}.X..{K\...
-00000480: 5c00 0000 1f00 0000 7061 6e64 616c 6962  \.......pandalib
-00000490: 732d 302e 312e 322e 6469 7374 2d69 6e66  s-0.1.2.dist-inf
-000004a0: 6f2f 5748 4545 4c0b cf48 4dcd d10d 4b2d  o/WHEEL..HM...K-
-000004b0: 2ace cccf b352 30d4 33e0 724f cd4b 2d4a  *....R0.3.rO.K-J
-000004c0: 2cc9 2fb2 5248 4ac9 2c2e 892f 07a9 51d0  ,./.RHJ.,../..Q.
-000004d0: 30d0 3331 d633 d0e4 0aca cf2f d1f5 2cd6  0.31.3...../..,.
-000004e0: 0d28 2d4a cdc9 4cb2 5228 292a 4de5 0a49  .(-J..L.R()*M..I
-000004f0: 4cb7 5228 a834 d6cd cbcf 4bd5 4dcc abe4  L.R(.4....K.M...
-00000500: e202 0050 4b03 0414 0000 0008 0006 7d87  ...PK.........}.
-00000510: 5829 8093 920c 0000 000a 0000 0027 0000  X)...........'..
-00000520: 0070 616e 6461 6c69 6273 2d30 2e31 2e32  .pandalibs-0.1.2
-00000530: 2e64 6973 742d 696e 666f 2f74 6f70 5f6c  .dist-info/top_l
-00000540: 6576 656c 2e74 7874 2b48 cc4b 49cc c94c  evel.txt+H.KI..L
-00000550: 2ae6 0200 504b 0304 1400 0000 0800 067d  *...PK.........}
-00000560: 8758 c53c 81ee 2f01 0000 cf01 0000 2000  .X.<../....... .
-00000570: 0000 7061 6e64 616c 6962 732d 302e 312e  ..pandalibs-0.1.
-00000580: 322e 6469 7374 2d69 6e66 6f2f 5245 434f  2.dist-info/RECO
-00000590: 5244 7dcc 4976 8230 0000 d0bd 6721 0868  RD}.Iv.0....g!.h
-000005a0: 0017 5d60 9807 1105 f1b9 c903 4935 c810  ..]`........I5..
-000005b0: 3556 e8e9 bbb2 edca 7f80 cf8a ae2a 1a5a  5V...........*.Z
-000005c0: dea7 18d3 8e72 8c45 360a f773 a140 f563  .....r.E6..s.@.c
-000005d0: ae99 56c2 6add 5d6e 0b80 53af cd01 f411  ..V.j.]n..S.....
-000005e0: 7924 6473 69e1 2a62 7e7e 7066 e7ed c3ce  y$dsi.*b~~pf....
-000005f0: 0469 c27e abb1 681b 4c5b d6df 38b9 fdfb  .i.~..h.L[..8...
-00000600: e063 f03d cb65 115e 19bb 1520 718a b43a  .c.=.e.^... q..:
-00000610: e672 525f 911b 7e9f d7e0 7ea8 7743 2c3d  .rR_..~...~.wC,=
-00000620: 2d41 51b4 f95f 0924 5116 15b1 a277 0e68  -AQ.._.$Q....w.h
-00000630: f7d9 4f23 2b35 4c23 355e f5d5 19aa 967a  ..O#+5L#5^.....z
-00000640: 5617 c8cd 4c1b b3d1 bcf0 2c2d ede5 703c  V...L.....,-..p<
-00000650: aab5 afed 01b9 fa71 646f b6ba 20cf d437  .......qdo.. ..7
-00000660: 73ee 5a56 f86a 1d5f e3f8 922f edf1 5916  s.ZV.j._.../..Y.
-00000670: a700 927e e1f5 d933 ccd5 7e8c 491a b409  ...~...3..~.I...
-00000680: 5850 d7de ad86 4458 286f 56de 33dc 902f  XP....DX(oV.3../
-00000690: d288 7ce0 afdd af48 e0d4 a4d1 21cc 698e  ..|....H....!.i.
-000006a0: 607f 8261 0900 72f4 d91e 9dfc 7590 29e8  `..a..r.....u.).
-000006b0: 11a1 a466 9120 4b6f f68d 85e2 8d29 0893  ...f. Ko.....)..
-000006c0: 1f50 4b01 0214 0014 0000 0008 001c 7087  .PK...........p.
-000006d0: 5800 0000 0002 0000 0000 0000 0015 0000  X...............
-000006e0: 0000 0000 0000 0000 00b6 8100 0000 0070  ...............p
-000006f0: 616e 6461 6c69 6273 2f5f 5f69 6e69 745f  andalibs/__init_
-00000700: 5f2e 7079 504b 0102 1400 1400 0000 0800  _.pyPK..........
-00000710: ad7c 8758 58f1 6794 4603 0000 e208 0000  .|.XX.g.F.......
-00000720: 1a00 0000 0000 0000 0000 0000 b681 3500  ..............5.
-00000730: 0000 7061 6e64 616c 6962 732f 7961 6d6c  ..pandalibs/yaml
-00000740: 5f69 6d70 6f72 7465 722e 7079 504b 0102  _importer.pyPK..
-00000750: 1400 1400 0000 0800 067d 8758 6007 893d  .........}.X`..=
-00000760: 7700 0000 8800 0000 2200 0000 0000 0000  w.......".......
-00000770: 0000 0000 b681 b303 0000 7061 6e64 616c  ..........pandal
-00000780: 6962 732d 302e 312e 322e 6469 7374 2d69  ibs-0.1.2.dist-i
-00000790: 6e66 6f2f 4d45 5441 4441 5441 504b 0102  nfo/METADATAPK..
-000007a0: 1400 1400 0000 0800 067d 8758 fc0e 7b4b  .........}.X..{K
-000007b0: 5c00 0000 5c00 0000 1f00 0000 0000 0000  \...\...........
-000007c0: 0000 0000 b681 6a04 0000 7061 6e64 616c  ......j...pandal
-000007d0: 6962 732d 302e 312e 322e 6469 7374 2d69  ibs-0.1.2.dist-i
-000007e0: 6e66 6f2f 5748 4545 4c50 4b01 0214 0014  nfo/WHEELPK.....
-000007f0: 0000 0008 0006 7d87 5829 8093 920c 0000  ......}.X)......
-00000800: 000a 0000 0027 0000 0000 0000 0000 0000  .....'..........
-00000810: 00b6 8103 0500 0070 616e 6461 6c69 6273  .......pandalibs
-00000820: 2d30 2e31 2e32 2e64 6973 742d 696e 666f  -0.1.2.dist-info
-00000830: 2f74 6f70 5f6c 6576 656c 2e74 7874 504b  /top_level.txtPK
-00000840: 0102 1400 1400 0000 0800 067d 8758 c53c  ...........}.X.<
-00000850: 81ee 2f01 0000 cf01 0000 2000 0000 0000  ../....... .....
-00000860: 0000 0000 0000 b481 5405 0000 7061 6e64  ........T...pand
-00000870: 616c 6962 732d 302e 312e 322e 6469 7374  alibs-0.1.2.dist
-00000880: 2d69 6e66 6f2f 5245 434f 5244 504b 0506  -info/RECORDPK..
-00000890: 0000 0000 0600 0600 cb01 0000 c106 0000  ................
-000008a0: 0000                                     ..
+00000000: 1f8b 0808 aee9 1266 02ff 7061 6e64 616c  .......f..pandal
+00000010: 6962 732d 302e 312e 332e 7461 7200 ed5d  ibs-0.1.3.tar..]
+00000020: 596f db48 12f6 b300 fd87 06f3 1069 56a1  Yo.H.........iV.
+00000030: 7849 7204 0858 c3b1 33c1 e442 9c2c b0c8  xIr..X..3..B.,..
+00000040: 1a44 4b6c cabd a1d8 dcee 666c 6d90 ffbe  .DKl......flm...
+00000050: d53c 244a 9632 9bc4 d660 c6f5 f9c1 24fb  .<$J.2...`....$.
+00000060: aa66 57d5 57c5 4b76 dfee fffd 2dbd f995  .fW.W.Kv....-...
+00000070: d188 c9a3 7b81 5362 df7f c7f1 83f5 b639  ....{.Sb.......9
+00000080: ee3a 9eeb 1d91 9ba3 0320 579a 4a18 fee8  .:....... W.J...
+00000090: 61c2 3b26 0bcd 176c e28e 5c6f e00e 068e  a.;&...l..\o....
+000000a0: 670f 7ddf 77dc 41eb 08f1 9747 46d3 8826  g.}.w.A....GF..&
+000000b0: 7caa 9e38 b66b fbfd fbb2 ffd1 68b4 dffe  |..8.k......h...
+000000c0: 61db 0d86 4e30 1806 c3c1 c8d8 7fe0 f947  a...N0.........G
+000000d0: 6480 f67f efb0 d1ff a3ff 47ff 8ffe bff2  d.........G.....
+000000e0: ff6f 7f7b fee4 c5eb f337 776d ffc3 e170  .o.{.....7wm...p
+000000f0: affd bbe0 f337 fdbf 3b30 fedf 41fb bf77  .....7..;0..A..w
+00000100: bc62 9a46 54d3 27ff 6052 7191 8e89 67bb  .b.FT.'.`Rq...g.
+00000110: edd6 6bba 6063 b252 8e76 6b55 5ca8 49bb  ..k.`c.R.vkU\.I.
+00000120: 7591 2f16 542e c7e4 d592 6450 2652 9a10  u./.T.....dP&R..
+00000130: a82a e1a0 dd6e 9de4 fa4a c831 49f9 fc4a  .*...n...J.1I..J
+00000140: 17dd 78c7 aed3 4697 82fc bf83 ffbd e16d  ..x...F........m
+00000150: fef7 91ff 0fc2 ff5e 93ff 6129 9e8e 6c07  .......^..a)..l.
+00000160: cdf4 c1f2 ffbb b393 67af ceec 4574 48fe  ........g...EtH.
+00000170: f7fd 8aff bd91 ebba 86ff 4d18 80fc 7f00  ..........M.....
+00000180: 3c22 bf8a 6ba2 05f9 a058 bb95 f18c f014  <"..k....X......
+00000190: ce48 9290 39d7 7fbb d23a 53e3 7e1f b6af  .H..9....:S.~...
+000001a0: f2a9 3d13 8bfe 26a3 f7df 9aad 97a0 3f36  ..=...&.......?6
+000001b0: d479 c4e6 f3c9 4aa3 d0b8 90ff 31ff ff33  .y....J.....1..3
+000001c0: e6ff de53 6f14 b818 053c 40fe 5fed f7ef  ...So....<@._...
+000001d0: d6fe bfef faaf e70f 1dbc fe8b f91f aeff  ................
+000001e0: 41f3 bfe0 e931 d820 e67f e8ff c1ff 8721  A....1. .......!
+000001f0: 4fb9 0e43 3b5b de73 feb7 f6ff 9e1f f8c6  O..C;[.s........
+00000200: fe83 c0c7 fc0f fd3f aeff 61fd ffc0 f59c  .......?..a.....
+00000210: c047 ff8f fe1f fc7f 9649 9eea 3015 4a48  .G.......I..0.JH
+00000220: fd53 24f0 7bfe dff3 eafb 7f83 a133 f0c1  .S$.{........3..
+00000230: fe21 11f0 d0ff 1f02 7c91 c1f2 9272 b1db  .!......|....r..
+00000240: 2df3 17b1 18f6 3be6 ae60 8ffc f2cb a76b  -.....;..`.....k
+00000250: 2ae7 aa3b 6eb7 08c0 b2ac 8b2b 6831 cb35  *..;n......+h1.5
+00000260: 8985 ac1a 926b aeaf 8851 149e ce49 c415  .....k...Q...I..
+00000270: 9d26 2cb2 a172 d9aa ac65 97ff aa9e 4ded  .&,..r...e....M.
+00000280: 30e2 33ad 26e7 3451 ac31 16de 2744 fe47  0.3.&.4Q.1..'D.G
+00000290: feff 03f8 df09 bc00 f33f e47f c3ff 4bba  .........?....K.
+000002a0: 48c2 921e 98bc 4ffe 0f7c 20fb 92ff fd61  H.....O..| ....a
+000002b0: 510f f8df c5fc ef90 fc2f 54bb 556d aae5  Q......../T.Um..
+000002c0: 7adb e840 1914 3c22 a770 a6c4 82b0 9b19  z..@..<".p......
+000002d0: cb34 1769 41ff 3391 c67c 9e4b 5a1c 6152  .4.iA.3..|.KZ.aR
+000002e0: 0a09 ad67 0955 8a9c 36cb ce4c 51e7 ac6e  ...g.U..6..LQ..n
+000002f0: 5c87 1319 545c 0d20 cc9d c754 c381 6767  \...T\. ...T..gg
+00000300: e727 1f5e be0f 4fdf bc3e 7ff1 3c3c 7ff1  .'.^..O..>..<<..
+00000310: f28c 4c88 558e 661b a9ac bad5 7306 d10b  ..L.U.f.....s...
+00000320: 85e8 43c4 44e6 696a 0210 9a65 099f 15e3  ..C.D.ij...e....
+00000330: 96e1 cc9c e9b0 7130 340d 3a73 11e6 5928  ......q04.:s..Y(
+00000340: 5216 26ec 334b ca28 a411 e794 1bef 98ce  R.&.3K.(........
+00000350: 65aa 88be 62cd 7eab 3125 e15a c1b6 6410  e...b.~.1%.Z..d.
+00000360: 0445 5cb2 9916 7249 a654 b188 40ad a295  .E\...rI.T..@...
+00000370: 9ce7 0b28 b78d c0a6 cb13 8871 aa61 0cb6  ...(.......q.a..
+00000380: e420 9da9 1049 8f88 e244 d1a4 3b26 2f62  . ...I...D..;&/b
+00000390: f25e e610 21c9 8630 db83 dae4 198b 699e  .^..!..0......i.
+000003a0: 803c 5a90 6232 ab11 ab49 3406 555a 8ec9  .<Z.b2...I4.UZ..
+000003b0: fba2 1b98 0734 d89e df7a 321b 93b4 b74e  .....4...z2....N
+000003c0: 0f2f 4e2e d55a 7640 717a c48a a5f8 2f4b  ./N..Zv@qz..../K
+000003d0: ad1e d938 9d06 8fc8 7951 062a c420 7c34  ...8....yQ.*. |4
+000003e0: 2162 af1c 7e41 539e e549 b560 75fd a268  !b..~AS..I.`u..h
+000003f0: 02aa 699b 2d1b 044a e982 9961 ec75 0fdd  ..i.-..J...a.u..
+00000400: 75fd f2e4 94cd 40ac 54e8 5ba7 9681 48b7  u.....@.T.[...H.
+00000410: 3a34 3b55 37a6 7c43 e277 6c0e 7249 a266  :4;U7.|C.wl.rI.f
+00000420: 9267 fa47 c4ad f7e9 5415 5a67 c407 8df8  .g.G....T.Zg....
+00000430: fcd1 b9ec de9d f06b 5bd8 b448 136a 13aa  .......k[..H.j..
+00000440: 0825 26d2 36fa 2497 6b93 d8a8 1b9a ba1d  .%&.6.$.k.......
+00000450: 1891 36ed a147 629e b0d0 8c35 d961 9510  ..6..Gb....5.a..
+00000460: c6e7 d358 2410 3b4e 2af3 b41a 26f4 52d0  ...X$.;N*...&.R.
+00000470: 8800 a318 a93e 33b9 2d9d e99a 4046 208c  .....>3.-...@F .
+00000480: e649 01d9 01d5 ac90 b952 b393 99f1 176a  .I.......R.....j
+00000490: 650b 450b 234b d1e9 6ae8 9e99 e235 4b12  e.E.#K..j....5K.
+000004a0: f3bf ac6b 547a 2e48 9ec1 d48b e954 3d36  ...kTz.H.....T=6
+000004b0: 6da4 e14e 8a04 86a7 d5a1 75cf dbea aee5  m..N......u.....
+000004c0: b2a1 1fa0 8690 c148 58f5 9d0e 667d 2e1b  .......HX...f}..
+000004d0: 0b0d 8bbb eabd d195 4139 78b8 a548 ff16  ........A9x..H..
+000004e0: 3ced 5423 f59a 735e 2d4c a3f7 2d05 fe7f  <.T#..s^-L..-...
+000004f0: 7b6d 76b5 21aa d1c3 ba09 bbe1 4aab 4ea3  {mv.!.......J.N.
+00000500: bfee d650 9272 50d1 1d7e 3fb6 4e6f 2ffc  ...P.rP..~?.No/.
+00000510: e32f ab61 bf3e 2e46 8a45 0ecb 4a35 1435  ./.a.>.F.E..J5.5
+00000520: 46f9 fad8 da10 abc8 3545 c6d2 a628 e079  F.......5E...(.y
+00000530: a4d5 35eb 1f6f 0995 2b06 5967 2c60 f266  ..5..o..+.Yg,`.f
+00000540: a56d 4563 b028 50cc 4ebc d1ad 319f 9449  .mEc.(P.N...1..I
+00000550: a381 9582 ff76 f6cf 0b12 2d41 4058 d624  .....v....-A@X.$
+00000560: 5912 f06d 0bf2 892d c119 4aa6 8cf7 e5a5  Y..m...-..J.....
+00000570: 8bbf add6 eb7e 9b9d 4d48 02e7 b053 8b64  .....~..MH...S.d
+00000580: 9bbe 3add 2d31 4e25 3342 344d d668 2bb0  ..:.-1N%3B4M.h+.
+00000590: af64 3bcc 7bdd b43a 1da6 198c f4e5 ebba  .d;.{..:........
+000005a0: c450 358c 65c4 6d88 b35b 514c f38f 50f9  .P5.e.m..[QL..P.
+000005b0: 12fa 5809 0afa dd81 631b 9256 2eab d1ac  ..X.....c..V....
+000005c0: 2e2d 6384 1d8a 60d6 a7a9 9fa5 c2b0 ad76  .-c...`........v
+000005d0: ab28 6177 f59d fa75 5245 1f44 cc66 b994  .(aw...uRE.D.f..
+000005e0: 2c1a 932f ecab 8597 12fe 0cf9 3f3e fff3  ,../........?>..
+000005f0: c7e5 ff3b dfff f1bc a7c7 23b4 9c87 9cff  ...;......#.....
+00000600: db6c 3e7f 627c 7fff 4eec fffb 9eff 099c  .l>.b|..N.......
+00000610: 8187 cfff e0f5 5f5c ffc3 5eff 2dfd 3f5e  ......_\..^.-.?^
+00000620: ff45 ffdf f0ff 3ffd 4ae8 f7bd ff59 5cff  .E....?.J....Y\.
+00000630: 853f bcfe 7b08 e0fb 9f98 ff21 ff23 ff23  .?..{......!.#.#
+00000640: ff23 ffef e1ff 8b37 1fde 9d9e 5dd8 fa46  .#.....7....]..F
+00000650: df0f ff07 8eb7 cdff 231f f9ff 2058 bdef  ........#... X..
+00000660: db52 4ce7 999d 2d5b 3b1f 016f ed7f 30b0  .RL...-[;..o..0.
+00000670: b5ff 9981 d637 c2c9 d6b7 556d 5771 c432  .....7....UmWq.2
+00000680: 9646 2c9d 2dc3 84a7 9fd4 be7a 92fd 27e7  .F,.-......z..'.
+00000690: 92ed 2dd7 222b efcb fcb8 4e23 ff23 ff23  ..-."+....N#.#.#
+000006a0: ff23 1e00 ffef f2ba 77ca ff8e e36e f2bf  .#......w....n..
+000006b0: e7b8 f8fc d761 80a6 8efc 8ffc 8ffc 8ffc  .....a..........
+000006c0: 8ffc bf87 ff9b d9d4 bde4 ff8e b37d fd7f  .............}..
+000006d0: 1804 43e4 ff83 acff d2e4 ec68 f0c8 ffc8  ..C........h....
+000006e0: ffc8 ffc8 ffc8 ff77 7fb5 f477 f9df ddbe  .......w...w....
+000006f0: fe3f 1c8c 02e4 ff83 ae3f da3c f23f 3eff  .?.......?.<.?>.
+00000700: fdf0 f81f 7fff 01f9 bfc1 ffe5 5de0 593c  ............].Y<
+00000710: bf63 fbff 26ff 0fbc edef 3f7a 01de ff3f  .c..&.....?z...?
+00000720: 083e 4298 179a 30ef b2dd d274 1e4e 739e  .>B...0....t.Ns.
+00000730: 4464 42ca bdc8 bc88 3621 8e79 410b 6d05  DdB.....6!.yA.m.
+00000740: f91f f3ff bf78 feef 39a3 63cc ff1f 3cff  .....x..9.c...<.
+00000750: fff4 273f bf8b ff07 a3e1 eafb 6fae 6bf2  ..'?........o.k.
+00000760: 7f30 7fcc ff0f 82e2 95f6 62d1 b510 8922  .0........b...."
+00000770: d587 5f62 9e46 6146 679f e89c a95e 59c1  .._b.FaFg....^Y.
+00000780: 0401 c546 a77c 23bb f826 84b5 5220 ab57  ...F.|#..&..R .W
+00000790: 7fd2 a56c 35d9 e8a3 c3d3 5992 476c f2b1  ...l5.....Y.Gl..
+000007a0: d1e2 b25b b5f9 5cbe 5d30 b10a 25ac 7b8a  ...[..\.]0..%.{.
+000007b0: 58f9 d98d a264 d77b 0675 455a bc6d 30b1  X....d.{.uEZ.m0.
+000007c0: 36df 36a8 4bab 1fb4 08eb fb58 4684 e2ae  6.6.K......XF...
+000007d0: 8775 59d5 2866 d528 af8f 6ba6 b4aa 8f6f  .uY.(f.(..k....o
+000007e0: 1e0e 55ce 354c bfa8 6246 ea96 9fe0 a87e  ..U.5L..bF.....~
+000007f0: 4d43 e6e9 d8ec 664b 902c 25f6 bf6a bb22  MC....fK.,%..j."
+00000800: d388 43eb eb2b c612 8ca9 1008 0402 8140  ..C..+.........@
+00000810: 2010 0804 0281 4020 1008 0402 8140 2010   .....@ .....@ .
+00000820: 0804 0281 4020 1008 0402 8140 fc08 fe07  ....@ .....@....
+00000830: 29f6 6357 00a0 0000                      ).cW....
```

## Comparing `tmp/pandalibs-0.1.2-py3-none-any.whl.zip` & `tmp/pandalibs-0.1.3.tar.gz`

```diff
@@ -1,139 +1,132 @@
-00000000: 504b 0304 1400 0000 0800 1c70 8758 0000  PK.........p.X..
-00000010: 0000 0200 0000 0000 0000 1500 0000 7061  ..............pa
-00000020: 6e64 616c 6962 732f 5f5f 696e 6974 5f5f  ndalibs/__init__
-00000030: 2e70 7903 0050 4b03 0414 0000 0008 00ad  .py..PK.........
-00000040: 7c87 5858 f167 9446 0300 00e2 0800 001a  |.XX.g.F........
-00000050: 0000 0070 616e 6461 6c69 6273 2f79 616d  ...pandalibs/yam
-00000060: 6c5f 696d 706f 7274 6572 2e70 79ad 56c1  l_importer.py.V.
-00000070: 8adb 3010 bd2f ec3f 0cee 611d 08a6 e785  ..0../.?..a.....
-00000080: 1c96 3429 4b97 16da eda1 9462 147b 9c55  ..4)K......b.{.U
-00000090: ab48 6624 6f9b 2efb ef9d b11d 5bf6 e650  .Hf$o.......[..P
-000000a0: 4a9d 4314 49f3 de1b cd1b c5fa 503b 0ae0  J.C.I.......P;..
-000000b0: fce5 85ee 86fe 388e 8fea 602e 2fe4 f30a  ......8...`./...
-000000c0: d68d 0fee 00f8 abc0 3a68 67a1 7204 85b3  ........:hg.r...
-000000d0: 95de 37a4 da19 2472 c4d1 8551 dec3 3a5e  ..7...$r...Q..:^
-000000e0: dbc8 52ba 3905 2fae 2f2f 809f 9a37 0e04  ..R.9././/...7..
-000000f0: cefa a06c e089 379b edcd e7bb fb7c fde1  ...l..7......|..
-00000100: fdf6 f66d bebd bddb c00a 928e 2d13 55c9  ...m........-.U.
-00000110: 29ea 2d06 4609 0fe0 2aa0 c65a 6df7 a0ea  ).-.F...*..Zm...
-00000120: dae8 a2e5 bdbc 28b1 823d 863c 9acc 2520  ......(..=.<..% 
-00000130: ddbb bca9 7367 3137 f888 66b5 55c6 e349  ....sg17..f.U..I
-00000140: 5892 24dd e023 8686 ac87 f080 316e cf49  X.$..#......1n.I
-00000150: a083 e731 a10d 506a c222 383a c24e 792c  ...1..Pj."8:.Ny,
-00000160: 8177 b551 b46f 0ebc 9e89 6081 bca1 bdef  .w.Q.o....`.....
-00000170: 69e4 99e9 8074 e79c 5982 6b0f 4a99 c535  i....t..Y.k.J..5
-00000180: dc56 704f 0d2e 8122 3173 d20c de60 a51a  .VpO..."1s...`..
-00000190: c37a 8283 3699 81b1 4f22 22f5 81ae e1be  .z..6...O"".....
-000001a0: 85e1 3c38 609e df98 cc24 c96c 763c ba3d  ..<8`....$.lv<.=
-000001b0: 5c15 02a5 6c9c 2524 15b9 df68 9325 4c8e  \...l.%$...h.%L.
-000001c0: 539e 57b0 6dd7 d842 5834 41ed 0c67 d4d2  S.W.m..BX4A..g..
-000001d0: 1f94 d575 63fa 829d f6b7 4b2b b666 26a3  ...uc.....K+.f&.
-000001e0: 8c05 5975 40a1 c946 84c5 b8bf 3b9c 2e8c  ..Yu@..F....;...
-000001f0: 6559 175e 1c2d b2a4 1780 f2a3 8791 f589  eY.^.-..........
-00000200: e28f b867 5d04 be20 5d87 7f91 7bfa ad76  ...g].. ]...{..v
-00000210: be75 9dc8 6747 3c7e 7dfd 6df1 ffc4 8fbd  .u..gG<~}.m.....
-00000220: 30ed c852 0505 ca83 e27a 16ad 9fe8 38b6  0..R.....z....8.
-00000230: c464 6f2e 7b53 6654 713f 2ca1 d206 73e1  .do.{SfTq?,...s.
-00000240: 5a9d e9ca 25f8 6657 3953 22ad faf6 4ca2  Z...%.fW9S"...L.
-00000250: 16ba 73aa 0465 4b51 f588 3457 27d0 a02d  ..s..eKQ..4W'..-
-00000260: bb8f 9d47 ae26 ad02 b69a 7b9b dd14 725f  ...G.&....{...r_
-00000270: f8a1 17da 08d1 d282 0ed4 4b49 f127 1a23  ..........KI.'.#
-00000280: dfdd 5eb1 f4de 4153 73ea 6d3a 3d62 dc23  ..^...ASs.m:=b.#
-00000290: d175 023f 7578 d0b6 9f1a 91e7 760f 748c  .u.?ux......v.t.
-000002a0: fcc1 36cc b910 5cf5 b317 cc78 9651 a1b9  ..6...\....x.Q..
-000002b0: b803 7a04 254f 479e cf8c f4dd 699b f64c  ..z.%OG.....i..L
-000002c0: cb38 e7a1 3011 facc c07f 8b1a 434d a48a  .8..0.......CM..
-000002d0: 0f4f 21f8 4bfb e0d3 086f 31a3 22a5 d9a2  .O!.K....o1."...
-000002e0: 67ee fd2a 59bf 2cfc d5d3 40fb 7cd5 3255  g..*Y.,...@.|.2U
-000002f0: aee1 b2aa c04b 11cb f355 3291 25a5 e22a  .....K...U2.%..*
-00000300: a38d a5f0 cd43 c942 ea5f cd44 351e 49db  .....C.B._.D5.I.
-00000310: ca71 f252 e9cc ab8a 3b8a 8d99 5613 5869  .q.R....;...V.Xi
-00000320: 1f8b 240e ec0d fe6e f3e5 1394 4716 c865  ..$....n....G..e
-00000330: 35e6 087c b71d e007 1ef9 3224 f472 fbea  5..|......2$.r..
-00000340: ee8a 7f69 eb11 3706 5b81 e133 4c4f 9232  ...i..7.[..3LO.2
-00000350: c14a 1733 196b 4211 11b7 acb8 95ff 7d69  .J.3.kB.......}i
-00000360: ce24 ad32 86f6 c721 61cc f4f4 3cae c85f  .$.2...!a...<.._
-00000370: 3573 89dc 48ce 79a3 48f8 57de fc8d 3106  5s..H.y.H.W...1.
-00000380: a1ec ef94 e726 4afb 2b2b 0a3b ad76 ef08  .....&J.++.;.v..
-00000390: 678c 20f5 89fd d919 0667 71c3 5bc2 f9ed  g. ......gq.[...
-000003a0: 67fd 75d3 bf7d 802b 8a86 08cb 6b78 c267  g.u..}.+....kx.g
-000003b0: 31ce 1f50 4b03 0414 0000 0008 0006 7d87  1..PK.........}.
-000003c0: 5860 0789 3d77 0000 0088 0000 0022 0000  X`..=w......."..
-000003d0: 0070 616e 6461 6c69 6273 2d30 2e31 2e32  .pandalibs-0.1.2
-000003e0: 2e64 6973 742d 696e 666f 2f4d 4554 4144  .dist-info/METAD
-000003f0: 4154 413d 8d3b 0ac3 3010 05fb 85bd c35e  ATA=.;..0......^
-00000400: c0c2 5215 d405 d23a 450c e9d7 58c4 027d  ..R....:E...X..}
-00000410: 1c69 55e8 f611 29dc ce0c ef2d 4e78 67e1  .iU...)....-Nxg.
-00000420: e9ed 4af5 3959 324a 233c 393a 4b27 a79d  ..J.9Y2J#<9:K'..
-00000430: 83df 2ac2 a567 a595 4158 5b8c 5cba a5a5  ..*..g..AX[.\...
-00000440: d339 5c4e 1c68 a465 4085 706f 72e4 6229  .9\N.h.e@.por.b)
-00000450: f9cf 21ff 1973 d333 c2cb 7d9b 2fae 4e0f  ..!..s.3..}./.N.
-00000460: 5f65 1cf4 ce31 2020 fc00 504b 0304 1400  _e...1  ..PK....
-00000470: 0000 0800 067d 8758 fc0e 7b4b 5c00 0000  .....}.X..{K\...
-00000480: 5c00 0000 1f00 0000 7061 6e64 616c 6962  \.......pandalib
-00000490: 732d 302e 312e 322e 6469 7374 2d69 6e66  s-0.1.2.dist-inf
-000004a0: 6f2f 5748 4545 4c0b cf48 4dcd d10d 4b2d  o/WHEEL..HM...K-
-000004b0: 2ace cccf b352 30d4 33e0 724f cd4b 2d4a  *....R0.3.rO.K-J
-000004c0: 2cc9 2fb2 5248 4ac9 2c2e 892f 07a9 51d0  ,./.RHJ.,../..Q.
-000004d0: 30d0 3331 d633 d0e4 0aca cf2f d1f5 2cd6  0.31.3...../..,.
-000004e0: 0d28 2d4a cdc9 4cb2 5228 292a 4de5 0a49  .(-J..L.R()*M..I
-000004f0: 4cb7 5228 a834 d6cd cbcf 4bd5 4dcc abe4  L.R(.4....K.M...
-00000500: e202 0050 4b03 0414 0000 0008 0006 7d87  ...PK.........}.
-00000510: 5829 8093 920c 0000 000a 0000 0027 0000  X)...........'..
-00000520: 0070 616e 6461 6c69 6273 2d30 2e31 2e32  .pandalibs-0.1.2
-00000530: 2e64 6973 742d 696e 666f 2f74 6f70 5f6c  .dist-info/top_l
-00000540: 6576 656c 2e74 7874 2b48 cc4b 49cc c94c  evel.txt+H.KI..L
-00000550: 2ae6 0200 504b 0304 1400 0000 0800 067d  *...PK.........}
-00000560: 8758 c53c 81ee 2f01 0000 cf01 0000 2000  .X.<../....... .
-00000570: 0000 7061 6e64 616c 6962 732d 302e 312e  ..pandalibs-0.1.
-00000580: 322e 6469 7374 2d69 6e66 6f2f 5245 434f  2.dist-info/RECO
-00000590: 5244 7dcc 4976 8230 0000 d0bd 6721 0868  RD}.Iv.0....g!.h
-000005a0: 0017 5d60 9807 1105 f1b9 c903 4935 c810  ..]`........I5..
-000005b0: 3556 e8e9 bbb2 edca 7f80 cf8a ae2a 1a5a  5V...........*.Z
-000005c0: dea7 18d3 8e72 8c45 360a f773 a140 f563  .....r.E6..s.@.c
-000005d0: ae99 56c2 6add 5d6e 0b80 53af cd01 f411  ..V.j.]n..S.....
-000005e0: 7924 6473 69e1 2a62 7e7e 7066 e7ed c3ce  y$dsi.*b~~pf....
-000005f0: 0469 c27e abb1 681b 4c5b d6df 38b9 fdfb  .i.~..h.L[..8...
-00000600: e063 f03d cb65 115e 19bb 1520 718a b43a  .c.=.e.^... q..:
-00000610: e672 525f 911b 7e9f d7e0 7ea8 7743 2c3d  .rR_..~...~.wC,=
-00000620: 2d41 51b4 f95f 0924 5116 15b1 a277 0e68  -AQ.._.$Q....w.h
-00000630: f7d9 4f23 2b35 4c23 355e f5d5 19aa 967a  ..O#+5L#5^.....z
-00000640: 5617 c8cd 4c1b b3d1 bcf0 2c2d ede5 703c  V...L.....,-..p<
-00000650: aab5 afed 01b9 fa71 646f b6ba 20cf d437  .......qdo.. ..7
-00000660: 73ee 5a56 f86a 1d5f e3f8 922f edf1 5916  s.ZV.j._.../..Y.
-00000670: a700 927e e1f5 d933 ccd5 7e8c 491a b409  ...~...3..~.I...
-00000680: 5850 d7de ad86 4458 286f 56de 33dc 902f  XP....DX(oV.3../
-00000690: d288 7ce0 afdd af48 e0d4 a4d1 21cc 698e  ..|....H....!.i.
-000006a0: 607f 8261 0900 72f4 d91e 9dfc 7590 29e8  `..a..r.....u.).
-000006b0: 11a1 a466 9120 4b6f f68d 85e2 8d29 0893  ...f. Ko.....)..
-000006c0: 1f50 4b01 0214 0014 0000 0008 001c 7087  .PK...........p.
-000006d0: 5800 0000 0002 0000 0000 0000 0015 0000  X...............
-000006e0: 0000 0000 0000 0000 00b6 8100 0000 0070  ...............p
-000006f0: 616e 6461 6c69 6273 2f5f 5f69 6e69 745f  andalibs/__init_
-00000700: 5f2e 7079 504b 0102 1400 1400 0000 0800  _.pyPK..........
-00000710: ad7c 8758 58f1 6794 4603 0000 e208 0000  .|.XX.g.F.......
-00000720: 1a00 0000 0000 0000 0000 0000 b681 3500  ..............5.
-00000730: 0000 7061 6e64 616c 6962 732f 7961 6d6c  ..pandalibs/yaml
-00000740: 5f69 6d70 6f72 7465 722e 7079 504b 0102  _importer.pyPK..
-00000750: 1400 1400 0000 0800 067d 8758 6007 893d  .........}.X`..=
-00000760: 7700 0000 8800 0000 2200 0000 0000 0000  w.......".......
-00000770: 0000 0000 b681 b303 0000 7061 6e64 616c  ..........pandal
-00000780: 6962 732d 302e 312e 322e 6469 7374 2d69  ibs-0.1.2.dist-i
-00000790: 6e66 6f2f 4d45 5441 4441 5441 504b 0102  nfo/METADATAPK..
-000007a0: 1400 1400 0000 0800 067d 8758 fc0e 7b4b  .........}.X..{K
-000007b0: 5c00 0000 5c00 0000 1f00 0000 0000 0000  \...\...........
-000007c0: 0000 0000 b681 6a04 0000 7061 6e64 616c  ......j...pandal
-000007d0: 6962 732d 302e 312e 322e 6469 7374 2d69  ibs-0.1.2.dist-i
-000007e0: 6e66 6f2f 5748 4545 4c50 4b01 0214 0014  nfo/WHEELPK.....
-000007f0: 0000 0008 0006 7d87 5829 8093 920c 0000  ......}.X)......
-00000800: 000a 0000 0027 0000 0000 0000 0000 0000  .....'..........
-00000810: 00b6 8103 0500 0070 616e 6461 6c69 6273  .......pandalibs
-00000820: 2d30 2e31 2e32 2e64 6973 742d 696e 666f  -0.1.2.dist-info
-00000830: 2f74 6f70 5f6c 6576 656c 2e74 7874 504b  /top_level.txtPK
-00000840: 0102 1400 1400 0000 0800 067d 8758 c53c  ...........}.X.<
-00000850: 81ee 2f01 0000 cf01 0000 2000 0000 0000  ../....... .....
-00000860: 0000 0000 0000 b481 5405 0000 7061 6e64  ........T...pand
-00000870: 616c 6962 732d 302e 312e 322e 6469 7374  alibs-0.1.2.dist
-00000880: 2d69 6e66 6f2f 5245 434f 5244 504b 0506  -info/RECORDPK..
-00000890: 0000 0000 0600 0600 cb01 0000 c106 0000  ................
-000008a0: 0000                                     ..
+00000000: 1f8b 0808 aee9 1266 02ff 7061 6e64 616c  .......f..pandal
+00000010: 6962 732d 302e 312e 332e 7461 7200 ed5d  ibs-0.1.3.tar..]
+00000020: 596f db48 12f6 b300 fd87 06f3 1069 56a1  Yo.H.........iV.
+00000030: 7849 7204 0858 c3b1 33c1 e442 9c2c b0c8  xIr..X..3..B.,..
+00000040: 1a44 4b6c cabd a1d8 dcee 666c 6d90 ffbe  .DKl......flm...
+00000050: d53c 244a 9632 9bc4 d660 c6f5 f9c1 24fb  .<$J.2...`....$.
+00000060: aa66 57d5 57c5 4b76 dfee fffd 2dbd f995  .fW.W.Kv....-...
+00000070: d188 c9a3 7b81 5362 df7f c7f1 83f5 b639  ....{.Sb.......9
+00000080: ee3a 9eeb 1d91 9ba3 0320 579a 4a18 fee8  .:....... W.J...
+00000090: 61c2 3b26 0bcd 176c e28e 5c6f e00e 068e  a.;&...l..\o....
+000000a0: 670f 7ddf 77dc 41eb 08f1 9747 46d3 8826  g.}.w.A....GF..&
+000000b0: 7caa 9e38 b66b fbfd fbb2 ffd1 68b4 dffe  |..8.k......h...
+000000c0: 61db 0d86 4e30 1806 c3c1 c8d8 7fe0 f947  a...N0.........G
+000000d0: 6480 f67f efb0 d1ff a3ff 47ff 8ffe bff2  d.........G.....
+000000e0: ff6f 7f7b fee4 c5eb f337 776d ffc3 e170  .o.{.....7wm...p
+000000f0: affd bbe0 f337 fdbf 3b30 fedf 41fb bf77  .....7..;0..A..w
+00000100: bc62 9a46 54d3 27ff 6052 7191 8e89 67bb  .b.FT.'.`Rq...g.
+00000110: edd6 6bba 6063 b252 8e76 6b55 5ca8 49bb  ..k.`c.R.vkU\.I.
+00000120: 7591 2f16 542e c7e4 d592 6450 2652 9a10  u./.T.....dP&R..
+00000130: a82a e1a0 dd6e 9de4 fa4a c831 49f9 fc4a  .*...n...J.1I..J
+00000140: 17dd 78c7 aed3 4697 82fc bf83 ffbd e16d  ..x...F........m
+00000150: fef7 91ff 0fc2 ff5e 93ff 6129 9e8e 6c07  .......^..a)..l.
+00000160: cdf4 c1f2 ffbb b393 67af ceec 4574 48fe  ........g...EtH.
+00000170: f7fd 8aff bd91 ebba 86ff 4d18 80fc 7f00  ..........M.....
+00000180: 3c22 bf8a 6ba2 05f9 a058 bb95 f18c f014  <"..k....X......
+00000190: ce48 9290 39d7 7fbb d23a 53e3 7e1f b6af  .H..9....:S.~...
+000001a0: f2a9 3d13 8bfe 26a3 f7df 9aad 97a0 3f36  ..=...&.......?6
+000001b0: d479 c4e6 f3c9 4aa3 d0b8 90ff 31ff ff33  .y....J.....1..3
+000001c0: e6ff de53 6f14 b818 053c 40fe 5fed f7ef  ...So....<@._...
+000001d0: d6fe bfef faaf e70f 1dbc fe8b f91f aeff  ................
+000001e0: 41f3 bfe0 e931 d820 e67f e8ff c1ff 8721  A....1. .......!
+000001f0: 4fb9 0e43 3b5b de73 feb7 f6ff 9e1f f8c6  O..C;[.s........
+00000200: fe83 c0c7 fc0f fd3f aeff 61fd ffc0 f59c  .......?..a.....
+00000210: c047 ff8f fe1f fc7f 9649 9eea 3015 4a48  .G.......I..0.JH
+00000220: fd53 24f0 7bfe dff3 eafb 7f83 a133 f0c1  .S$.{........3..
+00000230: fe21 11f0 d0ff 1f02 7c91 c1f2 9272 b1db  .!......|....r..
+00000240: 2df3 17b1 18f6 3be6 ae60 8ffc f2cb a76b  -.....;..`.....k
+00000250: 2ae7 aa3b 6eb7 08c0 b2ac 8b2b 6831 cb35  *..;n......+h1.5
+00000260: 8985 ac1a 926b aeaf 8851 149e ce49 c415  .....k...Q...I..
+00000270: 9d26 2cb2 a172 d9aa ac65 97ff aa9e 4ded  .&,..r...e....M.
+00000280: 30e2 33ad 26e7 3451 ac31 16de 2744 fe47  0.3.&.4Q.1..'D.G
+00000290: feff 03f8 df09 bc00 f33f e47f c3ff 4bba  .........?....K.
+000002a0: 48c2 921e 98bc 4ffe 0f7c 20fb 92ff fd61  H.....O..| ....a
+000002b0: 510f f8df c5fc ef90 fc2f 54bb 556d aae5  Q......../T.Um..
+000002c0: 7adb e840 1914 3c22 a770 a6c4 82b0 9b19  z..@..<".p......
+000002d0: cb34 1769 41ff 3391 c67c 9e4b 5a1c 6152  .4.iA.3..|.KZ.aR
+000002e0: 0a09 ad67 0955 8a9c 36cb ce4c 51e7 ac6e  ...g.U..6..LQ..n
+000002f0: 5c87 1319 545c 0d20 cc9d c754 c381 6767  \...T\. ...T..gg
+00000300: e727 1f5e be0f 4fdf bc3e 7ff1 3c3c 7ff1  .'.^..O..>..<<..
+00000310: f28c 4c88 558e 661b a9ac bad5 7306 d10b  ..L.U.f.....s...
+00000320: 85e8 43c4 44e6 696a 0210 9a65 099f 15e3  ..C.D.ij...e....
+00000330: 96e1 cc9c e9b0 7130 340d 3a73 11e6 5928  ......q04.:s..Y(
+00000340: 5216 26ec 334b ca28 a411 e794 1bef 98ce  R.&.3K.(........
+00000350: 65aa 88be 62cd 7eab 3125 e15a c1b6 6410  e...b.~.1%.Z..d.
+00000360: 0445 5cb2 9916 7249 a654 b188 40ad a295  .E\...rI.T..@...
+00000370: 9ce7 0b28 b78d c0a6 cb13 8871 aa61 0cb6  ...(.......q.a..
+00000380: e420 9da9 1049 8f88 e244 d1a4 3b26 2f62  . ...I...D..;&/b
+00000390: f25e e610 21c9 8630 db83 dae4 198b 699e  .^..!..0......i.
+000003a0: 803c 5a90 6232 ab11 ab49 3406 555a 8ec9  .<Z.b2...I4.UZ..
+000003b0: fba2 1b98 0734 d89e df7a 321b 93b4 b74e  .....4...z2....N
+000003c0: 0f2f 4e2e d55a 7640 717a c48a a5f8 2f4b  ./N..Zv@qz..../K
+000003d0: ad1e d938 9d06 8fc8 7951 062a c420 7c34  ...8....yQ.*. |4
+000003e0: 2162 af1c 7e41 539e e549 b560 75fd a268  !b..~AS..I.`u..h
+000003f0: 02aa 699b 2d1b 044a e982 9961 ec75 0fdd  ..i.-..J...a.u..
+00000400: 75fd f2e4 94cd 40ac 54e8 5ba7 9681 48b7  u.....@.T.[...H.
+00000410: 3a34 3b55 37a6 7c43 e277 6c0e 7249 a266  :4;U7.|C.wl.rI.f
+00000420: 9267 fa47 c4ad f7e9 5415 5a67 c407 8df8  .g.G....T.Zg....
+00000430: fcd1 b9ec de9d f06b 5bd8 b448 136a 13aa  .......k[..H.j..
+00000440: 0825 26d2 36fa 2497 6b93 d8a8 1b9a ba1d  .%&.6.$.k.......
+00000450: 1891 36ed a147 629e b0d0 8c35 d961 9510  ..6..Gb....5.a..
+00000460: c6e7 d358 2410 3b4e 2af3 b41a 26f4 52d0  ...X$.;N*...&.R.
+00000470: 8800 a318 a93e 33b9 2d9d e99a 4046 208c  .....>3.-...@F .
+00000480: e649 01d9 01d5 ac90 b952 b393 99f1 176a  .I.......R.....j
+00000490: 650b 450b 234b d1e9 6ae8 9e99 e235 4b12  e.E.#K..j....5K.
+000004a0: f3bf ac6b 547a 2e48 9ec1 d48b e954 3d36  ...kTz.H.....T=6
+000004b0: 6da4 e14e 8a04 86a7 d5a1 75cf dbea aee5  m..N......u.....
+000004c0: b2a1 1fa0 8690 c148 58f5 9d0e 667d 2e1b  .......HX...f}..
+000004d0: 0b0d 8bbb eabd d195 4139 78b8 a548 ff16  ........A9x..H..
+000004e0: 3ced 5423 f59a 735e 2d4c a3f7 2d05 fe7f  <.T#..s^-L..-...
+000004f0: 7b6d 76b5 21aa d1c3 ba09 bbe1 4aab 4ea3  {mv.!.......J.N.
+00000500: bfee d650 9272 50d1 1d7e 3fb6 4e6f 2ffc  ...P.rP..~?.No/.
+00000510: e32f ab61 bf3e 2e46 8a45 0ecb 4a35 1435  ./.a.>.F.E..J5.5
+00000520: 46f9 fad8 da10 abc8 3545 c6d2 a628 e079  F.......5E...(.y
+00000530: a4d5 35eb 1f6f 0995 2b06 5967 2c60 f266  ..5..o..+.Yg,`.f
+00000540: a56d 4563 b028 50cc 4ebc d1ad 319f 9449  .mEc.(P.N...1..I
+00000550: a381 9582 ff76 f6cf 0b12 2d41 4058 d624  .....v....-A@X.$
+00000560: 5912 f06d 0bf2 892d c119 4aa6 8cf7 e5a5  Y..m...-..J.....
+00000570: 8bbf add6 eb7e 9b9d 4d48 02e7 b053 8b64  .....~..MH...S.d
+00000580: 9bbe 3add 2d31 4e25 3342 344d d668 2bb0  ..:.-1N%3B4M.h+.
+00000590: af64 3bcc 7bdd b43a 1da6 198c f4e5 ebba  .d;.{..:........
+000005a0: c450 358c 65c4 6d88 b35b 514c f38f 50f9  .P5.e.m..[QL..P.
+000005b0: 12fa 5809 0afa dd81 631b 9256 2eab d1ac  ..X.....c..V....
+000005c0: 2e2d 6384 1d8a 60d6 a7a9 9fa5 c2b0 ad76  .-c...`........v
+000005d0: ab28 6177 f59d fa75 5245 1f44 cc66 b994  .(aw...uRE.D.f..
+000005e0: 2c1a 932f ecab 8597 12fe 0cf9 3f3e fff3  ,../........?>..
+000005f0: c7e5 ff3b dfff f1bc a7c7 23b4 9c87 9cff  ...;......#.....
+00000600: db6c 3e7f 627c 7fff 4eec fffb 9eff 099c  .l>.b|..N.......
+00000610: 8187 cfff e0f5 5f5c ffc3 5eff 2dfd 3f5e  ......_\..^.-.?^
+00000620: ff45 ffdf f0ff 3ffd 4ae8 f7bd ff59 5cff  .E....?.J....Y\.
+00000630: 853f bcfe 7b08 e0fb 9f98 ff21 ff23 ff23  .?..{......!.#.#
+00000640: ff23 ffef e1ff 8b37 1fde 9d9e 5dd8 fa46  .#.....7....]..F
+00000650: df0f ff07 8eb7 cdff 231f f9ff 2058 bdef  ........#... X..
+00000660: db52 4ce7 999d 2d5b 3b1f 016f ed7f 30b0  .RL...-[;..o..0.
+00000670: b5ff 9981 d637 c2c9 d6b7 556d 5771 c432  .....7....UmWq.2
+00000680: 9646 2c9d 2dc3 84a7 9fd4 be7a 92fd 27e7  .F,.-......z..'.
+00000690: 92ed 2dd7 222b efcb fcb8 4e23 ff23 ff23  ..-."+....N#.#.#
+000006a0: ff23 1e00 ffef f2ba 77ca ff8e e36e f2bf  .#......w....n..
+000006b0: e7b8 f8fc d761 80a6 8efc 8ffc 8ffc 8ffc  .....a..........
+000006c0: 8ffc bf87 ff9b d9d4 bde4 ff8e b37d fd7f  .............}..
+000006d0: 1804 43e4 ff83 acff d2e4 ec68 f0c8 ffc8  ..C........h....
+000006e0: ffc8 ffc8 ffc8 ff77 7fb5 f477 f9df ddbe  .......w...w....
+000006f0: fe3f 1c8c 02e4 ff83 ae3f da3c f23f 3eff  .?.......?.<.?>.
+00000700: fdf0 f81f 7fff 01f9 bfc1 ffe5 5de0 593c  ............].Y<
+00000710: bf63 fbff 26ff 0fbc edef 3f7a 01de ff3f  .c..&.....?z...?
+00000720: 083e 4298 179a 30ef b2dd d274 1e4e 739e  .>B...0....t.Ns.
+00000730: 4464 42ca bdc8 bc88 3621 8e79 410b 6d05  DdB.....6!.yA.m.
+00000740: f91f f3ff bf78 feef 39a3 63cc ff1f 3cff  .....x..9.c...<.
+00000750: fff4 273f bf8b ff07 a3e1 eafb 6fae 6bf2  ..'?........o.k.
+00000760: 7f30 7fcc ff0f 82e2 95f6 62d1 b510 8922  .0........b...."
+00000770: d587 5f62 9e46 6146 679f e89c a95e 59c1  .._b.FaFg....^Y.
+00000780: 0401 c546 a77c 23bb f826 84b5 5220 ab57  ...F.|#..&..R .W
+00000790: 7fd2 a56c 35d9 e8a3 c3d3 5992 476c f2b1  ...l5.....Y.Gl..
+000007a0: d1e2 b25b b5f9 5cbe 5d30 b10a 25ac 7b8a  ...[..\.]0..%.{.
+000007b0: 58f9 d98d a264 d77b 0675 455a bc6d 30b1  X....d.{.uEZ.m0.
+000007c0: 36df 36a8 4bab 1fb4 08eb fb58 4684 e2ae  6.6.K......XF...
+000007d0: 8775 59d5 2866 d528 af8f 6ba6 b4aa 8f6f  .uY.(f.(..k....o
+000007e0: 1e0e 55ce 354c bfa8 6246 ea96 9fe0 a87e  ..U.5L..bF.....~
+000007f0: 4d43 e6e9 d8ec 664b 902c 25f6 bf6a bb22  MC....fK.,%..j."
+00000800: d388 43eb eb2b c612 8ca9 1008 0402 8140  ..C..+.........@
+00000810: 2010 0804 0281 4020 1008 0402 8140 2010   .....@ .....@ .
+00000820: 0804 0281 4020 1008 0402 8140 fc08 fe07  ....@ .....@....
+00000830: 29f6 6357 00a0 0000                      ).cW....
```
