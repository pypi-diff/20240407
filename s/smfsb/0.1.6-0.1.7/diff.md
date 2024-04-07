# Comparing `tmp/smfsb-0.1.6.tar.gz` & `tmp/smfsb-0.1.7.tar.gz`

## Comparing `smfsb-0.1.6.tar` & `smfsb-0.1.7.tar`

### file list

```diff
@@ -1,130 +1,143 @@
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 smfsb-0.1.6/.readthedocs.yaml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 smfsb-0.1.6/Development.md
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 smfsb-0.1.6/Makefile
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/Makefile
--rw-r--r--   0        0        0   334279 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/abcRun.pdf
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/abcRun.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/abcRun.txt
--rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/create.pdf
--rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/create.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/create.txt
--rw-r--r--   0        0        0     7685 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/imdeath.pdf
--rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/imdeath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/imdeath.txt
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/metrop.pdf
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/metrop.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/metrop.txt
--rw-r--r--   0        0        0   312695 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/metropolisHastings.pdf
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/metropolisHastings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/metropolisHastings.txt
--rw-r--r--   0        0        0   329769 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/normgibbs.pdf
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/normgibbs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/normgibbs.txt
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/rcfmc.pdf
--rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/rcfmc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/rcfmc.txt
--rw-r--r--   0        0        0    52757 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/rdiff.pdf
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/rdiff.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/rdiff.txt
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/rfmc.pdf
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/rfmc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/rfmc.txt
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-bd.pdf
--rwxr-xr-x   0        0        0      313 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-bd.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-bd.txt
--rw-r--r--   0        0        0    16520 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-dimer.pdf
--rwxr-xr-x   0        0        0      354 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-dimer.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-dimer.txt
--rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-id.pdf
--rwxr-xr-x   0        0        0      313 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-id.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-id.txt
--rw-r--r--   0        0        0    19893 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-cle.pdf
--rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-cle.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-cle.txt
--rw-r--r--   0        0        0    15047 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-discretise.pdf
--rwxr-xr-x   0        0        0      402 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-discretise.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-discretise.txt
--rw-r--r--   0        0        0    17878 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-euler.pdf
--rwxr-xr-x   0        0        0      344 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-euler.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-euler.txt
--rw-r--r--   0        0        0    20491 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-frm.pdf
--rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-frm.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-frm.txt
--rw-r--r--   0        0        0    29071 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-gillespie.pdf
--rwxr-xr-x   0        0        0      313 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-gillespie.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-gillespie.txt
--rw-r--r--   0        0        0    13889 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-gillespied.pdf
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-gillespied.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-gillespied.txt
--rw-r--r--   0        0        0    15380 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-pts.pdf
--rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-pts.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv-pts.txt
--rw-r--r--   0        0        0    13026 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv.pdf
--rwxr-xr-x   0        0        0      337 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv.txt
--rw-r--r--   0        0        0    19682 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv2.pdf
--rwxr-xr-x   0        0        0      355 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv2.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-lv2.txt
--rw-r--r--   0        0        0    15662 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-mm.pdf
--rwxr-xr-x   0        0        0      333 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-mm.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-mm.txt
--rw-r--r--   0        0        0    12590 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-sir.pdf
--rwxr-xr-x   0        0        0      340 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-sir.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/s-m-sir.txt
--rwxr-xr-x   0        0        0      666 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/sbmlsh-demo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/sbmlsh-demo.txt
--rw-r--r--   0        0        0    10792 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/sbmlsh.pdf
--rw-r--r--   0        0        0    13884 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/simpleEuler.pdf
--rwxr-xr-x   0        0        0      502 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/simpleEuler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/simpleEuler.txt
--rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE1D.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE1D.txt
--rw-r--r--   0        0        0     9163 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE1D0.pdf
--rw-r--r--   0        0        0    10311 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE1D1.pdf
--rwxr-xr-x   0        0        0      477 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE1Df.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE1Df.txt
--rw-r--r--   0        0        0    41455 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE1Df0.pdf
--rw-r--r--   0        0        0    44512 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE1Df1.pdf
--rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE2D.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE2D.txt
--rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE2D0.pdf
--rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE2D1.pdf
--rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE2Df.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE2Df.txt
--rw-r--r--   0        0        0    74724 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE2Df0.pdf
--rw-r--r--   0        0        0    97084 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepCLE2Df1.pdf
--rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepGillespie1D.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepGillespie1D.txt
--rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepGillespie1D0.pdf
--rw-r--r--   0        0        0    10358 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepGillespie1D1.pdf
--rwxr-xr-x   0        0        0      430 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepGillespie2D.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepGillespie2D.txt
--rw-r--r--   0        0        0     8972 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepGillespie2D0.pdf
--rw-r--r--   0        0        0     9752 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepGillespie2D1.pdf
--rw-r--r--   0        0        0    33044 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepSDE.pdf
--rwxr-xr-x   0        0        0      610 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepSDE.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.6/demos/stepSDE.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 smfsb-0.1.6/docs/Makefile
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 smfsb-0.1.6/docs/conf.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 smfsb-0.1.6/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 smfsb-0.1.6/docs/make.bat
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 smfsb-0.1.6/docs/requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 smfsb-0.1.6/docs/source/modules.rst
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 smfsb-0.1.6/docs/source/smfsb.rst
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 smfsb-0.1.6/src/smfsb/__init__.py
--rw-r--r--   0        0        0     8665 2020-02-02 00:00:00.000000 smfsb-0.1.6/src/smfsb/inference.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 smfsb-0.1.6/src/smfsb/models.py
--rwxr-xr-x   0        0        0    15524 2020-02-02 00:00:00.000000 smfsb-0.1.6/src/smfsb/sim.py
--rwxr-xr-x   0        0        0     5371 2020-02-02 00:00:00.000000 smfsb-0.1.6/src/smfsb/smfsbSbml.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 smfsb-0.1.6/src/smfsb/spatial.py
--rwxr-xr-x   0        0        0    29107 2020-02-02 00:00:00.000000 smfsb-0.1.6/src/smfsb/spn.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 smfsb-0.1.6/tests/test_early.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 smfsb-0.1.6/tests/test_inference.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 smfsb-0.1.6/tests/test_sbmlsh.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 smfsb-0.1.6/tests/test_spatial.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 smfsb-0.1.6/tests/test_spn.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 smfsb-0.1.6/.gitignore
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 smfsb-0.1.6/LICENSE
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 smfsb-0.1.6/README.md
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 smfsb-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 smfsb-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 smfsb-0.1.7/.readthedocs.yaml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 smfsb-0.1.7/Development.md
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 smfsb-0.1.7/Makefile
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/Makefile
+-rw-r--r--   0        0        0   295219 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/abc-cal.pdf
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/abc-cal.py
+-rw-r--r--   0        0        0   298258 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/abc.pdf
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/abc.py
+-rw-r--r--   0        0        0   334041 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/abcRun.pdf
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/abcRun.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/abcRun.txt
+-rw-r--r--   0        0        0   103202 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/abcSmc.pdf
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/abcSmc.py
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/create.pdf
+-rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/create.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/create.txt
+-rw-r--r--   0        0        0     7685 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/imdeath.pdf
+-rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/imdeath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/imdeath.txt
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/mcmc.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/metrop.pdf
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/metrop.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/metrop.txt
+-rw-r--r--   0        0        0   312695 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/metropolisHastings.pdf
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/metropolisHastings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/metropolisHastings.txt
+-rw-r--r--   0        0        0   329769 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/normgibbs.pdf
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/normgibbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/normgibbs.txt
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/pfMLLik.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/pfMLLik.txt
+-rw-r--r--   0        0        0    17376 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/pmmh.pdf
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/pmmh.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/rcfmc.pdf
+-rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/rcfmc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/rcfmc.txt
+-rw-r--r--   0        0        0    52757 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/rdiff.pdf
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/rdiff.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/rdiff.txt
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/rfmc.pdf
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/rfmc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/rfmc.txt
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-bd.pdf
+-rwxr-xr-x   0        0        0      313 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-bd.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-bd.txt
+-rw-r--r--   0        0        0    16520 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-dimer.pdf
+-rwxr-xr-x   0        0        0      354 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-dimer.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-dimer.txt
+-rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-id.pdf
+-rwxr-xr-x   0        0        0      313 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-id.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-id.txt
+-rw-r--r--   0        0        0    19893 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-cle.pdf
+-rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-cle.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-cle.txt
+-rw-r--r--   0        0        0    15047 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-discretise.pdf
+-rwxr-xr-x   0        0        0      402 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-discretise.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-discretise.txt
+-rw-r--r--   0        0        0    17878 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-euler.pdf
+-rwxr-xr-x   0        0        0      344 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-euler.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-euler.txt
+-rw-r--r--   0        0        0    20491 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-frm.pdf
+-rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-frm.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-frm.txt
+-rw-r--r--   0        0        0    29071 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-gillespie.pdf
+-rwxr-xr-x   0        0        0      313 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-gillespie.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-gillespie.txt
+-rw-r--r--   0        0        0    13889 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-gillespied.pdf
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-gillespied.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-gillespied.txt
+-rw-r--r--   0        0        0    15380 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-pts.pdf
+-rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-pts.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv-pts.txt
+-rw-r--r--   0        0        0    13026 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv.pdf
+-rwxr-xr-x   0        0        0      337 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv.txt
+-rw-r--r--   0        0        0    19682 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv2.pdf
+-rwxr-xr-x   0        0        0      355 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv2.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-lv2.txt
+-rw-r--r--   0        0        0    15662 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-mm.pdf
+-rwxr-xr-x   0        0        0      333 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-mm.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-mm.txt
+-rw-r--r--   0        0        0    12590 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-sir.pdf
+-rwxr-xr-x   0        0        0      340 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-sir.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/s-m-sir.txt
+-rwxr-xr-x   0        0        0      666 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/sbmlsh-demo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/sbmlsh-demo.txt
+-rw-r--r--   0        0        0    10792 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/sbmlsh.pdf
+-rw-r--r--   0        0        0    13884 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/simpleEuler.pdf
+-rwxr-xr-x   0        0        0      502 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/simpleEuler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/simpleEuler.txt
+-rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE1D.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE1D.txt
+-rw-r--r--   0        0        0     9163 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE1D0.pdf
+-rw-r--r--   0        0        0    10311 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE1D1.pdf
+-rwxr-xr-x   0        0        0      477 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE1Df.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE1Df.txt
+-rw-r--r--   0        0        0    41455 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE1Df0.pdf
+-rw-r--r--   0        0        0    44512 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE1Df1.pdf
+-rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE2D.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE2D.txt
+-rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE2D0.pdf
+-rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE2D1.pdf
+-rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE2Df.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE2Df.txt
+-rw-r--r--   0        0        0    74724 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE2Df0.pdf
+-rw-r--r--   0        0        0    97084 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepCLE2Df1.pdf
+-rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepGillespie1D.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepGillespie1D.txt
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepGillespie1D0.pdf
+-rw-r--r--   0        0        0    10358 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepGillespie1D1.pdf
+-rwxr-xr-x   0        0        0      430 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepGillespie2D.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepGillespie2D.txt
+-rw-r--r--   0        0        0     8972 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepGillespie2D0.pdf
+-rw-r--r--   0        0        0     9752 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepGillespie2D1.pdf
+-rw-r--r--   0        0        0    33044 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepSDE.pdf
+-rwxr-xr-x   0        0        0      610 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepSDE.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smfsb-0.1.7/demos/stepSDE.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 smfsb-0.1.7/docs/Makefile
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 smfsb-0.1.7/docs/conf.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 smfsb-0.1.7/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 smfsb-0.1.7/docs/make.bat
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 smfsb-0.1.7/docs/requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 smfsb-0.1.7/docs/source/modules.rst
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 smfsb-0.1.7/docs/source/smfsb.rst
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 smfsb-0.1.7/src/smfsb/__init__.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 smfsb-0.1.7/src/smfsb/data.py
+-rw-r--r--   0        0        0    16939 2020-02-02 00:00:00.000000 smfsb-0.1.7/src/smfsb/inference.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 smfsb-0.1.7/src/smfsb/models.py
+-rwxr-xr-x   0        0        0    15524 2020-02-02 00:00:00.000000 smfsb-0.1.7/src/smfsb/sim.py
+-rwxr-xr-x   0        0        0     5371 2020-02-02 00:00:00.000000 smfsb-0.1.7/src/smfsb/smfsbSbml.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 smfsb-0.1.7/src/smfsb/spatial.py
+-rwxr-xr-x   0        0        0    29107 2020-02-02 00:00:00.000000 smfsb-0.1.7/src/smfsb/spn.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 smfsb-0.1.7/tests/test_data.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 smfsb-0.1.7/tests/test_early.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 smfsb-0.1.7/tests/test_inference.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 smfsb-0.1.7/tests/test_sbmlsh.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 smfsb-0.1.7/tests/test_spatial.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 smfsb-0.1.7/tests/test_spn.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 smfsb-0.1.7/.gitignore
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 smfsb-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 smfsb-0.1.7/README.md
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 smfsb-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 smfsb-0.1.7/PKG-INFO
```

### Comparing `smfsb-0.1.6/.readthedocs.yaml` & `smfsb-0.1.7/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/Development.md` & `smfsb-0.1.7/Development.md`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/abcRun.py` & `smfsb-0.1.7/demos/abcRun.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/create.pdf` & `smfsb-0.1.7/demos/create.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/imdeath.pdf` & `smfsb-0.1.7/demos/imdeath.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/metrop.pdf` & `smfsb-0.1.7/demos/metrop.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/metropolisHastings.pdf` & `smfsb-0.1.7/demos/metropolisHastings.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/metropolisHastings.py` & `smfsb-0.1.7/demos/metropolisHastings.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/normgibbs.pdf` & `smfsb-0.1.7/demos/normgibbs.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/normgibbs.py` & `smfsb-0.1.7/demos/normgibbs.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/rcfmc.pdf` & `smfsb-0.1.7/demos/rcfmc.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/rdiff.pdf` & `smfsb-0.1.7/demos/rdiff.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/rfmc.pdf` & `smfsb-0.1.7/demos/rfmc.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/s-m-bd.pdf` & `smfsb-0.1.7/demos/s-m-bd.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/s-m-dimer.pdf` & `smfsb-0.1.7/demos/s-m-dimer.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/s-m-id.pdf` & `smfsb-0.1.7/demos/s-m-id.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/s-m-lv-cle.pdf` & `smfsb-0.1.7/demos/s-m-lv-cle.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/s-m-lv-discretise.pdf` & `smfsb-0.1.7/demos/s-m-lv-discretise.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/s-m-lv-euler.pdf` & `smfsb-0.1.7/demos/s-m-lv-euler.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/s-m-lv-frm.pdf` & `smfsb-0.1.7/demos/s-m-lv-frm.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/s-m-lv-gillespie.pdf` & `smfsb-0.1.7/demos/s-m-lv-gillespie.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/s-m-lv-gillespied.pdf` & `smfsb-0.1.7/demos/s-m-lv-gillespied.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/s-m-lv-pts.pdf` & `smfsb-0.1.7/demos/s-m-lv-pts.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/s-m-lv.pdf` & `smfsb-0.1.7/demos/s-m-lv.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/s-m-lv2.pdf` & `smfsb-0.1.7/demos/s-m-lv2.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/s-m-mm.pdf` & `smfsb-0.1.7/demos/s-m-mm.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/s-m-sir.pdf` & `smfsb-0.1.7/demos/s-m-sir.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/sbmlsh-demo.py` & `smfsb-0.1.7/demos/sbmlsh-demo.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/sbmlsh.pdf` & `smfsb-0.1.7/demos/sbmlsh.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/simpleEuler.pdf` & `smfsb-0.1.7/demos/simpleEuler.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepCLE1D.txt` & `smfsb-0.1.7/demos/stepCLE1D.txt`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepCLE1D0.pdf` & `smfsb-0.1.7/demos/stepCLE1D0.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepCLE1D1.pdf` & `smfsb-0.1.7/demos/stepCLE1D1.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepCLE1Df.txt` & `smfsb-0.1.7/demos/stepCLE1Df.txt`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepCLE1Df0.pdf` & `smfsb-0.1.7/demos/stepCLE1Df0.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepCLE1Df1.pdf` & `smfsb-0.1.7/demos/stepCLE1Df1.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepCLE2D0.pdf` & `smfsb-0.1.7/demos/stepCLE2D0.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepCLE2D1.pdf` & `smfsb-0.1.7/demos/stepCLE2D1.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepCLE2Df0.pdf` & `smfsb-0.1.7/demos/stepCLE2Df0.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepCLE2Df1.pdf` & `smfsb-0.1.7/demos/stepCLE2Df1.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepGillespie1D0.pdf` & `smfsb-0.1.7/demos/stepGillespie1D0.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepGillespie1D1.pdf` & `smfsb-0.1.7/demos/stepGillespie1D1.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepGillespie2D0.pdf` & `smfsb-0.1.7/demos/stepGillespie2D0.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepGillespie2D1.pdf` & `smfsb-0.1.7/demos/stepGillespie2D1.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepSDE.pdf` & `smfsb-0.1.7/demos/stepSDE.pdf`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/demos/stepSDE.py` & `smfsb-0.1.7/demos/stepSDE.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/docs/Makefile` & `smfsb-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/docs/conf.py` & `smfsb-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/docs/make.bat` & `smfsb-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/docs/source/smfsb.rst` & `smfsb-0.1.7/docs/source/smfsb.rst`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 -------------------
 
 .. automodule:: smfsb.models
    :members:
    :undoc-members:
    :show-inheritance:
 
+smfsb.data module
+-----------------
+
+.. automodule:: smfsb.data
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 smfsb.spn module
 ------------------
 
 .. automodule:: smfsb.spn
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `smfsb-0.1.6/src/smfsb/models.py` & `smfsb-0.1.7/src/smfsb/models.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/src/smfsb/sim.py` & `smfsb-0.1.7/src/smfsb/sim.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/src/smfsb/smfsbSbml.py` & `smfsb-0.1.7/src/smfsb/smfsbSbml.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/src/smfsb/spatial.py` & `smfsb-0.1.7/src/smfsb/spatial.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/src/smfsb/spn.py` & `smfsb-0.1.7/src/smfsb/spn.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/tests/test_early.py` & `smfsb-0.1.7/tests/test_early.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/tests/test_inference.py` & `smfsb-0.1.7/tests/test_inference.py`

 * *Files 24% similar despite different names*

```diff
@@ -34,11 +34,69 @@
       return np.sqrt(np.sum(diff*diff))
     def rdis(th):
       return dist(sumStats(rmod(th)))
     p, d = smfsb.abcRun(100, rpr, rdis)
     assert(len(p) == 100)
     assert(len(d) == 100)
 
+def test_pfmllik():
+    def obsll(x, t, y, th):
+        return np.sum(sp.stats.norm.logpdf((y-x)/10))
+    def simX(t0, th):
+        return np.array([np.random.poisson(50), np.random.poisson(100)])
+    def step(x, t, dt, th):
+        sf = smfsb.models.lv(th).stepCLE()
+        return sf(x, t, dt)
+    mll = smfsb.pfMLLik(50, simX, 0, step, obsll, smfsb.data.LVnoise10)
+    assert (mll(np.array([1, 0.005, 0.6])) > mll(np.array([2, 0.005, 0.6])))
+
+def test_abcsmcstep():
+    data = np.random.normal(5, 2, 250)
+    def rpr():
+      return np.exp(np.random.uniform(-3, 3, 2))
+    def rmod(th):
+      return np.random.normal(np.exp(th[0]), np.exp(th[1]), 250)
+    def sumStats(dat):
+      return np.array([np.mean(dat), np.std(dat)])
+    ssd = sumStats(data)
+    def dist(ss):
+      diff = ss - ssd
+      return np.sqrt(np.sum(diff*diff))
+    def rdis(th):
+      return dist(sumStats(rmod(th)))
+    N = 100
+    samples = np.zeros((N,1))
+    samples = np.apply_along_axis(lambda x: rpr(), 1, samples)
+    th, lw = smfsb.abcSmcStep(lambda x: np.log(np.sum(((x<3)&(x>-3))/6)), samples,
+                              np.zeros(N) + np.log(1/N), rdis,
+                              lambda x: np.random.normal(x, 0.1),
+                              lambda x,y: np.sum(sp.stats.norm(x,0.1).logpdf(y)),
+                              10)
+    assert(th.shape == (N, 2))
+    assert(len(lw) == N)
+    
+def test_abcsmc():
+    data = np.random.normal(5, 2, 250)
+    def rpr():
+      return np.exp(np.random.uniform(-3, 3, 2))
+    def rmod(th):
+      return np.random.normal(np.exp(th[0]), np.exp(th[1]), 250)
+    def sumStats(dat):
+      return np.array([np.mean(dat), np.std(dat)])
+    ssd = sumStats(data)
+    def dist(ss):
+      diff = ss - ssd
+      return np.sqrt(np.sum(diff*diff))
+    def rdis(th):
+      return dist(sumStats(rmod(th)))
+    N = 100
+    post = smfsb.abcSmc(N, rpr, lambda x: np.log(np.sum(((x<3)&(x>-3))/6)),
+                              rdis, lambda x: np.random.normal(x, 0.1),
+                              lambda x,y: np.sum(sp.stats.norm.logpdf(y, x, 0.1)))
+    assert(post.shape == (N, 2))
+    
+
+
     
 # eof
```

### Comparing `smfsb-0.1.6/tests/test_sbmlsh.py` & `smfsb-0.1.7/tests/test_sbmlsh.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/tests/test_spatial.py` & `smfsb-0.1.7/tests/test_spatial.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/tests/test_spn.py` & `smfsb-0.1.7/tests/test_spn.py`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/.gitignore` & `smfsb-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/LICENSE` & `smfsb-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `smfsb-0.1.6/README.md` & `smfsb-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # smfsb for python
 
-Python library for the book, [Stochastic modelling for systems biology, third edition](https://github.com/darrenjw/smfsb/). *Please note that this package is still under development, and the coverage of the book is still incomplete. Currently, the package covers the code from Chapters 1 to 10 (inclusive). I will be adding code to cover Chapter 11 in due course.*
+Python library for the book, [Stochastic modelling for systems biology, third edition](https://github.com/darrenjw/smfsb/). This library is a Python port of the R package associated with the book.
 
 ## Install
 
 Latest stable version:
 ```bash
 pip install smfsb
 ```
@@ -65,15 +65,15 @@
 ```
 Note that if you are working with SBML models in Python using [libsbml](https://pypi.org/project/python-libsbml/), then there is also a function `model2Spn` which takes a libsbml model object.
 
 To read and parse an SBML-shorthand model, use
 ```python
 m = smfsb.mod2Spn("myModel.mod")
 ```
-There is also a function `sh2Spn` which expects a python string containing a shorthand model. This is convenient for embedding shorthand models inside python scripts, and is particularly convenient when working with things like Jupyter notebooks. Below follows a complete session to illustrate the idea by creating and simulating a realisation from a discrete stochastic SIER model.
+There is also a function `sh2Spn` which expects a python string containing a shorthand model. This is convenient for embedding shorthand models inside python scripts, and is particularly convenient when working with things like Jupyter notebooks. Below follows a complete session to illustrate the idea by creating and simulating a realisation from a discrete stochastic SEIR model.
 ```python
 import smfsb
 import numpy as np
 
 seirSH = """
 @model:3.1.1=SEIR "SEIR Epidemic model"
  s=item, t=second, v=litre, e=item
```

### Comparing `smfsb-0.1.6/pyproject.toml` & `smfsb-0.1.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "smfsb"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Darren Wilkinson", email="darrenjwilkinson@btinternet.com" },
 ]
 description = "Python code relating to the textbook, Stochastic modelling for systems biology, third edition"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `smfsb-0.1.6/PKG-INFO` & `smfsb-0.1.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: smfsb
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python code relating to the textbook, Stochastic modelling for systems biology, third edition
 Project-URL: Homepage, https://github.com/darrenjw/python-smfsb
 Project-URL: Documentation, https://python-smfsb.readthedocs.io/
 Project-URL: Issues, https://github.com/darrenjw/python-smfsb/issues
 Author-email: Darren Wilkinson <darrenjwilkinson@btinternet.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,15 +14,15 @@
 Requires-Dist: numpy<2
 Requires-Dist: sbmlsh
 Requires-Dist: scipy
 Description-Content-Type: text/markdown
 
 # smfsb for python
 
-Python library for the book, [Stochastic modelling for systems biology, third edition](https://github.com/darrenjw/smfsb/). *Please note that this package is still under development, and the coverage of the book is still incomplete. Currently, the package covers the code from Chapters 1 to 10 (inclusive). I will be adding code to cover Chapter 11 in due course.*
+Python library for the book, [Stochastic modelling for systems biology, third edition](https://github.com/darrenjw/smfsb/). This library is a Python port of the R package associated with the book.
 
 ## Install
 
 Latest stable version:
 ```bash
 pip install smfsb
 ```
@@ -83,15 +83,15 @@
 ```
 Note that if you are working with SBML models in Python using [libsbml](https://pypi.org/project/python-libsbml/), then there is also a function `model2Spn` which takes a libsbml model object.
 
 To read and parse an SBML-shorthand model, use
 ```python
 m = smfsb.mod2Spn("myModel.mod")
 ```
-There is also a function `sh2Spn` which expects a python string containing a shorthand model. This is convenient for embedding shorthand models inside python scripts, and is particularly convenient when working with things like Jupyter notebooks. Below follows a complete session to illustrate the idea by creating and simulating a realisation from a discrete stochastic SIER model.
+There is also a function `sh2Spn` which expects a python string containing a shorthand model. This is convenient for embedding shorthand models inside python scripts, and is particularly convenient when working with things like Jupyter notebooks. Below follows a complete session to illustrate the idea by creating and simulating a realisation from a discrete stochastic SEIR model.
 ```python
 import smfsb
 import numpy as np
 
 seirSH = """
 @model:3.1.1=SEIR "SEIR Epidemic model"
  s=item, t=second, v=litre, e=item
```

