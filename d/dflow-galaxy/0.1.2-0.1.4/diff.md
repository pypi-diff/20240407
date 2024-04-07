# Comparing `tmp/dflow_galaxy-0.1.2.tar.gz` & `tmp/dflow_galaxy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dflow_galaxy-0.1.2.tar", max compression
+gzip compressed data, was "dflow_galaxy-0.1.4.tar", max compression
```

## Comparing `dflow_galaxy-0.1.2.tar` & `dflow_galaxy-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,75 @@
--rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.2/LICENSE
--rw-r--r--   0        0        0     1103 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.2/dflow_galaxy/__init__.py
--rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.2/dflow_galaxy/core/__init__.py
--rw-r--r--   0        0        0    25307 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.2/dflow_galaxy/core/dflow.py
--rw-r--r--   0        0        0     3679 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.2/dflow_galaxy/core/dispatcher.py
--rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.2/dflow_galaxy/core/log.py
--rw-r--r--   0        0        0       97 2024-02-20 09:21:26.953252 dflow_galaxy-0.1.2/dflow_galaxy/core/pydantic.py
--rw-r--r--   0        0        0      541 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.2/dflow_galaxy/core/types.py
--rw-r--r--   0        0        0     5603 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.2/dflow_galaxy/core/util.py
--rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.2/dflow_galaxy/main.py
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.2/dflow_galaxy/workflow/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/__init__.py
--rw-r--r--   0        0        0     1704 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/config.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/domain/abacus.py
--rw-r--r--   0        0        0     6247 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/domain/cp2k.py
--rw-r--r--   0        0        0     9775 2024-02-25 16:58:10.948762 dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/domain/deepmd.py
--rw-r--r--   0        0        0     8019 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/domain/lammps.py
--rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/domain/lib.py
--rw-r--r--   0        0        0     6334 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/domain/model_devi.py
--rw-r--r--   0        0        0     7630 2024-02-26 01:47:46.472491 dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/main.py
--rw-r--r--   0        0        0      390 2024-02-26 01:48:05.942489 dflow_galaxy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1648 2024-04-07 12:32:34.406173 dflow_galaxy-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.4/dflow_galaxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.4/dflow_galaxy/app/__init__.py
+-rw-r--r--   0        0        0     2193 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/app/common.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.4/dflow_galaxy/app/cp2k_lightning/__init__.py
+-rw-r--r--   0        0        0     2047 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/app/cp2k_lightning/dflow.py
+-rw-r--r--   0        0        0     6456 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/app/cp2k_lightning/main.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/app/dynacat_md/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/app/dynacat_md/dflow.py
+-rw-r--r--   0        0        0     4562 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/app/dynacat_md/main.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.4/dflow_galaxy/app/dynacat_tesla/__init__.py
+-rw-r--r--   0        0        0      525 2024-04-07 06:31:41.633804 dflow_galaxy-0.1.4/dflow_galaxy/app/dynacat_tesla/main.py
+-rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.4/dflow_galaxy/core/__init__.py
+-rw-r--r--   0        0        0    28431 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/core/dflow.py
+-rw-r--r--   0        0        0     4655 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.4/dflow_galaxy/core/dispatcher.py
+-rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.4/dflow_galaxy/core/log.py
+-rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.4/dflow_galaxy/core/pydantic.py
+-rw-r--r--   0        0        0      541 2024-04-03 16:22:36.889294 dflow_galaxy-0.1.4/dflow_galaxy/core/types.py
+-rw-r--r--   0        0        0     5603 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.4/dflow_galaxy/core/util.py
+-rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.4/dflow_galaxy/main.py
+-rw-r--r--   0        0        0       98 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.4/dflow_galaxy/res/__init__.py
+-rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
+-rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
+-rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
+-rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ADMM
+-rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
+-rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
+-rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
+-rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
+-rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
+-rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MINIX
+-rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
+-rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
+-rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
+-rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
+-rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
+-rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
+-rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
+-rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
+-rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_SET
+-rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
+-rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
+-rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
+-rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/BASIS_pob
+-rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
+-rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
+-rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
+-rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
+-rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
+-rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
+-rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/HFX_BASIS
+-rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
+-rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
+-rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
+-rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
+-rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
+-rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/POTENTIAL
+-rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
+-rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/README.md
+-rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
+-rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.4/dflow_galaxy/res/cp2k_data/xTB_parameters
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.4/dflow_galaxy/workflow/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/__init__.py
+-rw-r--r--   0        0        0     1704 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/config.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/abacus.py
+-rw-r--r--   0        0        0     6298 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/cp2k.py
+-rw-r--r--   0        0        0     9775 2024-02-25 16:58:10.948762 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/deepmd.py
+-rw-r--r--   0        0        0     8016 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/lammps.py
+-rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/lib.py
+-rw-r--r--   0        0        0     6334 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/model_devi.py
+-rw-r--r--   0        0        0     7676 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/main.py
+-rw-r--r--   0        0        0      541 2024-04-07 12:34:47.066159 dflow_galaxy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.4/PKG-INFO
```

### Comparing `dflow_galaxy-0.1.2/LICENSE` & `dflow_galaxy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.2/dflow_galaxy/core/dflow.py` & `dflow_galaxy-0.1.4/dflow_galaxy/core/dflow.py`

 * *Files 11% similar despite different names*

```diff
@@ -113,14 +113,15 @@
                                          'dflow_output_artifacts',
                                          ])
 
 
 def bash_build_template(py_fn: Callable,
                         base_dir: str,
                         setup_script: str = '',
+                        default_archive: Optional[str] = 'default',
                         eof: str = '__EOF__') -> _BashTemplate:
     """
     build bash step from a python function
     """
     sig = inspect.signature(py_fn)
     assert len(sig.parameters) == 1, f'{py_fn} should have only one parameter'
     args_type = sig.parameters[next(iter(sig.parameters))].annotation
@@ -142,37 +143,49 @@
         ''
         f'mkdir -p {shlex.quote(output_artifacts_dir)}',
         '',
         '# Setup Variables',
     ]
 
     for f, v in iter_python_step_args(args_type):
-        if f.type.__metadata__[0] == types.Symbol.INPUT_PARAMETER:
+        meta = f.type.__metadata__[0]
+        if meta == types.Symbol.INPUT_PARAMETER:
             # input parameter can be a multiline string
             bash_name = f'_DF_INPUT_PARAMETER_{f.name}_'
             source.extend([
                 f"{bash_name}=$(cat << {eof}",
                 f"{{{{inputs.parameters.{f.name}}}}}",
                 eof,
                 ')',
             ])
             dflow_input_parameters[f.name] = dflow.InputParameter(name=f.name)
             args_dict[f.name] = f'${bash_name}'
-        elif f.type.__metadata__[0] == types.Symbol.INPUT_ARTIFACT:
+
+        elif meta == types.Symbol.INPUT_ARTIFACT or isinstance(meta, dflow.InputArtifact):
             bash_name = f'_DF_INPUT_ARTIFACT_{f.name}_'
             path = os.path.join(input_artifacts_dir, f.name)
             source.append(f'{bash_name}={shlex.quote(path)}')
-            dflow_input_artifacts[f.name] = dflow.InputArtifact(path=path)
+            artifact = meta
+            if not isinstance(artifact, dflow.InputArtifact):
+                artifact = dflow.InputArtifact(path=path, archive=default_archive)  # type: ignore
+            dflow_input_artifacts[f.name] = artifact
             args_dict[f.name] = f'${bash_name}'
-        elif f.type.__metadata__[0] == types.Symbol.OUTPUT_ARTIFACT:
+
+        elif meta == types.Symbol.OUTPUT_ARTIFACT or isinstance(meta, dflow.OutputArtifact):
             bash_name = f'_DF_OUTPUT_ARTIFACT_{f.name}_'
             path = os.path.join(output_artifacts_dir, f.name)
             source.append(f'{bash_name}={shlex.quote(path)}')
-            dflow_output_artifacts[f.name] = dflow.OutputArtifact(path=path)  # type: ignore
+            artifact = meta
+            if not isinstance(artifact, dflow.OutputArtifact):
+                artifact = dflow.OutputArtifact(path=path, archive=default_archive)  # type: ignore
+            dflow_output_artifacts[f.name] = artifact
+
             args_dict[f.name] = f'${bash_name}'
+        else:
+            raise ValueError(f'unsupported type {f.type}')
 
     bash_script = py_fn(ObjProxy(args_dict))
     if isinstance(bash_script, list):
         bash_script = '\n'.join(bash_script)
     assert isinstance(bash_script, str), f'{py_fn} should return a string or a list of string'
 
     source.extend([
@@ -197,14 +210,15 @@
                                              ])
 
 
 def python_build_template(py_fn: Callable,
                           base_dir: str,
                           setup_script: str = '',
                           python_cmd: str = 'python3',
+                          default_archive: Optional[str] = 'default',
                           eof: str = '__EOF__') -> _PythonTemplate:
     """
     build python template from a python function
     """
     sig = inspect.signature(py_fn)
     assert len(sig.parameters) == 1, f'{py_fn} should have only one parameter'
     args_type = sig.parameters[next(iter(sig.parameters))].annotation
@@ -243,30 +257,37 @@
         'os.makedirs(pkg_dir, exist_ok=True)',
         'os.makedirs(output_parameters_dir, exist_ok=True)',
         'os.makedirs(output_artifacts_dir, exist_ok=True)',
         'args = dict()',
     ]
 
     for f, v in iter_python_step_args(args_type):
-        if f.type.__metadata__[0] == types.Symbol.INPUT_PARAMETER:
+        meta = f.type.__metadata__[0]
+        if meta == types.Symbol.INPUT_PARAMETER:
             # FIXME: may have error in some corner cases
             if _is_str_type(f.type.__origin__):
                 val = f'"""{{{{inputs.parameters.{f.name}}}}}"""'
             else:
                 val = f'json.loads("""{{{{inputs.parameters.{f.name}}}}}""")'
             dflow_input_parameters[f.name] = dflow.InputParameter(name=f.name)
             source.append(f'args[{repr(f.name)}] = {val}')
-        elif f.type.__metadata__[0] == types.Symbol.INPUT_ARTIFACT:
+        elif meta == types.Symbol.INPUT_ARTIFACT or isinstance(meta, dflow.InputArtifact):
             path = os.path.join(input_artifacts_dir, f.name)
-            dflow_input_artifacts[f.name] = dflow.InputArtifact(path=path)
             source.append(f'args[{repr(f.name)}] = {repr(path)}')
-        elif f.type.__metadata__[0] == types.Symbol.OUTPUT_ARTIFACT:
+            artifact = meta
+            if not isinstance(artifact, dflow.InputArtifact):
+                artifact = dflow.InputArtifact(path=path, archive=default_archive)  # type: ignore
+            dflow_input_artifacts[f.name] = artifact
+        elif meta == types.Symbol.OUTPUT_ARTIFACT or isinstance(meta, dflow.OutputArtifact):
             path = os.path.join(output_artifacts_dir, f.name)
-            dflow_output_artifacts[f.name] = dflow.OutputArtifact(path=path)  # type: ignore
             source.append(f'args[{repr(f.name)}] = {repr(path)}')
+            artifact = meta
+            if not isinstance(artifact, dflow.OutputArtifact):
+                artifact = dflow.OutputArtifact(path=path, archive=default_archive)  # type: ignore
+            dflow_output_artifacts[f.name] = artifact
 
     source.extend([
         '',
         '# dump args to file',
         'with open(args_file, "w") as fp:',
         '    json.dump(args, fp, indent=2)',
         '',
@@ -336,65 +357,96 @@
     """
     A type friendly wrapper to build a DFlow workflow.
     """
 
     def __init__(self, name:str, s3_prefix: str,
                  default_executor: Optional[DispatcherExecutor] = None,
                  default_setup_script: str = '',
+                 default_archive: Optional[str] = 'default',
                  debug=False,
                  container_base_dir: str = '/tmp/dflow-builder',
+                 allow_abs_s3_url=False,
                  s3_debug_fn = _s3_copy_fn):
         """
         :param name: The name of the workflow.
         :param s3_prefix: The base prefix of the S3 bucket to store data generated by the workflow.
+        :param default_archive: The default archive method to use for Input/Output artifacts.
         :param default_executor: The default executor to run the workflow.
         :param default_setup_script: The default bash script to run at the beginning of each step.
         :param debug: If True, the workflow will be run in debug mode.
         :param local_mode: If True, the workflow will be run in local mode.
         :param container_base_dir: The base directory to mapping resources in remote container.
+        :param allow_abs_s3_url: If True, allow absolute s3 url in input artifacts
         :param s3_debug_fn: The function to upload file to S3 under debug mode.
         """
         if debug:
             dflow.config['mode'] = 'debug'
             # dflow.config['debug_copy_method'] =  'copy'
             s3_prefix = s3_prefix.lstrip('/')
 
         assert container_base_dir.startswith('/tmp'), 'dflow: container_base_dir must start with /tmp'
 
         self.name: Final[str] = name
         self.workflow: Final[dflow.Workflow] = dflow.Workflow(name=name)
         self.s3_base_prefix: Final[str] = s3_prefix
         self.container_base_dir: Final[str] = container_base_dir
 
+        self._default_archive = default_archive
         self._default_executor = default_executor
         self._default_setup_script = default_setup_script
         self._python_fns: Dict[Callable, str] = {}
         self._python_pkgs: Dict[str, str] = {}
         self._bash_scripts: Dict[Callable, str] = {}
         self._s3_cache: Dict[str, str] = {}
         self._s3_debug_fn = s3_debug_fn
+        self._allow_abs_s3_url = allow_abs_s3_url
         self._debug = debug
 
     def s3_prefix(self, key: str):
-        return os.path.join(self.s3_base_prefix, key).strip('/ ')
+        """
+        get the full s3 prefix of a key.
+        """
+        base_prefix = self.s3_base_prefix
+        # context prefix is inject by bohrium platform
+        # to isolate namespace of different job
+        context_prefix = dflow.s3_config.get('prefix')
+        if context_prefix and not self._debug:
+            base_prefix = os.path.join(context_prefix, base_prefix).strip('/ ')
+
+        return os.path.join(base_prefix, key).strip('/ ')
+
+    def s3_download(self, key: str, path: str = '.',
+                    recursive: bool = True,
+                    skip_exists: bool = False,
+                    keep_dir: bool = False,
+                    ):
+        """
+        Download file from S3 to local.
+        """
+        if self._debug:
+            return
+        dflow.download_s3(self.s3_prefix(key), path,  # type: ignore
+                          recursive=recursive, skip_exists=skip_exists, keep_dir=keep_dir,
+                          debug_func=self._s3_debug_fn)
 
     def s3_upload(self, path: Union[os.PathLike, str], key: str, cache: bool = False) -> str:
         """
         upload local file to S3.
 
         :param path: The local file path.
         :param keys: The keys of the S3 object.
         """
-        if isinstance(path, str):
-            path = Path(path)
+        if not isinstance(path, str):
+            path = str(path)
 
         prefix = self.s3_prefix(key)
         if cache and prefix in self._s3_cache:
             return self._s3_cache[prefix]
-        self._s3_cache[prefix] = dflow.upload_s3(path, prefix, debug_func=self._s3_debug_fn)
+        # FIXME: the type of dflow.upload_s3 is not correct
+        self._s3_cache[prefix] = dflow.upload_s3(path, prefix, debug_func=self._s3_debug_fn)  # type: ignore
         return self._s3_cache[prefix]
 
     def s3_dump(self, data: Union[bytes, str], key: str) -> str:
         """
         Dump data to s3.
 
         :param data: The bytes to upload.
@@ -415,21 +467,23 @@
     def add_steps(self, steps: Steps):
         """
         Add a list of steps to the workflow. The steps will be executed in parallel.
         """
         df_steps = _to_dflow_steps(steps)
         self.workflow.add(df_steps)
 
-    def run(self):
+    def run(self, raise_on_failed=True):
         """
         Run the workflow.
         """
         self.workflow.submit()
         try:
             self.workflow.wait()
+            if self.workflow.query_status() != 'Succeeded' and raise_on_failed:
+                raise RuntimeError(f'workflow {self.name} failed')
         finally:
             if self._debug:
                 resolve_ln(self.s3_base_prefix, mv=True)
 
     def make_bash_step(self, fn: Callable[[T_ARGS], types.ListStr], /,
                        uid: Optional[str] = None,
                        setup_script: str = '',
@@ -488,15 +542,18 @@
                                     with_param=with_param,
                                     executor=executor)
         return wrapped_fn
 
     def _create_bash_template(self, fn: Callable, uid: str,
                               setup_script: str = '',
                               bash_cmd: str = 'bash',):
-        _template = bash_build_template(fn, base_dir=self.container_base_dir, setup_script=setup_script)
+        _template = bash_build_template(fn,
+                                        base_dir=self.container_base_dir,
+                                        setup_script=setup_script,
+                                        default_archive=self._default_archive)
         dflow_template = ScriptOPTemplate(
             name='bash-template-' + uid,
             command=bash_cmd,
             script=_template.source,
         )
         dflow_template.inputs.parameters = _template.dflow_input_parameters
         dflow_template.inputs.artifacts = _template.dflow_input_artifacts
@@ -509,15 +566,16 @@
                                 bash_cmd: str = 'bash',
                                 pkgs: Optional[Iterable[str]] = None,
                                 ):
         if pkgs is None:
             pkgs = []
         _template = python_build_template(fn, base_dir=self.container_base_dir,
                                           python_cmd=python_cmd,
-                                          setup_script=setup_script)
+                                          setup_script=setup_script,
+                                          default_archive=self._default_archive)
         fn_hash = hashlib.sha256(_template.fn_str.encode()).hexdigest()
         dflow_template = ScriptOPTemplate(
             name='py-template-' + uid,
             command=bash_cmd,
             script=_template.source,
         )
         dflow_template.inputs.parameters = _template.dflow_input_parameters
@@ -566,37 +624,43 @@
 
     def _ensure_artifact(self, url_or_obj: DFLOW_ARTIFACT) -> DFLOW_ARTIFACT:
         if not isinstance(url_or_obj, str):
             return url_or_obj
         parsed = urlparse(url_or_obj)
         if parsed.scheme == 's3':
             key = parsed.path.lstrip('/')
-            assert parsed.netloc in ('', '.')
+            assert parsed.netloc in ('', '.'), f'unsupported s3 url {url_or_obj}'
             if '.' == parsed.netloc:
-                key = os.path.join(self.s3_base_prefix, key)
+                key = self.s3_prefix(key)
+            elif not self._allow_abs_s3_url:
+                raise ValueError(f'absolute s3 url {url_or_obj} is not allowed, use relative path instead, or set allow_abs_s3_url=True')
             if self._debug:
                 key = os.path.abspath(key)
             return dflow.S3Artifact(key=key)
         raise ValueError(f'unsupported url {url_or_obj}')
 
     def _build_step(self, name: str, args: T_ARGS, template,
                     with_param: Any=None,
                     executor: Optional[DispatcherExecutor] = None):
         if executor is None:
             executor = self._default_executor
 
         parameters = {}
         artifacts = {}
         for f, v in iter_python_step_args(args):
-            if f.type.__metadata__[0] == types.Symbol.INPUT_PARAMETER:
+            meta = f.type.__metadata__[0]
+            if meta == types.Symbol.INPUT_PARAMETER:
                 parameters[f.name] = v
-            elif f.type.__metadata__[0] == types.Symbol.INPUT_ARTIFACT:
+            elif meta == types.Symbol.INPUT_ARTIFACT or isinstance(meta, dflow.InputArtifact):
                 artifacts[f.name] = self._ensure_artifact(v)  # type: ignore
-            elif f.type.__metadata__[0] == types.Symbol.OUTPUT_ARTIFACT:
+            elif meta == types.Symbol.OUTPUT_ARTIFACT or isinstance(meta, dflow.OutputArtifact):
                 template.outputs.artifacts[f.name].save = [self._ensure_artifact(v)]  # type: ignore
+            else:
+                raise ValueError(f'unsupported type {f.type}')
+
         step = dflow.Step(
             name=name,
             template=template,
             with_param=with_param,
             parameters=parameters,
             artifacts=artifacts,
             executor=executor,
```

### Comparing `dflow_galaxy-0.1.2/dflow_galaxy/core/dispatcher.py` & `dflow_galaxy-0.1.4/dflow_galaxy/core/dispatcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 from .pydantic import BaseModel
 
 from typing import Optional
 from urllib.parse import urlparse
 import os
 
 
+class BohriumInputData(BaseModel):
+    image_name: str
+    job_type: str = 'container'
+    platform: str = 'ali'
+    scass_type: str = 'c2_m4_cpu'
+    job_name: str = 'bohrium_job'
+    disk_size: int = 20  # in GB
+
+
 class Resource(BaseModel):
     queue: Optional[str] = None
-    container: Optional[str] = None
+    image: Optional[str] = None
     sub_path: str = '.'
 
     nodes: int = 1
     cpu_per_node: int = 1
     gpu_per_node: int = 0
 
+    # use this for job running on bohrium
+    bohrium: Optional[BohriumInputData] = None
+
+
     def get_resource_dict(self):
         return {
             'number_node': self.nodes,
             'cpu_per_node': self.cpu_per_node,
             'gpu_per_node': self.gpu_per_node,
         }
 
 
 class BohriumConfig(BaseModel):
-    email: str
-    password: str
-    project_id: str
+    email: Optional[str] = None
+    password: Optional[str] = None
+    project_id: Optional[str] = None
 
 
 class HpcConfig(BaseModel):
     class SlurmConfig(BaseModel):
         ...
     class LsfConfig(BaseModel):
         ...
@@ -73,27 +86,41 @@
         return create_hpc_dispatcher(config.hpc, resource)
     elif config.bohrium:
         return create_bohrium_dispatcher(config.bohrium, resource)
     raise ValueError('At least one of hpc or bohrium should be provided')
 
 
 def create_bohrium_dispatcher(config: BohriumConfig, resource: Resource):
+    if resource.bohrium is None:
+        raise ValueError('Bohrium resource is required when using Bohrium dispatcher')
     from dflow.plugins.dispatcher import DispatcherExecutor
-    remote_profile = {
-        'email': config.email,
-        'password': config.password,
-        'program_id': config.project_id,
-    }
+    password = os.environ.get('BOHRIUM_PASSWORD') or config.password
+
+    # remote profile can also be config via global bohrium.config
+    remote_profile = {}
+    if config.email:
+        remote_profile['email'] = config.email
+
+    if config.project_id:
+        # I don't know which one is correct, so I set both
+        remote_profile['program_id'] = config.project_id
+        remote_profile['project_id'] = config.project_id
+    if password:
+        remote_profile['password'] = password
+
+    remote_profile['input_data'] = resource.bohrium.dict()
     machine_dict = {
         'batch_type': 'Bohrium',
         'context_type': 'Bohrium',
         'remote_profile': remote_profile,
     }
     return DispatcherExecutor(
         machine_dict=machine_dict,
+        # the following are not used in Bohrium dispatcher
+        image=resource.image,
         resources_dict= resource.get_resource_dict(),
     )
 
 
 def create_hpc_dispatcher(config: HpcConfig, resource: Resource):
     from dflow.plugins.dispatcher import DispatcherExecutor
     url = urlparse(config.url)
```

### Comparing `dflow_galaxy-0.1.2/dflow_galaxy/core/types.py` & `dflow_galaxy-0.1.4/dflow_galaxy/core/types.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.2/dflow_galaxy/core/util.py` & `dflow_galaxy-0.1.4/dflow_galaxy/core/util.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/config.py` & `dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/config.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/domain/cp2k.py` & `dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/cp2k.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,21 +73,23 @@
                 a_dict = {
                     'url': str(sys_dir / 'decent.xyz'),
                     'format': 'extxyz',
                     'attrs': deepcopy(self.systems[ancestor].attrs),
                 }
                 system_files.append(a_dict)  # type: ignore
 
-        assert limit > 0, 'limit should be greater than 0'
+        assert system_files, 'no system files found'
 
+        task_dir = os.path.join(args.work_dir, 'tasks')
+        ensure_dir(task_dir)
         task_dirs = make_cp2k_task_dirs(
             system_files=system_files,
             input_template=self.config.input_template,
             template_vars=self.config.template_vars,
-            base_dir=ensure_dir(f'{args.work_dir}/tasks'),
+            base_dir=task_dir,
             limit=limit,
             limit_method=self.config.limit_method,
             # not supported yet
             mode='default',
             wfn_warmup_template=None,
             # TODO: type_map is no longer needed, should be fixed in ai2-kit
             type_map=[],
```

### Comparing `dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/domain/deepmd.py` & `dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/deepmd.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/domain/lammps.py` & `dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/lammps.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from dflow_galaxy.core.pydantic import BaseModel
 from dflow_galaxy.core.dispatcher import BaseApp, PythonApp, create_dispatcher, ExecutorConfig
 from dflow_galaxy.core.dflow import DFlowBuilder
 from dflow_galaxy.core.util import bash_iter_ls_slice, safe_ln, bash_ln_cmd, inspect_dir, bash_inspect_dir
 from dflow_galaxy.core import types
 
-from ai2_kit.domain.lammps import make_lammps_task_dirs
+from ai2_kit.domain.lammps import make_lammps_task_dirs, FepOptions
 from ai2_kit.domain.constant import DP_FROZEN_MODEL
 from ai2_kit.core.artifact import Artifact, ArtifactDict
 from ai2_kit.core.util import cmd_with_checkpoint as cmd_cp, dump_text
 
 from dflow import argo_range
 
 
@@ -123,16 +123,16 @@
             mode='default',
             type_alias={},
             dp_modifier=None,
             dp_sel_type=None,
             preset_template='default',
             n_wise=0,
             fix_statement=None,
-            ai2_kit_cmd='python -m ai2_kit.main',
             rel_path=True,
+            fep_opts=FepOptions(),
         )
         # write ancestor to the task dirs
         for task_dir in task_dirs:
             path = os.path.join(task_dir['url'], 'ANCESTOR')
             dump_text(task_dir['attrs']['ancestor'], path)
```

### Comparing `dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/domain/lib.py` & `dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/lib.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/domain/model_devi.py` & `dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/domain/model_devi.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.2/dflow_galaxy/workflow/tesla/main.py` & `dflow_galaxy-0.1.4/dflow_galaxy/workflow/tesla/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
 
 def run_tesla(*config_files: str, s3_prefix: str, debug: bool = False, skip: bool = False, max_iters: int = 1):
     config_raw = load_yaml_files(*config_files)
     config = TeslaConfig(**config_raw)
     config.init()
 
-
-    builder = DFlowBuilder(name='tesla', s3_prefix=s3_prefix, debug=debug)
+    builder = DFlowBuilder(name='tesla', s3_prefix=s3_prefix, debug=debug,
+                           default_archive=None)
     step_switch = StepSwitch(skip)
     runtime_ctx = RuntimeContext()
 
     raw_workflow_cfg = config.workflow
     for iter_num in range(max_iters):
         workflow_cfg = WorkflowConfig(**raw_workflow_cfg)
 
@@ -157,15 +157,13 @@
             if iter_num == workflow_cfg.update.until_iter:
                 logger.info('Updating workflow config at iter %d', iter_num)
                 # the patch is applied to the original config, not the updated one
                 raw_workflow_cfg = deepcopy(config.workflow)
                 raw_workflow_cfg['workflow']['update'] = None  # clean the old update config
                 raw_workflow_cfg = merge_dict(raw_workflow_cfg, workflow_cfg.update.patch)
 
-
     builder.run()
 
 
-
 cmd_entry = CmdGroup({
     'run': run_tesla,
 }, doc='TESLA workflow')
```

