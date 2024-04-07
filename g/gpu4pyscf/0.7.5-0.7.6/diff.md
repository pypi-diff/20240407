# Comparing `tmp/gpu4pyscf-0.7.5.tar.gz` & `tmp/gpu4pyscf-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpu4pyscf-0.7.5.tar", last modified: Sat Mar 23 00:02:11 2024, max compression
+gzip compressed data, was "gpu4pyscf-0.7.6.tar", last modified: Sun Apr  7 17:40:23 2024, max compression
```

## Comparing `gpu4pyscf-0.7.5.tar` & `gpu4pyscf-0.7.6.tar`

### file list

```diff
@@ -1,117 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.847894 gpu4pyscf-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35122 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-23 00:02:11.847894 gpu4pyscf-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.831894 gpu4pyscf-0.7.5/gpu4pyscf/
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/__config__.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.831894 gpu4pyscf-0.7.5/gpu4pyscf/cc/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21043 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/cc/ccsd_incore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.835894 gpu4pyscf-0.7.5/gpu4pyscf/df/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/cderi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/df.py
--rw-r--r--   0 runner    (1001) docker     (127)    15653 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/df_jk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.835894 gpu4pyscf-0.7.5/gpu4pyscf/df/grad/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/grad/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/grad/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11762 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/grad/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/grad/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.835894 gpu4pyscf-0.7.5/gpu4pyscf/df/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24735 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/hessian/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/hessian/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    30873 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/hessian/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/hessian/uks.py
--rw-r--r--   0 runner    (1001) docker     (127)    63852 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/int3c2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/df/patch_pyscf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.835894 gpu4pyscf-0.7.5/gpu4pyscf/dft/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23594 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/dft/gen_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/dft/gks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/dft/libxc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/dft/libxc_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    63883 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/dft/numint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/dft/patch_pyscf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/dft/radi.py
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/dft/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/dft/roks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/dft/uks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/dft/xc_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/dft/xc_deriv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.839894 gpu4pyscf-0.7.5/gpu4pyscf/fci/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/fci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/fci/direct_spin1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.839894 gpu4pyscf-0.7.5/gpu4pyscf/grad/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/grad/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/grad/patch_pyscf.py
--rw-r--r--   0 runner    (1001) docker     (127)    23275 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/grad/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    18669 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/grad/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/grad/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13652 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/grad/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.839894 gpu4pyscf-0.7.5/gpu4pyscf/gto/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/gto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/gto/mole.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.839894 gpu4pyscf-0.7.5/gpu4pyscf/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/hessian/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)    24579 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/hessian/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    30689 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/hessian/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20524 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/hessian/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    42239 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/hessian/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.843894 gpu4pyscf-0.7.5/gpu4pyscf/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/lib/cublas.py
--rw-r--r--   0 runner    (1001) docker     (127)    19888 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/lib/cupy_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/lib/cusolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/lib/cutensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/lib/dftd3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/lib/dftd4.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/lib/diis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/lib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.843894 gpu4pyscf-0.7.5/gpu4pyscf/mp/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/mp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/mp/dfmp2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11837 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/mp/mp2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/patch_pyscf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.843894 gpu4pyscf-0.7.5/gpu4pyscf/qmmm/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/qmmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/qmmm/chelpg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.843894 gpu4pyscf-0.7.5/gpu4pyscf/scf/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/scf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/scf/cphf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/scf/diis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/scf/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/scf/ghf.py
--rw-r--r--   0 runner    (1001) docker     (127)    36347 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/scf/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/scf/int4c2e.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/scf/patch_pyscf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/scf/rohf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/scf/ucphf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/scf/uhf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.843894 gpu4pyscf-0.7.5/gpu4pyscf/solvent/
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/solvent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/solvent/_attach_solvent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.843894 gpu4pyscf-0.7.5/gpu4pyscf/solvent/grad/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/solvent/grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12921 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/solvent/grad/pcm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/solvent/grad/smd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.847894 gpu4pyscf-0.7.5/gpu4pyscf/solvent/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/solvent/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/solvent/hessian/pcm.py
--rw-r--r--   0 runner    (1001) docker     (127)    13153 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/solvent/hessian/smd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13770 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/solvent/pcm.py
--rw-r--r--   0 runner    (1001) docker     (127)    27453 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf/solvent/smd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 00:02:11.831894 gpu4pyscf-0.7.5/gpu4pyscf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/gpu4pyscf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 00:02:11.847894 gpu4pyscf-0.7.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4475 2024-03-23 00:02:11.000000 gpu4pyscf-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.621297 gpu4pyscf-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35122 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-07 17:40:23.621297 gpu4pyscf-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.605296 gpu4pyscf-0.7.6/gpu4pyscf/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/__config__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.609296 gpu4pyscf-0.7.6/gpu4pyscf/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24054 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/cc/ccsd_incore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.609296 gpu4pyscf-0.7.6/gpu4pyscf/df/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/cderi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11224 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/df.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15227 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/df_jk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.609296 gpu4pyscf-0.7.6/gpu4pyscf/df/grad/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/grad/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/grad/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/grad/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/grad/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.609296 gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30912 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/uks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66842 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/int3c2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.613296 gpu4pyscf-0.7.6/gpu4pyscf/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21779 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/gen_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/gks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/libxc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/libxc_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75728 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/numint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/radi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/roks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/uks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/xc_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/xc_deriv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.613296 gpu4pyscf-0.7.6/gpu4pyscf/fci/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/fci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/fci/direct_spin1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.613296 gpu4pyscf-0.7.6/gpu4pyscf/grad/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/grad/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25756 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/grad/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19167 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/grad/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/grad/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/grad/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.613296 gpu4pyscf-0.7.6/gpu4pyscf/gto/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/gto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/gto/mole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.613296 gpu4pyscf-0.7.6/gpu4pyscf/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/hessian/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25241 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/hessian/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30559 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/hessian/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20051 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/hessian/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42163 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/hessian/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.613296 gpu4pyscf-0.7.6/gpu4pyscf/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/cublas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23683 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/cupy_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/cusolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/cutensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/dftd3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/dftd4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/diis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.617296 gpu4pyscf-0.7.6/gpu4pyscf/mp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/mp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/mp/dfmp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/mp/mp2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.617296 gpu4pyscf-0.7.6/gpu4pyscf/qmmm/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/qmmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/qmmm/chelpg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.617296 gpu4pyscf-0.7.6/gpu4pyscf/scf/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/_response_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/cphf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/diis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/ghf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38435 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/int4c2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/rohf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/ucphf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/uhf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.617296 gpu4pyscf-0.7.6/gpu4pyscf/solvent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/_attach_solvent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.617296 gpu4pyscf-0.7.6/gpu4pyscf/solvent/grad/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12921 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/grad/pcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/grad/smd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.617296 gpu4pyscf-0.7.6/gpu4pyscf/solvent/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/hessian/pcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13153 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/hessian/smd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/pcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27453 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/smd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.605296 gpu4pyscf-0.7.6/gpu4pyscf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 17:40:23.621297 gpu4pyscf-0.7.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4469 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/setup.py
```

### Comparing `gpu4pyscf-0.7.5/LICENSE` & `gpu4pyscf-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/MANIFEST.in` & `gpu4pyscf-0.7.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/README.md` & `gpu4pyscf-0.7.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 GPU plugin for PySCF
 ====================
 Installation
 --------
 
 > [!NOTE]
-> The compiled binary packages support compute capability 6.0 and later (Pascal and later, such as Tesla P100, RTX 10 series and later). For older GPUs (GTX 10**, Tesla P100), please compile the package with the source code as follows.
+> The compiled binary packages support compute capability 6.0 and later (Pascal and later, such as Tesla P100, RTX 10 series and later).
 
 Run ```nvidia-smi``` in your terminal to check the installed CUDA version.
 
 Choose the proper package based on your CUDA environment.
 
 | Platform      | Command                               |
 ----------------| --------------------------------------|
 | **CUDA 11.x** |  ```pip3 install gpu4pyscf-cuda11x``` |
 | **CUDA 12.x** |  ```pip3 install gpu4pyscf-cuda12x``` |
 
 ```cuTensor``` is **highly recommended** for accelerating tensor contractions.
 
-For **CUDA 11.x**, ```pip3 install cutensor-cu11```
+For **CUDA 11.x**, ```pip3 install cutensor-cu11``` (requires CuPy V13.0 and later)
 
-For **CUDA 12.x**, ```pip3 install cutensor-cu12```
+For **CUDA 12.x**, ```pip3 install cutensor-cu12``` (requires CuPy V13.0 and later)
 
 Compilation
 --------
 One can compile the package with
 ```sh
 git clone https://github.com/pyscf/gpu4pyscf.git
 cd gpu4pyscf
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/__config__.py` & `gpu4pyscf-0.7.6/gpu4pyscf/__config__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/cc/ccsd_incore.py` & `gpu4pyscf-0.7.6/gpu4pyscf/cc/ccsd_incore.py`

 * *Files 19% similar despite different names*

```diff
@@ -525,19 +525,92 @@
     pPoO = poov = voov = None
     log.timer('CCSD integral transformation', *cput0)
 
     if FREE_CUPY_CACHE:
         cupy.get_default_memory_pool().free_all_blocks()
     return eris
 
-class CCSD(ccsd.CCSD):
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+class CCSDBase(lib.StreamObject):
+    # attributes
+    _keys                  = ccsd.CCSDBase._keys
+    max_cycle              = ccsd.CCSDBase.max_cycle
+    conv_tol               = ccsd.CCSDBase.conv_tol
+    iterative_damping      = ccsd.CCSDBase.iterative_damping
+    conv_tol_normt         = ccsd.CCSDBase.conv_tol_normt
+
+    diis                   = ccsd.CCSDBase.diis
+    diis_space             = ccsd.CCSDBase.diis_space
+    diis_file              = None
+    diis_start_cycle       = ccsd.CCSDBase.diis_start_cycle
+    diis_start_energy_diff = ccsd.CCSDBase.diis_start_energy_diff
+
+    direct                 = ccsd.CCSDBase.direct
+    async_io               = None
+    incore_complete        = ccsd.CCSDBase.incore_complete
+    cc2                    = ccsd.CCSDBase.cc2
+    callback               = None
+
+    # functions
+    __init__           = ccsd.CCSDBase.__init__
+    ecc                = ccsd.CCSDBase.ecc
+    e_tot              = ccsd.CCSDBase.e_tot
+    nocc               = ccsd.CCSDBase.nocc
+    nmo                = ccsd.CCSDBase.nmo
+    reset              = ccsd.CCSDBase.reset
+    get_nocc           = ccsd.CCSDBase.get_nocc
+    get_nmo            = ccsd.CCSDBase.get_nmo
+    get_frozen_mask    = ccsd.CCSDBase.get_frozen_mask
+    get_e_hf           = ccsd.CCSDBase.get_e_hf
+    set_frozen         = ccsd.CCSDBase.set_frozen
+    dump_flags         = ccsd.CCSDBase.dump_flags
+    get_init_guess     = ccsd.CCSDBase.get_init_guess
+    init_amps          = ccsd.CCSDBase.init_amps
+    energy             = ccsd.CCSDBase.energy
+    _add_vvvv          = ccsd.CCSDBase._add_vvvv
+    update_amps        = update_amps
+    kernel             = ccsd.CCSDBase.kernel
+    _finalize          = ccsd.CCSDBase._finalize
+    as_scanner         = ccsd.CCSDBase.as_scanner
+    restore_from_diis_ = ccsd.CCSDBase.restore_from_diis_
+
+    solve_lambda         = NotImplemented
+    ccsd_t               = NotImplemented
+    ipccsd               = NotImplemented
+    eaccsd               = NotImplemented
+    eeccsd               = NotImplemented
+    eomee_ccsd_singlet   = NotImplemented
+    eomee_ccsd_triplet   = NotImplemented
+    eomsf_ccsd           = NotImplemented
+    eomip_method         = NotImplemented
+    eomea_method         = NotImplemented
+    eomee_method         = NotImplemented
+    make_rdm1            = NotImplemented
+    make_rdm2            = NotImplemented
+    ao2mo                = _make_eris_incore
+    run_diis             = ccsd.CCSDBase.run_diis
+    amplitudes_to_vector = ccsd.CCSDBase.amplitudes_to_vector
+    vector_to_amplitudes = ccsd.CCSDBase.vector_to_amplitudes
+    dump_chk             = None
+    density_fit          = NotImplemented
+    nuc_grad_method      = NotImplemented
+
+    # to_cpu can be reused only when __init__ still takes mf
+    def to_cpu(self):
+        mf = self._scf.to_cpu()
+        from importlib import import_module
+        mod = import_module(self.__module__.replace('gpu4pyscf', 'pyscf'))
+        cls = getattr(mod, self.__class__.__name__)
+        obj = cls(mf)
+        return obj
+
+CCSDBase.ccsd = ccsd.CCSDBase.ccsd
+
+class CCSD(CCSDBase):
+    from gpu4pyscf.lib.utils import to_gpu, device
 
     def __init__(self, mf, *args, **kwargs):
         if hasattr(mf, 'to_cpu'):
             mf = mf.to_cpu()
         if hasattr(mf, 'with_df') and mf.with_df:
             lib.logger.warn(mf.mol, 'DF-CCSD not available. Run the standard CCSD.')
         ccsd.CCSD.__init__(self, mf, *args, **kwargs)
 
-    update_amps = update_amps
-    ao2mo = _make_eris_incore
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/__init__.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/cderi.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/cderi.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/df.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/df.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,32 +28,46 @@
 from gpu4pyscf import __config__
 from cupyx import scipy
 
 MIN_BLK_SIZE = getattr(__config__, 'min_ao_blksize', 128)
 ALIGNED = getattr(__config__, 'ao_aligned', 32)
 LINEAR_DEP_TOL = 1e-7
 
-class DF(df.DF):
+class DF(lib.StreamObject):
     from gpu4pyscf.lib.utils import to_gpu, device
 
-    _keys = {'intopt'}
+    _keys = {'intopt', 'mol', 'auxmol'}
 
     def __init__(self, mol, auxbasis=None):
-        super().__init__(mol, auxbasis)
+        self.mol = mol
+        self.stdout = mol.stdout
+        self.verbose = mol.verbose
+        self.max_memory = mol.max_memory
+        self._auxbasis = auxbasis
+
         self.auxmol = None
         self.intopt = None
         self.nao = None
         self.naux = None
         self.cd_low = None
         self._cderi = None
+        self._rsh_df = {}
+
+    @property
+    def auxbasis(self):
+        return self._auxbasis
+    @auxbasis.setter
+    def auxbasis(self, x):
+        if self._auxbasis != x:
+            self.reset()
+            self._auxbasis = x
 
     def to_cpu(self):
         from gpu4pyscf.lib.utils import to_cpu
         obj = to_cpu(self)
-        del obj.intopt, obj.cd_low, obj.nao, obj.naux
         return obj.reset()
 
     def build(self, direct_scf_tol=1e-14, omega=None):
         mol = self.mol
         auxmol = self.auxmol
         self.nao = mol.nao
         log = logger.new_logger(mol, mol.verbose)
@@ -163,23 +177,25 @@
             if isinstance(cderi_sparse, np.ndarray):
                 cupy.cuda.Device().synchronize()
 
             if buf_prefetch is not None:
                 buf = buf_prefetch
 
     def reset(self, mol=None):
-        '''
-        reset object for scanner
-        '''
-        super().reset(mol)
+        '''Reset mol and clean up relevant attributes for scanner mode'''
+        if mol is not None:
+            self.mol = mol
+            self.auxmol = None
+        self._cderi = None
+        self._vjopt = None
+        self._rsh_df = {}
         self.intopt = None
         self.nao = None
         self.naux = None
         self.cd_low = None
-        self._cderi = None
         return self
 
     get_ao_eri = get_eri = NotImplemented
     get_mo_eri = ao2mo = NotImplemented
 
 def cholesky_eri_gpu(intopt, mol, auxmol, cd_low, omega=None, sr_only=False):
     '''
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/df_jk.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/df_jk.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Author: Qiming Sun <osirpt.sun@gmail.com>
 # Modified by Xiaojie Wu <wxj6000@gmail.com>
 
 import copy
 import cupy
 import numpy
 from cupy import cublas
-from pyscf import lib, scf, __config__
+from pyscf import lib, __config__
 from pyscf.scf import dhf
 from pyscf.df import df_jk, addons
 from gpu4pyscf.lib import logger
 from gpu4pyscf.lib.cupy_helper import contract, take_last2d, transpose_sum, load_library, get_avail_mem
 from gpu4pyscf.dft import rks, uks, numint
 from gpu4pyscf.scf import hf, uhf
 from gpu4pyscf.df import df, int3c2e
@@ -81,52 +81,53 @@
             exchange. Same to RIJONX in ORCA
     Returns:
         An SCF object with a modified J, K matrix constructor which uses density
         fitting integrals to compute J and K
     Examples:
     '''
 
-    assert isinstance(mf, scf.hf.SCF)
+    assert isinstance(mf, hf.SCF)
 
     if with_df is None:
         if isinstance(mf, dhf.UHF):
             with_df = df.DF4C(mf.mol)
         else:
             with_df = df.DF(mf.mol)
         with_df.max_memory = mf.max_memory
         with_df.stdout = mf.stdout
         with_df.verbose = mf.verbose
         with_df.auxbasis = auxbasis
 
-    if isinstance(mf, df_jk._DFHF):
+    if isinstance(mf, _DFHF):
         if mf.with_df is None:
             mf.with_df = with_df
         elif getattr(mf.with_df, 'auxbasis', None) != auxbasis:
             #logger.warn(mf, 'DF might have been initialized twice.')
             mf = copy.copy(mf)
             mf.with_df = with_df
             mf.only_dfj = only_dfj
         return mf
 
     dfmf = _DFHF(mf, with_df, only_dfj)
     return lib.set_class(dfmf, (_DFHF, mf.__class__))
 
-class _DFHF(df_jk._DFHF):
+from gpu4pyscf.lib import utils
+class _DFHF:
     '''
     Density fitting SCF class
     Attributes for density-fitting SCF:
         auxbasis : str or basis dict
             Same format to the input attribute mol.basis.
             The default basis 'weigend+etb' means weigend-coulomb-fit basis
             for light elements and even-tempered basis for heavy elements.
         with_df : DF object
             Set mf.with_df = None to switch off density fitting mode.
     '''
-
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+    to_gpu = utils.to_gpu
+    device = utils.device
 
     _keys = {'rhoj', 'rhok', 'disp', 'screen_tol'}
 
     def __init__(self, mf, dfobj, only_dfj):
         self.__dict__.update(mf.__dict__)
         self._eri = None
         self.rhoj = None
@@ -177,41 +178,44 @@
             return uks_grad.Gradients(self)
         if isinstance(self, uhf.UHF):
             from gpu4pyscf.df.grad import uhf as uhf_grad
             return uhf_grad.Gradients(self)
         raise NotImplementedError()
 
     def Hessian(self):
-        from pyscf.dft.rks import KohnShamDFT
-        if isinstance(self, scf.rhf.RHF):
-            from gpu4pyscf.df.hessian import rhf, rks
+        from gpu4pyscf.dft.rks import KohnShamDFT
+        if isinstance(self, hf.RHF):
             if isinstance(self, KohnShamDFT):
-                return rks.Hessian(self)
+                from gpu4pyscf.df.hessian import rks as rks_hess
+                return rks_hess.Hessian(self)
             else:
-                return rhf.Hessian(self)
-        else:
-            from gpu4pyscf.df.hessian import uhf, uks
+                from gpu4pyscf.df.hessian import rhf as rhf_hess
+                return rhf_hess.Hessian(self)
+        elif isinstance(self, uhf.UHF):
             if isinstance(self, KohnShamDFT):
-                return uks.Hessian(self)
+                from gpu4pyscf.df.hessian import uks as uks_hess
+                return uks_hess.Hessian(self)
             else:
-                return uhf.Hessian(self)
-
+                from gpu4pyscf.df.hessian import uhf as uhf_hess
+                return uhf_hess.Hessian(self)
+        else:
+            raise NotImplementedError
     @property
     def auxbasis(self):
         return getattr(self.with_df, 'auxbasis', None)
 
     def get_veff(self, mol=None, dm=None, dm_last=None, vhf_last=0, hermi=1):
         '''
         effective potential
         '''
         if mol is None: mol = self.mol
         if dm is None: dm = self.make_rdm1()
 
         # for DFT
-        if isinstance(self, scf.hf.KohnShamDFT):
+        if isinstance(self, rks.KohnShamDFT):
             if dm.ndim == 2:
                 return rks.get_veff(self, dm=dm)
             elif dm.ndim == 3:
                 return uks.get_veff(self, dm=dm)
 
         if dm.ndim == 2:
             if self.direct_scf:
@@ -230,40 +234,18 @@
                 return vhf
             else:
                 vj, vk = self.get_jk(mol, dm, hermi=hermi)
                 return vj[0] + vj[1] - vk
         else:
             raise NotImplementedError("Please check the dimension of the density matrix, it should not reach here.")
 
-    def energy_tot(self, dm=None, h1e=None, vhf=None):
-        '''
-        compute tot energy
-        '''
-        nuc = self.energy_nuc()
-        e_tot = self.energy_elec(dm, h1e, vhf)[0] + nuc
-        self.scf_summary['nuc'] = nuc.real
-        return e_tot
-
-    '''
     def to_cpu(self):
         obj = self.undo_df().to_cpu().density_fit()
-        keys = dir(obj)
-        obj.__dict__.update(self.__dict__)
-        for key in set(dir(self)).difference(keys):
-            print(key)
-            delattr(obj, key)
-
-        for key in keys:
-            val = getattr(obj, key)
-            if isinstance(val, cupy.ndarray):
-                setattr(obj, key, cupy.asnumpy(val))
-            elif hasattr(val, 'to_cpu'):
-                setattr(obj, key, val.to_cpu())
-        return obj
-    '''
+        return utils.to_cpu(self, obj)
+
 
 def get_jk(dfobj, dms_tag, hermi=1, with_j=True, with_k=True, direct_scf_tol=1e-14, omega=None):
     '''
     get jk with density fitting
     outputs and input are on the same device
     TODO: separate into three cases: j only, k only, j and k
     '''
@@ -418,15 +400,15 @@
     intopt = getattr(dfobj, 'intopt', None)
     if intopt is None:
         dfobj.build(direct_scf_tol=direct_scf_tol)
         intopt = dfobj.intopt
     j2c = dfobj.j2c
     rhoj = int3c2e.get_j_int3c2e_pass1(intopt, dm)
     if dfobj.cd_low.tag == 'eig':
-        rhoj = cupy.linalg.lstsq(j2c, rhoj)
+        rhoj, _, _, _ = cupy.linalg.lstsq(j2c, rhoj)
     else:
         rhoj = cupy.linalg.solve(j2c, rhoj)
 
     rhoj *= 2.0
     vj = int3c2e.get_j_int3c2e_pass2(intopt, rhoj)
     return vj
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/grad/__init__.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/grad/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/grad/rhf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/grad/rhf.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,19 +13,18 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import copy
 import numpy
 import cupy
 from cupyx.scipy.linalg import solve_triangular
-from pyscf.df.grad import rhf
-from pyscf import lib, scf, gto
+from pyscf import scf
 from gpu4pyscf.df import int3c2e
 from gpu4pyscf.lib.cupy_helper import print_mem_info, tag_array, unpack_tril, contract, load_library, take_last2d
-from gpu4pyscf.grad.rhf import grad_elec
+from gpu4pyscf.grad import rhf as rhf_grad
 from gpu4pyscf import __config__
 from gpu4pyscf.lib import logger
 
 libcupy_helper = load_library('libcupy_helper')
 
 MIN_BLK_SIZE = getattr(__config__, 'min_ao_blksize', 128)
 ALIGNED = getattr(__config__, 'ao_aligned', 64)
@@ -181,30 +180,30 @@
             rhoj_tmp = rhoj_tmp.astype(cupy.float64, order='C')
 
         if(rhok_tmp.flags['C_CONTIGUOUS'] == False):
             rhok_tmp = rhok_tmp.astype(cupy.float64, order='C')
         '''
         '''
         # outcore implementation
-        int3c2e.get_int3c2e_ip_slice(intopt, cp_kl_id, 1, out=buf)
+        buf = int3c2e.get_int3c2e_ip_slice(intopt, cp_kl_id, 1)
         size = 3*(k1-k0)*nao_cart*nao_cart
         int3c_ip = buf[:size].reshape([3,k1-k0,nao_cart,nao_cart], order='C')
-        rhoj_tmp = contract('xpji,ij->xip', int3c_ip, dm_cart)
-        vj += contract('xip,p->xi', rhoj_tmp, rhoj_cart[k0:k1])
-        vk += contract('pji,xpji->xi', rhok_tmp, int3c_ip)
-
-        int3c2e.get_int3c2e_ip_slice(intopt, cp_kl_id, 2, out=buf)
-        rhoj_tmp = contract('xpji,ji->xp', int3c_ip, dm_cart)
-        vjaux[:, k0:k1] = contract('xp,p->xp', rhoj_tmp, rhoj_cart[k0:k1])
-        vkaux[:, k0:k1] = contract('xpji,pji->xp', int3c_ip, rhok_tmp)
+        rhoj_tmp0 = contract('xpji,ij->xip', int3c_ip, dm_cart)
+        vj_outcore = contract('xip,p->xi', rhoj_tmp0, rhoj_cart[k0:k1])
+        vk_outcore = contract('pji,xpji->xi', rhok_tmp, int3c_ip)
+
+        buf = int3c2e.get_int3c2e_ip_slice(intopt, cp_kl_id, 2)
+        int3c_ip = buf[:size].reshape([3,k1-k0,nao_cart,nao_cart], order='C')
+        rhoj_tmp0 = contract('xpji,ji->xp', int3c_ip, dm_cart)
+        vjaux_outcore = contract('xp,p->xp', rhoj_tmp0, rhoj_cart[k0:k1])
+        vkaux_outcore = contract('xpji,pji->xp', int3c_ip, rhok_tmp)
         '''
         vj_tmp, vk_tmp = int3c2e.get_int3c2e_ip_jk(intopt, cp_kl_id, 'ip1', rhoj_tmp, rhok_tmp, dm_cart, omega=omega)
         if with_j: vj += vj_tmp
         if with_k: vk += vk_tmp
-
         vj_tmp, vk_tmp = int3c2e.get_int3c2e_ip_jk(intopt, cp_kl_id, 'ip2', rhoj_tmp, rhok_tmp, dm_cart, omega=omega)
         if with_j: vjaux[:, k0:k1] = vj_tmp
         if with_k: vkaux[:, k0:k1] = vk_tmp
 
         rhoj_tmp = rhok_tmp = vj_tmp = vk_tmp = None
         t1 = log.timer_debug1(f'calculate {cp_kl_id:3d} / {len(intopt.aux_log_qs):3d}, {k1-k0:3d} slices', *t1)
 
@@ -233,19 +232,27 @@
     if with_k:
         vkaux = vkaux[:, rev_cart_aux_idx]
         vkaux_3c = cupy.asarray([-vkaux[:,p0:p1].sum(axis=1) for p0, p1 in auxslices[:,2:]])
         vkaux = vkaux_2c + vkaux_3c
     return vj, vk, vjaux, vkaux
 
 
-class Gradients(rhf.Gradients):
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+class Gradients(rhf_grad.Gradients):
+    from gpu4pyscf.lib.utils import to_gpu, device
+
+    _keys = {'with_df', 'auxbasis_response'}
+    def __init__(self, mf):
+        # Whether to include the response of DF auxiliary basis when computing
+        # nuclear gradients of J/K matrices
+        self.auxbasis_response = True
+        rhf_grad.Gradients.__init__(self, mf)
 
     get_jk = get_jk
-    grad_elec = grad_elec
+    grad_elec = rhf_grad.grad_elec
+    check_sanity = NotImplemented
 
     def get_j(self, mol=None, dm=None, hermi=0):
         vj, _, vjaux, _ = self.get_jk(mol, dm, with_k=False)
         return vj, vjaux
 
     def get_k(self, mol=None, dm=None, hermi=0):
         _, vk, _, vkaux = self.get_jk(mol, dm, with_j=False)
@@ -263,7 +270,9 @@
         return vhf
 
     def extra_force(self, atom_id, envs):
         if self.auxbasis_response:
             return envs['dvhf'].aux[atom_id]
         else:
             return 0
+
+Grad = Gradients
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/grad/rks.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/grad/rks.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 
 import numpy
 import cupy
 import pyscf
 from pyscf import lib
+from pyscf.df.grad import rks as df_rks_grad
 from gpu4pyscf.grad import rks as rks_grad
-from gpu4pyscf.df.grad.rhf import get_jk, grad_elec
+from gpu4pyscf.df.grad import rhf as df_rhf_grad
 from gpu4pyscf.lib.cupy_helper import contract, tag_array
 from gpu4pyscf.lib import logger
 
 def get_veff(ks_grad, mol=None, dm=None):
 
     '''Coulomb + XC functional
     '''
@@ -111,27 +112,32 @@
     if ks_grad.auxbasis_response:
         logger.debug1(ks_grad, 'sum(auxbasis response) %s', e1_aux.sum(axis=0))
     else:
         e1_aux = None
     vxc = tag_array(vxc, aux=e1_aux)
     return vxc
 
-class Gradients(rks_grad.Gradients, pyscf.df.grad.rks.Gradients):
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+class Gradients(rks_grad.Gradients):
+    from gpu4pyscf.lib.utils import to_gpu, device
 
-    get_jk = get_jk
+    _keys = df_rks_grad.Gradients._keys
+    __init__ = df_rks_grad.Gradients.__init__
+
+    get_jk = df_rhf_grad.Gradients.get_jk
+    grad_elec = df_rhf_grad.Gradients.grad_elec
     get_veff = get_veff
-    grad_elec = grad_elec
 
     def get_j(self, mol=None, dm=None, hermi=0, omega=None):
         vj, _, vjaux, _ = self.get_jk(mol, dm, with_k=False, omega=omega)
         return vj, vjaux
 
     def get_k(self, mol=None, dm=None, hermi=0, omega=None):
         _, vk, _, vkaux = self.get_jk(mol, dm, with_j=False, omega=omega)
         return vk, vkaux
 
     def extra_force(self, atom_id, envs):
         if self.auxbasis_response:
             return envs['dvhf'].aux[atom_id]
         else:
             return 0
+
+Grad = Gradients
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/grad/uhf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/grad/uhf.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,29 +12,23 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import numpy as np
 import cupy
 import copy
-import time
-import ctypes
 from cupyx.scipy.linalg import solve_triangular
-from gpu4pyscf.df.grad import rhf
-from pyscf import lib, scf, gto
+from pyscf import scf
 from gpu4pyscf.df import int3c2e
-from gpu4pyscf.lib.cupy_helper import print_mem_info, tag_array, unpack_tril, contract, load_library, take_last2d
+from gpu4pyscf.lib.cupy_helper import tag_array, contract, load_library, take_last2d
 from gpu4pyscf.grad import uhf as uhf_grad
-from gpu4pyscf.grad.rhf import grad_elec
 from gpu4pyscf import __config__
 from gpu4pyscf.lib import logger
-from gpu4pyscf.scf.hf import _VHFOpt
 
 libgvhf = load_library('libgvhf')
-LMAX_ON_GPU = 3
 FREE_CUPY_CACHE = True
 BINSIZE = 128
 
 def get_jk(mf_grad, mol=None, dm0=None, hermi=0, with_j=True, with_k=True, omega=None, mo_coeff=None, mo_occ=None, dm2 = None):
     if mol is None: mol = mf_grad.mol
     #TODO: dm has to be the SCF density matrix in this version.  dm should be
     # extended to any 1-particle density matrix
@@ -63,21 +57,21 @@
 
     if isinstance(mf_grad.base, scf.rohf.ROHF):
         raise NotImplementedError()
     if mo_coeff is None:
         mo_coeff = cupy.asarray(mf_grad.base.mo_coeff)
     if mo_occ is None:
         mo_occ = cupy.asarray(mf_grad.base.mo_occ)
-    sph_ao_idx = intopt.sph_ao_idx
-    dm = take_last2d(dm0, sph_ao_idx)
+    ao_idx = intopt.ao_idx
+    dm = take_last2d(dm0, ao_idx)
     if dm2 is not None:
-        dm2_tmp = take_last2d(dm2, sph_ao_idx)
+        dm2_tmp = take_last2d(dm2, ao_idx)
     # (L|ij) -> rhoj: (L), rhok: (L|oo)
     orbo = mo_coeff[:,mo_occ>0] * mo_occ[mo_occ>0] ** 0.5
-    orbo = orbo[sph_ao_idx, :]
+    orbo = orbo[ao_idx, :]
     nocc = orbo.shape[-1]
 
     # (L|ij) -> rhoj: (L), rhok: (L|oo)
     low = with_df.cd_low
     rows = with_df.intopt.cderi_row
     cols = with_df.intopt.cderi_col
     dm_sparse = dm[rows, cols]
@@ -110,30 +104,35 @@
     # (d/dX P|Q) contributions
     if omega and omega > 1e-10:
         with auxmol.with_range_coulomb(omega):
             int2c_e1 = auxmol.intor('int2c2e_ip1')
     else:
         int2c_e1 = auxmol.intor('int2c2e_ip1')
     int2c_e1 = cupy.asarray(int2c_e1)
-    sph_aux_idx = intopt.sph_aux_idx
-    rev_aux_idx = np.argsort(sph_aux_idx)
+    aux_ao_idx = intopt.aux_ao_idx
+    rev_aux_idx = np.argsort(aux_ao_idx)
     auxslices = auxmol.aoslice_by_atom()
     aux_cart2sph = intopt.aux_cart2sph
     low_t = low.T.copy()
     if with_j:
         if low.tag == 'eig':
             rhoj = cupy.dot(low_t.T, rhoj)
             if dm2 is not None:
                 rhoj2 = cupy.dot(low_t.T, rhoj2)
         elif low.tag == 'cd':
             rhoj = solve_triangular(low_t, rhoj, lower=False, overwrite_b=True)
             if dm2 is not None:
                 rhoj2 = solve_triangular(low_t, rhoj2, lower=False, overwrite_b=True)
-        rhoj_cart = contract('pq,q->p', aux_cart2sph, rhoj)
+        if not auxmol.cart:
+            rhoj_cart = contract('pq,q->p', aux_cart2sph, rhoj)
+        else:
+            rhoj_cart = rhoj
+
         rhoj = rhoj[rev_aux_idx]
+
         if dm2 is not None:
             rhoj2 = rhoj2[rev_aux_idx]
         tmp = contract('xpq,q->xp', int2c_e1, rhoj)
         if dm2 is not None:
             vjaux = -contract('xp,p->xp', tmp, rhoj2)
         else:
             vjaux = -contract('xp,p->xp', tmp, rhoj)
@@ -145,35 +144,44 @@
         elif low.tag == 'cd':
             rhok = solve_triangular(low_t, rhok.reshape(naux, -1), lower=False, overwrite_b=True).reshape(naux, nocc, nocc)
         tmp = contract('pij,qij->pq', rhok, rhok)
         tmp = take_last2d(tmp, rev_aux_idx)
         vkaux = -contract('xpq,pq->xp', int2c_e1, tmp)
         vkaux_2c = cupy.array([-vkaux[:,p0:p1].sum(axis=1) for p0, p1 in auxslices[:,2:]])
         vkaux = tmp = None
-        rhok_cart = contract('pq,qkl->pkl', aux_cart2sph, rhok)
+        if not auxmol.cart:
+            rhok_cart = contract('pq,qkl->pkl', aux_cart2sph, rhok)
+        else:
+            rhok_cart = rhok
         rhok = None
     low_t = None
     t0 = log.timer_debug1('rhoj and rhok', *t0)
     int2c_e1 = None
 
     nao_cart = intopt.mol.nao
     block_size = with_df.get_blksize(nao=nao_cart)
     intopt.clear()
     # rebuild with aosym
     intopt.build(mf.direct_scf_tol, diag_block_with_triu=True, aosym=False,
                  group_size_aux=block_size)#, group_size=block_size)
-
-    # sph2cart for ao
-    cart2sph = intopt.cart2sph
-    orbo_cart = cart2sph @ orbo
-    if dm2 is None:
-        dm_cart = cart2sph @ dm @ cart2sph.T
+    if not intopt._mol.cart:
+        # sph2cart for ao
+        cart2sph = intopt.cart2sph
+        orbo_cart = cart2sph @ orbo
+        if dm2 is None:
+            dm_cart = cart2sph @ dm @ cart2sph.T
+        else:
+            dm2_tmp = take_last2d(dm2, ao_idx)
+            dm_cart = cart2sph @ dm2_tmp @ cart2sph.T
     else:
-        dm2_tmp = take_last2d(dm2, sph_ao_idx)
-        dm_cart = cart2sph @ dm2_tmp @ cart2sph.T
+        if dm2 is None:
+            dm_cart = dm
+        else:
+            dm_cart = take_last2d(dm2, ao_idx)
+        orbo_cart = orbo
     dm = orbo = None
 
     vj = vk = rhoj_tmp = rhok_tmp = None
     vjaux = vkaux = None
 
     naux_cart = intopt.auxmol.nao
     if with_j:
@@ -273,18 +281,20 @@
 
     def get_k(self, mol=None, dm=None, hermi=0, mo_coeff=None, mo_occ=None, dm2 = None):
         _, vk, _, vkaux = self.get_jk(mol, dm, with_j=False, mo_coeff=mo_coeff, mo_occ=mo_occ, dm2=dm2)
         return vk, vkaux
 
 
     def get_veff(self, mol=None, dm=None):
-        vj0, vk0, vjaux0, vkaux0 = self.get_jk(mol, dm[0], mo_coeff=self.base.mo_coeff[0], mo_occ=self.base.mo_occ[0])
-        vj1, vk1, vjaux1, vkaux1 = self.get_jk(mol, dm[1], mo_coeff=self.base.mo_coeff[1], mo_occ=self.base.mo_occ[1])
-        vj0_m1, vjaux0_m1 = self.get_j(mol, dm[0], mo_coeff=self.base.mo_coeff[0], mo_occ=self.base.mo_occ[0], dm2=dm[1])
-        vj1_m0, vjaux1_m0 = self.get_j(mol, dm[1], mo_coeff=self.base.mo_coeff[1], mo_occ=self.base.mo_occ[1], dm2=dm[0])
+        mo_a, mo_b = self.base.mo_coeff
+        mo_occa, mo_occb = self.base.mo_occ
+        vj0, vk0, vjaux0, vkaux0 = self.get_jk(mol, dm[0], mo_coeff=mo_a, mo_occ=mo_occa)
+        vj1, vk1, vjaux1, vkaux1 = self.get_jk(mol, dm[1], mo_coeff=mo_b, mo_occ=mo_occb)
+        vj0_m1, vjaux0_m1 = self.get_j(mol, dm[0], mo_coeff=mo_a, mo_occ=mo_occa, dm2=dm[1])
+        vj1_m0, vjaux1_m0 = self.get_j(mol, dm[1], mo_coeff=mo_b, mo_occ=mo_occb, dm2=dm[0])
         vhf = vj0 + vj1 + vj0_m1 + vj1_m0 - vk0 - vk1
         if self.auxbasis_response:
             e1_aux = vjaux0 + vjaux1 + vjaux0_m1 + vjaux1_m0 - vkaux0 - vkaux1
             logger.debug1(self, 'sum(auxbasis response) %s', e1_aux.sum(axis=0))
         else:
             e1_aux = None
         vhf = tag_array(vhf, aux=e1_aux)
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/grad/uks.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/grad/uks.py`

 * *Files 25% similar despite different names*

```diff
@@ -87,28 +87,31 @@
     vxc+= contract('nik,ik->ni', tmp, occ_coeff1)
 
     aoslices = mol.aoslice_by_atom()
     vxc = [vxc[:,p0:p1].sum(axis=1) for p0, p1 in aoslices[:,2:]]
     vxc = cupy.asarray(vxc)
 
     if not ni.libxc.is_hybrid_xc(mf.xc):
-        vj0, vjaux0 = ks_grad.get_j(mol, dm[0], mo_coeff=ks_grad.base.mo_coeff[0], mo_occ=ks_grad.base.mo_occ[0])
-        vj1, vjaux1 = ks_grad.get_j(mol, dm[1], mo_coeff=ks_grad.base.mo_coeff[1], mo_occ=ks_grad.base.mo_occ[1])
-        vj0_m1, vjaux0_m1 = ks_grad.get_j(mol, dm[0], mo_coeff=ks_grad.base.mo_coeff[0], mo_occ=ks_grad.base.mo_occ[0], dm2=dm[1])
-        vj1_m0, vjaux1_m0 = ks_grad.get_j(mol, dm[1], mo_coeff=ks_grad.base.mo_coeff[1], mo_occ=ks_grad.base.mo_occ[1], dm2=dm[0])
+        mo_a, mo_b = ks_grad.base.mo_coeff
+        mo_occa, mo_occb = ks_grad.base.mo_occ
+        vj0, vjaux0 = ks_grad.get_j(mol, dm[0], mo_coeff=mo_a, mo_occ=mo_occa)
+        vj1, vjaux1 = ks_grad.get_j(mol, dm[1], mo_coeff=mo_b, mo_occ=mo_occb)
+        vj0_m1, vjaux0_m1 = ks_grad.get_j(mol, dm[0], mo_coeff=mo_a, mo_occ=mo_occa, dm2=dm[1])
+        vj1_m0, vjaux1_m0 = ks_grad.get_j(mol, dm[1], mo_coeff=mo_b, mo_occ=mo_occb, dm2=dm[0])
         if ks_grad.auxbasis_response:
             e1_aux = vjaux0 + vjaux1 + vjaux0_m1 + vjaux1_m0
         vxc += vj0 + vj1 + vj0_m1 + vj1_m0
     else:
         omega, alpha, hyb = ni.rsh_and_hybrid_coeff(mf.xc, spin=mol.spin)
-
-        vj0, vk0, vjaux0, vkaux0 = ks_grad.get_jk(mol, dm[0], mo_coeff=ks_grad.base.mo_coeff[0], mo_occ=ks_grad.base.mo_occ[0])
-        vj1, vk1, vjaux1, vkaux1 = ks_grad.get_jk(mol, dm[1], mo_coeff=ks_grad.base.mo_coeff[1], mo_occ=ks_grad.base.mo_occ[1])
-        vj0_m1, vjaux0_m1 = ks_grad.get_j(mol, dm[0], mo_coeff=ks_grad.base.mo_coeff[0], mo_occ=ks_grad.base.mo_occ[0], dm2=dm[1])
-        vj1_m0, vjaux1_m0 = ks_grad.get_j(mol, dm[1], mo_coeff=ks_grad.base.mo_coeff[1], mo_occ=ks_grad.base.mo_occ[1], dm2=dm[0])
+        mo_a, mo_b = ks_grad.base.mo_coeff
+        mo_occa, mo_occb = ks_grad.base.mo_occ
+        vj0, vk0, vjaux0, vkaux0 = ks_grad.get_jk(mol, dm[0], mo_coeff=mo_a, mo_occ=mo_occa)
+        vj1, vk1, vjaux1, vkaux1 = ks_grad.get_jk(mol, dm[1], mo_coeff=mo_b, mo_occ=mo_occb)
+        vj0_m1, vjaux0_m1 = ks_grad.get_j(mol, dm[0], mo_coeff=mo_a, mo_occ=mo_occa, dm2=dm[1])
+        vj1_m0, vjaux1_m0 = ks_grad.get_j(mol, dm[1], mo_coeff=mo_b, mo_occ=mo_occb, dm2=dm[0])
         vj = vj0 + vj1 + vj0_m1 + vj1_m0
         vk = (vk0 + vk1) * hyb
         if ks_grad.auxbasis_response:
             vj_aux = vjaux0 + vjaux1 + vjaux0_m1 + vjaux1_m0
             vk_aux = (vkaux0+vkaux1) * hyb
 
         if omega != 0:
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/hessian/__init__.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/hessian/rhf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/rhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -574,15 +574,16 @@
         if with_k:
             vk1 = vk1_int3c[ia] + _ao2mo(vk1_ao)
         yield ia, h1, vj1, vk1
 
 class Hessian(rhf_hess.Hessian):
     '''Non-relativistic restricted Hartree-Fock hessian'''
 
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
-
+    from gpu4pyscf.lib.utils import to_gpu, device
     def __init__(self, mf):
         self.auxbasis_response = 1
         rhf_hess.Hessian.__init__(self, mf)
 
     partial_hess_elec = partial_hess_elec
     make_h1 = make_h1
+    kernel = rhf_hess.kernel
+    hess = kernel
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/hessian/rks.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/rks.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 Non-relativistic RKS analytical Hessian
 '''
 
 
 import numpy
 import cupy
 from pyscf import lib
+from gpu4pyscf.hessian import rhf as rhf_hess
 from gpu4pyscf.hessian import rks as rks_hess
 from gpu4pyscf.df.hessian import rhf as df_rhf_hess
 from gpu4pyscf.lib import logger
 from gpu4pyscf.lib.cupy_helper import contract
 
 def partial_hess_elec(hessobj, mo_energy=None, mo_coeff=None, mo_occ=None,
                       atmlst=None, max_memory=4000, verbose=None):
@@ -109,17 +110,11 @@
     '''Non-relativistic RKS hessian'''
     from gpu4pyscf.lib.utils import to_gpu, device
 
     def __init__(self, mf):
         self.auxbasis_response = 1
         rks_hess.Hessian.__init__(self, mf)
 
-    def to_cpu(self):
-        from gpu4pyscf.lib.utils import to_cpu
-        from pyscf.df.hessian.rks import Hessian
-        # to_cpu returns an rhf.Hessian object
-        obj = to_cpu(self)
-        return obj.view(Hessian)
-
     partial_hess_elec = partial_hess_elec
     make_h1 = make_h1
-
+    kernel = rhf_hess.kernel
+    hess = kernel
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/hessian/uhf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/uhf.py`

 * *Files 1% similar despite different names*

```diff
@@ -680,15 +680,17 @@
             vk1a = vk1a_int3c[ia] + _ao2mo(vk1a_ao, mocca, mo_coeff[0])
             vk1b = vk1b_int3c[ia] + _ao2mo(vk1b_ao, moccb, mo_coeff[1])
         yield ia, (h1a, h1b), (vj1a, vj1b), (vk1a, vk1b)
 
 class Hessian(uhf_hess.Hessian):
     '''Non-relativistic restricted Hartree-Fock hessian'''
 
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+    from gpu4pyscf.lib.utils import to_gpu, device
 
     def __init__(self, mf):
         self.auxbasis_response = 1
         uhf_hess.Hessian.__init__(self, mf)
 
     partial_hess_elec = partial_hess_elec
     make_h1 = make_h1
+    kernel = rhf_hess.kernel
+    hess = kernel
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/hessian/uks.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/uks.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,23 +122,17 @@
     '''Non-relativistic RKS hessian'''
     from gpu4pyscf.lib.utils import to_gpu, device
 
     def __init__(self, mf):
         self.auxbasis_response = 1
         uks_hess.Hessian.__init__(self, mf)
 
-    def to_cpu(self):
-        from gpu4pyscf.lib.utils import to_cpu
-        from pyscf.df.hessian.uks import Hessian
-        # to_cpu returns an rhf.Hessian object
-        obj = to_cpu(self)
-        return obj.view(Hessian)
-
     def solve_mo1(self, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
                   fx=None, atmlst=None, max_memory=4000, verbose=None):
         return uhf_hess.solve_mo1(self.base, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
                          fx, atmlst, max_memory, verbose)
 
     partial_hess_elec = partial_hess_elec
     make_h1 = make_h1
     hess_elec = uhf_hess.hess_elec
     kernel = rhf_hess.kernel
+    hess = kernel
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/int3c2e.py` & `gpu4pyscf-0.7.6/gpu4pyscf/df/int3c2e.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     block_c2s_diag, cart2sph, block_diag, contract, load_library, c2s_l, get_avail_mem, print_mem_info, take_last2d)
 from gpu4pyscf.lib import logger
 
 LMAX_ON_GPU = 8
 FREE_CUPY_CACHE = True
 STACK_SIZE_PER_THREAD = 8192 * 4
 BLKSIZE = 128
+NROOT_ON_GPU = 7
 
 libgvhf = load_library('libgvhf')
 libgint = load_library('libgint')
 libcupy_helper = load_library('libcupy_helper')
 
 def basis_seg_contraction(mol, allow_replica=False):
     '''transform generally contracted basis to segment contracted basis
@@ -162,14 +163,16 @@
 
         self.cp_idx = None
         self.cp_jdx = None
 
         self.log_qs = None
         self.aux_log_qs = None
 
+    init_cvhf_direct = _vhf.VHFOpt.init_cvhf_direct
+
     def clear(self):
         _vhf.VHFOpt.__del__(self)
         libgvhf.GINTdel_basis_prod(ctypes.byref(self.bpcache))
         return self
 
     def __del__(self):
         try:
@@ -194,16 +197,17 @@
         _, _, fake_uniq_l_ctr, fake_l_ctr_counts = sort_mol(fake_mol)
 
         # sort auxiliary mol
         sorted_auxmol, sorted_aux_idx, aux_uniq_l_ctr, aux_l_ctr_counts = sort_mol(self.auxmol)
         if group_size_aux is not None:
             aux_uniq_l_ctr, aux_l_ctr_counts = _split_l_ctr_groups(aux_uniq_l_ctr, aux_l_ctr_counts, group_size_aux)
 
-        tmp_mol = gto.mole.conc_mol(fake_mol, sorted_auxmol)
-        tot_mol = gto.mole.conc_mol(sorted_mol, tmp_mol)
+        tot_mol = sorted_mol + fake_mol + sorted_auxmol
+        tot_mol.cart = True
+        self.tot_mol = tot_mol
 
         # Initialize vhfopt after reordering mol._bas
         _vhf.VHFOpt.__init__(self, sorted_mol, self._intor, self._prescreen,
                              self._qcondname, self._dmcondname)
         self.direct_scf_tol = cutoff
 
         # TODO: is it more accurate to filter with overlap_cond (or exp_cond)?
@@ -232,16 +236,21 @@
         # cartesian ao index
         nao = cart_ao_loc[-1]
         ao_idx = np.array_split(np.arange(nao), cart_ao_loc[1:-1])
         self.cart_ao_idx = np.hstack([ao_idx[i] for i in sorted_idx])
         ncart = cart_ao_loc[-1]
         nsph = sph_ao_loc[-1]
         self.cart2sph = block_c2s_diag(ncart, nsph, self.angular, l_ctr_counts)
-        inv_idx = np.argsort(self.sph_ao_idx, kind='stable').astype(np.int32)
-        self.coeff = self.cart2sph[:, inv_idx]
+
+        if self._mol.cart:
+            inv_idx = np.argsort(self.cart_ao_idx, kind='stable').astype(np.int32)
+            self.coeff = cupy.eye(ncart)[:,inv_idx]
+        else:
+            inv_idx = np.argsort(self.sph_ao_idx, kind='stable').astype(np.int32)
+            self.coeff = self.cart2sph[:, inv_idx]
         cput1 = logger.timer_debug1(sorted_mol, 'AO cart2sph coeff', *cput1)
 
         # pairing auxiliary basis with fake basis set
         fake_l_ctr_offsets = np.append(0, np.cumsum(fake_l_ctr_counts))
         fake_l_ctr_offsets += l_ctr_offsets[-1]
         aux_l_ctr_offsets = np.append(0, np.cumsum(aux_l_ctr_counts))
 
@@ -261,16 +270,21 @@
         # cartesian aux index
         naux = cart_aux_loc[-1]
         ao_idx = np.array_split(np.arange(naux), cart_aux_loc[1:-1])
         self.cart_aux_idx = np.hstack([ao_idx[i] for i in sorted_aux_idx])
         ncart = cart_aux_loc[-1]
         nsph = sph_aux_loc[-1]
         self.aux_cart2sph = block_c2s_diag(ncart, nsph, self.aux_angular, aux_l_ctr_counts)
-        inv_idx = np.argsort(self.sph_aux_idx, kind='stable').astype(np.int32)
-        self.aux_coeff = self.aux_cart2sph[:, inv_idx]
+
+        if self._auxmol.cart:
+            inv_idx = np.argsort(self.cart_aux_idx, kind='stable').astype(np.int32)
+            self.aux_coeff = cupy.eye(ncart)[:,inv_idx]
+        else:
+            inv_idx = np.argsort(self.sph_aux_idx, kind='stable').astype(np.int32)
+            self.aux_coeff = self.aux_cart2sph[:, inv_idx]
         aux_l_ctr_offsets += fake_l_ctr_offsets[-1]
         cput1 = logger.timer_debug1(tot_mol, 'aux cart2sph coeff', *cput1)
 
         ao_loc = sorted_mol.ao_loc_nr(cart=self._mol.cart)
         self.ao_pairs_row, self.ao_pairs_col = get_ao_pairs(pair2bra, pair2ket, ao_loc)
         cderi_row = cupy.hstack(self.ao_pairs_row)
         cderi_col = cupy.hstack(self.ao_pairs_col)
@@ -279,28 +293,33 @@
         self.cderi_diag = cupy.argwhere(cderi_row == cderi_col)[:,0]
         cput1 = logger.timer_debug1(tot_mol, 'Get AO pairs', *cput1)
 
         aux_pair2bra = []
         aux_pair2ket = []
         aux_log_qs = []
         for p0, p1 in zip(aux_l_ctr_offsets[:-1], aux_l_ctr_offsets[1:]):
-            aux_pair2bra.append(np.arange(p0,p1))
-            aux_pair2ket.append(fake_l_ctr_offsets[0] * np.ones(p1-p0))
-            aux_log_qs.append(np.ones(p1-p0))
+            aux_pair2bra.append(np.arange(p0,p1,dtype=np.int32))
+            aux_pair2ket.append(fake_l_ctr_offsets[0] * np.ones(p1-p0, dtype=np.int32))
+            aux_log_qs.append(np.ones(p1-p0, dtype=np.int32))
 
         self.aux_log_qs = aux_log_qs.copy()
         pair2bra += aux_pair2bra
         pair2ket += aux_pair2ket
 
+        self.aux_pair2bra = aux_pair2bra
+        self.aux_pair2ket = aux_pair2ket
+
         uniq_l_ctr = np.concatenate([uniq_l_ctr, fake_uniq_l_ctr, aux_uniq_l_ctr])
         l_ctr_offsets = np.concatenate([
             l_ctr_offsets,
             fake_l_ctr_offsets[1:],
             aux_l_ctr_offsets[1:]])
 
+        self.pair2bra = pair2bra
+        self.pair2ket = pair2ket
         bas_pair2shls = np.hstack(pair2bra + pair2ket).astype(np.int32).reshape(2,-1)
         bas_pairs_locs = np.append(0, np.cumsum([x.size for x in pair2bra])).astype(np.int32)
         log_qs = log_qs + aux_log_qs
         ao_loc = tot_mol.ao_loc_nr(cart=True)
         ncptype = len(log_qs)
 
         self.bpcache = ctypes.POINTER(BasisProdCache)()
@@ -477,14 +496,23 @@
     nao = intopt.mol.nao
     naux = intopt.auxmol.nao
     norb = nao + naux + 1
     ao_loc = intopt.ao_loc
     aux_ao_loc = intopt.aux_ao_loc
     comp = 3**order
 
+    lmax = intopt.mol._bas[:gto.ANG_OF].max()
+    aux_lmax = intopt.auxmol._bas[:gto.ANG_OF].max()
+    nroots = (lmax + aux_lmax + order)//2 + 1
+    if nroots > NROOT_ON_GPU:
+        from pyscf.gto.moleintor import getints, make_cintopt
+        pmol = intopt.tot_mol
+        intor = pmol._add_suffix('int3c2e_' + ip_type)
+        opt = make_cintopt(pmol._atm, pmol._bas, pmol._env, intor)
+
     nbins = 1
     for aux_id, log_q_kl in enumerate(intopt.aux_log_qs):
         cp_kl_id = aux_id + len(intopt.log_qs)
         lk = intopt.aux_angular[aux_id]
 
         for cp_ij_id, log_q_ij in enumerate(intopt.log_qs):
             cpi = intopt.cp_idx[cp_ij_id]
@@ -501,30 +529,40 @@
 
             bins_locs_ij = np.array([0, len(log_q_ij)], dtype=np.int32)
             bins_locs_kl = np.array([0, len(log_q_kl)], dtype=np.int32)
 
             ao_offsets = np.array([i0,j0,nao+1+k0,nao], dtype=np.int32)
             strides = np.array([1, ni, ni*nj, ni*nj*nk], dtype=np.int32)
 
-            int3c_blk = cupy.zeros([comp, nk, nj, ni], order='C', dtype=np.float64)
-            err = fn(
-                ctypes.cast(stream.ptr, ctypes.c_void_p),
-                intopt.bpcache,
-                ctypes.cast(int3c_blk.data.ptr, ctypes.c_void_p),
-                ctypes.c_int(norb),
-                strides.ctypes.data_as(ctypes.c_void_p),
-                ao_offsets.ctypes.data_as(ctypes.c_void_p),
-                bins_locs_ij.ctypes.data_as(ctypes.c_void_p),
-                bins_locs_kl.ctypes.data_as(ctypes.c_void_p),
-                ctypes.c_int(nbins),
-                ctypes.c_int(cp_ij_id),
-                ctypes.c_int(cp_kl_id),
-                ctypes.c_double(omega))
-            if err != 0:
-                raise RuntimeError(f'GINT_fill_int3c2e general failed, err={err}')
+            # Use GPU kernels for low-angular momentum
+            if (li + lj + lk + order)//2 + 1 < NROOT_ON_GPU:
+                int3c_blk = cupy.zeros([comp, nk, nj, ni], order='C', dtype=np.float64)
+                err = fn(
+                    ctypes.cast(stream.ptr, ctypes.c_void_p),
+                    intopt.bpcache,
+                    ctypes.cast(int3c_blk.data.ptr, ctypes.c_void_p),
+                    ctypes.c_int(norb),
+                    strides.ctypes.data_as(ctypes.c_void_p),
+                    ao_offsets.ctypes.data_as(ctypes.c_void_p),
+                    bins_locs_ij.ctypes.data_as(ctypes.c_void_p),
+                    bins_locs_kl.ctypes.data_as(ctypes.c_void_p),
+                    ctypes.c_int(nbins),
+                    ctypes.c_int(cp_ij_id),
+                    ctypes.c_int(cp_kl_id),
+                    ctypes.c_double(omega))
+                if err != 0:
+                    raise RuntimeError(f'GINT_fill_int3c2e general failed, err={err}')
+            else:
+                # TODO: sph2cart in CPU?
+                ishl0, ishl1 = intopt.pair2bra[cp_ij_id][0], intopt.pair2bra[cp_ij_id][-1]+1
+                jshl0, jshl1 = intopt.pair2ket[cp_ij_id][0], intopt.pair2ket[cp_ij_id][-1]+1
+                kshl0, kshl1 = intopt.aux_pair2bra[aux_id][0], intopt.aux_pair2bra[aux_id][-1]+1
+                shls_slice = np.array([ishl0, ishl1, jshl0, jshl1, kshl0, kshl1], dtype=np.int64)
+                int3c_cpu = getints(intor, pmol._atm, pmol._bas, pmol._env, shls_slice, cintopt=opt).transpose([0,3,2,1])
+                int3c_blk = cupy.asarray(int3c_cpu)
 
             if not intopt._auxmol.cart:
                 int3c_blk = cart2sph(int3c_blk, axis=1, ang=lk)
             if not intopt._mol.cart:
                 int3c_blk = cart2sph(int3c_blk, axis=2, ang=lj)
                 int3c_blk = cart2sph(int3c_blk, axis=3, ang=li)
 
@@ -663,17 +701,16 @@
         bins_locs_ij.ctypes.data_as(ctypes.c_void_p),
         bins_locs_kl.ctypes.data_as(ctypes.c_void_p),
         ctypes.c_int(ncp_ij),
         ctypes.c_int(ncp_kl))
     if err != 0:
         raise RuntimeError('CUDA error in get_j_pass1')
 
-    if not intopt._auxmol.cart:
-        aux_coeff = intopt.aux_coeff
-        rhoj = cupy.dot(rhoj, aux_coeff)
+    aux_coeff = intopt.aux_coeff
+    rhoj = cupy.dot(rhoj, aux_coeff)
     return rhoj
 
 def get_j_int3c2e_pass2(intopt, rhoj):
     '''
     get vj pass2 for int3c2e
     '''
     n_dm = 1
@@ -686,17 +723,16 @@
 
     bins_locs_ij = np.append(0, np.cumsum(num_cp_ij)).astype(np.int32)
     bins_locs_kl = np.append(0, np.cumsum(num_cp_kl)).astype(np.int32)
 
     ncp_ij = len(intopt.log_qs)
     ncp_kl = len(intopt.aux_log_qs)
 
-    if not intopt._auxmol.cart:
-        aux_coeff = intopt.aux_coeff
-        rhoj = cupy.dot(aux_coeff, rhoj)
+    aux_coeff = intopt.aux_coeff
+    rhoj = cupy.dot(aux_coeff, rhoj)
 
     err = libgvhf.GINTbuild_j_int3c2e_pass2(
         intopt.bpcache,
         ctypes.cast(vj.data.ptr, ctypes.c_void_p),
         ctypes.cast(rhoj.data.ptr, ctypes.c_void_p),
         ctypes.c_int(norb),
         ctypes.c_int(naux),
@@ -1063,30 +1099,34 @@
     if out is None:
         int3c_blk = cupy.zeros([3, nk, nao, nao], order='C', dtype=np.float64)
         strides = np.array([1, nao, nao*nao, nao*nao*nk], dtype=np.int32)
     else:
         int3c_blk = out
         # will be filled in f-contiguous
         strides = np.array([1, nao, nao*nao, nao*nao*nk], dtype=np.int32)
-
+    if ip_type == 1:
+        fn = libgint.GINTfill_int3c2e_ip1
+    elif ip_type == 2:
+        fn = libgint.GINTfill_int3c2e_ip2
+    else:
+        raise
     for cp_ij_id, log_q_ij in enumerate(intopt.log_qs):
         bins_locs_ij = np.array([0, len(log_q_ij)], dtype=np.int32)
-        err = libgint.GINTfill_int3c2e_ip(
+        err = fn(
             ctypes.cast(stream.ptr, ctypes.c_void_p),
             intopt.bpcache,
             ctypes.cast(int3c_blk.data.ptr, ctypes.c_void_p),
             ctypes.c_int(norb),
             strides.ctypes.data_as(ctypes.c_void_p),
             ao_offsets.ctypes.data_as(ctypes.c_void_p),
             bins_locs_ij.ctypes.data_as(ctypes.c_void_p),
             bins_locs_kl.ctypes.data_as(ctypes.c_void_p),
             ctypes.c_int(nbins),
             ctypes.c_int(cp_ij_id),
             ctypes.c_int(cp_kl_id),
-            ctypes.c_int(ip_type),
             ctypes.c_double(omega))
 
         if err != 0:
             raise RuntimeError(f'GINT_fill_int2e_ip failed, err={err}')
 
     return int3c_blk
 
@@ -1193,14 +1233,24 @@
 
     nao = mol.nao
     naux = auxmol.nao
 
     intopt = VHFOpt(mol, auxmol, 'int2e')
     intopt.build(direct_scf_tol, diag_block_with_triu=True, aosym=False, group_size=BLKSIZE, group_size_aux=BLKSIZE)
 
+    lmax = mol._bas[:gto.ANG_OF].max()
+    aux_lmax = auxmol._bas[:gto.ANG_OF].max()
+    nroots = (lmax + aux_lmax + order)//2 + 1
+    if nroots > NROOT_ON_GPU:
+        from pyscf.gto.moleintor import getints, make_cintopt
+        mol = intopt.mol
+        pmol = intopt.tot_mol
+        intor = pmol._add_suffix('int3c2e_' + ip_type)
+        opt = make_cintopt(pmol._atm, pmol._bas, pmol._env, intor)
+
     nao_cart = intopt.mol.nao
     naux_cart = intopt.auxmol.nao
     norb_cart = nao_cart + naux_cart + 1
     ao_loc = intopt.ao_loc
     aux_ao_loc = intopt.aux_ao_loc
     comp = 3**order
     int3c = cupy.zeros([comp, naux, nao, nao], order='C')
@@ -1223,30 +1273,39 @@
 
             bins_locs_ij = np.array([0, len(log_q_ij)], dtype=np.int32)
             bins_locs_kl = np.array([0, len(log_q_kl)], dtype=np.int32)
 
             ao_offsets = np.array([i0,j0,nao_cart+1+k0,nao_cart], dtype=np.int32)
             strides = np.array([1, ni, ni*nj, ni*nj*nk], dtype=np.int32)
 
-            int3c_blk = cupy.zeros([comp, nk, nj, ni], order='C', dtype=np.float64)
-            err = fn(
-                ctypes.cast(stream.ptr, ctypes.c_void_p),
-                intopt.bpcache,
-                ctypes.cast(int3c_blk.data.ptr, ctypes.c_void_p),
-                ctypes.c_int(norb_cart),
-                strides.ctypes.data_as(ctypes.c_void_p),
-                ao_offsets.ctypes.data_as(ctypes.c_void_p),
-                bins_locs_ij.ctypes.data_as(ctypes.c_void_p),
-                bins_locs_kl.ctypes.data_as(ctypes.c_void_p),
-                ctypes.c_int(nbins),
-                ctypes.c_int(cp_ij_id),
-                ctypes.c_int(cp_kl_id),
-                ctypes.c_double(omega))
-            if err != 0:
-                raise RuntimeError("int3c2e failed\n")
+            # Use GPU kernels for low-angular momentum
+            if (li + lj + lk + order)//2 + 1 < NROOT_ON_GPU:
+                int3c_blk = cupy.zeros([comp, nk, nj, ni], order='C', dtype=np.float64)
+                err = fn(
+                    ctypes.cast(stream.ptr, ctypes.c_void_p),
+                    intopt.bpcache,
+                    ctypes.cast(int3c_blk.data.ptr, ctypes.c_void_p),
+                    ctypes.c_int(norb_cart),
+                    strides.ctypes.data_as(ctypes.c_void_p),
+                    ao_offsets.ctypes.data_as(ctypes.c_void_p),
+                    bins_locs_ij.ctypes.data_as(ctypes.c_void_p),
+                    bins_locs_kl.ctypes.data_as(ctypes.c_void_p),
+                    ctypes.c_int(nbins),
+                    ctypes.c_int(cp_ij_id),
+                    ctypes.c_int(cp_kl_id),
+                    ctypes.c_double(omega))
+                if err != 0:
+                    raise RuntimeError("int3c2e failed\n")
+            else:
+                ishl0, ishl1 = intopt.pair2bra[cp_ij_id][0], intopt.pair2bra[cp_ij_id][-1]+1
+                jshl0, jshl1 = intopt.pair2ket[cp_ij_id][0], intopt.pair2ket[cp_ij_id][-1]+1
+                kshl0, kshl1 = intopt.aux_pair2bra[aux_id][0], intopt.aux_pair2bra[aux_id][-1]+1
+                shls_slice = np.array([ishl0, ishl1, jshl0, jshl1, kshl0, kshl1], dtype=np.int64)
+                int3c_cpu = getints(intor, pmol._atm, pmol._bas, pmol._env, shls_slice, cintopt=opt).transpose([0,3,2,1])
+                int3c_blk = cupy.asarray(int3c_cpu)
 
             if not intopt._auxmol.cart:
                 int3c_blk = cart2sph(int3c_blk, axis=1, ang=lk)
             if not intopt._mol.cart:
                 int3c_blk = cart2sph(int3c_blk, axis=2, ang=lj)
                 int3c_blk = cart2sph(int3c_blk, axis=3, ang=li)
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/df/patch_pyscf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/scf/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,19 +11,13 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-'''
-Patch pyscf SCF modules to make all subclass of SCF class support GPU mode.
-'''
-
-from gpu4pyscf.df.df_jk import _density_fit, _get_jk
-from pyscf import df
-
-# The device attribute is patched to the pyscf base SCF module. It will be
-# seen by all subclasses.
-
-df.df_jk.density_fit = _density_fit
-df.df_jk.get_jk = _get_jk
+from . import hf
+from .hf import RHF
+from .uhf import UHF
+from .ghf import GHF
+from .rohf import ROHF
+from . import dispersion
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/dft/gen_grid.py` & `gpu4pyscf-0.7.6/gpu4pyscf/dft/gen_grid.py`

 * *Files 6% similar despite different names*

```diff
@@ -454,95 +454,44 @@
 
     if callable(var):
         return staticmethod(var)
     else:
         return var
 
 from pyscf.dft import gen_grid
-class Grids(gen_grid.Grids):
-    '''DFT mesh grids
+from gpu4pyscf.lib import utils
+class Grids(lib.StreamObject):
 
-    Attributes for Grids:
-        level : int
-            To control the number of radial and angular grids. Large number
-            leads to large mesh grids. The default level 3 corresponds to
-            (50,302) for H, He;
-            (75,302) for second row;
-            (80~105,434) for rest.
-
-            Grids settings at other levels can be found in
-            pyscf.dft.gen_grid.RAD_GRIDS and pyscf.dft.gen_grid.ANG_ORDER
-
-        atomic_radii : 1D array
-            | radi.BRAGG_RADII  (default)
-            | radi.COVALENT_RADII
-            | None : to switch off atomic radii adjustment
-
-        radii_adjust : function(mol, atomic_radii) => (function(atom_id, atom_id, g) => array_like_g)
-            Function to adjust atomic radii, can be one of
-            | radi.treutler_atomic_radii_adjust
-            | radi.becke_atomic_radii_adjust
-            | None : to switch off atomic radii adjustment
-
-        radi_method : function(n) => (rad_grids, rad_weights)
-            scheme for radial grids, can be one of
-            | radi.treutler  (default)
-            | radi.delley
-            | radi.mura_knowles
-            | radi.gauss_chebyshev
-
-        becke_scheme : function(v) => array_like_v
-            weight partition function, can be one of
-            | gen_grid.original_becke  (default)
-            | gen_grid.stratmann
-
-        prune : function(nuc, rad_grids, n_ang) => list_n_ang_for_each_rad_grid
-            scheme to reduce number of grids, can be one of
-            | gen_grid.nwchem_prune  (default)
-            | gen_grid.sg1_prune
-            | gen_grid.treutler_prune
-            | None : to switch off grid pruning
-
-        symmetry : bool
-            whether to symmetrize mesh grids (TODO)
-
-        atom_grid : dict
-            Set (radial, angular) grids for particular atoms.
-            Eg, grids.atom_grid = {'H': (20,110)} will generate 20 radial
-            grids and 110 angular grids for H atom.
-
-    Examples:
-
-    >>> mol = gto.M(atom='H 0 0 0; H 0 0 1.1')
-    >>> grids = dft.gen_grid.Grids(mol)
-    >>> grids.level = 4
-    >>> grids.build()
-    '''
-
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+    from gpu4pyscf.lib.utils import to_gpu, device
 
     atomic_radii = _load_conf(radi, 'dft_gen_grid_Grids_atomic_radii',
                                    radi.BRAGG_RADII)
     radii_adjust = _load_conf(radi, 'dft_gen_grid_Grids_radii_adjust',
                                    radi.treutler_atomic_radii_adjust)
     radi_method = _load_conf(radi, 'dft_gen_grid_Grids_radi_method',
                                   radi.treutler)
     becke_scheme = _load_conf(None, 'dft_gen_grid_Grids_becke_scheme',
                               original_becke)
     prune = _load_conf(None, 'dft_gen_grid_Grids_prune', nwchem_prune)
     level = getattr(__config__, 'dft_gen_grid_Grids_level', 3)
+    alignment    = ALIGNMENT_UNIT
+    cutoff       = CUTOFF
+    _keys        = gen_grid.Grids._keys
 
-    alignment = ALIGNMENT_UNIT
-    cutoff = CUTOFF
+    __init__    = gen_grid.Grids.__init__
 
     def __setattr__(self, key, val):
         if key in ('atom_grid', 'atomic_radii', 'radii_adjust', 'radi_method',
                    'becke_scheme', 'prune', 'level'):
             self.reset()
-        super(Grids, self).__setattr__(key, val)
+        super().__setattr__(key, val)
+
+    @property
+    def size(self):
+        return getattr(self.weights, 'size', 0)
 
     def build(self, mol=None, with_non0tab=False, sort_grids=True, **kwargs):
         if mol is None: mol = self.mol
         if self.verbose >= logger.WARN:
             self.check_sanity()
         atom_grids_tab = self.gen_atomic_grids(
             mol, self.atom_grid, self.radi_method, self.level, self.prune, **kwargs)
@@ -623,12 +572,17 @@
                     self.coords = cupy.vstack(
                         [self.coords, cupy.repeat([[1e4]*3], padding, axis=0)])
                     self.weights = cupy.hstack([self.weights, cupy.zeros(padding)])
             self.non0tab = self.make_mask(mol, self.coords)
             self.screen_index = self.non0tab
         return self
 
+    def to_cpu(self):
+        grids = gen_grid.Grids(self.mol)
+        utils.to_cpu(self, out=grids)
+        return grids
+
 _default_rad = gen_grid._default_rad
 RAD_GRIDS = gen_grid.RAD_GRIDS
 _default_ang = gen_grid._default_ang
 ANG_ORDER = gen_grid.ANG_ORDER
 _padding_size = gen_grid._padding_size
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/dft/gks.py` & `gpu4pyscf-0.7.6/gpu4pyscf/dft/gks.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/dft/libxc.py` & `gpu4pyscf-0.7.6/gpu4pyscf/dft/libxc.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 import ctypes.util
 import cupy
 from pyscf import dft
 from gpu4pyscf.dft.libxc_structs import xc_func_type
 
 import site
 path_list = [os.path.abspath(os.path.join(__file__, '..', '..', '..'))] + site.getsitepackages()
+__version__ = '6.1' # hard coded
+
+# CPU routines
+is_nlc           = dft.libxc.is_nlc
+is_hybrid_xc     = dft.libxc.is_hybrid_xc
+test_deriv_order = dft.libxc.test_deriv_order
 
 for path in path_list:
     try:
         _libxc = np.ctypeslib.load_library(
             'libxc', os.path.abspath(os.path.join(path, 'gpu4pyscf', 'lib', 'deps', 'lib')))
     except Exception:
         _libxc = None
@@ -96,14 +102,16 @@
         # TODO: deallocate xc func
         #_libxc.xc_func_end(self.xc_func)
         #_libxc.xc_func_free(self.xc_func)
 
     def needs_laplacian(self):
         return dft.libxc.needs_laplacian(self.func_id)
 
+    rsh_coeff = dft.libxc.rsh_coeff
+
     def compute(self, inp, output=None, do_exc=True, do_vxc=True, do_fxc=False, do_kxc=False, do_lxc=False):
         if isinstance(inp, cupy.ndarray):
             inp = {"rho": cupy.asarray(inp, dtype=cupy.double)}
         elif isinstance(inp, dict):
             inp = {k: cupy.asarray(v, dtype=cupy.double) for k, v in inp.items()}
         else:
             raise KeyError("Input must have a 'rho' variable or a single array.")
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/dft/libxc_structs.py` & `gpu4pyscf-0.7.6/gpu4pyscf/dft/libxc_structs.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/dft/numint.py` & `gpu4pyscf-0.7.6/gpu4pyscf/dft/numint.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 import cupy
 
 from pyscf import gto, lib, dft
 from pyscf.dft import numint
 from pyscf.gto.eval_gto import NBINS, CUTOFF, make_screen_index
 from gpu4pyscf.scf.hf import basis_seg_contraction
 from gpu4pyscf.lib.cupy_helper import (
-    contract, get_avail_mem, load_library, add_sparse, release_gpu_stack, take_last2d, transpose_sum)
+    contract, get_avail_mem, load_library, add_sparse, release_gpu_stack, take_last2d, transpose_sum,
+    grouped_dot, grouped_gemm)
 from gpu4pyscf.dft import xc_deriv, xc_alias, libxc
 from gpu4pyscf import __config__
 from gpu4pyscf.lib import logger
 
 LMAX_ON_GPU = 6
 BAS_ALIGNED = 1
 GRID_BLKSIZE = 32
@@ -574,14 +575,250 @@
     if len(dm_shape) == 2:
         nelec = nelec[0]
         excsum = excsum[0]
         vmat = vmat[0]
 
     return nelec, excsum, vmat
 
+def eval_rho_group(mol, ao_group, mo_coeff_group, mo_occ, non0tab=None, xctype='LDA',
+              with_lapl=True, verbose=None, out=None):
+    groups = len(ao_group)
+    xctype = xctype.upper()
+    if xctype == 'LDA' or xctype == 'HF':
+        ngrids_group = []
+        for ao in ao_group:
+            _, ngrids = ao.shape
+            ngrids_group.append(ngrids)
+    else:
+        ngrids_group = []
+        for ao in ao_group:
+            _, ngrids = ao[0].shape
+            ngrids_group.append(ngrids)
+
+    shls_slice = (0, mol.nbas)
+    ao_loc = mol.ao_loc_nr()
+
+    cpos_group = []
+    for groups_idx in range(groups):
+        cpos = (mo_coeff_group[groups_idx] * mo_occ**0.5)[:,mo_occ>0]
+        cpos_group.append(cpos)
+    if xctype == 'LDA' or xctype == 'HF':
+        c0_group = grouped_gemm(cpos_group, ao_group)
+        rho_group = []
+        for c0 in c0_group:
+            rho = _contract_rho(c0, c0)
+            rho_group.append(rho)
+    elif xctype in ('GGA', 'NLC'):
+        c0_group = []
+        cpos_group4 = []
+        ao_group4 = []
+        for ao, cpos in zip(ao_group, cpos_group):
+            for i in range(4):
+                cpos_group4.append(cpos)
+                ao_group4.append(ao[i])
+        c0_group = grouped_gemm(cpos_group4, ao_group4)
+
+        rho_group = []
+        for groups_idx in range(groups):
+            rho = cupy.empty((4, ngrids_group[groups_idx]))
+            c0 = c0_group[4*groups_idx:4*(groups_idx+1)]
+            _contract_rho(c0[0], c0[0], rho=rho[0])
+            for i in range(1, 4):
+                _contract_rho(c0[0], c0[i], rho=rho[i])
+            rho[1:] *= 2
+            rho_group.append(rho)
+    else: # meta-GGA
+        c0_group = []
+        cpos_group4 = []
+        ao_group4 = []
+        for ao, cpos in zip(ao_group, cpos_group):
+            for i in range(4):
+                cpos_group4.append(cpos)
+                ao_group4.append(ao[i])
+        c0_group = grouped_gemm(cpos_group4, ao_group4)
+
+        rho_group = []
+        for groups_idx in range(groups):
+            ngrids = ngrids_group[groups_idx]
+            c0 = c0_group[4*groups_idx:4*(groups_idx+1)]
+            if with_lapl:
+                rho = cupy.empty((6, ngrids))
+                tau_idx = 5
+            else:
+                rho = cupy.empty((5, ngrids))
+                tau_idx = 4
+            _contract_rho(c0[0], c0[0], rho=rho[0])
+            rho[tau_idx] = 0
+            for i in range(1, 4):
+                _contract_rho(c0[0], c0[i], rho[i])
+                rho[tau_idx] += _contract_rho(c0[i], c0[i])
+
+            if with_lapl:
+                ao = ao_group[groups_idx]
+                if ao.shape[0] > 4:
+                    XX, YY, ZZ = 4, 7, 9
+                    ao2 = ao[XX] + ao[YY] + ao[ZZ]
+                    c1 = _dot_ao_dm(mol, ao2, cpos, non0tab, shls_slice, ao_loc)
+                    rho[4] = _contract_rho(c0[0], c1)
+                    rho[4] += rho[5]
+                    rho[4] *= 2
+                else:
+                    rho[4] = 0
+            rho[1:4] *= 2
+            rho[tau_idx] *= .5
+            rho_group.append(rho)
+    return rho_group
+
+def nr_rks_group(ni, mol, grids, xc_code, dms, relativity=0, hermi=1,
+           max_memory=2000, verbose=None):
+    log = logger.new_logger(mol, verbose)
+    xctype = ni._xc_type(xc_code)
+    opt = getattr(ni, 'gdftopt', None)
+    if opt is None:
+        ni.build(mol, grids.coords)
+        opt = ni.gdftopt
+
+    mo_coeff = getattr(dms, 'mo_coeff', None)
+    mo_occ = getattr(dms,'mo_occ', None)
+
+    mol = opt.mol
+    coeff = cupy.asarray(opt.coeff)
+    nao, nao0 = coeff.shape
+    dms = cupy.asarray(dms)
+    dm_shape = dms.shape
+    #dms = [coeff @ dm @ coeff.T for dm in dms.reshape(-1,nao0,nao0)]
+    dms = dms.reshape(-1,nao0,nao0)
+    dms = take_last2d(dms, opt.ao_idx)
+    nset = len(dms)
+
+    if mo_coeff is not None:
+        mo_coeff = mo_coeff[opt.ao_idx]
+
+    nelec = cupy.zeros(nset)
+    excsum = cupy.zeros(nset)
+    vmat = cupy.zeros((nset, nao, nao))
+
+    release_gpu_stack()
+    if xctype == 'LDA':
+        ao_deriv = 0
+    else:
+        ao_deriv = 1
+    with_lapl = MGGA_DENSITY_LAPL
+    ngrids = grids.weights.size
+    if xctype == 'LDA':
+        rho_tot = cupy.empty([nset,1,ngrids])
+    elif xctype == 'GGA':
+        rho_tot = cupy.empty([nset,4,ngrids])
+    else:
+        if with_lapl:
+            rho_tot = cupy.empty([nset,6,ngrids])
+        else:
+            rho_tot = cupy.empty([nset,5,ngrids])
+    p0 = p1 = 0
+    t1 = t0 = log.init_timer()
+    for ao_mask, idx, weight, _ in ni.block_loop(mol, grids, nao, ao_deriv):
+        p1 = p0 + weight.size
+        for i in range(nset):
+            if mo_coeff is None:
+                rho_tot[i,:,p0:p1] = eval_rho(mol, ao_mask, dms[i][np.ix_(idx,idx)], xctype=xctype, hermi=1, with_lapl=with_lapl)
+            else:
+                mo_coeff_mask = mo_coeff[idx,:]
+                rho_tot[i,:,p0:p1] = eval_rho2(mol, ao_mask, mo_coeff_mask, mo_occ, None, xctype, with_lapl)
+        p0 = p1
+        t1 = log.timer_debug2('eval rho slice', *t1)
+    t0 = log.timer_debug1('eval rho', *t0)
+
+    wv = []
+    for i in range(nset):
+        if xctype == 'LDA':
+            exc, vxc = ni.eval_xc_eff(xc_code, rho_tot[i][0], deriv=1, xctype=xctype)[:2]
+        else:
+            exc, vxc = ni.eval_xc_eff(xc_code, rho_tot[i], deriv=1, xctype=xctype)[:2]
+        vxc = cupy.asarray(vxc, order='C')
+        exc = cupy.asarray(exc, order='C')
+        den = rho_tot[i][0] * grids.weights
+        nelec[i] = den.sum()
+        excsum[i] = cupy.sum(den * exc[:,0])
+        wv.append(vxc * grids.weights)
+        if xctype == 'GGA':
+            wv[i][0] *= .5
+        if xctype == 'MGGA':
+            wv[i][[0,4]] *= .5
+    t0 = log.timer_debug1('eval vxc', *t0)
+
+    t1 = t0
+    p0 = p1 = 0
+    for ao_mask_group, idx_group, weight_group, _ in ni.grouped_block_loop(mol, grids, nao, ao_deriv):
+        p0_raw = p0
+        for i in range(nset):
+            p0 = p0_raw
+            if xctype == 'LDA':
+                aow_group = []
+                for weight, ao_mask in zip(weight_group, ao_mask_group):
+                    p1 = p0 + weight.size
+                    aow = _scale_ao(ao_mask, wv[i][0,p0:p1])
+                    p0 = p1
+                    aow_group.append(aow)
+                dot_res_group = grouped_dot(ao_mask_group, aow_group)
+                for dot_res, idx in zip(dot_res_group, idx_group):
+                    add_sparse(vmat[i], dot_res, idx)
+            elif xctype == 'GGA':
+                aow_group = []
+                ao0_mask_group = []
+                for weight, ao_mask in zip(weight_group, ao_mask_group):
+                    p1 = p0 + weight.size
+                    aow = _scale_ao(ao_mask, wv[i][:,p0:p1])
+                    p0 = p1
+                    aow_group.append(aow)
+                    ao0_mask_group.append(ao_mask[0])
+                vmat_group = grouped_dot(ao0_mask_group, aow_group)
+                for vmat_tmp, idx in zip(vmat_group, idx_group):
+                    add_sparse(vmat[i], vmat_tmp, idx)
+            elif xctype == 'NLC':
+                raise NotImplementedError('NLC')
+            elif xctype == 'MGGA':
+                aow_group = []
+                ao0_mask_group = []
+                p0_tmp = p0
+                for weight, ao_mask in zip(weight_group, ao_mask_group):
+                    p1 = p0 + weight.size
+                    aow = _scale_ao(ao_mask, wv[i][:4,p0:p1])
+                    p0 = p1
+                    aow_group.append(aow)
+                    ao0_mask_group.append(ao_mask[0])
+                vmat_group = grouped_dot(ao0_mask_group, aow_group)
+                p0 = p0_tmp
+                for weight, vmat_tmp, ao_mask, idx in zip(weight_group, vmat_group, ao_mask_group, idx_group):
+                    p1 = p0 + weight.size
+                    vmat_tmp += _tau_dot(ao_mask, ao_mask, wv[i][4,p0:p1])
+                    add_sparse(vmat[i], vmat_tmp, idx)
+                    p0 = p1
+            elif xctype == 'HF':
+                pass
+            else:
+                raise NotImplementedError(f'numint.nr_rks for functional {xc_code}')
+        t1 = log.timer_debug2('integration', *t1)
+    t0 = log.timer_debug1('vxc integration', *t0)
+    rev_ao_idx = opt.rev_ao_idx
+    vmat = take_last2d(vmat, rev_ao_idx)
+
+    if xctype != 'LDA':
+        transpose_sum(vmat)
+
+    if FREE_CUPY_CACHE:
+        dms = None
+        cupy.get_default_memory_pool().free_all_blocks()
+
+    if len(dm_shape) == 2:
+        nelec = nelec[0]
+        excsum = excsum[0]
+        vmat = vmat[0]
+
+    return nelec, excsum, vmat
+
 def nr_uks(ni, mol, grids, xc_code, dms, relativity=0, hermi=1,
            max_memory=2000, verbose=None):
     log = logger.new_logger(mol, verbose)
     xctype = ni._xc_type(xc_code)
     opt = getattr(ni, 'gdftopt', None)
     if opt is None:
         ni.build(mol, grids.coords)
@@ -1218,14 +1455,66 @@
     for xc, w in xc_names:
         xcfun = libxc.XCfun(xc, spin_polarized)
         xcfuns.append((xcfun,w))
         if dft.libxc.needs_laplacian(xcfun.func_id):
             raise NotImplementedError()
     return xcfuns
 
+def _sparse_index(mol, coords, l_ctr_offsets):
+    '''
+    determine sparse AO indices
+    '''
+    log = logger.new_logger(mol, mol.verbose)
+    t1 = log.init_timer()
+    stream = cupy.cuda.get_current_stream()
+    cutoff = AO_THRESHOLD
+    ng = coords.shape[0]
+    ao_loc = mol.ao_loc_nr()
+    nbas = mol.nbas
+    non0shl_idx = cupy.zeros(len(ao_loc)-1, dtype=np.int32)
+    libgdft.GDFTscreen_index(
+        ctypes.cast(stream.ptr, ctypes.c_void_p),
+        ctypes.cast(non0shl_idx.data.ptr, ctypes.c_void_p),
+        ctypes.c_double(cutoff),
+        ctypes.cast(coords.data.ptr, ctypes.c_void_p),
+        ctypes.c_int(ng),
+        ao_loc.ctypes.data_as(ctypes.c_void_p),
+        ctypes.c_int(nbas),
+        mol._bas.ctypes.data_as(ctypes.c_void_p))
+    non0shl_idx = non0shl_idx.get()
+
+    # offset of contraction pattern, used in eval_ao
+    cumsum = np.cumsum(non0shl_idx, dtype=np.int32)
+    glob_ctr_offsets = l_ctr_offsets
+    ctr_offsets_slice = cumsum[glob_ctr_offsets-1]
+    ctr_offsets_slice[0] = 0
+
+    from pyscf import gto
+    gto_type = 'cart' if mol.cart else 'sph'
+    non0shl_idx = non0shl_idx == 1
+    ao_loc_slice = gto.moleintor.make_loc(mol._bas[non0shl_idx,:], gto_type)
+    ao_loc_slice = cupy.asarray(ao_loc_slice, dtype=np.int32)
+    non0ao_idx = []
+    zero_idx = []
+    for sh_idx in range(len(ao_loc)-1):
+        p0, p1 = ao_loc[sh_idx], ao_loc[sh_idx+1]
+        if non0shl_idx[sh_idx]:
+            non0ao_idx += range(p0,p1)
+        else:
+            zero_idx += range(p0,p1)
+
+    idx = cupy.asarray(non0ao_idx, dtype=np.int32)
+    zero_idx = cupy.asarray(zero_idx, dtype=np.int32)
+    pad = (len(idx) + AO_ALIGNMENT - 1) // AO_ALIGNMENT * AO_ALIGNMENT - len(idx)
+    idx = cupy.hstack([idx, zero_idx[:pad]])
+    pad = min(pad, len(zero_idx))
+    non0shl_idx = cupy.asarray(np.where(non0shl_idx)[0], dtype=np.int32)
+    t1 = log.timer_debug2('init ao sparsity', *t1)
+    return pad, idx, non0shl_idx, ctr_offsets_slice, ao_loc_slice
+
 def _block_loop(ni, mol, grids, nao=None, deriv=0, max_memory=2000,
                 non0tab=None, blksize=None, buf=None, extra=0):
     '''
     Define this macro to loop over grids by blocks.
     Sparsity is not implemented yet
     sorted_ao: by default ao_value is sorted for GPU
     '''
@@ -1257,62 +1546,17 @@
         t1 = log.init_timer()
         for ip0, ip1 in lib.prange(0, ngrids, blksize):
             coords = grids.coords[ip0:ip1]
             weight = grids.weights[ip0:ip1]
             t1 = log.init_timer()
             # cache ao indices
             if (block_id, blksize, ngrids) not in ni.non0ao_idx:
-                stream = cupy.cuda.get_current_stream()
-                cutoff = AO_THRESHOLD
-                ng = ip1 - ip0
-                ao_loc = mol.ao_loc_nr()
-                nbas = mol.nbas
-                non0shl_idx = cupy.zeros(len(ao_loc)-1, dtype=np.int32)
-                libgdft.GDFTscreen_index(
-                    ctypes.cast(stream.ptr, ctypes.c_void_p),
-                    ctypes.cast(non0shl_idx.data.ptr, ctypes.c_void_p),
-                    ctypes.c_double(cutoff),
-                    ctypes.cast(coords.data.ptr, ctypes.c_void_p),
-                    ctypes.c_int(ng),
-                    ao_loc.ctypes.data_as(ctypes.c_void_p),
-                    ctypes.c_int(nbas),
-                    mol._bas.ctypes.data_as(ctypes.c_void_p))
-                non0shl_idx = non0shl_idx.get()
-
-                # offset of contraction pattern, used in eval_ao
-                cumsum = np.cumsum(non0shl_idx, dtype=np.int32)
-                glob_ctr_offsets = opt.l_ctr_offsets
-                ctr_offsets_slice = cumsum[glob_ctr_offsets-1]
-                ctr_offsets_slice[0] = 0
-
-                from pyscf import gto
-                gto_type = 'cart' if mol.cart else 'sph'
-                non0shl_idx = non0shl_idx == 1
-                ao_loc_slice = gto.moleintor.make_loc(mol._bas[non0shl_idx,:], gto_type)
-                ao_loc_slice = cupy.asarray(ao_loc_slice, dtype=np.int32)
-                non0ao_idx = []
-                zero_idx = []
-                for sh_idx in range(len(ao_loc)-1):
-                    p0, p1 = ao_loc[sh_idx], ao_loc[sh_idx+1]
-                    if non0shl_idx[sh_idx]:
-                        non0ao_idx += range(p0,p1)
-                    else:
-                        zero_idx += range(p0,p1)
-
-                idx = cupy.asarray(non0ao_idx, dtype=np.int32)
-                zero_idx = cupy.asarray(zero_idx, dtype=np.int32)
-                pad = (len(idx) + AO_ALIGNMENT - 1) // AO_ALIGNMENT * AO_ALIGNMENT - len(idx)
-                idx = cupy.hstack([idx, zero_idx[:pad]])
-                pad = min(pad, len(zero_idx))
-                non0shl_idx = cupy.asarray(np.where(non0shl_idx)[0], dtype=np.int32)
-                ni.non0ao_idx[block_id, blksize, ngrids] = (pad, idx, non0shl_idx, ctr_offsets_slice, ao_loc_slice)
-                t1 = log.timer_debug2('init ao sparsity', *t1)
-            else:
-                pad, idx, non0shl_idx, ctr_offsets_slice, ao_loc_slice = ni.non0ao_idx[block_id, blksize, ngrids]
+                ni.non0ao_idx[block_id, blksize, ngrids] = _sparse_index(mol, coords, opt.l_ctr_offsets)
 
+            pad, idx, non0shl_idx, ctr_offsets_slice, ao_loc_slice = ni.non0ao_idx[block_id, blksize, ngrids]
             ao_mask = eval_ao(
                 ni, mol, coords, deriv,
                 nao_slice=len(idx),
                 shls_slice=non0shl_idx,
                 ao_loc_slice=ao_loc_slice,
                 ctr_offsets_slice=ctr_offsets_slice)
 
@@ -1321,26 +1565,124 @@
                 if deriv == 0:
                     ao_mask[-pad:,:] = 0.0
                 else:
                     ao_mask[:,-pad:,:] = 0.0
             block_id += 1
             yield ao_mask, idx, weight, coords
 
-class NumInt(numint.NumInt):
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+def _grouped_block_loop(ni, mol, grids, nao=None, deriv=0, max_memory=2000,
+                non0tab=None, blksize=None, buf=None, extra=0):
+    '''
+    Define this macro to loop over grids by blocks.
+    Sparsity is not implemented yet
+    sorted_ao: by default ao_value is sorted for GPU
+    '''
+    if grids.coords is None:
+        grids.build(with_non0tab=False, sort_grids=True)
+    if nao is None:
+        nao = mol.nao
+    ngrids = grids.coords.shape[0]
+    comp = (deriv+1)*(deriv+2)*(deriv+3)//6
+    log = logger.new_logger(mol, mol.verbose)
 
-    _keys = {'screen_idx', 'xcfuns', 'gdftopt'}
+    if blksize is None:
+        #cupy.get_default_memory_pool().free_all_blocks()
+        mem_avail = get_avail_mem()
+        blksize = int((mem_avail*.2/8/((comp+1)*nao + extra))/ ALIGNED) * ALIGNED
+        blksize = min(blksize, MIN_BLK_SIZE)
+        log.debug1('Available GPU mem %f Mb, block_size %d', mem_avail/1e6, blksize)
+        if blksize < ALIGNED:
+            raise RuntimeError('Not enough GPU memory')
+
+    opt = getattr(ni, 'gdftopt', None)
+    if opt is None:
+        ni.build(mol, grids.coords)
+        opt = ni.gdftopt
 
-    def __init__(self, xc='LDA'):
-        super().__init__()
-        self.gdftopt = None
-        self.pair_mask = None
-        self.screen_index = None
-        self.xcfuns = None        # can be multiple xc functionals
-        self.xc = xc
+    ao_mask_group = []
+    idx_group = []
+    weight_group = []
+    coords_group = []
+    total_used_bytes = 0
+    mem_limit = get_avail_mem()
+
+    mol = opt.mol
+    with opt.gdft_envs_cache():
+        block_id = 0
+        t1 = log.init_timer()
+        for ip0, ip1 in lib.prange(0, ngrids, blksize):
+            coords = grids.coords[ip0:ip1]
+            weight = grids.weights[ip0:ip1]
+            # cache ao indices
+            if (block_id, blksize, ngrids) not in ni.non0ao_idx:
+                ni.non0ao_idx[block_id, blksize, ngrids] = _sparse_index(mol, coords, opt.l_ctr_offsets)
+
+            pad, idx, non0shl_idx, ctr_offsets_slice, ao_loc_slice = ni.non0ao_idx[block_id, blksize, ngrids]
+
+            ao_mask = eval_ao(
+                ni, mol, coords, deriv,
+                nao_slice=len(idx),
+                shls_slice=non0shl_idx,
+                ao_loc_slice=ao_loc_slice,
+                ctr_offsets_slice=ctr_offsets_slice)
+
+            if pad > 0:
+                if deriv == 0:
+                    ao_mask[-pad:,:] = 0.0
+                else:
+                    ao_mask[:,-pad:,:] = 0.0
+            block_id += 1
+            total_used_bytes += ao_mask.nbytes
+            ao_mask_group.append(ao_mask)
+            idx_group.append(idx)
+            weight_group.append(weight)
+            coords_group.append(coords)
+            if total_used_bytes > 0.2 * mem_limit:
+                t1 = log.timer_debug2('evaluate ao slice', *t1)
+                yield ao_mask_group, idx_group, weight_group, coords_group
+                ao_mask_group = []
+                idx_group = []
+                weight_group = []
+                coords_group = []
+                total_used_bytes = 0
+        if total_used_bytes > 0:
+            t1 = log.timer_debug2('evaluate ao slice', *t1)
+            yield ao_mask_group, idx_group, weight_group, coords_group
+
+class LibXCMixin:
+    libxc = libxc
+    omega = None
+    to_cpu = NotImplemented
+
+    def hybrid_coeff(self, xc_code, spin=0):
+        return dft.libxc.hybrid_coeff(xc_code, spin)
+
+    def nlc_coeff(self, xc_code):
+        return dft.libxc.nlc_coeff(xc_code)
+
+    def rsh_coeff(sef, xc_code):
+        return dft.libxc.rsh_coeff(xc_code)
+    eval_xc      = NotImplemented
+    eval_xc_eff  = NotImplemented
+
+    def _xc_type(self, xc_code):
+        return dft.libxc.xc_type(xc_code)
+
+    rsh_and_hybrid_coeff = numint.LibXCMixin.rsh_and_hybrid_coeff
+
+_NumIntMixin = LibXCMixin
+from gpu4pyscf.lib import utils
+class NumInt(lib.StreamObject, LibXCMixin):
+    from gpu4pyscf.lib.utils import to_gpu, device
+
+    _keys = {'screen_idx', 'xcfuns', 'gdftopt'}
+    gdftopt      = None
+    pair_mask    = None
+    screen_index = None
+    xcfuns       = None        # can be multiple xc functionals
 
     def build(self, mol, coords):
         self.gdftopt = _GDFTOpt.from_mol(mol)
         if USE_SPARSITY == 1:
             pmol = self.gdftopt.mol
             nbas4 = pmol.nbas // BAS_ALIGNED
             ovlp_cond = pmol.get_overlap_cond()
@@ -1372,14 +1714,18 @@
     # cannot patch this function
     eval_xc_eff = eval_xc_eff
     block_loop = _block_loop
     eval_rho2 = eval_rho2
     eval_ao = eval_ao
     #eval_rho2 = staticmethod(eval_rho2)
 
+    def to_cpu(self):
+        ni = numint.NumInt()
+        return ni
+
 def _make_pairs2shls_idx(pair_mask, l_bas_loc, hermi=0):
     if hermi:
         pair_mask = np.tril(pair_mask)
     locs = l_bas_loc // BAS_ALIGNED
     assert locs[-1] == pair_mask.shape[0]
     pair2bra = []
     pair2ket = []
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/dft/radi.py` & `gpu4pyscf-0.7.6/gpu4pyscf/dft/radi.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/dft/rks.py` & `gpu4pyscf-0.7.6/gpu4pyscf/dft/rks.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 import cupy
 
 from pyscf import lib
 from pyscf.dft import rks
 
 from gpu4pyscf.lib import logger
 from gpu4pyscf.dft import numint, gen_grid
-from gpu4pyscf.scf.hf import RHF
+from gpu4pyscf.scf import hf
 from gpu4pyscf.lib.cupy_helper import load_library, tag_array
+from pyscf import __config__
 
 __all__ = [
     'get_veff', 'RKS'
 ]
 
 libcupy_helper = load_library('libcupy_helper')
 
@@ -226,40 +227,80 @@
     e2 = ecoul + exc
     ks.scf_summary['e1'] = e1
     ks.scf_summary['coul'] = ecoul
     ks.scf_summary['exc'] = exc
     logger.debug(ks, 'E1 = %s  Ecoul = %s  Exc = %s', e1, ecoul, exc)
     return e1+e2, e2
 
-class RKS(rks.RKS, RHF):
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+class KohnShamDFT:
 
+    _keys = rks.KohnShamDFT._keys
+
+    def __init__(self, xc='LDA,VWN'):
+        self.xc = xc
+        self.disp = None
+        self.disp_with_3body = None
+        self.nlc = ''
+        self.grids = gen_grid.Grids(self.mol)
+        self.grids.level = getattr(
+            __config__, 'dft_rks_RKS_grids_level', self.grids.level)
+        self.nlcgrids = gen_grid.Grids(self.mol)
+        self.nlcgrids.level = getattr(
+            __config__, 'dft_rks_RKS_nlcgrids_level', self.nlcgrids.level)
+        # Use rho to filter grids
+        self.small_rho_cutoff = getattr(
+            __config__, 'dft_rks_RKS_small_rho_cutoff', 1e-7)
+##################################################
+# don't modify the following attributes, they are not input options
+        self._numint = numint.NumInt()
+    @property
+    def omega(self):
+        return self._numint.omega
+    @omega.setter
+    def omega(self, v):
+        self._numint.omega = float(v)
+
+    def dump_flags(self, verbose=None):
+        # TODO: add this later
+        return
+
+    reset = rks.KohnShamDFT.reset
+
+hf.KohnShamDFT = KohnShamDFT
+from gpu4pyscf.lib import utils
+
+class RKS(KohnShamDFT, hf.RHF):
+
+    to_gpu = utils.to_gpu
+    device = utils.device
     _keys = {'disp'}
 
     def __init__(self, mol, xc='LDA,VWN', disp=None):
-        super().__init__(mol, xc)
-        self._numint = numint.NumInt(xc=xc)
+        hf.RHF.__init__(self, mol)
+        KohnShamDFT.__init__(self, xc)
         self.disp = disp
-        self.screen_tol = 1e-14
 
-        grids_level = self.grids.level
-        self.grids = gen_grid.Grids(mol)
-        self.grids.level = grids_level
-
-        nlcgrids_level = self.nlcgrids.level
-        self.nlcgrids = gen_grid.Grids(mol)
-        self.nlcgrids.level = nlcgrids_level
+    def dump_flags(self, verbose=None):
+        hf.RHF.dump_flags(self, verbose)
+        return KohnShamDFT.dump_flags(self, verbose)
 
     def reset(self, mol=None):
         super().reset(mol)
         self.grids.reset(mol)
         self.nlcgrids.reset(mol)
         self._numint.gdftopt = None
         return self
 
     def nuc_grad_method(self):
         from gpu4pyscf.grad import rks as rks_grad
         return rks_grad.Gradients(self)
 
+    def to_cpu(self):
+        mf = rks.RKS(self.mol)
+        utils.to_cpu(self, out=mf)
+        return mf
+
     energy_elec = energy_elec
+    energy_tot = hf.RHF.energy_tot
     get_veff = get_veff
     to_hf = NotImplemented
+    init_guess_by_vsap = rks.init_guess_by_vsap
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/dft/roks.py` & `gpu4pyscf-0.7.6/gpu4pyscf/dft/roks.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/dft/uks.py` & `gpu4pyscf-0.7.6/gpu4pyscf/dft/uks.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import cupy
 from pyscf.dft import uks
 from pyscf import lib
 from gpu4pyscf.lib import logger
 from gpu4pyscf.dft import numint, gen_grid, rks
-from gpu4pyscf.scf.uhf import UHF
+from gpu4pyscf.scf import hf, uhf
 from gpu4pyscf.lib.cupy_helper import tag_array
 
 
 def get_veff(ks, mol=None, dm=None, dm_last=0, vhf_last=0, hermi=1):
     '''Coulomb + XC functional for UKS.  See pyscf/dft/rks.py
     :func:`get_veff` fore more details.
     '''
@@ -108,31 +108,33 @@
     if vhf is None or getattr(vhf, 'ecoul', None) is None:
         vhf = ks.get_veff(ks.mol, dm)
     if not (isinstance(dm, cupy.ndarray) and dm.ndim == 2):
         dm = dm[0] + dm[1]
     return rks.energy_elec(ks, dm, h1e, vhf)
 
 
-class UKS(uks.UKS, UHF):
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+class UKS(rks.KohnShamDFT, uhf.UHF):
+    from gpu4pyscf.lib.utils import to_gpu, device
     _keys = {'disp', 'screen_tol'}
 
     def __init__(self, mol, xc='LDA,VWN', disp=None):
-        super().__init__(mol, xc)
+        uhf.UHF.__init__(self, mol)
+        rks.KohnShamDFT.__init__(self, xc)
         self.disp = disp
-        self._numint = numint.NumInt()
-        self.screen_tol = 1e-14
 
-        grids_level = self.grids.level
-        self.grids = gen_grid.Grids(mol)
-        self.grids.level = grids_level
-
-        nlcgrids_level = self.nlcgrids.level
-        self.nlcgrids = gen_grid.Grids(mol)
-        self.nlcgrids.level = nlcgrids_level
-
-    energy_elec = energy_elec
     get_veff = get_veff
+    get_vasp = uks.get_vsap
+    energy_elec = energy_elec
+    energy_tot = hf.RHF.energy_tot
+    init_guess_by_vsap = uks.UKS.init_guess_by_vsap
+
     to_hf = NotImplemented
     def nuc_grad_method(self):
         from gpu4pyscf.grad import uks as uks_grad
         return uks_grad.Gradients(self)
+
+    def to_cpu(self):
+        from gpu4pyscf.lib import utils
+        mf = uks.UKS(self.mol, xc=self.xc)
+        mf.disp = self.disp
+        utils.to_cpu(self, mf)
+        return mf
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/dft/xc_alias.py` & `gpu4pyscf-0.7.6/gpu4pyscf/dft/xc_alias.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/dft/xc_deriv.py` & `gpu4pyscf-0.7.6/gpu4pyscf/dft/xc_deriv.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/fci/direct_spin1.py` & `gpu4pyscf-0.7.6/gpu4pyscf/fci/direct_spin1.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/grad/dispersion.py` & `gpu4pyscf-0.7.6/gpu4pyscf/grad/dispersion.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 
 
 '''
 gradient of dispersion correction for HF and DFT
 '''
 
 import numpy
-from pyscf.scf.hf import KohnShamDFT
+from gpu4pyscf import dft
 
 def get_dispersion(mf_grad, disp_version=None):
     '''gradient of dispersion correction for RHF/RKS'''
     if disp_version is None:
         disp_version = mf_grad.base.disp
     mol = mf_grad.base.mol
     disp_version = mf_grad.base.disp
     if disp_version is None:
         return numpy.zeros([mol.natm,3])
 
-    if isinstance(mf_grad.base, KohnShamDFT):
+    if isinstance(mf_grad.base, dft.rks.KohnShamDFT):
         method = mf_grad.base.xc
     else:
         method = 'hf'
 
     if disp_version[:2].upper() == 'D3':
         # raised error in SCF module, assuming dftd3 installed
         from gpu4pyscf.lib import dftd3
@@ -42,15 +42,19 @@
         res = dftd3_model.get_dispersion(grad=True)
         return res['gradient']
 
     elif disp_version[:2].upper() == 'D4':
         from gpu4pyscf.lib import dftd4
         dftd4_model = dftd4.DFTD4Dispersion(mol, xc=method)
         res = dftd4_model.get_dispersion(grad=True)
+        print(method, disp_version)
+        print(res.get("gradient"))
         return res.get("gradient")
     else:
         raise RuntimeError(f'dispersion correction: {disp_version} is not supported.')
 
 # Inject to Gradient
-from gpu4pyscf.grad import rhf, uhf
+from gpu4pyscf.grad import rhf, uhf, rks, uks
 rhf.Gradients.get_dispersion = get_dispersion
-uhf.Gradients.get_dispersion = get_dispersion
+uhf.Gradients.get_dispersion = get_dispersion
+rks.Gradients.get_dispersion = get_dispersion
+uks.Gradients.get_dispersion = get_dispersion
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/grad/rhf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/grad/rhf.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import ctypes
 import numpy as np
 import cupy
 import numpy
 from pyscf import lib, gto
 from pyscf.grad import rhf
 from gpu4pyscf.lib.cupy_helper import load_library
-from gpu4pyscf.scf.hf import _VHFOpt
+from gpu4pyscf.scf.hf import _VHFOpt, KohnShamDFT
 from gpu4pyscf.lib.cupy_helper import tag_array, contract, take_last2d
 from gpu4pyscf.df import int3c2e      #TODO: move int3c2e to out of df
 from gpu4pyscf.lib import logger
 
 LMAX_ON_GPU = 3
 FREE_CUPY_CACHE = True
 BINSIZE = 128
@@ -517,36 +517,36 @@
         dh1e = int3c2e.get_dh1e(mol, dm0)
 
         if mol.has_ecp():
             dh1e += get_dh1e_ecp(mol, dm0)
         t3 = log.timer_debug1('gradients of h1e', *t3)
 
         dvhf = mf_grad.get_veff(mol, dm0)
-        t4 = log.timer_debug1('gradients of veff', *t3)
+        log.timer_debug1('gradients of veff', *t3)
         log.debug('Computing Gradients of NR-HF Coulomb repulsion')
 
         dm0 = tag_array(dm0, mo_coeff=mo_coeff, mo_occ=mo_occ)
         extra_force = cupy.zeros((len(atmlst),3))
         for k, ia in enumerate(atmlst):
             extra_force[k] += mf_grad.extra_force(ia, locals())
 
-        t2 = log.timer_debug1('gradients of 2e part', *t3)
+        log.timer_debug1('gradients of 2e part', *t3)
 
     dh = contract('xij,ij->xi', h1, dm0)
     ds = contract('xij,ij->xi', s1, dme0)
     delec = 2.0*(dh - ds)
 
     delec = cupy.asarray([cupy.sum(delec[:, p0:p1], axis=1) for p0, p1 in aoslices[:,2:]])
     de = 2.0 * dvhf + dh1e + delec + extra_force
 
+    # for backforward compatiability
     if(hasattr(mf, 'disp') and mf.disp is not None):
         g_disp = mf_grad.get_dispersion()
         mf_grad.grad_disp = g_disp
         mf_grad.grad_mf = de
-        de += cupy.asarray(g_disp)
 
     if log.verbose >= logger.DEBUG:
         log.timer_debug1('gradients of electronic part', *t0)
 
     # net force should be zero
     de -= cupy.sum(de, axis=0)/len(atmlst)
     return de.get()
@@ -597,17 +597,89 @@
         h1ao[:,p0:p1] += h1[:,p0:p1]
         h1ao += h1ao.transpose([0,2,1])
         h1ao = cupy.asarray(h1ao)
         h1mo = contract('xij,jo->xio', h1ao, orbo)
         dh1e[:,atm_id] += contract('xio,ip->xpo', h1mo, mo_coeff)
     return dh1e
 
-class Gradients(rhf.Gradients):
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+def as_scanner(mf_grad):
+    if isinstance(mf_grad, lib.GradScanner):
+        return mf_grad
+
+    logger.info(mf_grad, 'Create scanner for %s', mf_grad.__class__)
+    name = mf_grad.__class__.__name__ + SCF_GradScanner.__name_mixin__
+    return lib.set_class(SCF_GradScanner(mf_grad),
+                         (SCF_GradScanner, mf_grad.__class__), name)
+
+class SCF_GradScanner(lib.GradScanner):
+    def __init__(self, g):
+        lib.GradScanner.__init__(self, g)
+
+    def __call__(self, mol_or_geom, **kwargs):
+        if isinstance(mol_or_geom, gto.MoleBase):
+            assert mol_or_geom.__class__ == gto.Mole
+            mol = mol_or_geom
+        else:
+            mol = self.mol.set_geom_(mol_or_geom, inplace=False)
+
+        self.reset(mol)
+        mf_scanner = self.base
+        e_tot = mf_scanner(mol)
+
+        if isinstance(mf_scanner, KohnShamDFT):
+            if getattr(self, 'grids', None):
+                self.grids.reset(mol)
+            if getattr(self, 'nlcgrids', None):
+                self.nlcgrids.reset(mol)
+
+        de = self.kernel(**kwargs)
+        return e_tot, de
+
+class GradientsBase(lib.StreamObject):
+    '''
+    Basic nuclear gradient functions for non-relativistic methods
+    '''
 
+    _keys = {'mol', 'base', 'unit', 'atmlst', 'de'}
+    __init__ = rhf.GradientsBase.__init__
+
+    def dump_flags(self, verbose=None):
+        return
+
+    reset       = rhf.GradientsBase.reset
+    get_hcore   = rhf.GradientsBase.get_hcore
+    get_ovlp    = rhf.GradientsBase.get_ovlp
+    get_jk      = rhf.GradientsBase.get_jk
+    get_j       = rhf.GradientsBase.get_j
+    get_k       = rhf.GradientsBase.get_k
+    get_veff    = NotImplemented
+    make_rdm1e  = rhf.GradientsBase.make_rdm1e
+    grad_nuc    = rhf.GradientsBase.grad_nuc
+    optimizer   = rhf.GradientsBase.optimizer
+    extra_force = rhf.GradientsBase.extra_force
+    kernel      = rhf.GradientsBase.kernel
+    grad        = rhf.GradientsBase.grad
+    _finalize   = rhf.GradientsBase._finalize
+    _write      = rhf.GradientsBase._write
+    as_scanner  = as_scanner
+    _tag_rdm1   = rhf.GradientsBase._tag_rdm1
+
+    # to_cpu can be reused only when __init__ still takes mf
+    def to_cpu(self):
+        mf = self.base.to_cpu()
+        from importlib import import_module
+        mod = import_module(self.__module__.replace('gpu4pyscf', 'pyscf'))
+        cls = getattr(mod, self.__class__.__name__)
+        obj = cls(mf)
+        return obj
+
+class Gradients(GradientsBase):
+    from gpu4pyscf.lib.utils import to_gpu, device
+
+    make_rdm1e = rhf.Gradients.make_rdm1e
     grad_elec = grad_elec
     grad_nuc = grad_nuc
     get_veff = get_veff
     get_jk = _get_jk
 
     _keys = {'auxbasis_response', 'grad_disp', 'grad_mf'}
 
@@ -619,8 +691,10 @@
         _, vk = self.get_jk(mol, dm, with_j=False, omega=omega)
         return vk
 
     def extra_force(self, atom_id, envs):
         '''
         grid response is implemented get_veff
         '''
-        return 0
+        return 0
+
+Grad = Gradients
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/grad/rks.py` & `gpu4pyscf-0.7.6/gpu4pyscf/grad/rks.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 '''Non-relativistic RKS analytical nuclear gradients'''
 import ctypes
 import numpy
 import cupy
 import pyscf
 from pyscf import lib, gto
 from pyscf.dft import radi
+from pyscf.grad import rks as rks_grad
 from gpu4pyscf.lib.utils import patch_cpu_kernel
 from gpu4pyscf.grad import rhf as rhf_grad
 from gpu4pyscf.dft import numint, xc_deriv, rks
 from gpu4pyscf.dft.numint import _GDFTOpt, AO_THRESHOLD
 from gpu4pyscf.lib.cupy_helper import (
     contract, get_avail_mem, add_sparse, tag_array, load_library, take_last2d)
 from gpu4pyscf.lib import logger
@@ -498,11 +499,28 @@
         z = 1./pbecke.sum(axis=0)
         w1 = dpbecke[:,ia] * z
         w1 -= pbecke[ia] * z**2 * dpbecke.sum(axis=1)
         w1 *= vol
         w0 = vol * pbecke[ia] * z
         yield coords, w0, w1
 
-class Gradients(rhf_grad.Gradients, pyscf.grad.rks.Gradients):
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+class Gradients(rhf_grad.Gradients):
+    from gpu4pyscf.lib.utils import to_gpu, device
+    # attributes
+    grid_response = rks_grad.Gradients.grid_response
+    _keys = rks_grad.Gradients._keys
+
+    # method
+    def __init__ (self, mf):
+        rhf_grad.Gradients.__init__(self, mf)
+        self.grids = None
+        self.nlcgrids = None
+        self.grid_response = False
 
     get_veff = _get_veff
+    # TODO: add grid response into this function
+    def extra_force(self, atom_id, envs):
+        return 0
+
+Grad = Gradients
+from gpu4pyscf import dft
+dft.rks.RKS.Gradients = lib.class_as_method(Gradients)
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/grad/uhf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/grad/uhf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Copyright 2024 The GPU4PySCF Authors. All Rights Reserved.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 import time
 import ctypes
 import numpy as np
 import cupy
 import numpy
 from pyscf import lib, gto
 from pyscf.grad import uhf
@@ -14,16 +29,14 @@
 from gpu4pyscf.grad import rhf as rhf_grad
 
 LMAX_ON_GPU = 3
 FREE_CUPY_CACHE = True
 BINSIZE = 128
 libgvhf = load_library('libgvhf')
 
-
-
 def get_jk(mol, dm, hermi=1, vhfopt=None, with_j=True, with_k=True, omega=None,
            verbose=None, atmlst=None):
     if atmlst is None:
         atmlst = range(mol.natm)
 
     cput0 = (logger.process_clock(), logger.perf_counter())
     log = logger.new_logger(mol, verbose)
@@ -207,15 +220,15 @@
         cupy.get_default_memory_pool().free_all_blocks()
 
     if dm0.ndim != 2:
         if with_j:
             vj = vj.reshape(2,3,nao0,nao0)
         if with_k:
             vk = vk.reshape(2,3,nao0,nao0)
-    
+
     if out_cupy:
         return vj, vk
     else:
         return vj.get() if vj is not None else None, \
             vk.get() if vk is not None else None
 
 def get_veff(mf_grad, mol, dm):
@@ -254,23 +267,23 @@
     mo_energy = cupy.asarray(mo_energy)
     mo_occ = cupy.asarray(mo_occ)
     mo_coeff = cupy.asarray(mo_coeff)
     dm0 = mf.make_rdm1(mo_coeff, mo_occ)
     dme0 = mf_grad.make_rdm1e(mo_energy, mo_coeff, mo_occ)
     dm0 = tag_array(dm0, mo_coeff=mo_coeff, mo_occ=mo_occ)
     dm0_sf = dm0[0] + dm0[1]
-    dme0_sf = dme0[0] + dme0[1] 
-    
+    dme0_sf = dme0[0] + dme0[1]
+
     s1 = mf_grad.get_ovlp(mol)
-    
+
     if atmlst is None:
         atmlst = range(mol.natm)
     aoslices = mol.aoslice_by_atom()
     de = cupy.zeros((len(atmlst),3))
-        
+
     def calculate_h1e(h1_gpu, s1_gpu):
         # (\nabla i | hcore | j) - (\nabla i | j)
         h1_cpu = mf_grad.get_hcore(mol)
         s1_cpu = mf_grad.get_ovlp(mol)
         h1_gpu[:] = cupy.asarray(h1_cpu)
         s1_gpu[:] = cupy.asarray(s1_cpu)
         return
@@ -279,64 +292,74 @@
     s1 = cupy.empty([3, dm0.shape[1], dm0.shape[2]])
     with lib.call_in_background(calculate_h1e) as calculate_hs:
         calculate_hs(h1, s1)
         # (i | \nabla hcore | j)
         t3 = log.init_timer()
         dh1e = int3c2e.get_dh1e(mol, dm0_sf)
 
-        t4 = log.timer_debug1("get_dh1e", *t3)
+        log.timer_debug1("get_dh1e", *t3)
         if mol.has_ecp():
             dh1e += rhf_grad.get_dh1e_ecp(mol, dm0_sf)
         t1 = log.timer_debug1('gradients of h1e', *t0)
         log.debug('Computing Gradients of NR-HF Coulomb repulsion')
         dvhf = mf_grad.get_veff(mol, dm0)
 
         extra_force = cupy.zeros((len(atmlst),3))
         for k, ia in enumerate(atmlst):
             extra_force[k] += mf_grad.extra_force(ia, locals())
-
-        t2 = log.timer_debug1('gradients of 2e part', *t1)
+        log.timer_debug1('gradients of 2e part', *t1)
 
     dh = contract('xij,ij->xi', h1, dm0_sf)
     ds = contract('xij,ij->xi', s1, dme0_sf)
     delec = 2.0*(dh - ds)
     delec = cupy.asarray([cupy.sum(delec[:, p0:p1], axis=1) for p0, p1 in aoslices[:,2:]])
-    
+
+
+    '''
+    print('dvhf')
+    print(dvhf)
+    print('dh1e')
+    print(dh1e)
+    print('delec')
+    print(delec)
+    print('extra')
+    print(extra_force)
+    '''
     de = 2.0 * dvhf + dh1e + delec + extra_force
-    
+
+    # for backward compatiability
     if(hasattr(mf, 'disp') and mf.disp is not None):
         g_disp = mf_grad.get_dispersion()
         mf_grad.grad_disp = g_disp
         mf_grad.grad_mf = de
-        de += cupy.asarray(g_disp)
 
     de -= cupy.sum(de, axis=0)/len(atmlst)
     return de.get()
 
 
-class Gradients(uhf.Gradients):
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
-    
+class Gradients(rhf_grad.GradientsBase):
+    from gpu4pyscf.lib.utils import to_gpu, device
+
     grad_elec = grad_elec
-    grad_nuc = rhf_grad.grad_nuc 
+    grad_nuc = rhf_grad.grad_nuc
     get_veff =  get_veff
-    get_jk = rhf_grad._get_jk 
-    
+    get_jk = rhf_grad._get_jk
+
     def get_j(self, mol=None, dm=None, hermi=0, omega=None):
         vj, _ = self.get_jk(mol, dm, with_k=False, omega=omega)
         return vj
 
     def get_k(self, mol=None, dm=None, hermi=0, omega=None):
         _, vk = self.get_jk(mol, dm, with_j=False, omega=omega)
         return vk
-    
+
     def make_rdm1e(self, mo_energy=None, mo_coeff=None, mo_occ=None):
         if mo_energy is None: mo_energy = self.base.mo_energy
         if mo_coeff is None: mo_coeff = self.base.mo_coeff
         if mo_occ is None: mo_occ = self.base.mo_occ
         return make_rdm1e(mo_energy, mo_coeff, mo_occ)
-    
+
     def extra_force(self, atom_id, envs):
         '''
         grid response is implemented get_veff
         '''
-        return 0
+        return 0
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/grad/uks.py` & `gpu4pyscf-0.7.6/gpu4pyscf/grad/uks.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 '''Non-relativistic UKS analytical nuclear gradients'''
 
 import ctypes
 import numpy as np
 import cupy
 import pyscf
 from pyscf import lib
+from pyscf.grad import uks as uks_grad
 from gpu4pyscf.grad import uhf as uhf_grad
 from gpu4pyscf.grad import rks as rks_grad
 from gpu4pyscf.dft import numint, xc_deriv
 from gpu4pyscf.lib.cupy_helper import contract, get_avail_mem, add_sparse, load_library, take_last2d, tag_array
 from gpu4pyscf.lib import logger
 from pyscf import __config__
 
@@ -339,11 +340,26 @@
     rev_ao_idx = opt.rev_ao_idx
     vmat = take_last2d(vmat, rev_ao_idx)
     exc = None
     # - sign because nabla_X = -nabla_x
     return exc, -vmat
 
 
-class Gradients(uhf_grad.Gradients, pyscf.grad.uks.Gradients):
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+class Gradients(uhf_grad.Gradients):
+    from gpu4pyscf.lib.utils import to_gpu, device
+    grid_response = uks_grad.Gradients.grid_response
+    _keys = uks_grad.Gradients._keys
+
+    def __init__(self, mf):
+        uhf_grad.Gradients.__init__(self, mf)
+        self.grids = None
+        self.nlcgrids = None
+        self.grid_response = False
 
     get_veff = get_veff
+    # TODO: add grid response into this function
+    def extra_force(self, atom_id, envs):
+        return 0
+
+Grad = Gradients
+from gpu4pyscf import dft
+dft.uks.UKS.Gradients = lib.class_as_method(Gradients)
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/gto/__init__.py` & `gpu4pyscf-0.7.6/gpu4pyscf/gto/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/gto/mole.py` & `gpu4pyscf-0.7.6/gpu4pyscf/gto/mole.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/hessian/__init__.py` & `gpu4pyscf-0.7.6/gpu4pyscf/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/hessian/dispersion.py` & `gpu4pyscf-0.7.6/gpu4pyscf/hessian/dispersion.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,36 +15,37 @@
 
 
 '''
 Hessian of dispersion correction for HF and DFT
 '''
 
 import numpy
-from pyscf.scf.hf import KohnShamDFT
+from gpu4pyscf import dft
 
 def get_dispersion(hessobj, disp_version=None):
     if disp_version is None:
         disp_version = hessobj.base.disp
     mol = hessobj.base.mol
     natm = mol.natm
     mf = hessobj.base
     h_disp = numpy.zeros([natm,natm,3,3])
     if disp_version is None:
         return h_disp
-    if isinstance(hessobj.base, KohnShamDFT):
+    if isinstance(hessobj.base, dft.rks.KohnShamDFT):
         method = hessobj.base.xc
     else:
         method = 'hf'
 
     if mf.disp[:2].upper() == 'D3':
         from gpu4pyscf.lib import dftd3
         coords = mol.atom_coords()
         natm = mol.natm
         h_d3 = numpy.zeros([mol.natm, mol.natm, 3,3])
         pmol = mol.copy()
+        pmol.verbose = 0
         eps = 1e-5
         for i in range(natm):
             for j in range(3):
                 coords[i,j] += eps
                 pmol.set_geom_(coords, unit='Bohr')
                 pmol.build()
                 dftd3_model = dftd3.DFTD3Dispersion(pmol, xc=method, version=disp_version)
@@ -63,14 +64,15 @@
         return h_d3
 
     elif mf.disp[:2].upper() == 'D4':
         from gpu4pyscf.lib import dftd4
         coords = mol.atom_coords()
         natm = mol.natm
         pmol = mol.copy()
+        pmol.verbose = 0
         h_d4 = numpy.zeros([mol.natm, mol.natm, 3,3])
         eps = 1e-5
         for i in range(natm):
             for j in range(3):
                 coords[i,j] += eps
                 pmol.set_geom_(coords, unit='Bohr')
                 pmol.build()
@@ -89,10 +91,12 @@
                 h_d4[i,:,j,:] = (g1 - g2)/(2.0*eps)
 
         return h_d4
     else:
         raise RuntimeError(f'dispersion correction: {disp_version} is not supported.')
 
 # Inject to SCF class
-from gpu4pyscf.hessian import rhf, uhf
+from gpu4pyscf.hessian import rhf, uhf, rks, uks
 rhf.Hessian.get_dispersion = get_dispersion
-uhf.Hessian.get_dispersion = get_dispersion
+uhf.Hessian.get_dispersion = get_dispersion
+rks.Hessian.get_dispersion = get_dispersion
+uks.Hessian.get_dispersion = get_dispersion
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/hessian/rhf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/hessian/rhf.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import cupy
 from pyscf.hessian import rhf as rhf_hess
 from pyscf import lib
 from pyscf import gto
 from pyscf.scf import _vhf
 
 # import _response_functions to load gen_response methods in SCF class
-from pyscf.scf import _response_functions  # noqa
+from gpu4pyscf.scf import _response_functions  # noqa
 # import pyscf.grad.rhf to activate nuc_grad_method method
 from pyscf.grad import rhf  # noqa
 from gpu4pyscf.scf import cphf
 from gpu4pyscf.lib.cupy_helper import contract, tag_array, print_mem_info
 from gpu4pyscf.lib import logger
 from gpu4pyscf.df import int3c2e
 
@@ -580,35 +580,67 @@
             with mol.with_rinv_at_nucleus(iatm):
                 shls_slice = (jsh0, jsh1, 0, nbas)
                 if with_ecp and iatm in ecp_atoms:
                     rinv2aa = -mol.intor('ECPscalar_ipiprinv', comp=9, shls_slice=shls_slice)
                     rinv2ab = -mol.intor('ECPscalar_iprinvip', comp=9, shls_slice=shls_slice)
                     rinv2aa = cupy.asarray(rinv2aa)
                     rinv2ab = cupy.asarray(rinv2ab)
-                if rinv2aa is not None or rinv2ab is not None:
                     hcore[:,:,j0:j1] += rinv2aa.reshape(3,3,j1-j0,nao)
                     hcore[:,:,j0:j1] += rinv2ab.reshape(3,3,j1-j0,nao).transpose(1,0,2,3)
-
             with mol.with_rinv_at_nucleus(jatm):
                 shls_slice = (ish0, ish1, 0, nbas)
                 if with_ecp and jatm in ecp_atoms:
                     rinv2aa = -mol.intor('ECPscalar_ipiprinv', comp=9, shls_slice=shls_slice)
                     rinv2ab = -mol.intor('ECPscalar_iprinvip', comp=9, shls_slice=shls_slice)
                     rinv2aa = cupy.asarray(rinv2aa)
                     rinv2ab = cupy.asarray(rinv2ab)
-                if rinv2aa is not None or rinv2ab is not None:
                     hcore[:,:,i0:i1] += rinv2aa.reshape(3,3,i1-i0,nao)
                     hcore[:,:,i0:i1] += rinv2ab.reshape(3,3,i1-i0,nao)
         return hcore + hcore.conj().transpose(0,1,3,2)
     return get_hcore
 
-class Hessian(rhf_hess.Hessian):
+class HessianBase(lib.StreamObject):
+    # attributes
+    max_cycle   = rhf_hess.HessianBase.max_cycle
+    level_shift = rhf_hess.HessianBase.level_shift
+    _keys       = rhf_hess.HessianBase._keys
+
+    # methods
+    __init__        = rhf_hess.HessianBase.__init__
+    hess_elec       = rhf_hess.HessianBase.hess_elec
+    make_h1         = rhf_hess.HessianBase.make_h1
+    hcore_generator = hcore_generator  # the functionality is different from cpu version
+    kernel          = kernel
+    hess            = kernel
+
+    def get_hcore(self, mol=None):
+        if mol is None: mol = self.mol
+        return get_hcore(mol)
+
+    def solve_mo1(self, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
+                  fx=None, atmlst=None, max_memory=4000, verbose=None):
+        return solve_mo1(self.base, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
+                         fx, atmlst, max_memory, verbose)
+
+    def hess_nuc(self, mol=None, atmlst=None):
+        if mol is None: mol = self.mol
+        return hess_nuc(mol, atmlst)
+
+    def to_cpu(self):
+        mf = self.base.to_cpu()
+        from importlib import import_module
+        mod = import_module(self.__module__.replace('gpu4pyscf', 'pyscf'))
+        cls = getattr(mod, self.__class__.__name__)
+        obj = cls(mf)
+        return obj
+
+class Hessian(HessianBase):
     '''Non-relativistic restricted Hartree-Fock hessian'''
 
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+    from gpu4pyscf.lib.utils import to_gpu, device
 
     def __init__(self, scf_method):
         self.verbose = scf_method.verbose
         self.stdout = scf_method.stdout
         self.mol = scf_method.mol
         self.base = scf_method
         self.chkfile = None #scf_method.chkfile
@@ -616,30 +648,14 @@
         self.atmlst = range(self.mol.natm)
         self.de = numpy.zeros((0,0,3,3))  # (A,B,dR_A,dR_B)
         self._keys = set(self.__dict__.keys())
 
     partial_hess_elec = partial_hess_elec
     hess_elec = hess_elec
     make_h1 = make_h1
-
-    def get_hcore(self, mol=None):
-        if mol is None: mol = self.mol
-        return get_hcore(mol)
-
-
-    def solve_mo1(self, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
-                  fx=None, atmlst=None, max_memory=4000, verbose=None):
-        return solve_mo1(self.base, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
-                         fx, atmlst, max_memory, verbose)
-
-    def hess_nuc(self, mol=None, atmlst=None):
-        if mol is None: mol = self.mol
-        return hess_nuc(mol, atmlst)
-
-    kernel = kernel
-    hess = kernel
-
+    hess = NotImplemented
+    kernel = NotImplemented
     gen_hop = gen_hop
 
 # Inject to RHF class
 from gpu4pyscf import scf
 scf.hf.RHF.Hessian = lib.class_as_method(Hessian)
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/hessian/rks.py` & `gpu4pyscf-0.7.6/gpu4pyscf/hessian/rks.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 Non-relativistic RKS analytical Hessian
 '''
 
 
 import numpy
 import cupy
 from pyscf import lib
+from pyscf.hessian import rks as rks_hess
 from gpu4pyscf.hessian import rhf as rhf_hess
 from gpu4pyscf.grad import rks as rks_grad
 from gpu4pyscf.dft import numint
 from gpu4pyscf.lib.cupy_helper import contract, add_sparse, take_last2d
 from gpu4pyscf.lib import logger
 
 # import pyscf.grad.rks to activate nuc_grad_method method
@@ -184,15 +185,15 @@
     mol = hessobj.mol
     mf = hessobj.base
     if hessobj.grids is not None:
         grids = hessobj.grids
     else:
         grids = mf.grids
     if grids.coords is None:
-        grids.build(with_non0tab=True)
+        grids.build(with_non0tab=False)
 
     # move data to GPU
     mo_occ = cupy.asarray(mo_occ)
     mo_coeff = cupy.asarray(mo_coeff)
 
     nao_sph, nmo = mo_coeff.shape
     ni = mf._numint
@@ -404,15 +405,15 @@
             t1 = log.timer_debug2('eval rho', *t1)
             vxc, fxc = ni.eval_xc_eff(mf.xc, rho, 2, xctype=xctype)[1:3]
             t1 = log.timer_debug2('eval vxc', *t1)
             wv = weight * vxc[0]
             aow = [numint._scale_ao(ao[i], wv) for i in range(1, 4)]
             _d1d2_dot_(ipip, mol, aow, ao[1:4], mask, ao_loc, False)
             dm0_mask = dm0_sorted[numpy.ix_(mask, mask)]
-            
+
             ao_dm_mask = contract('nig,ij->njg', ao_mask[:4], dm0_mask)
             ao_dm0 = numint._dot_ao_dm(mol, ao[0], dm0, mask, shls_slice, ao_loc)
             wf = weight * fxc[0,0]
             for ia in range(mol.natm):
                 p0, p1 = aoslices[ia][2:]
                 # *2 for \nabla|ket> in rho1
                 rho1 = contract('xig,ig->xg', ao[1:,p0:p1,:], ao_dm0[p0:p1,:]) * 2
@@ -672,29 +673,27 @@
 
         vmat_tmp = contract('xij,jq->xiq', vmat_tmp, mocc)
         vmat_tmp = contract('xiq,ip->xpq', vmat_tmp, mo_coeff)
         vmat[ia] -= vmat_tmp
     return vmat
 
 
-class Hessian(rhf_hess.Hessian):
+class Hessian(rhf_hess.HessianBase):
     '''Non-relativistic RKS hessian'''
+
     from gpu4pyscf.lib.utils import to_gpu, device
 
+    _keys = {'grids', 'grid_response'}
+
     def __init__(self, mf):
         rhf_hess.Hessian.__init__(self, mf)
         self.grids = None
         self.grid_response = False
-        self._keys = self._keys.union(['grids'])
-
-    def to_cpu(self):
-        from gpu4pyscf.lib.utils import to_cpu
-        from pyscf.hessian.rks import Hessian
-        # to_cpu returns an rhf.Hessian object
-        obj = to_cpu(self)
-        return obj.view(Hessian)
 
     partial_hess_elec = partial_hess_elec
+    hess_elec = rhf_hess.hess_elec
     make_h1 = make_h1
+    hess = NotImplemented
+    kernel = NotImplemented
 
-from pyscf import dft
-dft.rks.RKS.Hessian = dft.rks_symm.RKS.Hessian = lib.class_as_method(Hessian)
+from gpu4pyscf import dft
+dft.rks.RKS.Hessian = lib.class_as_method(Hessian)
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/hessian/uhf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/hessian/uhf.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,22 +29,22 @@
 from pyscf.hessian import rhf as rhf_hess
 from pyscf.hessian import uhf as uhf_hess
 from pyscf import lib
 from pyscf import gto
 from pyscf.scf import _vhf
 
 # import _response_functions to load gen_response methods in SCF class
-from pyscf.scf import _response_functions  # noqa
+from gpu4pyscf.scf import _response_functions  # noqa
 # import pyscf.grad.rhf to activate nuc_grad_method method
 from pyscf.grad import rhf  # noqa
 from gpu4pyscf.scf import ucphf
 from gpu4pyscf.lib.cupy_helper import contract, tag_array, print_mem_info
 from gpu4pyscf.lib import logger
 from gpu4pyscf.df import int3c2e
-from gpu4pyscf.hessian import rhf as rhf_hess_gpu
+from gpu4pyscf.hessian.rhf import HessianBase
 
 def hess_elec(hessobj, mo_energy=None, mo_coeff=None, mo_occ=None,
               mo1=None, mo_e1=None, h1ao=None,
               atmlst=None, max_memory=4000, verbose=None):
 
     log = logger.new_logger(hessobj, verbose)
     time0 = t1 = (logger.process_clock(), logger.perf_counter())
@@ -500,38 +500,26 @@
             hx[ja] -= numpy.einsum('xpq,qp->x', s1a[:,q0:q1], dme1[:,q0:q1]) * 2
         return hx.ravel()
 
     hdiag = numpy.einsum('aaxx->ax', de2).ravel()
     return h_op, hdiag
 
 
-class Hessian(rhf_hess.HessianBase):
-    '''Non-relativistic restricted Hartree-Fock hessian'''
-
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
-
-    def __init__(self, scf_method):
-        self.verbose = scf_method.verbose
-        self.stdout = scf_method.stdout
-        self.mol = scf_method.mol
-        self.base = scf_method
-        self.chkfile = None #scf_method.chkfile
-        self.max_memory = self.mol.max_memory
-        self.atmlst = range(self.mol.natm)
-        self.de = numpy.zeros((0,0,3,3))  # (A,B,dR_A,dR_B)
-        self._keys = set(self.__dict__.keys())
+class Hessian(HessianBase):
+    '''Non-relativistic unrestricted Hartree-Fock hessian'''
 
     partial_hess_elec = partial_hess_elec
     hess_elec = hess_elec
     make_h1 = make_h1
-    kernel = rhf_hess_gpu.kernel
+    kernel = NotImplemented
+    hess = NotImplemented
 
     def solve_mo1(self, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
                   fx=None, atmlst=None, max_memory=4000, verbose=None):
         return solve_mo1(self.base, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
                          fx, atmlst, max_memory, verbose)
 
     gen_hop = gen_hop
 
 # Inject to UHF class
 from gpu4pyscf import scf
-scf.uhf.UHF.Hessian = lib.class_as_method(Hessian)
+scf.uhf.UHF.Hessian = lib.class_as_method(Hessian)
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/hessian/uks.py` & `gpu4pyscf-0.7.6/gpu4pyscf/hessian/uks.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 Non-relativistic UKS analytical Hessian
 '''
 
 
 import numpy
 import cupy
 from pyscf import lib
-from pyscf.hessian import rhf as rhf_hess
+from gpu4pyscf.hessian import rhf as rhf_hess
+from gpu4pyscf.hessian import uhf as uhf_hess
+from gpu4pyscf.hessian import uks as uks_hess
 from gpu4pyscf.grad import rks as rks_grad
 from gpu4pyscf.dft import numint
 from gpu4pyscf.lib.cupy_helper import contract, add_sparse, take_last2d
 from gpu4pyscf.lib import logger
 
 # import pyscf.grad.rks to activate nuc_grad_method method
 from gpu4pyscf.grad import rks  # noqa
@@ -181,15 +183,15 @@
     mol = hessobj.mol
     mf = hessobj.base
     if hessobj.grids is not None:
         grids = hessobj.grids
     else:
         grids = mf.grids
     if grids.coords is None:
-        grids.build(with_non0tab=True)
+        grids.build(with_non0tab=False)
 
     # move data to GPU
     mo_occ = cupy.asarray(mo_occ)
     mo_coeff = cupy.asarray(mo_coeff)
 
     nao_sph, nmo = mo_coeff[0].shape
     ni = mf._numint
@@ -849,22 +851,17 @@
     '''Non-relativistic UKS hessian'''
     from gpu4pyscf.lib.utils import to_gpu, device
 
     def __init__(self, mf):
         rhf_hess.Hessian.__init__(self, mf)
         self.grids = None
         self.grid_response = False
-        self._keys = self._keys.union(['grids'])
-
-    def to_cpu(self):
-        from gpu4pyscf.lib.utils import to_cpu
-        from pyscf.hessian.rks import Hessian
-        # to_cpu returns an rhf.Hessian object
-        obj = to_cpu(self)
-        return obj.view(Hessian)
 
+    hess_elec = uhf_hess.hess_elec
+    solve_mo1 = uhf_hess.Hessian.solve_mo1
     partial_hess_elec = partial_hess_elec
     make_h1 = make_h1
-    kernel = rhf_hess_gpu.kernel
+    kernel = NotImplemented
+    hess = NotImplemented
 
 from gpu4pyscf import dft
 dft.uks.UKS.Hessian = lib.class_as_method(Hessian)
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/lib/__init__.py` & `gpu4pyscf-0.7.6/gpu4pyscf/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/lib/cublas.py` & `gpu4pyscf-0.7.6/gpu4pyscf/lib/cublas.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/lib/cupy_helper.py` & `gpu4pyscf-0.7.6/gpu4pyscf/lib/cupy_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -235,15 +235,14 @@
     cols = [np.array([0], dtype='int32')]
     offsets = []
     for l, count in zip(angular, counts):
         r, c = c2s_l[l].shape
         rows.append(rows[-1][-1] + np.arange(1,count+1, dtype='int32') * r)
         cols.append(cols[-1][-1] + np.arange(1,count+1, dtype='int32') * c)
         offsets += [c2s_offset[l]] * count
-
     rows = cupy.hstack(rows)
     cols = cupy.hstack(cols)
     offsets = cupy.asarray(offsets, dtype='int32')
 
     stream = cupy.cuda.get_current_stream()
     err = libcupy_helper.block_diag(
         ctypes.cast(stream.ptr, ctypes.c_void_p),
@@ -600,7 +599,130 @@
     '''
     a = cupy.asarray(a)
     w, v = cupy.linalg.eigh(a)
     mask = w > lindep
     v1 = v[:,mask]
     j2c = cupy.dot(v1/w[mask], v1.conj().T)
     return j2c
+
+def cond(a):
+    return cupy.linalg.norm(a,2)*cupy.linalg.norm(cupy.linalg.inv(a),2)
+
+def grouped_dot(As, Bs, Cs=None):
+    '''
+    todo: layout of cutlass kernel
+    As: cupy 2D array list.
+    Bs: cupy 2D array list.
+    Cs: cupy 2D array list.
+    einsum('ik,jk->ij', A, B, C) C=A@B.T
+    '''
+    assert len(As) > 0
+    assert len(As) == len(Bs)
+    assert As[0].flags.c_contiguous
+    assert Bs[0].flags.c_contiguous
+    groups = len(As)
+    Ms, Ns, Ks = [], [], []
+    for a, b in zip(As, Bs):
+        Ms.append(a.shape[0])
+        Ns.append(b.shape[0])
+        Ks.append(a.shape[1])
+
+    if Cs is None:
+        Cs = []
+        for i in range(groups):
+            Cs.append(cupy.empty((Ms[i], Ns[i])))
+
+    As_ptr, Bs_ptr, Cs_ptr = [], [], []
+    for a, b, c in zip(As, Bs, Cs):
+        As_ptr.append(a.data.ptr)
+        Bs_ptr.append(b.data.ptr)
+        Cs_ptr.append(c.data.ptr)
+
+    As_ptr = np.array(As_ptr)
+    Bs_ptr = np.array(Bs_ptr)
+    Cs_ptr = np.array(Cs_ptr)
+
+    Ms = np.array(Ms)
+    Ns = np.array(Ns)
+    Ks = np.array(Ks)
+    total_size = 68 * groups
+    '''
+    68 is the result of
+    sizeof(cutlass::gemm::GemmCoord) +
+    sizeof(typename DeviceKernel::ElementA*) +
+    sizeof(typename DeviceKernel::ElementB*) +
+    sizeof(typename DeviceKernel::ElementC*) +
+    sizeof(typename DeviceKernel::ElementC*) +
+    sizeof(int64_t) + sizeof(int64_t) + sizeof(int64_t)
+    '''
+    padding = 8 - (total_size % 8)
+    total_size += padding
+    cutlass_space = cupy.empty(total_size, dtype=cupy.uint8)
+
+    stream = cupy.cuda.get_current_stream()
+    err = libcupy_helper.grouped_dot(
+        ctypes.cast(stream.ptr, ctypes.c_void_p),
+        ctypes.cast(Cs_ptr.ctypes.data, ctypes.c_void_p),
+        ctypes.cast(As_ptr.ctypes.data, ctypes.c_void_p),
+        ctypes.cast(Bs_ptr.ctypes.data, ctypes.c_void_p),
+        ctypes.cast(Ms.ctypes.data, ctypes.c_void_p),
+        ctypes.cast(Ns.ctypes.data, ctypes.c_void_p),
+        ctypes.cast(Ks.ctypes.data, ctypes.c_void_p),
+        ctypes.cast(cutlass_space.data.ptr, ctypes.c_void_p),
+        ctypes.c_int(groups)
+    )
+    if err != 0:
+        raise RuntimeError('failed in grouped_gemm kernel')
+    return Cs
+
+def grouped_gemm(As, Bs, Cs=None):
+    '''
+    As: cupy 2D array list.
+    Bs: cupy 2D array list.
+    Cs: cupy 2D array list.
+    assuming (X, 64).T @ (X, Y)
+    einsum('ki,kj->ij', A, B, C) C=A.T@B
+    Compare with grouped_dot, this function handles the case M < 128
+    '''
+    assert len(As) > 0
+    assert len(As) == len(Bs)
+    assert As[0].flags.c_contiguous
+    assert Bs[0].flags.c_contiguous
+    groups = len(As)
+    Ms, Ns, Ks = [], [], []
+    for a, b in zip(As, Bs):
+        Ms.append(a.shape[1])
+        Ns.append(b.shape[1])
+        Ks.append(a.shape[0])
+
+    if Cs is None:
+        Cs = []
+        for i in range(groups):
+            Cs.append(cupy.empty((Ms[i], Ns[i])))
+
+    As_ptr, Bs_ptr, Cs_ptr = [], [], []
+    for a, b, c in zip(As, Bs, Cs):
+        As_ptr.append(a.data.ptr)
+        Bs_ptr.append(b.data.ptr)
+        Cs_ptr.append(c.data.ptr)
+    As_ptr = np.array(As_ptr)
+    Bs_ptr = np.array(Bs_ptr)
+    Cs_ptr = np.array(Cs_ptr)
+
+    Ms = np.array(Ms)
+    Ns = np.array(Ns)
+    Ks = np.array(Ks)
+
+    stream = cupy.cuda.get_current_stream()
+    err = libcupy_helper.grouped_gemm(
+        ctypes.cast(stream.ptr, ctypes.c_void_p),
+        ctypes.cast(Cs_ptr.ctypes.data, ctypes.c_void_p),
+        ctypes.cast(As_ptr.ctypes.data, ctypes.c_void_p),
+        ctypes.cast(Bs_ptr.ctypes.data, ctypes.c_void_p),
+        ctypes.cast(Ms.ctypes.data, ctypes.c_void_p),
+        ctypes.cast(Ns.ctypes.data, ctypes.c_void_p),
+        ctypes.cast(Ks.ctypes.data, ctypes.c_void_p),
+        ctypes.c_int(groups)
+    )
+    if err != 0:
+        raise RuntimeError('failed in grouped_gemm kernel')
+    return Cs
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/lib/cusolver.py` & `gpu4pyscf-0.7.6/gpu4pyscf/lib/cusolver.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/lib/cutensor.py` & `gpu4pyscf-0.7.6/gpu4pyscf/lib/cutensor.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/lib/dftd3.py` & `gpu4pyscf-0.7.6/gpu4pyscf/lib/dftd3.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/lib/dftd4.py` & `gpu4pyscf-0.7.6/gpu4pyscf/lib/dftd4.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,29 +29,29 @@
 libdftd4.dftd4_new_structure.restype         = _d4_p
 libdftd4.dftd4_new_d4_model.restype          = _d4_p
 libdftd4.dftd4_load_rational_damping.restype = _d4_p
 
 class DFTD4Dispersion(lib.StreamObject):
     def __init__(self, mol, xc, atm=False):
         coords = np.asarray(mol.atom_coords(), dtype=np.double, order='C')
-        charges = np.asarray(mol.atom_charges(), dtype=np.int32)
+        charge = np.array([mol.charge], dtype=np.double)
         nuc_types = [gto.charge(mol.atom_symbol(ia))
                      for ia in range(mol.natm)]
         nuc_types = np.asarray(nuc_types, dtype=np.int32)
         self.natm = mol.natm
         self._lattice = lib.c_null_ptr()
         self._periodic = lib.c_null_ptr()
 
         err = libdftd4.dftd4_new_error()
         self._mol = libdftd4.dftd4_new_structure(
             err,
             ctypes.c_int(mol.natm),
             nuc_types.ctypes.data_as(ctypes.c_void_p),
             coords.ctypes.data_as(ctypes.c_void_p),
-            charges.ctypes.data_as(ctypes.c_void_p),
+            charge.ctypes.data_as(ctypes.c_void_p),
             self._lattice,
             self._periodic,
         )
 
         self._disp = libdftd4.dftd4_new_d4_model(err, self._mol)
         self._param = libdftd4.dftd4_load_rational_damping(
             err,
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/lib/diis.py` & `gpu4pyscf-0.7.6/gpu4pyscf/lib/diis.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/lib/logger.py` & `gpu4pyscf-0.7.6/gpu4pyscf/lib/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 def _timer_debug2(rec, msg, cpu0=None, wall0=None, gpu0=None, sync=True):
     if rec.verbose >= DEBUG2:
         return timer(rec, msg, cpu0, wall0, gpu0)
     return cpu0, wall0, gpu0
 
 info = lib.logger.info
 note = lib.logger.note
+warn = lib.logger.warn
 debug = lib.logger.debug
 debug1 = lib.logger.debug1
 debug2 = lib.logger.debug2
 timer_debug1 = _timer_debug1
 timer_debug2 = _timer_debug2
 
 class Logger(lib.logger.Logger):
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/mp/__init__.py` & `gpu4pyscf-0.7.6/gpu4pyscf/mp/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from . import mp2
 from . import dfmp2
 
 def MP2(mf, frozen=None, mo_coeff=None, mo_occ=None):
     if mf.istype('UHF'):
-        return UMP2(mf, frozen, mo_coeff, mo_occ)
+        raise NotImplementedError
+        #return UMP2(mf, frozen, mo_coeff, mo_occ)
     elif mf.istype('GHF'):
-        return GMP2(mf, frozen, mo_coeff, mo_occ)
+        raise NotImplementedError
+        #return GMP2(mf, frozen, mo_coeff, mo_occ)
     else:
         return RMP2(mf, frozen, mo_coeff, mo_occ)
 
 def RMP2(mf, frozen=None, mo_coeff=None, mo_occ=None):
     from pyscf import lib
 
     if mf.istype('UHF'):
         raise RuntimeError('RMP2 cannot be used with UHF method.')
     elif mf.istype('ROHF'):
+        raise NotImplementedError
         lib.logger.warn(mf, 'RMP2 method does not support ROHF method. ROHF object '
                         'is converted to UHF object and UMP2 method is called.')
-        return UMP2(mf, frozen, mo_coeff, mo_occ)
+        #return UMP2(mf, frozen, mo_coeff, mo_occ)
 
-    mf = mf.remove_soscf()
+    #mf = mf.remove_soscf()
     if not mf.istype('RHF'):
         mf = mf.to_rhf()
 
     if getattr(mf, 'with_df', None):
         return dfmp2.DFMP2(mf, frozen, mo_coeff, mo_occ)
     else:
         return mp2.RMP2(mf, frozen, mo_coeff, mo_occ)
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/mp/dfmp2.py` & `gpu4pyscf-0.7.6/gpu4pyscf/mp/dfmp2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -128,8 +128,8 @@
         raise NotImplementedError
 
     # For non-canonical MP2
     def update_amps(self, t2, eris):
         raise NotImplementedError
 
     def init_amps(self, mo_energy=None, mo_coeff=None, eris=None, with_t2=WITH_T2):
-        return kernel(self, mo_energy, mo_coeff, eris, with_t2)
+        return kernel(self, mo_energy, mo_coeff, eris, with_t2)
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/mp/mp2.py` & `gpu4pyscf-0.7.6/gpu4pyscf/mp/mp2.py`

 * *Files 4% similar despite different names*

```diff
@@ -205,15 +205,14 @@
     _keys = {
         'max_cycle', 'conv_tol', 'conv_tol_normt', 'mol', 'max_memory',
         'frozen', 'level_shift', 'mo_coeff', 'mo_occ', 'e_hf', 'e_corr',
         'e_corr_ss', 'e_corr_os', 't2',
     }
 
     def __init__(self, mf, frozen=None, mo_coeff=None, mo_occ=None):
-        mf = mf.to_gpu()
         if mo_coeff is None: mo_coeff = mf.mo_coeff
         if mo_occ is None: mo_occ = mf.mo_occ
 
         self.mol = mf.mol
         self._scf = mf
         self.verbose = self.mol.verbose
         self.stdout = self.mol.stdout
@@ -344,10 +343,19 @@
 
     def nuc_grad_method(self):
         raise NotImplementedError
 
     def init_amps(self, mo_energy=None, mo_coeff=None, eris=None, with_t2=WITH_T2):
         return kernel(self, mo_energy, mo_coeff, eris, with_t2)
 
+    # to_cpu can be reused only when __init__ still takes mf
+    def to_cpu(self):
+        mf = self._scf.to_cpu()
+        from importlib import import_module
+        mod = import_module(self.__module__.replace('gpu4pyscf', 'pyscf'))
+        cls = getattr(mod, self.__class__.__name__)
+        obj = cls(mf)
+        return obj
+
 RMP2 = MP2
 from gpu4pyscf import scf
 scf.hf.RHF.MP2 = lib.class_as_method(MP2)
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/qmmm/__init__.py` & `gpu4pyscf-0.7.6/gpu4pyscf/qmmm/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/qmmm/chelpg.py` & `gpu4pyscf-0.7.6/gpu4pyscf/qmmm/chelpg.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/scf/cphf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/scf/cphf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/scf/diis.py` & `gpu4pyscf-0.7.6/gpu4pyscf/scf/diis.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/scf/dispersion.py` & `gpu4pyscf-0.7.6/gpu4pyscf/scf/dispersion.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 
 
 '''
 dispersion correction for HF and DFT
 '''
 
 
-import numpy
-from pyscf.scf.hf import KohnShamDFT
+from gpu4pyscf.scf import hf, uhf
+from gpu4pyscf.dft import rks, uks
 
 def get_dispersion(mf, disp_version=None):
     if disp_version is None:
         disp_version = mf.disp
     mol = mf.mol
     if disp_version is None:
         return 0.0
-    if isinstance(mf, KohnShamDFT):
+    if isinstance(mf, rks.KohnShamDFT):
         method = mf.xc
     else:
         method = 'hf'
 
     # for dftd3
     if disp_version[:2].upper() == 'D3':
         from gpu4pyscf.lib import dftd3
@@ -47,11 +47,11 @@
         dftd4_model = dftd4.DFTD4Dispersion(mol, xc=method)
         res = dftd4_model.get_dispersion()
         return res.get("energy")
     else:
         raise RuntimeError(f'dipersion correction: {disp_version} is not supported.')
 
 # Inject to SCF class
-from gpu4pyscf.scf import hf
-from gpu4pyscf.scf import uhf
 hf.RHF.get_dispersion = get_dispersion
-uhf.UHF.get_dispersion = get_dispersion
+uhf.UHF.get_dispersion = get_dispersion
+rks.RKS.get_dispersion = get_dispersion
+uks.UKS.get_dispersion = get_dispersion
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/scf/ghf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/scf/ghf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/scf/hf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/scf/hf.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import scipy.linalg
 from functools import reduce
 from pyscf import gto
 from pyscf import lib as pyscf_lib
 from pyscf.scf import hf, jk, _vhf
 from gpu4pyscf import lib
 from gpu4pyscf.lib.cupy_helper import (eigh, load_library, tag_array,
-                                       return_cupy_array, to_cupy)
+                                       return_cupy_array, cond)
 from gpu4pyscf.scf import diis
 from gpu4pyscf.lib import logger
 
 __all__ = [
     'get_jk', 'get_occ', 'get_grad', 'damping', 'level_shift', 'get_fock',
     'energy_elec', 'RHF'
 ]
@@ -83,35 +83,36 @@
     direct_scf_tol = vhfopt.direct_scf_tol
     cp_idx, cp_jdx = np.tril_indices(len(vhfopt.uniq_l_ctr))
     l_ctr_shell_locs = vhfopt.l_ctr_offsets
     l_ctr_ao_locs = vhfopt.mol.ao_loc[l_ctr_shell_locs]
     dm_ctr_cond = np.max(
         [pyscf_lib.condense('absmax', x, l_ctr_ao_locs) for x in dms.get()], axis=0)
 
-    dm_shl = cupy.zeros([l_ctr_shell_locs[-1], l_ctr_shell_locs[-1]])
+    dm_shl = cupy.zeros([n_dm, l_ctr_shell_locs[-1], l_ctr_shell_locs[-1]])
     assert dms.flags.c_contiguous
     size_l = np.array([1,3,6,10,15,21,28])
     l_ctr = vhfopt.uniq_l_ctr[:,0]
     r = 0
     for i, li in enumerate(l_ctr):
         i0 = l_ctr_ao_locs[i]
         i1 = l_ctr_ao_locs[i+1]
         ni_shls = (i1-i0)//size_l[li]
         c = 0
         for j, lj in enumerate(l_ctr):
             j0 = l_ctr_ao_locs[j]
             j1 = l_ctr_ao_locs[j+1]
             nj_shls = (j1-j0)//size_l[lj]
-            sub_dm = dms[0][i0:i1,j0:j1].reshape([ni_shls, size_l[li], nj_shls, size_l[lj]])
-            dm_shl[r:r+ni_shls, c:c+nj_shls] = cupy.max(sub_dm, axis=[1,3])
+            for idm in range(n_dm):
+                sub_dm = dms[idm][i0:i1,j0:j1].reshape([ni_shls, size_l[li], nj_shls, size_l[lj]])
+                dm_shl[idm, r:r+ni_shls, c:c+nj_shls] = cupy.max(cupy.abs(sub_dm), axis=[1,3])
             c += nj_shls
         r += ni_shls
-
+    dm_shl = cupy.max(dm_shl, axis=0)
     dm_shl = cupy.log(dm_shl)
-    nshls = dm_shl.shape[0]
+    nshls = dm_shl.shape[1]
     if hermi != 1:
         dm_ctr_cond = (dm_ctr_cond + dm_ctr_cond.T) * .5
     fn = libgvhf.GINTbuild_jk
     for cp_ij_id, log_q_ij in enumerate(log_qs):
         cpi = cp_idx[cp_ij_id]
         cpj = cp_jdx[cp_ij_id]
         li = vhfopt.uniq_l_ctr[cpi,0]
@@ -173,14 +174,15 @@
                 detail = f'CUDA Error for ({l_symb[li]}{l_symb[lj]}|{l_symb[lk]}{l_symb[ll]})'
                 raise RuntimeError(detail)
             #log.debug1('(%s%s|%s%s) on GPU %.3fs',
             #           l_symb[li], l_symb[lj], l_symb[lk], l_symb[ll],
             #           time.perf_counter() - t0)
             #print(li, lj, lk, ll, time.perf_counter() - t0)
             #exit()
+
     if with_j:
         vj_ao = []
         #vj = [cupy.einsum('pi,pq,qj->ij', coeff, x, coeff) for x in vj]
         for x in vj:
             #x = cupy.einsum('pi,pq->iq', coeff, x)
             #x = cupy.einsum('iq,qj->ij', x, coeff)
             x = coeff.T @ x @ coeff
@@ -276,15 +278,14 @@
             with mol.with_range_coulomb(omega):
                 vhfopt = _VHFOpt(mol, getattr(mf.opt, '_intor', 'int2e'),
                                 getattr(mf.opt, 'prescreen', 'CVHFnrs8_prescreen'),
                                 getattr(mf.opt, '_qcondname', 'CVHFsetnr_direct_scf'),
                                 getattr(mf.opt, '_dmcondname', 'CVHFsetnr_direct_scf_dm'))
                 vhfopt.build(mf.direct_scf_tol)
                 mf._opt_gpu_omega = vhfopt
-
     vj, vk = get_jk(mol, dm, hermi, vhfopt, with_j, with_k, omega, verbose=log)
     log.timer('vj and vk on gpu', *cput0)
     return vj, vk
 
 def make_rdm1(mf, mo_coeff=None, mo_occ=None, **kwargs):
     if mo_occ is None: mo_occ = mf.mo_occ
     if mo_coeff is None: mo_coeff = mf.mo_coeff
@@ -385,15 +386,15 @@
     log = logger.new_logger(mol, verbose)
     t0 = log.init_timer()
     if(conv_tol_grad is None):
         conv_tol_grad = conv_tol**.5
         logger.info(mf, 'Set gradient conv threshold to %g', conv_tol_grad)
 
     if(dm0 is None):
-        dm0 = mf.get_init_guess(mol)
+        dm0 = mf.get_init_guess(mol, mf.init_guess)
 
     dm = cupy.asarray(dm0, order='C')
     if hasattr(dm0, 'mo_coeff') and hasattr(dm0, 'mo_occ'):
         if dm0.ndim == 2:
             mo_coeff = cupy.asarray(dm0.mo_coeff)
             mo_occ = cupy.asarray(dm0.mo_occ)
             occ_coeff = cupy.asarray(mo_coeff[:,mo_occ>0])
@@ -454,89 +455,14 @@
             break
 
     if(cycle == mf.max_cycle):
         logger.warn("SCF failed to converge")
 
     return scf_conv, e_tot, mo_energy, mo_coeff, mo_occ
 
-# tempory implemention, will be replaced after pyscf 2.2.0
-def _gen_rhf_response(mf, mo_coeff=None, mo_occ=None,
-                      singlet=None, hermi=0, max_memory=None):
-    '''Generate a function to compute the product of RHF response function and
-    RHF density matrices.
-
-    Kwargs:
-        singlet (None or boolean) : If singlet is None, response function for
-            orbital hessian or CPHF will be generated. If singlet is boolean,
-            it is used in TDDFT response kernel.
-    '''
-    if mo_coeff is None: mo_coeff = mf.mo_coeff
-    if mo_occ is None: mo_occ = mf.mo_occ
-    mol = mf.mol
-    if isinstance(mf, hf.KohnShamDFT):
-        from pyscf.dft import numint
-        ni = mf._numint
-        ni.libxc.test_deriv_order(mf.xc, 2, raise_error=True)
-        if getattr(mf, 'nlc', '') != '':
-            logger.warn(mf, 'NLC functional found in DFT object.  Its second '
-                        'deriviative is not available. Its contribution is '
-                        'not included in the response function.')
-        omega, alpha, hyb = ni.rsh_and_hybrid_coeff(mf.xc, mol.spin)
-        hybrid = abs(hyb) > 1e-10
-
-        # mf can be pbc.dft.RKS object with multigrid
-        if (not hybrid and
-            'MultiGridFFTDF' == getattr(mf, 'with_df', None).__class__.__name__):
-            from pyscf.pbc.dft import multigrid
-            dm0 = mf.make_rdm1(mo_coeff, mo_occ)
-            return multigrid._gen_rhf_response(mf, dm0, singlet, hermi)
-
-        if singlet is None:
-            # for ground state orbital hessian
-            rho0, vxc, fxc = ni.cache_xc_kernel(mol, mf.grids, mf.xc,
-                                                mo_coeff, mo_occ, 0)
-        else:
-            rho0, vxc, fxc = ni.cache_xc_kernel(mol, mf.grids, mf.xc,
-                                                [mo_coeff]*2, [mo_occ*.5]*2, spin=1)
-        dm0 = None  #mf.make_rdm1(mo_coeff, mo_occ)
-
-        if singlet is None:
-            # Without specify singlet, used in ground state orbital hessian
-            def vind(dm1):
-                # The singlet hessian
-                if hermi == 2:
-                    v1 = cupy.zeros_like(dm1)
-                else:
-                    v1 = ni.nr_rks_fxc(mol, mf.grids, mf.xc, dm0, dm1, 0, hermi,
-                                       rho0, vxc, fxc, max_memory=max_memory)
-                if hybrid or abs(alpha) > 1e-10:
-                    if hermi != 2:
-                        vj, vk = mf.get_jk(mol, dm1, hermi=hermi)
-                        vk *= hyb
-                        if omega > 1e-10:  # For range separated Coulomb
-                            vk += mf.get_k(mol, dm1, hermi, omega) * (alpha-hyb)
-                        v1 += vj - .5 * vk
-                    else:
-                        v1 -= .5 * hyb * mf.get_k(mol, dm1, hermi=hermi)
-                elif hermi != 2:
-                    v1 += mf.get_j(mol, dm1, hermi=hermi)
-                return v1
-        else:
-            raise NotImplementedError('only singlet response is supported!')
-
-    else:  # HF
-        if (singlet is None or singlet) and hermi != 2:
-            def vind(dm1):
-                vj, vk = mf.get_jk(mol, dm1, hermi=hermi)
-                return vj - .5 * vk
-        else:
-            def vind(dm1):
-                return -.5 * mf.get_k(mol, dm1, hermi=hermi)
-
-    return vind
 
 def _quad_moment(mf, mol=None, dm=None, unit='Debye-Ang'):
     from pyscf.data import nist
     if mol is None: mol = mf.mol
     if dm is None: dm = mf.make_rdm1()
     nao = mol.nao
     with mol.with_common_orig((0,0,0)):
@@ -596,31 +522,170 @@
                             dm0=dm0, callback=mf.callback,
                             conv_check=mf.conv_check, **kwargs)[1]
 
     logger.timer(mf, 'SCF', *cput0)
     mf._finalize()
     return mf.e_tot
 
-class RHF(hf.RHF):
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+def as_scanner(mf):
+    if isinstance(mf, pyscf_lib.SinglePointScanner):
+        return mf
+
+    logger.info(mf, 'Create scanner for %s', mf.__class__)
+    name = mf.__class__.__name__ + SCF_Scanner.__name_mixin__
+    return pyscf_lib.set_class(SCF_Scanner(mf), (SCF_Scanner, mf.__class__), name)
+
+class SCF_Scanner(pyscf_lib.SinglePointScanner):
+    def __init__(self, mf_obj):
+        self.__dict__.update(mf_obj.__dict__)
+        self._last_mol_fp = mf_obj.mol.ao_loc
+
+    def __call__(self, mol_or_geom, **kwargs):
+        if isinstance(mol_or_geom, gto.MoleBase):
+            mol = mol_or_geom
+        else:
+            mol = self.mol.set_geom_(mol_or_geom, inplace=False)
+
+        # Cleanup intermediates associated to the previous mol object
+        self.reset(mol)
+
+        if 'dm0' in kwargs:
+            dm0 = kwargs.pop('dm0')
+        elif self.mo_coeff is None:
+            dm0 = None
+        else:
+            dm0 = None
+            if cupy.array_equal(self._last_mol_fp, mol.ao_loc):
+                dm0 = self.make_rdm1()
+            else:
+                raise NotImplementedError
+        self.mo_coeff = None  # To avoid last mo_coeff being used by SOSCF
+        e_tot = self.kernel(dm0=dm0, **kwargs)
+        self._last_mol_fp = mol.ao_loc
+        return e_tot
+
+class SCF(pyscf_lib.StreamObject):
+
+    # attributes
+    conv_tol            = hf.SCF.conv_tol
+    conv_tol_grad       = hf.SCF.conv_tol_grad
+    max_cycle           = hf.SCF.max_cycle
+    init_guess          = hf.SCF.init_guess
+
+    disp                = None
+    DIIS                = hf.SCF.DIIS
+    diis                = hf.SCF.diis
+    diis_space          = hf.SCF.diis_space
+    diis_damp           = hf.SCF.diis_damp
+    diis_start_cycle    = hf.SCF.diis_start_cycle
+    diis_file           = hf.SCF.diis_file
+    diis_space_rollback = hf.SCF.diis_space_rollback
+    damp                = hf.SCF.damp
+    level_shift         = hf.SCF.level_shift
+    direct_scf          = hf.SCF.direct_scf
+    direct_scf_tol      = hf.SCF.direct_scf_tol
+    conv_check          = hf.SCF.conv_check
+    callback            = hf.SCF.callback
+    _keys               = hf.SCF._keys
+
+    # methods
+    __init__                 = hf.SCF.__init__
+
+    def check_sanity(self):
+        s1e = self.get_ovlp()
+        if isinstance(s1e, cupy.ndarray) and s1e.ndim == 2:
+            c = cond(s1e)
+        else:
+            c = cupy.asarray([cond(xi) for xi in s1e])
+        logger.debug(self, 'cond(S) = %s', c)
+        if cupy.max(c)*1e-17 > self.conv_tol:
+            logger.warn(self, 'Singularity detected in overlap matrix (condition number = %4.3g). '
+                        'SCF may be inaccurate and hard to converge.', cupy.max(c))
+        return super().check_sanity()
+
+    build                    = hf.SCF.build
+    opt                      = NotImplemented
+    dump_flags               = hf.SCF.dump_flags
+    get_fock                 = hf.SCF.get_fock
+    get_occ                  = hf.SCF.get_occ
+    get_grad                 = hf.SCF.get_grad
+    dump_chk                 = NotImplemented
+    init_guess_by_minao      = hf.SCF.init_guess_by_minao
+    init_guess_by_atom       = hf.SCF.init_guess_by_atom
+    init_guess_by_huckel     = hf.SCF.init_guess_by_huckel
+    init_guess_by_mod_huckel = hf.SCF.init_guess_by_mod_huckel
+    init_guess_by_1e         = hf.SCF.init_guess_by_1e
+    init_guess_by_chkfile    = NotImplemented
+    from_chk                 = NotImplemented
+    get_init_guess           = hf.SCF.get_init_guess
+    make_rdm1                = hf.SCF.make_rdm1
+    make_rdm2                = hf.SCF.make_rdm2
+    energy_elec              = hf.SCF.energy_elec
+    energy_tot               = hf.SCF.energy_tot
+    energy_nuc               = hf.SCF.energy_nuc
+    check_convergence        = None
+    _eigh                    = staticmethod(eigh)
+    eig                      = hf.SCF.eig
+
+    scf                      = hf.SCF.scf
+    as_scanner               = hf.SCF.as_scanner
+    _finalize                = hf.SCF._finalize
+    init_direct_scf          = hf.SCF.init_direct_scf
+    get_jk                   = hf.SCF.get_jk
+    get_j                    = hf.SCF.get_j
+    get_k                    = hf.SCF.get_k
+    get_veff                 = hf.SCF.get_veff
+    analyze                  = hf.SCF.analyze
+    mulliken_meta            = hf.SCF.mulliken_meta
+    pop                      = hf.SCF.pop
+    dip_moment               = hf.SCF.dip_moment
+    _is_mem_enough           = NotImplemented
+    density_fit              = NotImplemented
+    sfx2c1e                  = NotImplemented
+    x2c1e                    = NotImplemented
+    x2c                      = NotImplemented
+    newton                   = NotImplemented
+    remove_soscf             = NotImplemented
+    stability                = NotImplemented
+    nuc_grad_method          = NotImplemented
+    update_                  = NotImplemented
+    istype                   = hf.SCF.istype
+
+    def reset(self, mol=None):
+        if mol is not None:
+            self.mol = mol
+        self._opt_gpu = None
+        self._opt_gpu_omega = None
+        self.scf_summary = {}
+        return self
+
+class KohnShamDFT:
+    '''
+    A mock DFT base class, to be compatible with PySCF
+    '''
+
+from gpu4pyscf.lib import utils
+class RHF(SCF):
+
+    to_gpu = utils.to_gpu
+    device = utils.device
 
     _keys = {'e_disp', 'h1e', 's1e', 'e_mf', 'screen_tol', 'conv_tol_cpscf'}
 
     screen_tol = 1e-14
     conv_tol_cpscf = 1e-3
     DIIS = diis.SCF_DIIS
     get_jk = _get_jk
     _eigh = staticmethod(eigh)
     make_rdm1 = make_rdm1
     energy_elec = energy_elec
     get_fock = get_fock
     get_occ = get_occ
     get_veff = get_veff
     get_grad = staticmethod(get_grad)
-    gen_response = _gen_rhf_response
     quad_moment = _quad_moment
     energy_tot = energy_tot
 
     get_hcore = return_cupy_array(hf.RHF.get_hcore)
     get_ovlp = return_cupy_array(hf.RHF.get_ovlp)
     get_init_guess = return_cupy_array(hf.RHF.get_init_guess)
     init_direct_scf = NotImplemented
@@ -641,29 +706,28 @@
     stability = NotImplemented
     mulliken_pop = NotImplemented
     mulliken_meta = NotImplemented
 
     scf = scf
     kernel = scf
 
-    def reset(self, mol=None):
-        super().reset(mol)
-        self._opt_gpu = None
-        self._opt_gpu_omega = None
-        return self
-
     def nuc_grad_method(self):
         from gpu4pyscf.grad import rhf
         return rhf.Gradients(self)
 
     def density_fit(self, auxbasis=None, with_df=None, only_dfj=False):
         import gpu4pyscf.df.df_jk
         return gpu4pyscf.df.df_jk.density_fit(self, auxbasis, with_df, only_dfj)
 
-class _VHFOpt(_vhf.VHFOpt):
+    def to_cpu(self):
+        mf = hf.RHF(self.mol)
+        utils.to_cpu(self, out=mf)
+        return mf
+
+class _VHFOpt:
     from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
 
     def __init__(self, mol, intor, prescreen='CVHFnoscreen',
                  qcondname='CVHFsetnr_direct_scf', dmcondname=None):
         self.mol, self.coeff = basis_seg_contraction(mol)
         self.coeff = cupy.asarray(self.coeff)
         # Note mol._bas will be sorted in .build() method. VHFOpt should be
@@ -813,14 +877,18 @@
             self.bas_pairs_locs.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(ncptype),
             mol._atm.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(mol.natm),
             mol._bas.ctypes.data_as(ctypes.c_void_p), ctypes.c_int(mol.nbas),
             mol._env.ctypes.data_as(ctypes.c_void_p))
         logger.timer(mol, 'Initialize GPU cache', *cput1)
         return self
 
+    init_cvhf_direct = _vhf.VHFOpt.init_cvhf_direct
+    get_q_cond       = _vhf.VHFOpt.get_q_cond
+    set_dm           = _vhf.VHFOpt.set_dm
+
     def clear(self):
         _vhf.VHFOpt.__del__(self)
         libgvhf.GINTdel_basis_prod(ctypes.byref(self.bpcache))
         return self
 
     def __del__(self):
         try:
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/scf/int4c2e.py` & `gpu4pyscf-0.7.6/gpu4pyscf/scf/int4c2e.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/scf/rohf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/scf/rohf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/scf/ucphf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/scf/ucphf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/scf/uhf.py` & `gpu4pyscf-0.7.6/gpu4pyscf/scf/uhf.py`

 * *Files 24% similar despite different names*

```diff
@@ -105,31 +105,127 @@
     if diis and cycle >= diis_start_cycle:
         f = diis.update(s1e, dm, f, mf, h1e, vhf)
     if abs(shifta)+abs(shiftb) > 1e-4:
         f = (level_shift(s1e, dm[0], f[0], shifta),
              level_shift(s1e, dm[1], f[1], shiftb))
     return f
 
+def get_grad(mo_coeff, mo_occ, fock_ao):
+    '''UHF Gradients'''
+    occidxa = mo_occ[0] > 0
+    occidxb = mo_occ[1] > 0
+    viridxa = ~occidxa
+    viridxb = ~occidxb
+
+    ga = mo_coeff[0][:,viridxa].conj().T.dot(fock_ao[0].dot(mo_coeff[0][:,occidxa]))
+    gb = mo_coeff[1][:,viridxb].conj().T.dot(fock_ao[1].dot(mo_coeff[1][:,occidxb]))
+    return cupy.hstack((ga.ravel(), gb.ravel()))
+
+def energy_elec(mf, dm=None, h1e=None, vhf=None):
+    '''Electronic energy of Unrestricted Hartree-Fock
+
+    Note this function has side effects which cause mf.scf_summary updated.
+
+    Returns:
+        Hartree-Fock electronic energy and the 2-electron part contribution
+    '''
+    if dm is None: dm = mf.make_rdm1()
+    if h1e is None:
+        h1e = mf.get_hcore()
+    if isinstance(dm, cupy.ndarray) and dm.ndim == 2:
+        dm = cupy.array((dm*.5, dm*.5))
+    if vhf is None:
+        vhf = mf.get_veff(mf.mol, dm)
+    if h1e[0].ndim < dm[0].ndim:  # get [0] because h1e and dm may not be ndarrays
+        h1e = (h1e, h1e)
+    e1 = cupy.einsum('ij,ji->', h1e[0], dm[0])
+    e1+= cupy.einsum('ij,ji->', h1e[1], dm[1])
+    e_coul =(cupy.einsum('ij,ji->', vhf[0], dm[0]) +
+             cupy.einsum('ij,ji->', vhf[1], dm[1])) * .5
+    e1 = e1.get()[()]
+    e_coul = e_coul.get()[()]
+    e_elec = (e1 + e_coul).real
+    mf.scf_summary['e1'] = e1.real
+    mf.scf_summary['e2'] = e_coul.real
+    logger.debug(mf, 'E1 = %s  Ecoul = %s', e1, e_coul.real)
+    return e_elec, e_coul
 
-class UHF(uhf.UHF):
-    from gpu4pyscf.lib.utils import to_cpu, to_gpu, device
+class UHF(hf.SCF):
+    from gpu4pyscf.lib.utils import to_gpu, device
 
     _keys = {'e_disp', 'screen_tol', 'conv_tol_cpscf', 'h1e', 's1e'}
+    def __init__(self, mol):
+        hf.SCF.__init__(self, mol)
+        self.nelec = None
+
+    @property
+    def nelec(self):
+        if self._nelec is not None:
+            return self._nelec
+        else:
+            return self.mol.nelec
+    @nelec.setter
+    def nelec(self, x):
+        self._nelec = x
+
+    @property
+    def nelectron_alpha(self):
+        return self.nelec[0]
+    @nelectron_alpha.setter
+    def nelectron_alpha(self, x):
+        logger.warn(self, 'WARN: Attribute .nelectron_alpha is deprecated. '
+                    'Set .nelec instead')
+        #raise RuntimeError('API updates')
+        self.nelec = (x, self.mol.nelectron-x)
+
+    def dump_flags(self, verbose=None):
+        return
+
+    get_jk = hf._get_jk
+    _eigh = staticmethod(eigh)
+    get_fock = get_fock
+    get_occ = uhf.get_occ
+
+    def get_grad(self, mo_coeff, mo_occ, fock=None):
+        if fock is None:
+            dm1 = self.make_rdm1(mo_coeff, mo_occ)
+            fock = self.get_hcore(self.mol) + self.get_veff(self.mol, dm1)
+        return get_grad(mo_coeff, mo_occ, fock)
+
+    make_rdm2                = NotImplemented
+    energy_elec              = energy_elec
+    get_init_guess           = hf.return_cupy_array(uhf.UHF.get_init_guess)
+    init_guess_by_minao      = uhf.UHF.init_guess_by_minao
+    init_guess_by_atom       = uhf.UHF.init_guess_by_atom
+    init_guess_by_huckel     = uhf.UHF.init_guess_by_huckel
+    init_guess_by_mod_huckel = uhf.UHF.init_guess_by_mod_huckel
+    init_guess_by_1e         = uhf.UHF.init_guess_by_1e
+    init_guess_by_chkfile    = NotImplemented
+
+    analyze            = NotImplemented
+    mulliken_pop       = NotImplemented
+    mulliken_spin_pop  = NotImplemented
+    mulliken_meta      = NotImplemented
+    mulliken_meta_spin = NotImplemented
+    canonicalize       = NotImplemented
+    det_ovlp           = NotImplemented
+    make_asym_dm       = NotImplemented
+    _finalize          = uhf.UHF._finalize
 
     screen_tol = 1e-14
     conv_tol_cpscf = 1e-3
     DIIS = diis.SCF_DIIS
-    get_jk = _get_jk
-    _eigh = staticmethod(eigh)
-    get_fock = get_fock
+    #get_jk = _get_jk
+
     get_hcore = hf.RHF.get_hcore
     get_ovlp = hf.RHF.get_ovlp
     get_init_guess = hf.return_cupy_array(uhf.UHF.get_init_guess)
     density_fit = hf.RHF.density_fit
     energy_tot = hf.RHF.energy_tot
+    energy_elec = energy_elec
 
     make_rdm2 = NotImplemented
     dump_chk = NotImplemented
     newton = NotImplemented
     x2c = x2c1e = sfx2c1e = NotImplemented
     to_rhf = NotImplemented
     to_uhf = NotImplemented
@@ -188,7 +284,12 @@
             s = self.get_ovlp()
         return spin_square(mo_coeff, s)
 
     def nuc_grad_method(self):
         from gpu4pyscf.grad import uhf
         return uhf.Gradients(self)
 
+    def to_cpu(self):
+        from gpu4pyscf.lib import utils
+        mf = uhf.UHF(self.mol)
+        utils.to_cpu(self, mf)
+        return mf
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/solvent/__init__.py` & `gpu4pyscf-0.7.6/gpu4pyscf/solvent/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/solvent/_attach_solvent.py` & `gpu4pyscf-0.7.6/gpu4pyscf/solvent/_attach_solvent.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/solvent/grad/__init__.py` & `gpu4pyscf-0.7.6/gpu4pyscf/solvent/grad/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/solvent/grad/pcm.py` & `gpu4pyscf-0.7.6/gpu4pyscf/solvent/grad/pcm.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/solvent/grad/smd.py` & `gpu4pyscf-0.7.6/gpu4pyscf/solvent/grad/smd.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/solvent/hessian/pcm.py` & `gpu4pyscf-0.7.6/gpu4pyscf/solvent/hessian/pcm.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 Gradient of PCM family solvent model
 '''
 # pylint: disable=C0103
 
 import numpy
 import cupy
 from cupyx import scipy
-from pyscf import lib, scf, gto, df
+from pyscf import lib, gto, df
 from pyscf.grad import rhf as rhf_grad
+from gpu4pyscf import scf
 from gpu4pyscf.solvent.pcm import PI, switch_h
 from gpu4pyscf.solvent.grad.pcm import grad_switch_h, get_dF_dA, get_dD_dS, grad_qv, grad_solver, grad_nuc
 from gpu4pyscf.df import int3c2e
 from gpu4pyscf.lib.cupy_helper import contract
 from gpu4pyscf.lib import logger
 
 libdft = lib.load_library('libdft')
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/solvent/hessian/smd.py` & `gpu4pyscf-0.7.6/gpu4pyscf/solvent/hessian/smd.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/solvent/pcm.py` & `gpu4pyscf-0.7.6/gpu4pyscf/solvent/pcm.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,18 +211,24 @@
         #nrij = cupy.sum(drij * norm_vec, axis=-1)
 
         D = S*nrij/rij**2 -2.0*xi_r_ij/PI**0.5*cupy.exp(-xi_r_ij**2)*nrij/rij**3
         cupy.fill_diagonal(D, -charge_exp * (2.0 / PI)**0.5 / (2.0 * R_vdw))
 
     return D, S
 
-class PCM(ddcosmo.DDCOSMO):
+class PCM(lib.StreamObject):
     _keys = {
-        'method', 'vdw_scale', 'surface', 'r_probe', 'intopt'
+        'method', 'vdw_scale', 'surface', 'r_probe', 'intopt',
+        'mol', 'radii_table', 'atom_radii', 'lebedev_order', 'lmax', 'eta',
+        'eps', 'grids', 'max_cycle', 'conv_tol', 'state_id', 'frozen',
+        'equilibrium_solvation', 'e', 'v',
     }
+
+    kernel = ddcosmo.DDCOSMO.kernel
+
     def __init__(self, mol):
         ddcosmo.DDCOSMO.__init__(self, mol)
         self.method = 'C-PCM'
         self.vdw_scale = 1.2 # default value in qchem
         self.r_probe = 0.0
         self.radii_table = None
         self.surface = {}
@@ -373,17 +379,20 @@
         from gpu4pyscf import scf
         if isinstance(hess_method.base, (scf.hf.RHF, scf.uhf.UHF)):
             return pcm_hess.make_hess_object(hess_method)
         else:
             raise RuntimeError('Only SCF gradient is supported')
 
     def reset(self, mol=None):
+        if mol is not None:
+            self.mol = mol
+            self.grids.reset(mol)
+        self._intermediates = None
         self.surface = None
         self.intopt = None
-        super().reset(mol)
         return self
 
     def _B_dot_x(self, dms):
         if not self._intermediates:
             self.build()
         out_shape = dms.shape
         nao = dms.shape[-1]
```

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf/solvent/smd.py` & `gpu4pyscf-0.7.6/gpu4pyscf/solvent/smd.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.5/gpu4pyscf.egg-info/SOURCES.txt` & `gpu4pyscf-0.7.6/gpu4pyscf.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 gpu4pyscf/__config__.py
 gpu4pyscf/__init__.py
-gpu4pyscf/patch_pyscf.py
 gpu4pyscf.egg-info/PKG-INFO
 gpu4pyscf.egg-info/SOURCES.txt
 gpu4pyscf.egg-info/dependency_links.txt
 gpu4pyscf.egg-info/requires.txt
 gpu4pyscf.egg-info/top_level.txt
 gpu4pyscf/cc/__init__.py
 gpu4pyscf/cc/ccsd_incore.py
 gpu4pyscf/df/__init__.py
 gpu4pyscf/df/cderi.py
 gpu4pyscf/df/df.py
 gpu4pyscf/df/df_jk.py
 gpu4pyscf/df/int3c2e.py
-gpu4pyscf/df/patch_pyscf.py
 gpu4pyscf/df/grad/__init__.py
 gpu4pyscf/df/grad/rhf.py
 gpu4pyscf/df/grad/rks.py
 gpu4pyscf/df/grad/uhf.py
 gpu4pyscf/df/grad/uks.py
 gpu4pyscf/df/hessian/__init__.py
 gpu4pyscf/df/hessian/rhf.py
@@ -30,26 +28,24 @@
 gpu4pyscf/df/hessian/uks.py
 gpu4pyscf/dft/__init__.py
 gpu4pyscf/dft/gen_grid.py
 gpu4pyscf/dft/gks.py
 gpu4pyscf/dft/libxc.py
 gpu4pyscf/dft/libxc_structs.py
 gpu4pyscf/dft/numint.py
-gpu4pyscf/dft/patch_pyscf.py
 gpu4pyscf/dft/radi.py
 gpu4pyscf/dft/rks.py
 gpu4pyscf/dft/roks.py
 gpu4pyscf/dft/uks.py
 gpu4pyscf/dft/xc_alias.py
 gpu4pyscf/dft/xc_deriv.py
 gpu4pyscf/fci/__init__.py
 gpu4pyscf/fci/direct_spin1.py
 gpu4pyscf/grad/__init__.py
 gpu4pyscf/grad/dispersion.py
-gpu4pyscf/grad/patch_pyscf.py
 gpu4pyscf/grad/rhf.py
 gpu4pyscf/grad/rks.py
 gpu4pyscf/grad/uhf.py
 gpu4pyscf/grad/uks.py
 gpu4pyscf/gto/__init__.py
 gpu4pyscf/gto/mole.py
 gpu4pyscf/hessian/__init__.py
@@ -70,21 +66,21 @@
 gpu4pyscf/lib/utils.py
 gpu4pyscf/mp/__init__.py
 gpu4pyscf/mp/dfmp2.py
 gpu4pyscf/mp/mp2.py
 gpu4pyscf/qmmm/__init__.py
 gpu4pyscf/qmmm/chelpg.py
 gpu4pyscf/scf/__init__.py
+gpu4pyscf/scf/_response_functions.py
 gpu4pyscf/scf/cphf.py
 gpu4pyscf/scf/diis.py
 gpu4pyscf/scf/dispersion.py
 gpu4pyscf/scf/ghf.py
 gpu4pyscf/scf/hf.py
 gpu4pyscf/scf/int4c2e.py
-gpu4pyscf/scf/patch_pyscf.py
 gpu4pyscf/scf/rohf.py
 gpu4pyscf/scf/ucphf.py
 gpu4pyscf/scf/uhf.py
 gpu4pyscf/solvent/__init__.py
 gpu4pyscf/solvent/_attach_solvent.py
 gpu4pyscf/solvent/pcm.py
 gpu4pyscf/solvent/smd.py
```

### Comparing `gpu4pyscf-0.7.5/setup.py` & `gpu4pyscf-0.7.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,12 +121,12 @@
         "pytest-cov==4.0.0",
         "pytest-cover==3.0.0",
         "pytest-coverage==0.0",
     ],
     cmdclass={'build_py': CMakeBuildPy},
     install_requires=[
         'pyscf>=2.5.0',
-        f'cupy-cuda{CUDA_VERSION}>=13.0',
+        f'cupy-cuda{CUDA_VERSION}',
         'geometric',
         f'gpu4pyscf-libxc-cuda{CUDA_VERSION}',
     ]
 )
```

