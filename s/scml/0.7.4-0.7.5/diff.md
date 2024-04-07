# Comparing `tmp/scml-0.7.4.tar.gz` & `tmp/scml-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scml-0.7.4.tar", last modified: Wed Apr  3 06:18:11 2024, max compression
+gzip compressed data, was "scml-0.7.5.tar", last modified: Sun Apr  7 04:19:54 2024, max compression
```

## Comparing `scml-0.7.4.tar` & `scml-0.7.5.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.810520 scml-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-03 06:18:02.000000 scml-0.7.4/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-03 06:18:02.000000 scml-0.7.4/.cookiecutterrc
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-03 06:18:02.000000 scml-0.7.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-03 06:18:02.000000 scml-0.7.4/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-03 06:18:02.000000 scml-0.7.4/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 06:18:02.000000 scml-0.7.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19223 2024-04-03 06:18:02.000000 scml-0.7.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-03 06:18:02.000000 scml-0.7.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-03 06:18:02.000000 scml-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-03 06:18:02.000000 scml-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21741 2024-04-03 06:18:11.810520 scml-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-03 06:18:02.000000 scml-0.7.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-03 06:18:11.810520 scml-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-03 06:18:02.000000 scml-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.778519 scml-0.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.786519 scml-0.7.4/src/scml/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   132032 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    69113 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/cliadv.py
--rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12599 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.786519 scml-0.7.4/src/scml/oneshot/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    21685 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.790519 scml-0.7.4/src/scml/oneshot/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/agents/aspiration.py
--rw-r--r--   0 runner    (1001) docker     (127)    15070 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/agents/greedy.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/agents/nothing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/agents/rand.py
--rw-r--r--   0 runner    (1001) docker     (127)    40941 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/awi.py
--rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    84620 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.790519 scml-0.7.4/src/scml/oneshot/rl/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/env.py
--rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/rl/reward.py
--rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/sysagents.py
--rw-r--r--   0 runner    (1001) docker     (127)    47513 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/ufun.py
--rw-r--r--   0 runner    (1001) docker     (127)   127475 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/oneshot/world.py
--rw-r--r--   0 runner    (1001) docker     (127)    26784 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.794520 scml-0.7.4/src/scml/scml2019/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6793 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14656 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20378 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/awi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11734 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/bank.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    57559 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23625 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/consumers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.794520 scml-0.7.4/src/scml/scml2019/factory_managers/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/factory_managers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    38211 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/factory_managers/builtins.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1027 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7189 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/insurance.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8296 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/miners.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29292 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/schedulers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46519 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/simulators.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    59623 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/utils19.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2257 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/visualizers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   106736 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2019/world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.794520 scml-0.7.4/src/scml/scml2020/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25851 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.798519 scml-0.7.4/src/scml/scml2020/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/bcse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/decentralizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/do_nothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/indneg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/moving.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/reactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/agents/satisficer.py
--rw-r--r--   0 runner    (1001) docker     (127)    29681 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/awi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.798519 scml-0.7.4/src/scml/scml2020/components/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32704 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/components/negotiation.py
--rw-r--r--   0 runner    (1001) docker     (127)    20521 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/components/prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)    13477 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/components/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/components/signing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/components/trading.py
--rw-r--r--   0 runner    (1001) docker     (127)    21804 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.798519 scml-0.7.4/src/scml/scml2020/services/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/services/controllers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27113 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/services/simulators.py
--rw-r--r--   0 runner    (1001) docker     (127)   133308 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/scml2020/world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.798519 scml-0.7.4/src/scml/std/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.802520 scml-0.7.4/src/scml/std/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/agents/aspiration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/agents/greedy.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/agents/nothing.py
--rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/agents/rand.py
--rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/awi.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.802520 scml-0.7.4/src/scml/std/rl/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/action.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/rl/reward.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/sysagents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/ufun.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/std/world.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   148769 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.802520 scml-0.7.4/src/scml/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.802520 scml-0.7.4/src/scml/vendor/quick/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/vendor/quick/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/vendor/quick/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/vendor/quick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29361 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/vendor/quick/quick.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 06:18:02.000000 scml-0.7.4/src/scml/vendor/quick/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.810520 scml-0.7.4/src/scml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21741 2024-04-03 06:18:11.000000 scml-0.7.4/src/scml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-03 06:18:11.000000 scml-0.7.4/src/scml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:18:11.000000 scml-0.7.4/src/scml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 06:18:11.000000 scml-0.7.4/src/scml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:18:11.000000 scml-0.7.4/src/scml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 06:18:11.000000 scml-0.7.4/src/scml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 06:18:11.000000 scml-0.7.4/src/scml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.802520 scml-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.802520 scml-0.7.4/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.806520 scml-0.7.4/tests/etc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/etc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-04-03 06:18:02.000000 scml-0.7.4/tests/etc/test_can_run_tutorial2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-03 06:18:02.000000 scml-0.7.4/tests/etc/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 06:18:02.000000 scml-0.7.4/tests/etc/test_jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.806520 scml-0.7.4/tests/old/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/old/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17345 2024-04-03 06:18:02.000000 scml-0.7.4/tests/old/test_factory2019.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20339 2024-04-03 06:18:02.000000 scml-0.7.4/tests/old/test_scheduler2019.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      553 2024-04-03 06:18:02.000000 scml-0.7.4/tests/old/test_scml2019.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12090 2024-04-03 06:18:02.000000 scml-0.7.4/tests/old/test_scml2019factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2606 2024-04-03 06:18:02.000000 scml-0.7.4/tests/old/test_scml2019tournaments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.806520 scml-0.7.4/tests/oneshot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_oneshot_do_nothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_oneshot_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    12865 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_oneshot_ufun.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    34929 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_scml2021oneshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_scml2023oneshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_scml2024oneshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-04-03 06:18:02.000000 scml-0.7.4/tests/oneshot/test_sync_jackson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.806520 scml-0.7.4/tests/rl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-03 06:18:02.000000 scml-0.7.4/tests/rl/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29750 2024-04-03 06:18:02.000000 scml-0.7.4/tests/rl/test_rl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.806520 scml-0.7.4/tests/std/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std/test_std.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:11.810520 scml-0.7.4/tests/std2020design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std2020design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std2020design/test_scml2020.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std2020design/test_scml2020factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3960 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std2020design/test_scml2020tournaments.py
--rw-r--r--   0 runner    (1001) docker     (127)    19570 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std2020design/test_scml2021.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8392 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std2020design/test_scml2021tournaments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-03 06:18:02.000000 scml-0.7.4/tests/std2020design/test_scml2023.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-03 06:18:02.000000 scml-0.7.4/tests/switches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-03 06:18:02.000000 scml-0.7.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.728901 scml-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-07 04:19:45.000000 scml-0.7.5/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-07 04:19:45.000000 scml-0.7.5/.cookiecutterrc
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-07 04:19:45.000000 scml-0.7.5/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-07 04:19:45.000000 scml-0.7.5/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-07 04:19:45.000000 scml-0.7.5/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-07 04:19:45.000000 scml-0.7.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-04-07 04:19:45.000000 scml-0.7.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-07 04:19:45.000000 scml-0.7.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-07 04:19:45.000000 scml-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-07 04:19:45.000000 scml-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21974 2024-04-07 04:19:54.728901 scml-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-07 04:19:45.000000 scml-0.7.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-07 04:19:54.728901 scml-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-07 04:19:46.000000 scml-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.692901 scml-0.7.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.700901 scml-0.7.5/src/scml/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   132276 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69113 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/cliadv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12599 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.704901 scml-0.7.5/src/scml/oneshot/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21685 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.704901 scml-0.7.5/src/scml/oneshot/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/agents/aspiration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15146 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/agents/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/agents/nothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/agents/rand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40941 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/awi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84620 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.704901 scml-0.7.5/src/scml/oneshot/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/rl/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/rl/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/rl/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/rl/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/rl/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/rl/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/rl/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/rl/reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/sysagents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47513 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/ufun.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127475 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/oneshot/world.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26784 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.708901 scml-0.7.5/src/scml/scml2019/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6793 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14656 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20378 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/awi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11734 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/bank.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57559 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23625 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/consumers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.708901 scml-0.7.5/src/scml/scml2019/factory_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/factory_managers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38211 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/factory_managers/builtins.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1027 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7189 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/insurance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8296 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/miners.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29292 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/schedulers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46519 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/simulators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    59623 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/utils19.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2257 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/visualizers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   106736 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2019/world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.712901 scml-0.7.5/src/scml/scml2020/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25851 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.712901 scml-0.7.5/src/scml/scml2020/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/agents/bcse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/agents/decentralizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/agents/do_nothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/agents/indneg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/agents/moving.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/agents/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/agents/reactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/agents/satisficer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29681 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/awi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.712901 scml-0.7.5/src/scml/scml2020/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32704 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/components/negotiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20521 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/components/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13477 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/components/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/components/signing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/components/trading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21804 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.712901 scml-0.7.5/src/scml/scml2020/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/services/controllers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27113 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/services/simulators.py
+-rw-r--r--   0 runner    (1001) docker     (127)   133308 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/scml2020/world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.716901 scml-0.7.5/src/scml/std/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.716901 scml-0.7.5/src/scml/std/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/agents/aspiration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/agents/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/agents/nothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/agents/rand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/awi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.716901 scml-0.7.5/src/scml/std/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/rl/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/rl/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/rl/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/rl/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/rl/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/rl/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/rl/reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/sysagents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/ufun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/std/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   148861 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.716901 scml-0.7.5/src/scml/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.720901 scml-0.7.5/src/scml/vendor/quick/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/vendor/quick/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/vendor/quick/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/vendor/quick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29361 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/vendor/quick/quick.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-07 04:19:46.000000 scml-0.7.5/src/scml/vendor/quick/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.724901 scml-0.7.5/src/scml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21974 2024-04-07 04:19:54.000000 scml-0.7.5/src/scml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-07 04:19:54.000000 scml-0.7.5/src/scml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 04:19:54.000000 scml-0.7.5/src/scml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-07 04:19:54.000000 scml-0.7.5/src/scml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 04:19:54.000000 scml-0.7.5/src/scml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-07 04:19:54.000000 scml-0.7.5/src/scml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 04:19:54.000000 scml-0.7.5/src/scml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.720901 scml-0.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:46.000000 scml-0.7.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.720901 scml-0.7.5/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:46.000000 scml-0.7.5/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.720901 scml-0.7.5/tests/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:46.000000 scml-0.7.5/tests/etc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-04-07 04:19:46.000000 scml-0.7.5/tests/etc/test_can_run_tutorial2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-07 04:19:46.000000 scml-0.7.5/tests/etc/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-07 04:19:46.000000 scml-0.7.5/tests/etc/test_jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.720901 scml-0.7.5/tests/old/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:46.000000 scml-0.7.5/tests/old/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17345 2024-04-07 04:19:46.000000 scml-0.7.5/tests/old/test_factory2019.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20339 2024-04-07 04:19:46.000000 scml-0.7.5/tests/old/test_scheduler2019.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      553 2024-04-07 04:19:46.000000 scml-0.7.5/tests/old/test_scml2019.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12090 2024-04-07 04:19:46.000000 scml-0.7.5/tests/old/test_scml2019factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2606 2024-04-07 04:19:46.000000 scml-0.7.5/tests/old/test_scml2019tournaments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.724901 scml-0.7.5/tests/oneshot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:46.000000 scml-0.7.5/tests/oneshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-07 04:19:46.000000 scml-0.7.5/tests/oneshot/test_oneshot_do_nothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-07 04:19:46.000000 scml-0.7.5/tests/oneshot/test_oneshot_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12865 2024-04-07 04:19:46.000000 scml-0.7.5/tests/oneshot/test_oneshot_ufun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-07 04:19:46.000000 scml-0.7.5/tests/oneshot/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34929 2024-04-07 04:19:46.000000 scml-0.7.5/tests/oneshot/test_scml2021oneshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-07 04:19:46.000000 scml-0.7.5/tests/oneshot/test_scml2023oneshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-04-07 04:19:46.000000 scml-0.7.5/tests/oneshot/test_scml2024oneshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-04-07 04:19:46.000000 scml-0.7.5/tests/oneshot/test_sync_jackson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.724901 scml-0.7.5/tests/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:46.000000 scml-0.7.5/tests/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-07 04:19:46.000000 scml-0.7.5/tests/rl/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29750 2024-04-07 04:19:46.000000 scml-0.7.5/tests/rl/test_rl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.724901 scml-0.7.5/tests/std/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:46.000000 scml-0.7.5/tests/std/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-04-07 04:19:46.000000 scml-0.7.5/tests/std/test_std.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:54.724901 scml-0.7.5/tests/std2020design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:19:46.000000 scml-0.7.5/tests/std2020design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-07 04:19:46.000000 scml-0.7.5/tests/std2020design/test_scml2020.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-07 04:19:46.000000 scml-0.7.5/tests/std2020design/test_scml2020factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3960 2024-04-07 04:19:46.000000 scml-0.7.5/tests/std2020design/test_scml2020tournaments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19570 2024-04-07 04:19:46.000000 scml-0.7.5/tests/std2020design/test_scml2021.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8392 2024-04-07 04:19:46.000000 scml-0.7.5/tests/std2020design/test_scml2021tournaments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-07 04:19:46.000000 scml-0.7.5/tests/std2020design/test_scml2023.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-07 04:19:46.000000 scml-0.7.5/tests/switches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-07 04:19:46.000000 scml-0.7.5/tox.ini
```

### Comparing `scml-0.7.4/.cookiecutterrc` & `scml-0.7.5/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/.travis.yml` & `scml-0.7.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/CHANGELOG.rst` & `scml-0.7.5/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+0.7.5 (2024.04.07)
+------------------
+
+* bugfix in greedy (when needs cannot be found)
+* requiring latest negams (0.10.23) to improve tournament timeout
+* Adding a 30min simulation timeout while keeping the 2min negotiation timeout
+
 0.7.4 (2024.04.03)
 ------------------
 
 * AWI: Correcting n_competitors and adding my_competitors
 * slightly faster random oneshot
 * bugfix in builtin_std_agents
 * Adding more contexts
```

### Comparing `scml-0.7.4/CONTRIBUTING.rst` & `scml-0.7.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/LICENSE` & `scml-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/MANIFEST.in` & `scml-0.7.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/PKG-INFO` & `scml-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scml
-Version: 0.7.4
+Version: 0.7.5
 Summary: ANAC Supply Chain Management League Platform
 Home-page: https://github.com/yasserfarouk/scml
 Author: Yasser Mohammad
 Author-email: yasserfarouk@gmail.com
 Project-URL: Documentation, https://scml.readthedocs.io/
 Project-URL: Changelog, https://scml.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/yasserfarouk/scml/issues
@@ -23,15 +23,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: click
 Requires-Dist: pytest
 Requires-Dist: hypothesis
-Requires-Dist: negmas>=0.10.20
+Requires-Dist: negmas>=0.10.23
 Requires-Dist: joblib
 Requires-Dist: jupyter
 Requires-Dist: gif
 Requires-Dist: gymnasium
 Provides-Extra: gui
 Requires-Dist: pyqt5; extra == "gui"
 
@@ -97,14 +97,21 @@
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
 
 Changelog
 =========
 
+0.7.5 (2024.04.07)
+------------------
+
+* bugfix in greedy (when needs cannot be found)
+* requiring latest negams (0.10.23) to improve tournament timeout
+* Adding a 30min simulation timeout while keeping the 2min negotiation timeout
+
 0.7.4 (2024.04.03)
 ------------------
 
 * AWI: Correcting n_competitors and adding my_competitors
 * slightly faster random oneshot
 * bugfix in builtin_std_agents
 * Adding more contexts
```

### Comparing `scml-0.7.4/README.rst` & `scml-0.7.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/scml
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/scml.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/scml
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/yasserfarouk/scml/v0.7.4.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/yasserfarouk/scml/v0.7.5.svg
     :alt: Commits since latest release
-    :target: https://github.com/yasserfarouk/scml/compare/v0.7.4...master
+    :target: https://github.com/yasserfarouk/scml/compare/v0.7.5...master
 
 .. |CI| image:: https://github.com/yasserfarouk/scml/workflows/CI/badge.svg
     :target: https://www.github.com/yasserfarouk/scml
     :alt: Build Status
 
 .. |PyPiPublished| image:: https://github.com/yasserfarouk/scml/workflows/PyPI/badge.svg
     :target: https://pypi.python.org/pypi/scml
```

### Comparing `scml-0.7.4/setup.cfg` & `scml-0.7.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/setup.py` & `scml-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="scml",
-    version="0.7.4",
+    version="0.7.5",
     description="ANAC Supply Chain Management League Platform",
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
@@ -59,15 +59,15 @@
         # eg: 'keyword1', 'keyword2', 'keyword3',
     ],
     python_requires=">=3.10",
     install_requires=[
         "click",
         "pytest",
         "hypothesis",
-        "negmas>=0.10.20",
+        "negmas>=0.10.23",
         "joblib",
         "jupyter",
         "gif",
         "gymnasium",
         # "python-constraint",
         # "prettytable",
         # "pulp",
```

### Comparing `scml-0.7.4/src/scml/cli.py` & `scml-0.7.5/src/scml/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python
 """The SCML universal command line tool"""
+
 import math
 import os
 import sys
 import traceback
 from collections import defaultdict
 from functools import partial
 from pathlib import Path
@@ -3373,14 +3374,20 @@
     help="The config to use. It can be std, or oneshot",
 )
 @click.option(
     "--timeout",
     "-t",
     default=-1,
     type=int,
+    help="Timeout for every world simulation (0 for infinite)",
+)
+@click.option(
+    "--total-timeout",
+    default=-1,
+    type=int,
     help="Timeout the whole tournament after the given number of seconds (0 for infinite)",
 )
 @click.option(
     "--configs",
     default=5,
     type=int,
     help="Number of unique configurations to generate.",
@@ -3472,14 +3479,15 @@
     help="A file to save the final results to",
 )
 @click_config_file.configuration_option()
 def tournament2024(
     name,
     steps,
     timeout,
+    total_timeout,
     ttype,
     log,
     verbosity,
     runs,
     configs,
     max_runs,
     competitors,
@@ -3510,14 +3518,16 @@
             kwargs.update(load(wc))
     log = _path(log)
     if len(path) > 0:
         sys.path.append(path)
     warning_n_runs = 2000
     if timeout <= 0:
         timeout = None
+    if total_timeout <= 0:
+        total_timeout = None
     if name == "random":
         name = unique_name(base="", rand_digits=0)
     if max_runs <= 0:
         max_runs = None
     if compact:
         log_ufuns = False
 
@@ -3622,15 +3632,16 @@
         non_competitor_params=non_competitor_params,
         agent_names_reveal_type=reveal_names,
         n_competitors_per_world=cw,
         n_configs=configs,
         n_runs_per_world=runs,
         max_worlds_per_config=worlds_per_config,
         tournament_path=log,
-        total_timeout=timeout,
+        total_timeout=total_timeout,
+        time_limit=timeout,
         name=name,
         verbose=verbosity > 0,
         compact=compact,
         n_steps=steps,
         parallelism=parallelism,
         world_progress_callback=prog_callback,
         log_ufuns=log_ufuns,
```

### Comparing `scml-0.7.4/src/scml/cliadv.py` & `scml-0.7.5/src/scml/cliadv.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/common.py` & `scml-0.7.5/src/scml/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/experiment.py` & `scml-0.7.5/src/scml/experiment.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/__init__.py` & `scml-0.7.5/src/scml/oneshot/__init__.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/adapter.py` & `scml-0.7.5/src/scml/oneshot/adapter.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/agent.py` & `scml-0.7.5/src/scml/oneshot/agent.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/agents/aspiration.py` & `scml-0.7.5/src/scml/oneshot/agents/aspiration.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/agents/greedy.py` & `scml-0.7.5/src/scml/oneshot/agents/greedy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import itertools
 import random
+import math
 from collections import defaultdict
 
 from negmas import Outcome, ResponseType, SAOResponse
 
 from scml.oneshot.agent import (
     OneShotAgent,
     OneShotSingleAgreementAgent,
@@ -151,15 +152,16 @@
         else:
             self._best_buying = min(up, self._best_buying)
             partner = nmi.annotation["seller"]
             self._best_opp_buying[partner] = self._best_buying
         return response
 
     def best_offer(self, negotiator_id):
-        my_needs = int(self._needed(negotiator_id))
+        _need = self._needed(negotiator_id)
+        my_needs = int(_need) if _need and not math.isinf(_need) else 0
         if my_needs <= 0:
             return None
         nmi = self.get_nmi(negotiator_id)
         if not nmi:
             return None
         quantity_issue = nmi.issues[QUANTITY]
         unit_price_issue = nmi.issues[UNIT_PRICE]
```

### Comparing `scml-0.7.4/src/scml/oneshot/agents/nothing.py` & `scml-0.7.5/src/scml/oneshot/agents/nothing.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/agents/rand.py` & `scml-0.7.5/src/scml/oneshot/agents/rand.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/awi.py` & `scml-0.7.5/src/scml/oneshot/awi.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/common.py` & `scml-0.7.5/src/scml/oneshot/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/context.py` & `scml-0.7.5/src/scml/oneshot/context.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/helper.py` & `scml-0.7.5/src/scml/oneshot/helper.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/mixins.py` & `scml-0.7.5/src/scml/oneshot/mixins.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/policy.py` & `scml-0.7.5/src/scml/oneshot/policy.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/rl/action.py` & `scml-0.7.5/src/scml/oneshot/rl/action.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/rl/agent.py` & `scml-0.7.5/src/scml/oneshot/rl/agent.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/rl/common.py` & `scml-0.7.5/src/scml/oneshot/rl/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/rl/env.py` & `scml-0.7.5/src/scml/oneshot/rl/env.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/rl/helpers.py` & `scml-0.7.5/src/scml/oneshot/rl/helpers.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/rl/observation.py` & `scml-0.7.5/src/scml/oneshot/rl/observation.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/rl/policies.py` & `scml-0.7.5/src/scml/oneshot/rl/policies.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/rl/reward.py` & `scml-0.7.5/src/scml/oneshot/rl/reward.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/sysagents.py` & `scml-0.7.5/src/scml/oneshot/sysagents.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/ufun.py` & `scml-0.7.5/src/scml/oneshot/ufun.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/oneshot/world.py` & `scml-0.7.5/src/scml/oneshot/world.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/runner.py` & `scml-0.7.5/src/scml/runner.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/__init__.py` & `scml-0.7.5/src/scml/scml2019/__init__.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/agent.py` & `scml-0.7.5/src/scml/scml2019/agent.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/awi.py` & `scml-0.7.5/src/scml/scml2019/awi.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/bank.py` & `scml-0.7.5/src/scml/scml2019/bank.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/common.py` & `scml-0.7.5/src/scml/scml2019/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/consumers.py` & `scml-0.7.5/src/scml/scml2019/consumers.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/factory_managers/builtins.py` & `scml-0.7.5/src/scml/scml2019/factory_managers/builtins.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/helpers.py` & `scml-0.7.5/src/scml/scml2019/helpers.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/insurance.py` & `scml-0.7.5/src/scml/scml2019/insurance.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/miners.py` & `scml-0.7.5/src/scml/scml2019/miners.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/schedulers.py` & `scml-0.7.5/src/scml/scml2019/schedulers.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/simulators.py` & `scml-0.7.5/src/scml/scml2019/simulators.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/utils19.py` & `scml-0.7.5/src/scml/scml2019/utils19.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/visualizers.py` & `scml-0.7.5/src/scml/scml2019/visualizers.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2019/world.py` & `scml-0.7.5/src/scml/scml2019/world.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/__init__.py` & `scml-0.7.5/src/scml/scml2020/__init__.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/agent.py` & `scml-0.7.5/src/scml/scml2020/agent.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/agents/bcse.py` & `scml-0.7.5/src/scml/scml2020/agents/bcse.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/agents/decentralizing.py` & `scml-0.7.5/src/scml/scml2020/agents/decentralizing.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/agents/do_nothing.py` & `scml-0.7.5/src/scml/scml2020/agents/do_nothing.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/agents/indneg.py` & `scml-0.7.5/src/scml/scml2020/agents/indneg.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/agents/moving.py` & `scml-0.7.5/src/scml/scml2020/agents/moving.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/agents/random.py` & `scml-0.7.5/src/scml/scml2020/agents/random.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/agents/reactive.py` & `scml-0.7.5/src/scml/scml2020/agents/reactive.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/agents/satisficer.py` & `scml-0.7.5/src/scml/scml2020/agents/satisficer.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/awi.py` & `scml-0.7.5/src/scml/scml2020/awi.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/common.py` & `scml-0.7.5/src/scml/scml2020/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/components/negotiation.py` & `scml-0.7.5/src/scml/scml2020/components/negotiation.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/components/prediction.py` & `scml-0.7.5/src/scml/scml2020/components/prediction.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/components/production.py` & `scml-0.7.5/src/scml/scml2020/components/production.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/components/signing.py` & `scml-0.7.5/src/scml/scml2020/components/signing.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/components/simulation.py` & `scml-0.7.5/src/scml/scml2020/components/simulation.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/components/trading.py` & `scml-0.7.5/src/scml/scml2020/components/trading.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/factory.py` & `scml-0.7.5/src/scml/scml2020/factory.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/services/controllers.py` & `scml-0.7.5/src/scml/scml2020/services/controllers.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/services/simulators.py` & `scml-0.7.5/src/scml/scml2020/services/simulators.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/scml2020/world.py` & `scml-0.7.5/src/scml/scml2020/world.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/std/__init__.py` & `scml-0.7.5/src/scml/std/__init__.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/std/agent.py` & `scml-0.7.5/src/scml/std/agent.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/std/agents/greedy.py` & `scml-0.7.5/src/scml/std/agents/greedy.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/std/agents/rand.py` & `scml-0.7.5/src/scml/std/agents/rand.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/std/awi.py` & `scml-0.7.5/src/scml/std/awi.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/std/common.py` & `scml-0.7.5/src/scml/std/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/std/context.py` & `scml-0.7.5/src/scml/std/context.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/std/policy.py` & `scml-0.7.5/src/scml/std/policy.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/std/rl/env.py` & `scml-0.7.5/src/scml/std/rl/env.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/std/ufun.py` & `scml-0.7.5/src/scml/std/ufun.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/std/world.py` & `scml-0.7.5/src/scml/std/world.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/utils.py` & `scml-0.7.5/src/scml/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,16 @@
     "anac2023_oneshot",
     "anac2023_std",
     "anac2023_collusion",
     "anac2024_oneshot",
     "anac2024_std",
 ]
 
+ONESHOT_TIMEOUT = 60 * 30
+ONESHOT_NEG_TIMEOUT = 120
 
 FORCED_LOGS_FRACTION = 1.0
 
 
 ROUND_ROBIN = True
 
 
@@ -353,16 +355,16 @@
         for j in range(n):
             agent_processes.append(i)
     if oneshot_world or std_world:
         world_params = dict(
             name=world_name,
             agent_types=agent_types,
             agent_params=manager_params,
-            time_limit=7200 + 3600,
-            neg_time_limit=120,
+            time_limit=ONESHOT_TIMEOUT,
+            neg_time_limit=ONESHOT_NEG_TIMEOUT,
             neg_n_steps=20,
             neg_step_time_limit=10,
             negotiation_speed=21,
             start_negotiations_immediately=False,
             agent_processes=agent_processes,
             n_processes=np,
             n_steps=n_steps,
@@ -372,16 +374,16 @@
             random_agent_types=False,
         )
     else:
         world_params = dict(
             name=world_name,
             agent_types=agent_types,
             agent_params=manager_params,
-            time_limit=7200 + 3600,
-            neg_time_limit=120,
+            time_limit=ONESHOT_TIMEOUT,
+            neg_time_limit=ONESHOT_NEG_TIMEOUT,
             neg_n_steps=20,
             neg_step_time_limit=10,
             negotiation_speed=21,
             spot_market_global_loss=0.2,
             interest_rate=0.08,
             bankruptcy_limit=1.0,
             initial_balance=None,
```

### Comparing `scml-0.7.4/src/scml/vendor/quick/LICENSE` & `scml-0.7.5/src/scml/vendor/quick/LICENSE`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/vendor/quick/README.md` & `scml-0.7.5/src/scml/vendor/quick/README.md`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml/vendor/quick/quick.py` & `scml-0.7.5/src/scml/vendor/quick/quick.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/src/scml.egg-info/PKG-INFO` & `scml-0.7.5/src/scml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scml
-Version: 0.7.4
+Version: 0.7.5
 Summary: ANAC Supply Chain Management League Platform
 Home-page: https://github.com/yasserfarouk/scml
 Author: Yasser Mohammad
 Author-email: yasserfarouk@gmail.com
 Project-URL: Documentation, https://scml.readthedocs.io/
 Project-URL: Changelog, https://scml.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/yasserfarouk/scml/issues
@@ -23,15 +23,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: click
 Requires-Dist: pytest
 Requires-Dist: hypothesis
-Requires-Dist: negmas>=0.10.20
+Requires-Dist: negmas>=0.10.23
 Requires-Dist: joblib
 Requires-Dist: jupyter
 Requires-Dist: gif
 Requires-Dist: gymnasium
 Provides-Extra: gui
 Requires-Dist: pyqt5; extra == "gui"
 
@@ -97,14 +97,21 @@
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
 
 Changelog
 =========
 
+0.7.5 (2024.04.07)
+------------------
+
+* bugfix in greedy (when needs cannot be found)
+* requiring latest negams (0.10.23) to improve tournament timeout
+* Adding a 30min simulation timeout while keeping the 2min negotiation timeout
+
 0.7.4 (2024.04.03)
 ------------------
 
 * AWI: Correcting n_competitors and adding my_competitors
 * slightly faster random oneshot
 * bugfix in builtin_std_agents
 * Adding more contexts
```

### Comparing `scml-0.7.4/src/scml.egg-info/SOURCES.txt` & `scml-0.7.5/src/scml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/etc/test_can_run_tutorial2.py` & `scml-0.7.5/tests/etc/test_can_run_tutorial2.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/etc/test_cli.py` & `scml-0.7.5/tests/etc/test_cli.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/etc/test_jupyter.py` & `scml-0.7.5/tests/etc/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/old/test_factory2019.py` & `scml-0.7.5/tests/old/test_factory2019.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/old/test_scheduler2019.py` & `scml-0.7.5/tests/old/test_scheduler2019.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/old/test_scml2019.py` & `scml-0.7.5/tests/old/test_scml2019.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/old/test_scml2019factory.py` & `scml-0.7.5/tests/old/test_scml2019factory.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/old/test_scml2019tournaments.py` & `scml-0.7.5/tests/old/test_scml2019tournaments.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/oneshot/test_oneshot_do_nothing.py` & `scml-0.7.5/tests/oneshot/test_oneshot_do_nothing.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/oneshot/test_oneshot_sync.py` & `scml-0.7.5/tests/oneshot/test_oneshot_sync.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/oneshot/test_oneshot_ufun.py` & `scml-0.7.5/tests/oneshot/test_oneshot_ufun.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/oneshot/test_runner.py` & `scml-0.7.5/tests/oneshot/test_runner.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/oneshot/test_scml2021oneshot.py` & `scml-0.7.5/tests/oneshot/test_scml2021oneshot.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/oneshot/test_scml2023oneshot.py` & `scml-0.7.5/tests/oneshot/test_scml2023oneshot.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/oneshot/test_scml2024oneshot.py` & `scml-0.7.5/tests/oneshot/test_scml2024oneshot.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/oneshot/test_sync_jackson.py` & `scml-0.7.5/tests/oneshot/test_sync_jackson.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/rl/test_context.py` & `scml-0.7.5/tests/rl/test_context.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/rl/test_rl.py` & `scml-0.7.5/tests/rl/test_rl.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/std/test_std.py` & `scml-0.7.5/tests/std/test_std.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/std2020design/test_scml2020.py` & `scml-0.7.5/tests/std2020design/test_scml2020.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/std2020design/test_scml2020factory.py` & `scml-0.7.5/tests/std2020design/test_scml2020factory.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/std2020design/test_scml2020tournaments.py` & `scml-0.7.5/tests/std2020design/test_scml2020tournaments.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/std2020design/test_scml2021.py` & `scml-0.7.5/tests/std2020design/test_scml2021.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/std2020design/test_scml2021tournaments.py` & `scml-0.7.5/tests/std2020design/test_scml2021tournaments.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/std2020design/test_scml2023.py` & `scml-0.7.5/tests/std2020design/test_scml2023.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tests/switches.py` & `scml-0.7.5/tests/switches.py`

 * *Files identical despite different names*

### Comparing `scml-0.7.4/tox.ini` & `scml-0.7.5/tox.ini`

 * *Files identical despite different names*

