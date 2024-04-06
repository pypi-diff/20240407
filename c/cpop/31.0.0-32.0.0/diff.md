# Comparing `tmp/cpop-31.0.0.tar.gz` & `tmp/cpop-32.0.0.tar.gz`

## Comparing `cpop-31.0.0.tar` & `cpop-32.0.0.tar`

### file list

```diff
@@ -1,179 +1,177 @@
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 cpop-31.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 cpop-31.0.0/src/cpop/contract.pyx
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-31.0.0/src/cpop/data.pyx
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-31.0.0/src/hub/__init__.py
--rwxr-xr-x   0        0        0     5679 2020-02-02 00:00:00.000000 cpop-31.0.0/src/hub/__main__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/config.yaml
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/dirs.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/exc.py
--rw-r--r--   0        0        0    24866 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/hub.py
--rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/loader.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/ref.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/scanner.py
--rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/verify.py
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/log/async.py
--rw-r--r--   0        0        0     7547 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/mods/config.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/mods/contract.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/mods/dyne.py
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/mods/sub.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/mods/task.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-31.0.0/src/pop/mods/test.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/conftest.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/alias/init.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/cmods/ctest.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/cmods/contracts/ctest.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/contracts/ctx.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/contracts/ctx_args.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/contracts/ctx_update.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/contracts/many.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/contracts/priv.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/contracts/test.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/contracts/testing.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/coro/test.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/coro/contracts/test.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/csigs/sigs.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/csigs/contracts/sigs.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/external_module/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/func/__init__.py
--rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/func/test_basic.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/func/test_bench.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/func/test_cli.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/func/test_contract_ctx.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/func/test_coro.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/func/test_fail.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/func/test_no_raise_on_pre_failure.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/func/test_raise_on_pre_failure.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/func/test_serial.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/func/test_sub.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/contract_ordering/single_module/thing.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/contract_ordering/single_module/contracts/default.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/contract_ordering/single_module/contracts/dunder.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/contract_ordering/single_module/contracts/init.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/contract_ordering/single_module/contracts/thing.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/contracted/test_contracted_access.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/contracted/mods/contracted_access.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/contracted/mods/contracts/contracted_access.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/recursive_contract/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/recursive_contract/test_sub.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/bad.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/falias_dict.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/falias_func.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/falias_wrap.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/foo.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/fork.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/many.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/priv.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/proc.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/test.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/testing.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/vbad.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/virt.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/vtrue.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/alias_bad/init.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/alias_clash/init.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/bad_import/bad_import.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/contract_ctx/ctx.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/contract_ctx/ctx_args.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/contract_ctx/ctx_update.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/contract_sig/fail_sigs.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/contract_sig/pass_sigs.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/contract_sig/contracts/init.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/coro/coro.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/iter/bar.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/iter/foo.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/iter/init.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/nest/basic.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/same_vname/will_load.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/same_vname/will_not_load.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/subinit/init.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/mods/subinit/subinit.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/regression/contract_masking/test_contract_masking.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/regression/contract_masking/test_duplicate_contracts.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/regression/contract_masking/contract1/init.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/regression/contract_masking/contract2/init.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/regression/contract_masking/sub/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/sdirs/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/sdirs/l11/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/sdirs/l11/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/sdirs/l12/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/sdirs/l12/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/sdirs/l13/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/sdirs/l13/l2/test.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/README.rst
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/ca/config.yaml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/ca/contract_alias/init.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/cn/config.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/cn/contract/test.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/cn/contract/contracts/test.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/config.yaml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/init.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/clash.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/dup1.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/dup2.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/float.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/init.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/invalid.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/neg.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/neg_last.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/pos.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/pos_first.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/pos_first_tie.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/unordered_1.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/unordered_2.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/verify_fail.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/verify_pass.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/verify_raise.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/contracts/zero.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/nest/init.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/recursive_contracts/clash.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/recursive_contracts/init.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_3.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_4.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/config/config.yaml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dn1/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dn1/dn1/nest/dn1.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dn1/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dn2/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dn2/dn1/nest/dn2.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dn2/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dn3/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dn3/dn1/nest/dn3.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dn3/dn1/nest/over.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dn3/dn1/nest/next/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dn3/dn1/nest/next/last/test.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne1/config.yaml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne1/dyne1/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne1/dyne1/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne1/nest/dyne/nest.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne2/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne2/dyne2/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne2/dyne2/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne2/nest/dyne/nest.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne3/config.yaml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne3/dyne3/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne3/dyne3/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne3/nest/dyne/nest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne4/config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne4/dyne4/nest/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/dyne4/dyne4/nest/subvert.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/fork/config.yaml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/fork/fork/rsub.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/fork/fork/nest/init.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/v1/config.yaml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/tpath/v1/v1/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/unit/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/unit/test_contract.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 cpop-31.0.0/tests/unit/test_sigs.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-31.0.0/.gitignore
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 cpop-31.0.0/README.rst
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 cpop-31.0.0/pyproject.toml
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 cpop-31.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 cpop-32.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 cpop-32.0.0/src/cpop/contract.pyx
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-32.0.0/src/cpop/data.pyx
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/config.yaml
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/dirs.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/exc.py
+-rw-r--r--   0        0        0    24850 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/hub.py
+-rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/loader.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/ref.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/scanner.py
+-rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/verify.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/log/async.py
+-rw-r--r--   0        0        0     7547 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/mods/config.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/mods/contract.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/mods/dyne.py
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/mods/sub.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/mods/task.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-32.0.0/src/pop/mods/test.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/conftest.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/alias/init.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/cmods/ctest.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/cmods/contracts/ctest.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/contracts/ctx.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/contracts/ctx_args.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/contracts/ctx_update.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/contracts/many.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/contracts/priv.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/contracts/test.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/contracts/testing.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/coro/test.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/coro/contracts/test.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/csigs/sigs.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/csigs/contracts/sigs.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/external_module/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/func/__init__.py
+-rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/func/test_basic.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/func/test_bench.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/func/test_cli.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/func/test_contract_ctx.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/func/test_coro.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/func/test_fail.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/func/test_no_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/func/test_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/func/test_serial.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/func/test_sub.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/contract_ordering/single_module/thing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/contract_ordering/single_module/contracts/default.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/contract_ordering/single_module/contracts/dunder.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/contract_ordering/single_module/contracts/init.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/contract_ordering/single_module/contracts/thing.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/contracted/test_contracted_access.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/contracted/mods/contracted_access.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/contracted/mods/contracts/contracted_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/recursive_contract/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/recursive_contract/test_sub.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/bad.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/falias_dict.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/falias_func.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/falias_wrap.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/foo.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/fork.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/many.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/priv.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/proc.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/test.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/testing.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/vbad.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/virt.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/vtrue.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/alias_bad/init.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/alias_clash/init.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/bad_import/bad_import.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/contract_ctx/ctx.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/contract_ctx/ctx_args.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/contract_ctx/ctx_update.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/contract_sig/fail_sigs.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/contract_sig/pass_sigs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/contract_sig/contracts/init.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/coro/coro.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/iter/bar.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/iter/foo.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/iter/init.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/nest/basic.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/same_vname/will_load.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/same_vname/will_not_load.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/subinit/init.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/mods/subinit/subinit.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/regression/contract_masking/test_contract_masking.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/regression/contract_masking/test_duplicate_contracts.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/regression/contract_masking/contract1/init.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/regression/contract_masking/contract2/init.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/regression/contract_masking/sub/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/sdirs/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/sdirs/l11/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/sdirs/l11/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/sdirs/l12/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/sdirs/l12/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/sdirs/l13/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/sdirs/l13/l2/test.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/README.rst
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/ca/config.yaml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/ca/contract_alias/init.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/cn/config.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/cn/contract/test.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/cn/contract/contracts/test.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/config.yaml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/init.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/clash.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/dup1.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/dup2.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/float.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/init.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/invalid.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/neg.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/neg_last.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/pos.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/pos_first.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/pos_first_tie.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/unordered_1.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/unordered_2.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/verify_fail.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/verify_pass.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/verify_raise.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/contracts/zero.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/nest/init.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/recursive_contracts/clash.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/recursive_contracts/init.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_3.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_4.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/config/config.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dn1/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dn1/dn1/nest/dn1.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dn1/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dn2/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dn2/dn1/nest/dn2.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dn2/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dn3/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dn3/dn1/nest/dn3.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dn3/dn1/nest/over.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dn3/dn1/nest/next/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dn3/dn1/nest/next/last/test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne1/config.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne1/dyne1/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne1/dyne1/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne1/nest/dyne/nest.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne2/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne2/dyne2/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne2/dyne2/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne2/nest/dyne/nest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne3/config.yaml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne3/dyne3/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne3/dyne3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne3/nest/dyne/nest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne4/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne4/dyne4/nest/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/dyne4/dyne4/nest/subvert.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/fork/config.yaml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/fork/fork/rsub.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/fork/fork/nest/init.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/v1/config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/tpath/v1/v1/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/unit/test_contract.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 cpop-32.0.0/tests/unit/test_sigs.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-32.0.0/.gitignore
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 cpop-32.0.0/README.rst
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cpop-32.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 cpop-32.0.0/PKG-INFO
```

### Comparing `cpop-31.0.0/.pre-commit-config.yaml` & `cpop-32.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/src/cpop/contract.pyx` & `cpop-32.0.0/src/cpop/contract.pyx`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/src/cpop/data.pyx` & `cpop-32.0.0/src/cpop/data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/src/pop/config.yaml` & `cpop-32.0.0/src/pop/config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,9 @@
-
 # This is where we put things that USED to be in the conf.py
 config:
-  pop_cli:
-    ref:
-      default: "."
-    cli:
-      default: ""
-    args:
-      default: []
-    interactive:
-      default: False
-    hub_state:
-      default: f"/run/user/{hub.lib.os.getuid()}/pop/hub.pkl"
   pop:
     config:
       default: ~/.pop/config.yaml
       os: POP_CONFIG
   log:
     log_plugin:
       default: async
@@ -33,32 +21,14 @@
       os: POP_LOG_FMT_CONSOLE
       default: "[%(levelname)-8s] %(message)s"
     log_datefmt:
       os: POP_LOG_DATEFMT
       default: "%H:%M:%S"
 
 cli_config:
-  pop_cli:
-    ref:
-      help: The reference on the hub to call
-      positional: True
-      nargs: "?"
-    cli:
-      help: The namespace to use as the authoritative CLI
-    args:
-      help: Any additional arguments to forward to the next cli
-      positional: True
-      nargs: "..."
-    interactive:
-      help: Start a python console that contains a hub and can await functions
-      action: store_true
-      options:
-        - -i
-    hub_state:
-      help: The location of a pickle file that has a re-usable hub object
   pop:
     config:
       help: The config file used for POP
       options:
         - -c
       subcommands:
         - __global__
@@ -90,30 +60,29 @@
       subcommands:
         - __global__
     log_datefmt:
       help: The date format to display in the logs
       group: Logging Options
       subcommands:
         - __global__
+
 dyne:
   log:
     - log
 
 # python imports to put on the hub for this plugin
 import:
   - aiologger.handlers.files
   - argparse
   - asyncio
   - collections
   - importlib
   - importlib.resources
   - os
   - pathlib
-  - pickle
-  - pprint
   - pop.exc
   - cpop.contract
   - cpop.data
   - pop.hub
   - signal
   - sys
   - yaml
```

### Comparing `cpop-31.0.0/src/pop/dirs.py` & `cpop-32.0.0/src/pop/dirs.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/src/pop/exc.py` & `cpop-32.0.0/src/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/src/pop/hub.py` & `cpop-32.0.0/src/pop/hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             await self._load_all()
 
             if load_config:
                 # Overwrite opt with config data
                 self._opt = await self.pop.config.load(cli=cli, **self._dynamic.config)
 
         # Set up a logger
-        if load_config and "log" in self._subs and logs:
+        if "log" in self._subs and logs:
             await self.log[self._opt.log.log_plugin].setup(self._opt.log.copy())
 
     @property
     def OPT(self):
         return self._opt
 
     async def _load_all(self):
```

### Comparing `cpop-31.0.0/src/pop/loader.py` & `cpop-32.0.0/src/pop/loader.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/src/pop/ref.py` & `cpop-32.0.0/src/pop/ref.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/src/pop/scanner.py` & `cpop-32.0.0/src/pop/scanner.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/src/pop/verify.py` & `cpop-32.0.0/src/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/src/pop/log/async.py` & `cpop-32.0.0/src/pop/log/async.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/src/pop/mods/config.py` & `cpop-32.0.0/src/pop/mods/config.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/src/pop/mods/contract.py` & `cpop-32.0.0/src/pop/mods/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/src/pop/mods/sub.py` & `cpop-32.0.0/src/pop/mods/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/src/pop/mods/task.py` & `cpop-32.0.0/src/pop/mods/task.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/src/pop/mods/test.py` & `cpop-32.0.0/src/pop/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/conftest.py` & `cpop-32.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/contracts/ctx.py` & `cpop-32.0.0/tests/contracts/ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/contracts/many.py` & `cpop-32.0.0/tests/contracts/many.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/contracts/test.py` & `cpop-32.0.0/tests/contracts/test.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/func/test_basic.py` & `cpop-32.0.0/tests/func/test_basic.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/func/test_contract_ctx.py` & `cpop-32.0.0/tests/func/test_contract_ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/func/test_fail.py` & `cpop-32.0.0/tests/func/test_fail.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/func/test_no_raise_on_pre_failure.py` & `cpop-32.0.0/tests/func/test_no_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/func/test_raise_on_pre_failure.py` & `cpop-32.0.0/tests/func/test_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/integration/contract_ordering/single_module/contracts/default.py` & `cpop-32.0.0/tests/integration/contract_ordering/single_module/contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/integration/contract_ordering/single_module/contracts/dunder.py` & `cpop-32.0.0/tests/integration/contract_ordering/single_module/contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/integration/contract_ordering/single_module/contracts/init.py` & `cpop-32.0.0/tests/integration/contract_ordering/single_module/contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/integration/contract_ordering/single_module/contracts/thing.py` & `cpop-32.0.0/tests/integration/contract_ordering/single_module/contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py` & `cpop-32.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py` & `cpop-32.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py` & `cpop-32.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py` & `cpop-32.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py` & `cpop-32.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py` & `cpop-32.0.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/mods/falias_wrap.py` & `cpop-32.0.0/tests/mods/falias_wrap.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/mods/proc.py` & `cpop-32.0.0/tests/mods/proc.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/mods/test.py` & `cpop-32.0.0/tests/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/regression/contract_masking/test_contract_masking.py` & `cpop-32.0.0/tests/regression/contract_masking/test_contract_masking.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/regression/contract_masking/test_duplicate_contracts.py` & `cpop-32.0.0/tests/regression/contract_masking/test_duplicate_contracts.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/tpath/cn/contract/test.py` & `cpop-32.0.0/tests/tpath/cn/contract/test.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/tpath/co1/contract_ordering/init.py` & `cpop-32.0.0/tests/tpath/co1/contract_ordering/init.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/tpath/co1/contract_ordering/nest/init.py` & `cpop-32.0.0/tests/tpath/co1/contract_ordering/nest/init.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/unit/test_contract.py` & `cpop-32.0.0/tests/unit/test_contract.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/tests/unit/test_sigs.py` & `cpop-32.0.0/tests/unit/test_sigs.py`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/.gitignore` & `cpop-32.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cpop-31.0.0/README.rst` & `cpop-32.0.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 worlds, software can be built in small pieces, making development easier to
 maintain. The small pieces can then be merged and deployed in a single
 binary, making code deployment easy as well.
 
 All this using Cython, one of the world's most popular and powerful programming
 languages.
 
-Getting Started
-===============
+Instalation
+===========
 
 First off, install ``cPop`` from pypi:
 
 .. code-block:: bash
 
     pip3 install cPop
 
@@ -42,61 +42,16 @@
 
 
     async def main():
         hub = await pop.hub.AsyncHub()
         await hub.my_sub.init.cli()
 
 
-You can also initialize pop from the cli:
-
-.. code-block:: bash
-
-    python -m hub my_sub.init.cli
-
-or:
-
-.. code-block:: bash
-
-    hub my_sub.init.cli
-
-Specify a namespace that should host the authoritative CLI by calling using --cli as the first argument:
-
-.. code-block:: bash
-
-    hub --cli=my_app my_sub.init.cli
-
-If you don't specify a --cli, unknown args will be forwarded as parameters to the reference you give:
-
-
-.. code-block:: bash
-
-    hub pop.test.func arg1 arg2 --kwarg1=asdf --kwarg2 asdf
-
-
-You can access anything that is on the hub, this is very useful for debugging.
-
-Try this to see the subs that made it onto the hub:
-
-.. code-block:: bash
-
-    hub _subs
-
-You can do this to see everything that made it into hub.OPT:
-
-.. code-block:: bash
-
-    hub OPT
-
-Start an interactive python shell that includes a hub and allows async code to be run:
-
-.. code-block:: bash
-
-    hub -i
-    #>>> await hub.lib.asyncio.sleep(0)
-
+Configuration
+=============
 
 When creating a cpop app, we put all of the pop configuration in a config.yaml
 
 .. code-block:: yaml
 
     # Every config option for your plugin
     config:
```

### Comparing `cpop-31.0.0/pyproject.toml` & `cpop-32.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-cython"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpop"
-version = "31.0.0"
+version = "32.0.0"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch45@gmail.com"},
 ]
 classifiers = [
@@ -17,41 +17,42 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
 ]
 requires-python = ">=3.10"
 dependencies = [
-    "aioconsole",
     "aiofiles",
     "aiologger",
     "argparse",
     "PyYaml",
     "uvloop; sys_platform != 'win32'",
 ]
 
 [project.optional-dependencies]
+cli = [
+    "pop-cli",
+]
+
 test = [
     "pytest",
     "pytest-asyncio",
 ]
+
 build = [
     "Cython",
     "hatch-cython",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = [
     "src/cpop",
     "src/pop",
-    "src/hub",
 ]
 
-[project.scripts]
-hub = "hub.__main__:main"
 
 [tool.hatch.build.targets.wheel.hooks.cython.options]
 include_numpy = false
 include_pyarrow = false
 include_pythran = false
 
 directives = { boundscheck = false, nonecheck = false, language_level = 3, binding = true }
```

### Comparing `cpop-31.0.0/PKG-INFO` & `cpop-32.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 31.0.0
+Version: 32.0.0
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch45@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
-Requires-Dist: aioconsole
 Requires-Dist: aiofiles
 Requires-Dist: aiologger
 Requires-Dist: argparse
 Requires-Dist: pyyaml
 Requires-Dist: uvloop; sys_platform != 'win32'
 Provides-Extra: build
 Requires-Dist: cython; extra == 'build'
 Requires-Dist: hatch-cython; extra == 'build'
+Provides-Extra: cli
+Requires-Dist: pop-cli; extra == 'cli'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Description-Content-Type: text/x-rst
 
 ====
 cPOP
@@ -41,16 +42,16 @@
 worlds, software can be built in small pieces, making development easier to
 maintain. The small pieces can then be merged and deployed in a single
 binary, making code deployment easy as well.
 
 All this using Cython, one of the world's most popular and powerful programming
 languages.
 
-Getting Started
-===============
+Instalation
+===========
 
 First off, install ``cPop`` from pypi:
 
 .. code-block:: bash
 
     pip3 install cPop
 
@@ -68,61 +69,16 @@
 
 
     async def main():
         hub = await pop.hub.AsyncHub()
         await hub.my_sub.init.cli()
 
 
-You can also initialize pop from the cli:
-
-.. code-block:: bash
-
-    python -m hub my_sub.init.cli
-
-or:
-
-.. code-block:: bash
-
-    hub my_sub.init.cli
-
-Specify a namespace that should host the authoritative CLI by calling using --cli as the first argument:
-
-.. code-block:: bash
-
-    hub --cli=my_app my_sub.init.cli
-
-If you don't specify a --cli, unknown args will be forwarded as parameters to the reference you give:
-
-
-.. code-block:: bash
-
-    hub pop.test.func arg1 arg2 --kwarg1=asdf --kwarg2 asdf
-
-
-You can access anything that is on the hub, this is very useful for debugging.
-
-Try this to see the subs that made it onto the hub:
-
-.. code-block:: bash
-
-    hub _subs
-
-You can do this to see everything that made it into hub.OPT:
-
-.. code-block:: bash
-
-    hub OPT
-
-Start an interactive python shell that includes a hub and allows async code to be run:
-
-.. code-block:: bash
-
-    hub -i
-    #>>> await hub.lib.asyncio.sleep(0)
-
+Configuration
+=============
 
 When creating a cpop app, we put all of the pop configuration in a config.yaml
 
 .. code-block:: yaml
 
     # Every config option for your plugin
     config:
```

