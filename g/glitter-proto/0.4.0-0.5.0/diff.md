# Comparing `tmp/glitter_proto-0.4.0.tar.gz` & `tmp/glitter_proto-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glitter_proto-0.4.0.tar", max compression
+gzip compressed data, was "glitter_proto-0.5.0.tar", max compression
```

## Comparing `glitter_proto-0.4.0.tar` & `glitter_proto-0.5.0.tar`

### file list

```diff
@@ -1,140 +1,139 @@
--rw-r--r--   0        0        0       33 2023-08-26 03:12:16.545137 glitter_proto-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.084722 glitter_proto-0.4.0/glitter_proto/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.084846 glitter_proto-0.4.0/glitter_proto/blockved/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.084893 glitter_proto-0.4.0/glitter_proto/blockved/glitterchain/__init__.py
--rw-r--r--   0        0        0    29786 2023-08-26 04:28:32.085995 glitter_proto-0.4.0/glitter_proto/blockved/glitterchain/index/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.086109 glitter_proto-0.4.0/glitter_proto/cosmos/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.086164 glitter_proto-0.4.0/glitter_proto/cosmos/auth/__init__.py
--rw-r--r--   0        0        0     8257 2023-08-26 04:28:32.086299 glitter_proto-0.4.0/glitter_proto/cosmos/auth/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.086447 glitter_proto-0.4.0/glitter_proto/cosmos/authz/__init__.py
--rw-r--r--   0        0        0    15411 2023-08-26 04:28:32.086569 glitter_proto-0.4.0/glitter_proto/cosmos/authz/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.086746 glitter_proto-0.4.0/glitter_proto/cosmos/bank/__init__.py
--rw-r--r--   0        0        0    25810 2023-08-26 04:28:32.086861 glitter_proto-0.4.0/glitter_proto/cosmos/bank/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.086955 glitter_proto-0.4.0/glitter_proto/cosmos/base/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.087008 glitter_proto-0.4.0/glitter_proto/cosmos/base/abci/__init__.py
--rw-r--r--   0        0        0     6011 2023-08-26 04:28:32.087143 glitter_proto-0.4.0/glitter_proto/cosmos/base/abci/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.087374 glitter_proto-0.4.0/glitter_proto/cosmos/base/kv/__init__.py
--rw-r--r--   0        0        0      632 2023-08-26 04:28:32.087601 glitter_proto-0.4.0/glitter_proto/cosmos/base/kv/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.087705 glitter_proto-0.4.0/glitter_proto/cosmos/base/query/__init__.py
--rw-r--r--   0        0        0     2275 2023-08-26 04:28:32.087816 glitter_proto-0.4.0/glitter_proto/cosmos/base/query/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.087902 glitter_proto-0.4.0/glitter_proto/cosmos/base/reflection/__init__.py
--rw-r--r--   0        0        0     4758 2023-08-26 04:28:32.088024 glitter_proto-0.4.0/glitter_proto/cosmos/base/reflection/v1beta1/__init__.py
--rw-r--r--   0        0        0    20944 2023-08-26 04:28:32.088201 glitter_proto-0.4.0/glitter_proto/cosmos/base/reflection/v2alpha1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.088290 glitter_proto-0.4.0/glitter_proto/cosmos/base/snapshots/__init__.py
--rw-r--r--   0        0        0     2402 2023-08-26 04:28:32.088393 glitter_proto-0.4.0/glitter_proto/cosmos/base/snapshots/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.088474 glitter_proto-0.4.0/glitter_proto/cosmos/base/store/__init__.py
--rw-r--r--   0        0        0     1714 2023-08-26 04:28:32.088662 glitter_proto-0.4.0/glitter_proto/cosmos/base/store/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.088764 glitter_proto-0.4.0/glitter_proto/cosmos/base/tendermint/__init__.py
--rw-r--r--   0        0        0    14434 2023-08-26 04:28:32.088879 glitter_proto-0.4.0/glitter_proto/cosmos/base/tendermint/v1beta1/__init__.py
--rw-r--r--   0        0        0     1289 2023-08-26 04:28:32.089044 glitter_proto-0.4.0/glitter_proto/cosmos/base/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.089124 glitter_proto-0.4.0/glitter_proto/cosmos/capability/__init__.py
--rw-r--r--   0        0        0     1960 2023-08-26 04:28:32.089226 glitter_proto-0.4.0/glitter_proto/cosmos/capability/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.089305 glitter_proto-0.4.0/glitter_proto/cosmos/crisis/__init__.py
--rw-r--r--   0        0        0     2933 2023-08-26 04:28:32.089408 glitter_proto-0.4.0/glitter_proto/cosmos/crisis/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.089486 glitter_proto-0.4.0/glitter_proto/cosmos/crypto/__init__.py
--rw-r--r--   0        0        0     1012 2023-08-26 04:28:32.089592 glitter_proto-0.4.0/glitter_proto/cosmos/crypto/ed25519/__init__.py
--rw-r--r--   0        0        0      711 2023-08-26 04:28:32.089736 glitter_proto-0.4.0/glitter_proto/cosmos/crypto/multisig/__init__.py
--rw-r--r--   0        0        0     1045 2023-08-26 04:28:32.089877 glitter_proto-0.4.0/glitter_proto/cosmos/crypto/multisig/v1beta1/__init__.py
--rw-r--r--   0        0        0      838 2023-08-26 04:28:32.090009 glitter_proto-0.4.0/glitter_proto/cosmos/crypto/secp256k1/__init__.py
--rw-r--r--   0        0        0      812 2023-08-26 04:28:32.090151 glitter_proto-0.4.0/glitter_proto/cosmos/crypto/secp256r1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.090232 glitter_proto-0.4.0/glitter_proto/cosmos/distribution/__init__.py
--rw-r--r--   0        0        0    40219 2023-08-26 04:28:32.090360 glitter_proto-0.4.0/glitter_proto/cosmos/distribution/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.090445 glitter_proto-0.4.0/glitter_proto/cosmos/evidence/__init__.py
--rw-r--r--   0        0        0     7859 2023-08-26 04:28:32.090550 glitter_proto-0.4.0/glitter_proto/cosmos/evidence/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.090645 glitter_proto-0.4.0/glitter_proto/cosmos/feegrant/__init__.py
--rw-r--r--   0        0        0    15250 2023-08-26 04:28:32.090751 glitter_proto-0.4.0/glitter_proto/cosmos/feegrant/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.090845 glitter_proto-0.4.0/glitter_proto/cosmos/genutil/__init__.py
--rw-r--r--   0        0        0      498 2023-08-26 04:28:32.090942 glitter_proto-0.4.0/glitter_proto/cosmos/genutil/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.091019 glitter_proto-0.4.0/glitter_proto/cosmos/gov/__init__.py
--rw-r--r--   0        0        0    31135 2023-08-26 04:28:32.091124 glitter_proto-0.4.0/glitter_proto/cosmos/gov/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.091206 glitter_proto-0.4.0/glitter_proto/cosmos/mint/__init__.py
--rw-r--r--   0        0        0     7573 2023-08-26 04:28:32.091300 glitter_proto-0.4.0/glitter_proto/cosmos/mint/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.091393 glitter_proto-0.4.0/glitter_proto/cosmos/params/__init__.py
--rw-r--r--   0        0        0     3278 2023-08-26 04:28:32.091485 glitter_proto-0.4.0/glitter_proto/cosmos/params/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.091562 glitter_proto-0.4.0/glitter_proto/cosmos/slashing/__init__.py
--rw-r--r--   0        0        0    11818 2023-08-26 04:28:32.091664 glitter_proto-0.4.0/glitter_proto/cosmos/slashing/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.091771 glitter_proto-0.4.0/glitter_proto/cosmos/staking/__init__.py
--rw-r--r--   0        0        0    58934 2023-08-26 04:28:32.091883 glitter_proto-0.4.0/glitter_proto/cosmos/staking/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.091966 glitter_proto-0.4.0/glitter_proto/cosmos/tx/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.092010 glitter_proto-0.4.0/glitter_proto/cosmos/tx/signing/__init__.py
--rw-r--r--   0        0        0     4010 2023-08-26 04:28:32.092110 glitter_proto-0.4.0/glitter_proto/cosmos/tx/signing/v1beta1/__init__.py
--rw-r--r--   0        0        0    21893 2023-08-26 04:28:32.092263 glitter_proto-0.4.0/glitter_proto/cosmos/tx/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.092346 glitter_proto-0.4.0/glitter_proto/cosmos/upgrade/__init__.py
--rw-r--r--   0        0        0    12565 2023-08-26 04:28:32.092445 glitter_proto-0.4.0/glitter_proto/cosmos/upgrade/v1beta1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.092539 glitter_proto-0.4.0/glitter_proto/cosmos/vesting/__init__.py
--rw-r--r--   0        0        0     9706 2023-08-26 04:28:32.092656 glitter_proto-0.4.0/glitter_proto/cosmos/vesting/v1beta1/__init__.py
--rw-r--r--   0        0        0      212 2023-08-26 04:28:32.092821 glitter_proto-0.4.0/glitter_proto/cosmos_proto/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.092912 glitter_proto-0.4.0/glitter_proto/cosmwasm/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.092954 glitter_proto-0.4.0/glitter_proto/cosmwasm/wasm/__init__.py
--rw-r--r--   0        0        0    47983 2023-08-26 04:28:32.093078 glitter_proto-0.4.0/glitter_proto/cosmwasm/wasm/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.093155 glitter_proto-0.4.0/glitter_proto/ethermint/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.093198 glitter_proto-0.4.0/glitter_proto/ethermint/crypto/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.093239 glitter_proto-0.4.0/glitter_proto/ethermint/crypto/v1/__init__.py
--rw-r--r--   0        0        0      771 2023-08-26 04:28:32.093338 glitter_proto-0.4.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/__init__.py
--rw-r--r--   0        0        0      558 2023-08-26 03:12:16.627000 glitter_proto-0.4.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/keys.proto
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.093416 glitter_proto-0.4.0/glitter_proto/ethermint/evm/__init__.py
--rw-r--r--   0        0        0    40331 2023-08-26 04:28:32.093540 glitter_proto-0.4.0/glitter_proto/ethermint/evm/v1/__init__.py
--rw-r--r--   0        0        0     9239 2023-08-26 03:12:16.634744 glitter_proto-0.4.0/glitter_proto/ethermint/evm/v1/evm.proto
--rw-r--r--   0        0        0     1098 2023-08-26 03:12:16.634241 glitter_proto-0.4.0/glitter_proto/ethermint/evm/v1/genesis.proto
--rw-r--r--   0        0        0     9727 2023-08-26 03:12:16.633838 glitter_proto-0.4.0/glitter_proto/ethermint/evm/v1/query.proto
--rw-r--r--   0        0        0     6114 2023-08-26 03:12:16.632908 glitter_proto-0.4.0/glitter_proto/ethermint/evm/v1/tx.proto
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.093618 glitter_proto-0.4.0/glitter_proto/ethermint/feemarket/__init__.py
--rw-r--r--   0        0        0     7355 2023-08-26 04:28:32.093715 glitter_proto-0.4.0/glitter_proto/ethermint/feemarket/v1/__init__.py
--rw-r--r--   0        0        0     1403 2023-08-26 03:12:16.632005 glitter_proto-0.4.0/glitter_proto/ethermint/feemarket/v1/feemarket.proto
--rw-r--r--   0        0        0      662 2023-08-26 03:12:16.631581 glitter_proto-0.4.0/glitter_proto/ethermint/feemarket/v1/genesis.proto
--rw-r--r--   0        0        0     1840 2023-08-26 03:12:16.631277 glitter_proto-0.4.0/glitter_proto/ethermint/feemarket/v1/query.proto
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.093807 glitter_proto-0.4.0/glitter_proto/ethermint/types/__init__.py
--rw-r--r--   0        0        0     2725 2023-08-26 04:28:32.093903 glitter_proto-0.4.0/glitter_proto/ethermint/types/v1/__init__.py
--rw-r--r--   0        0        0      835 2023-08-26 03:12:16.628425 glitter_proto-0.4.0/glitter_proto/ethermint/types/v1/account.proto
--rw-r--r--   0        0        0      479 2023-08-26 03:12:16.627945 glitter_proto-0.4.0/glitter_proto/ethermint/types/v1/dynamic_fee.proto
--rw-r--r--   0        0        0      877 2023-08-26 03:12:16.629609 glitter_proto-0.4.0/glitter_proto/ethermint/types/v1/indexer.proto
--rw-r--r--   0        0        0      891 2023-08-26 03:12:16.629208 glitter_proto-0.4.0/glitter_proto/ethermint/types/v1/web3.proto
--rw-r--r--   0        0        0      207 2023-08-26 04:28:32.094034 glitter_proto-0.4.0/glitter_proto/gogoproto/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.094108 glitter_proto-0.4.0/glitter_proto/google/__init__.py
--rw-r--r--   0        0        0    13671 2023-08-26 04:28:32.094210 glitter_proto-0.4.0/glitter_proto/google/api/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 03:12:16.553884 glitter_proto-0.4.0/glitter_proto/google/protobuf/__init__.py
--rw-r--r--   0        0        0     6214 2023-08-26 03:12:16.554550 glitter_proto-0.4.0/glitter_proto/google/protobuf/compiler/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.094297 glitter_proto-0.4.0/glitter_proto/ibc/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.094338 glitter_proto-0.4.0/glitter_proto/ibc/applications/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.094379 glitter_proto-0.4.0/glitter_proto/ibc/applications/fee/__init__.py
--rw-r--r--   0        0        0    33167 2023-08-26 04:28:32.094495 glitter_proto-0.4.0/glitter_proto/ibc/applications/fee/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.094583 glitter_proto-0.4.0/glitter_proto/ibc/applications/interchain_accounts/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.094627 glitter_proto-0.4.0/glitter_proto/ibc/applications/interchain_accounts/controller/__init__.py
--rw-r--r--   0        0        0     2892 2023-08-26 04:28:32.094728 glitter_proto-0.4.0/glitter_proto/ibc/applications/interchain_accounts/controller/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.094814 glitter_proto-0.4.0/glitter_proto/ibc/applications/interchain_accounts/host/__init__.py
--rw-r--r--   0        0        0     3027 2023-08-26 04:28:32.094916 glitter_proto-0.4.0/glitter_proto/ibc/applications/interchain_accounts/host/v1/__init__.py
--rw-r--r--   0        0        0     5211 2023-08-26 04:28:32.095057 glitter_proto-0.4.0/glitter_proto/ibc/applications/interchain_accounts/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.095153 glitter_proto-0.4.0/glitter_proto/ibc/applications/transfer/__init__.py
--rw-r--r--   0        0        0    13022 2023-08-26 04:28:32.095256 glitter_proto-0.4.0/glitter_proto/ibc/applications/transfer/v1/__init__.py
--rw-r--r--   0        0        0      916 2023-08-26 04:28:32.095403 glitter_proto-0.4.0/glitter_proto/ibc/applications/transfer/v2/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.095478 glitter_proto-0.4.0/glitter_proto/ibc/core/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.095521 glitter_proto-0.4.0/glitter_proto/ibc/core/channel/__init__.py
--rw-r--r--   0        0        0    61493 2023-08-26 04:28:32.095678 glitter_proto-0.4.0/glitter_proto/ibc/core/channel/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.095758 glitter_proto-0.4.0/glitter_proto/ibc/core/client/__init__.py
--rw-r--r--   0        0        0    32886 2023-08-26 04:28:32.095885 glitter_proto-0.4.0/glitter_proto/ibc/core/client/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.095981 glitter_proto-0.4.0/glitter_proto/ibc/core/commitment/__init__.py
--rw-r--r--   0        0        0     1643 2023-08-26 04:28:32.096080 glitter_proto-0.4.0/glitter_proto/ibc/core/commitment/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.096156 glitter_proto-0.4.0/glitter_proto/ibc/core/connection/__init__.py
--rw-r--r--   0        0        0    28130 2023-08-26 04:28:32.096257 glitter_proto-0.4.0/glitter_proto/ibc/core/connection/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.096334 glitter_proto-0.4.0/glitter_proto/ibc/core/types/__init__.py
--rw-r--r--   0        0        0      874 2023-08-26 04:28:32.096428 glitter_proto-0.4.0/glitter_proto/ibc/core/types/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.096502 glitter_proto-0.4.0/glitter_proto/ibc/lightclients/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.096543 glitter_proto-0.4.0/glitter_proto/ibc/lightclients/localhost/__init__.py
--rw-r--r--   0        0        0      684 2023-08-26 04:28:32.096639 glitter_proto-0.4.0/glitter_proto/ibc/lightclients/localhost/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.096714 glitter_proto-0.4.0/glitter_proto/ibc/lightclients/solomachine/__init__.py
--rw-r--r--   0        0        0     7740 2023-08-26 04:28:32.096815 glitter_proto-0.4.0/glitter_proto/ibc/lightclients/solomachine/v1/__init__.py
--rw-r--r--   0        0        0     7733 2023-08-26 04:28:32.096968 glitter_proto-0.4.0/glitter_proto/ibc/lightclients/solomachine/v2/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.097058 glitter_proto-0.4.0/glitter_proto/ibc/lightclients/tendermint/__init__.py
--rw-r--r--   0        0        0     5136 2023-08-26 04:28:32.097156 glitter_proto-0.4.0/glitter_proto/ibc/lightclients/tendermint/v1/__init__.py
--rw-r--r--   0        0        0    10180 2023-08-26 04:28:32.097299 glitter_proto-0.4.0/glitter_proto/ics23/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.097398 glitter_proto-0.4.0/glitter_proto/tendermint/__init__.py
--rw-r--r--   0        0        0    33422 2023-08-26 04:28:32.097505 glitter_proto-0.4.0/glitter_proto/tendermint/abci/__init__.py
--rw-r--r--   0        0        0     1849 2023-08-26 04:28:32.097635 glitter_proto-0.4.0/glitter_proto/tendermint/crypto/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 04:28:32.097708 glitter_proto-0.4.0/glitter_proto/tendermint/libs/__init__.py
--rw-r--r--   0        0        0      409 2023-08-26 04:28:32.097798 glitter_proto-0.4.0/glitter_proto/tendermint/libs/bits/__init__.py
--rw-r--r--   0        0        0     1320 2023-08-26 04:28:32.097923 glitter_proto-0.4.0/glitter_proto/tendermint/p2p/__init__.py
--rw-r--r--   0        0        0    11130 2023-08-26 04:28:32.098080 glitter_proto-0.4.0/glitter_proto/tendermint/types/__init__.py
--rw-r--r--   0        0        0      949 2023-08-26 04:28:32.098246 glitter_proto-0.4.0/glitter_proto/tendermint/version/__init__.py
--rw-r--r--   0        0        0      320 2023-08-26 04:27:37.654936 glitter_proto-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5318 1970-01-01 00:00:00.000000 glitter_proto-0.4.0/setup.py
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 glitter_proto-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       33 2023-08-26 03:12:16.545137 glitter_proto-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.444587 glitter_proto-0.5.0/glitter_proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.444655 glitter_proto-0.5.0/glitter_proto/blockved/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.444695 glitter_proto-0.5.0/glitter_proto/blockved/glitterchain/__init__.py
+-rw-r--r--   0        0        0    29786 2024-04-07 08:06:03.446132 glitter_proto-0.5.0/glitter_proto/blockved/glitterchain/index/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.446200 glitter_proto-0.5.0/glitter_proto/cosmos/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.446241 glitter_proto-0.5.0/glitter_proto/cosmos/auth/__init__.py
+-rw-r--r--   0        0        0     8257 2024-04-07 08:06:03.446907 glitter_proto-0.5.0/glitter_proto/cosmos/auth/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.446957 glitter_proto-0.5.0/glitter_proto/cosmos/authz/__init__.py
+-rw-r--r--   0        0        0    15411 2024-04-07 08:06:03.447550 glitter_proto-0.5.0/glitter_proto/cosmos/authz/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.447600 glitter_proto-0.5.0/glitter_proto/cosmos/bank/__init__.py
+-rw-r--r--   0        0        0    25810 2024-04-07 08:06:03.447722 glitter_proto-0.5.0/glitter_proto/cosmos/bank/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.447770 glitter_proto-0.5.0/glitter_proto/cosmos/base/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.447808 glitter_proto-0.5.0/glitter_proto/cosmos/base/abci/__init__.py
+-rw-r--r--   0        0        0     6011 2024-04-07 08:06:03.448535 glitter_proto-0.5.0/glitter_proto/cosmos/base/abci/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.448638 glitter_proto-0.5.0/glitter_proto/cosmos/base/kv/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-07 08:06:03.449638 glitter_proto-0.5.0/glitter_proto/cosmos/base/kv/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.449700 glitter_proto-0.5.0/glitter_proto/cosmos/base/query/__init__.py
+-rw-r--r--   0        0        0     2275 2024-04-07 08:06:03.449813 glitter_proto-0.5.0/glitter_proto/cosmos/base/query/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.449863 glitter_proto-0.5.0/glitter_proto/cosmos/base/reflection/__init__.py
+-rw-r--r--   0        0        0     4758 2024-04-07 08:06:03.449989 glitter_proto-0.5.0/glitter_proto/cosmos/base/reflection/v1beta1/__init__.py
+-rw-r--r--   0        0        0    20944 2024-04-07 08:06:03.450664 glitter_proto-0.5.0/glitter_proto/cosmos/base/reflection/v2alpha1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.450717 glitter_proto-0.5.0/glitter_proto/cosmos/base/snapshots/__init__.py
+-rw-r--r--   0        0        0     2402 2024-04-07 08:06:03.450827 glitter_proto-0.5.0/glitter_proto/cosmos/base/snapshots/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.450877 glitter_proto-0.5.0/glitter_proto/cosmos/base/store/__init__.py
+-rw-r--r--   0        0        0     1714 2024-04-07 08:06:03.451151 glitter_proto-0.5.0/glitter_proto/cosmos/base/store/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.451203 glitter_proto-0.5.0/glitter_proto/cosmos/base/tendermint/__init__.py
+-rw-r--r--   0        0        0    14434 2024-04-07 08:06:03.451322 glitter_proto-0.5.0/glitter_proto/cosmos/base/tendermint/v1beta1/__init__.py
+-rw-r--r--   0        0        0     1289 2024-04-07 08:06:03.451491 glitter_proto-0.5.0/glitter_proto/cosmos/base/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.451537 glitter_proto-0.5.0/glitter_proto/cosmos/capability/__init__.py
+-rw-r--r--   0        0        0     1960 2024-04-07 08:06:03.451638 glitter_proto-0.5.0/glitter_proto/cosmos/capability/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.451682 glitter_proto-0.5.0/glitter_proto/cosmos/crisis/__init__.py
+-rw-r--r--   0        0        0     2933 2024-04-07 08:06:03.451798 glitter_proto-0.5.0/glitter_proto/cosmos/crisis/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.451842 glitter_proto-0.5.0/glitter_proto/cosmos/crypto/__init__.py
+-rw-r--r--   0        0        0     1012 2024-04-07 08:06:03.451938 glitter_proto-0.5.0/glitter_proto/cosmos/crypto/ed25519/__init__.py
+-rw-r--r--   0        0        0      711 2024-04-07 08:06:03.452052 glitter_proto-0.5.0/glitter_proto/cosmos/crypto/multisig/__init__.py
+-rw-r--r--   0        0        0     1045 2024-04-07 08:06:03.452162 glitter_proto-0.5.0/glitter_proto/cosmos/crypto/multisig/v1beta1/__init__.py
+-rw-r--r--   0        0        0      838 2024-04-07 08:06:03.452273 glitter_proto-0.5.0/glitter_proto/cosmos/crypto/secp256k1/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-07 08:06:03.452383 glitter_proto-0.5.0/glitter_proto/cosmos/crypto/secp256r1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.452427 glitter_proto-0.5.0/glitter_proto/cosmos/distribution/__init__.py
+-rw-r--r--   0        0        0    40219 2024-04-07 08:06:03.453691 glitter_proto-0.5.0/glitter_proto/cosmos/distribution/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.453739 glitter_proto-0.5.0/glitter_proto/cosmos/evidence/__init__.py
+-rw-r--r--   0        0        0     7859 2024-04-07 08:06:03.453846 glitter_proto-0.5.0/glitter_proto/cosmos/evidence/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.453890 glitter_proto-0.5.0/glitter_proto/cosmos/feegrant/__init__.py
+-rw-r--r--   0        0        0    15250 2024-04-07 08:06:03.454011 glitter_proto-0.5.0/glitter_proto/cosmos/feegrant/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.454055 glitter_proto-0.5.0/glitter_proto/cosmos/genutil/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-07 08:06:03.454447 glitter_proto-0.5.0/glitter_proto/cosmos/genutil/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.454491 glitter_proto-0.5.0/glitter_proto/cosmos/gov/__init__.py
+-rw-r--r--   0        0        0    31135 2024-04-07 08:06:03.454898 glitter_proto-0.5.0/glitter_proto/cosmos/gov/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.454946 glitter_proto-0.5.0/glitter_proto/cosmos/mint/__init__.py
+-rw-r--r--   0        0        0     7573 2024-04-07 08:06:03.455052 glitter_proto-0.5.0/glitter_proto/cosmos/mint/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.455145 glitter_proto-0.5.0/glitter_proto/cosmos/params/__init__.py
+-rw-r--r--   0        0        0     3278 2024-04-07 08:06:03.455247 glitter_proto-0.5.0/glitter_proto/cosmos/params/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.455290 glitter_proto-0.5.0/glitter_proto/cosmos/slashing/__init__.py
+-rw-r--r--   0        0        0    11818 2024-04-07 08:06:03.455399 glitter_proto-0.5.0/glitter_proto/cosmos/slashing/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.455442 glitter_proto-0.5.0/glitter_proto/cosmos/staking/__init__.py
+-rw-r--r--   0        0        0    58934 2024-04-07 08:06:03.456457 glitter_proto-0.5.0/glitter_proto/cosmos/staking/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.456506 glitter_proto-0.5.0/glitter_proto/cosmos/tx/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.456541 glitter_proto-0.5.0/glitter_proto/cosmos/tx/signing/__init__.py
+-rw-r--r--   0        0        0     4010 2024-04-07 08:06:03.456657 glitter_proto-0.5.0/glitter_proto/cosmos/tx/signing/v1beta1/__init__.py
+-rw-r--r--   0        0        0    21893 2024-04-07 08:06:03.456789 glitter_proto-0.5.0/glitter_proto/cosmos/tx/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.456841 glitter_proto-0.5.0/glitter_proto/cosmos/upgrade/__init__.py
+-rw-r--r--   0        0        0    12565 2024-04-07 08:06:03.456948 glitter_proto-0.5.0/glitter_proto/cosmos/upgrade/v1beta1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.456992 glitter_proto-0.5.0/glitter_proto/cosmos/vesting/__init__.py
+-rw-r--r--   0        0        0     9706 2024-04-07 08:06:03.457668 glitter_proto-0.5.0/glitter_proto/cosmos/vesting/v1beta1/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-07 08:06:03.457811 glitter_proto-0.5.0/glitter_proto/cosmos_proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.457859 glitter_proto-0.5.0/glitter_proto/cosmwasm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.457900 glitter_proto-0.5.0/glitter_proto/cosmwasm/wasm/__init__.py
+-rw-r--r--   0        0        0    47983 2024-04-07 08:06:03.458432 glitter_proto-0.5.0/glitter_proto/cosmwasm/wasm/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.458496 glitter_proto-0.5.0/glitter_proto/ethermint/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.458537 glitter_proto-0.5.0/glitter_proto/ethermint/crypto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.458572 glitter_proto-0.5.0/glitter_proto/ethermint/crypto/v1/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-07 08:06:03.458697 glitter_proto-0.5.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/__init__.py
+-rw-r--r--   0        0        0      558 2023-08-26 03:12:16.627000 glitter_proto-0.5.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/keys.proto
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.458746 glitter_proto-0.5.0/glitter_proto/ethermint/evm/__init__.py
+-rw-r--r--   0        0        0    40331 2024-04-07 08:06:03.459387 glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/__init__.py
+-rw-r--r--   0        0        0     9239 2023-08-26 03:12:16.634744 glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/evm.proto
+-rw-r--r--   0        0        0     1098 2023-08-26 03:12:16.634241 glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/genesis.proto
+-rw-r--r--   0        0        0     9727 2023-08-26 03:12:16.633838 glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/query.proto
+-rw-r--r--   0        0        0     6114 2023-08-26 03:12:16.632908 glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/tx.proto
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.459437 glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/__init__.py
+-rw-r--r--   0        0        0     7355 2024-04-07 08:06:03.459549 glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/__init__.py
+-rw-r--r--   0        0        0     1403 2023-08-26 03:12:16.632005 glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/feemarket.proto
+-rw-r--r--   0        0        0      662 2023-08-26 03:12:16.631581 glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/genesis.proto
+-rw-r--r--   0        0        0     1840 2023-08-26 03:12:16.631277 glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/query.proto
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.459596 glitter_proto-0.5.0/glitter_proto/ethermint/types/__init__.py
+-rw-r--r--   0        0        0     2725 2024-04-07 08:06:03.459706 glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/__init__.py
+-rw-r--r--   0        0        0      835 2023-08-26 03:12:16.628425 glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/account.proto
+-rw-r--r--   0        0        0      479 2023-08-26 03:12:16.627945 glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/dynamic_fee.proto
+-rw-r--r--   0        0        0      877 2023-08-26 03:12:16.629609 glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/indexer.proto
+-rw-r--r--   0        0        0      891 2023-08-26 03:12:16.629208 glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/web3.proto
+-rw-r--r--   0        0        0      207 2024-04-07 08:06:03.459815 glitter_proto-0.5.0/glitter_proto/gogoproto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.459857 glitter_proto-0.5.0/glitter_proto/google/__init__.py
+-rw-r--r--   0        0        0    13671 2024-04-07 08:06:03.459959 glitter_proto-0.5.0/glitter_proto/google/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-26 03:12:16.553884 glitter_proto-0.5.0/glitter_proto/google/protobuf/__init__.py
+-rw-r--r--   0        0        0     6214 2023-08-26 03:12:16.554550 glitter_proto-0.5.0/glitter_proto/google/protobuf/compiler/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.460001 glitter_proto-0.5.0/glitter_proto/ibc/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.460039 glitter_proto-0.5.0/glitter_proto/ibc/applications/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.460073 glitter_proto-0.5.0/glitter_proto/ibc/applications/fee/__init__.py
+-rw-r--r--   0        0        0    33167 2024-04-07 08:06:03.460467 glitter_proto-0.5.0/glitter_proto/ibc/applications/fee/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.460571 glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.460609 glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/controller/__init__.py
+-rw-r--r--   0        0        0     2892 2024-04-07 08:06:03.460723 glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/controller/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.460775 glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/host/__init__.py
+-rw-r--r--   0        0        0     3027 2024-04-07 08:06:03.460890 glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/host/v1/__init__.py
+-rw-r--r--   0        0        0     5211 2024-04-07 08:06:03.461012 glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.461058 glitter_proto-0.5.0/glitter_proto/ibc/applications/transfer/__init__.py
+-rw-r--r--   0        0        0    13022 2024-04-07 08:06:03.461168 glitter_proto-0.5.0/glitter_proto/ibc/applications/transfer/v1/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-07 08:06:03.461515 glitter_proto-0.5.0/glitter_proto/ibc/applications/transfer/v2/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.461571 glitter_proto-0.5.0/glitter_proto/ibc/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.461621 glitter_proto-0.5.0/glitter_proto/ibc/core/channel/__init__.py
+-rw-r--r--   0        0        0    61493 2024-04-07 08:06:03.462831 glitter_proto-0.5.0/glitter_proto/ibc/core/channel/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.462896 glitter_proto-0.5.0/glitter_proto/ibc/core/client/__init__.py
+-rw-r--r--   0        0        0    32886 2024-04-07 08:06:03.463729 glitter_proto-0.5.0/glitter_proto/ibc/core/client/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.463790 glitter_proto-0.5.0/glitter_proto/ibc/core/commitment/__init__.py
+-rw-r--r--   0        0        0     1643 2024-04-07 08:06:03.463913 glitter_proto-0.5.0/glitter_proto/ibc/core/commitment/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.463963 glitter_proto-0.5.0/glitter_proto/ibc/core/connection/__init__.py
+-rw-r--r--   0        0        0    28130 2024-04-07 08:06:03.464817 glitter_proto-0.5.0/glitter_proto/ibc/core/connection/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.464875 glitter_proto-0.5.0/glitter_proto/ibc/core/types/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-07 08:06:03.464985 glitter_proto-0.5.0/glitter_proto/ibc/core/types/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.465032 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.465070 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/localhost/__init__.py
+-rw-r--r--   0        0        0      684 2024-04-07 08:06:03.465171 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/localhost/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.465219 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/solomachine/__init__.py
+-rw-r--r--   0        0        0     7740 2024-04-07 08:06:03.465331 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/solomachine/v1/__init__.py
+-rw-r--r--   0        0        0     7733 2024-04-07 08:06:03.465454 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/solomachine/v2/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.465500 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/tendermint/__init__.py
+-rw-r--r--   0        0        0     5136 2024-04-07 08:06:03.465606 glitter_proto-0.5.0/glitter_proto/ibc/lightclients/tendermint/v1/__init__.py
+-rw-r--r--   0        0        0    10180 2024-04-07 08:06:03.465780 glitter_proto-0.5.0/glitter_proto/ics23/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.465821 glitter_proto-0.5.0/glitter_proto/tendermint/__init__.py
+-rw-r--r--   0        0        0    33422 2024-04-07 08:06:03.465973 glitter_proto-0.5.0/glitter_proto/tendermint/abci/__init__.py
+-rw-r--r--   0        0        0     1849 2024-04-07 08:06:03.466098 glitter_proto-0.5.0/glitter_proto/tendermint/crypto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:06:03.466143 glitter_proto-0.5.0/glitter_proto/tendermint/libs/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-07 08:06:03.466262 glitter_proto-0.5.0/glitter_proto/tendermint/libs/bits/__init__.py
+-rw-r--r--   0        0        0     1320 2024-04-07 08:06:03.466369 glitter_proto-0.5.0/glitter_proto/tendermint/p2p/__init__.py
+-rw-r--r--   0        0        0    11130 2024-04-07 08:06:03.466503 glitter_proto-0.5.0/glitter_proto/tendermint/types/__init__.py
+-rw-r--r--   0        0        0      949 2024-04-07 08:06:03.466624 glitter_proto-0.5.0/glitter_proto/tendermint/version/__init__.py
+-rw-r--r--   0        0        0      352 2024-04-07 09:16:59.042346 glitter_proto-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 glitter_proto-0.5.0/PKG-INFO
```

### Comparing `glitter_proto-0.4.0/glitter_proto/blockved/glitterchain/index/__init__.py` & `glitter_proto-0.5.0/glitter_proto/blockved/glitterchain/index/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/auth/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/auth/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/authz/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/authz/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/bank/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/bank/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/base/abci/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/base/abci/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/base/kv/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/base/kv/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/base/query/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/base/query/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/base/reflection/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/base/reflection/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/base/reflection/v2alpha1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/base/reflection/v2alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/base/snapshots/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/base/snapshots/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/base/store/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/base/store/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/base/tendermint/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/base/tendermint/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/base/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/base/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/capability/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/capability/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/crisis/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/crisis/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/crypto/ed25519/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/crypto/ed25519/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/crypto/multisig/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/crypto/multisig/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/crypto/multisig/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/crypto/multisig/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/crypto/secp256k1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/crypto/secp256k1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/crypto/secp256r1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/crypto/secp256r1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/distribution/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/distribution/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/evidence/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/evidence/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/feegrant/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/feegrant/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/gov/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/gov/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/mint/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/mint/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/params/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/params/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/slashing/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/slashing/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/staking/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/staking/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/tx/signing/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/tx/signing/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/tx/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/tx/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/upgrade/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/upgrade/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmos/vesting/v1beta1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmos/vesting/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/cosmwasm/wasm/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/cosmwasm/wasm/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/keys.proto` & `glitter_proto-0.5.0/glitter_proto/ethermint/crypto/v1/ethsecp256k1/keys.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/evm/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/evm/v1/evm.proto` & `glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/evm.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/evm/v1/genesis.proto` & `glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/genesis.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/evm/v1/query.proto` & `glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/query.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/evm/v1/tx.proto` & `glitter_proto-0.5.0/glitter_proto/ethermint/evm/v1/tx.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/feemarket/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/feemarket/v1/feemarket.proto` & `glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/feemarket.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/feemarket/v1/genesis.proto` & `glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/genesis.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/feemarket/v1/query.proto` & `glitter_proto-0.5.0/glitter_proto/ethermint/feemarket/v1/query.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/types/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/types/v1/account.proto` & `glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/account.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/types/v1/indexer.proto` & `glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/indexer.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ethermint/types/v1/web3.proto` & `glitter_proto-0.5.0/glitter_proto/ethermint/types/v1/web3.proto`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/google/api/__init__.py` & `glitter_proto-0.5.0/glitter_proto/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/google/protobuf/compiler/__init__.py` & `glitter_proto-0.5.0/glitter_proto/google/protobuf/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/applications/fee/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/applications/fee/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/applications/interchain_accounts/controller/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/controller/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/applications/interchain_accounts/host/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/host/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/applications/interchain_accounts/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/applications/interchain_accounts/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/applications/transfer/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/applications/transfer/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/applications/transfer/v2/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/applications/transfer/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/core/channel/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/core/channel/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/core/client/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/core/client/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/core/commitment/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/core/commitment/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/core/connection/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/core/connection/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/core/types/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/core/types/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/lightclients/localhost/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/lightclients/localhost/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/lightclients/solomachine/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/lightclients/solomachine/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/lightclients/solomachine/v2/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/lightclients/solomachine/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ibc/lightclients/tendermint/v1/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ibc/lightclients/tendermint/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/ics23/__init__.py` & `glitter_proto-0.5.0/glitter_proto/ics23/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/tendermint/abci/__init__.py` & `glitter_proto-0.5.0/glitter_proto/tendermint/abci/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/tendermint/crypto/__init__.py` & `glitter_proto-0.5.0/glitter_proto/tendermint/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/tendermint/p2p/__init__.py` & `glitter_proto-0.5.0/glitter_proto/tendermint/p2p/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/tendermint/types/__init__.py` & `glitter_proto-0.5.0/glitter_proto/tendermint/types/__init__.py`

 * *Files identical despite different names*

### Comparing `glitter_proto-0.4.0/glitter_proto/tendermint/version/__init__.py` & `glitter_proto-0.5.0/glitter_proto/tendermint/version/__init__.py`

 * *Files identical despite different names*

