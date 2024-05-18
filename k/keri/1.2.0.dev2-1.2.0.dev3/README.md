# Comparing `tmp/keri-1.2.0.dev2.tar.gz` & `tmp/keri-1.2.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keri-1.2.0.dev2.tar", last modified: Thu May  2 02:06:53 2024, max compression
+gzip compressed data, was "keri-1.2.0.dev3.tar", last modified: Sat May 18 21:02:18 2024, max compression
```

## Comparing `keri-1.2.0.dev2.tar` & `keri-1.2.0.dev3.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.908031 keri-1.2.0.dev2/
--rw-r--r--   0 pfeairheller   (501) staff       (20)    11357 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/LICENSE
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1594 2024-05-02 02:06:53.907755 keri-1.2.0.dev2/PKG-INFO
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2457 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/README.md
--rw-r--r--   0 pfeairheller   (501) staff       (20)       38 2024-05-02 02:06:53.908078 keri-1.2.0.dev2/setup.cfg
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4061 2024-05-02 01:55:35.000000 keri-1.2.0.dev2/setup.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.880052 keri-1.2.0.dev2/src/
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.882593 keri-1.2.0.dev2/src/keri/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       83 2024-05-02 01:55:35.000000 keri-1.2.0.dev2/src/keri/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.887565 keri-1.2.0.dev2/src/keri/app/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       58 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    37921 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/agenting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2780 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/apping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1648 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/challenging.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.887977 keri-1.2.0.dev2/src/keri/app/cli/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       62 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.890932 keri-1.2.0.dev2/src/keri/app/cli/commands/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.891427 keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1529 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4353 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/respond.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5565 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/verify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1847 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/clean.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.891660 keri-1.2.0.dev2/src/keri/app/cli/commands/contacts/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/contacts/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2662 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/contacts/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2074 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/decrypt.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.892008 keri-1.2.0.dev2/src/keri/app/cli/commands/delegate/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/delegate/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9425 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/delegate/confirm.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4076 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/delegate/request.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.892196 keri-1.2.0.dev2/src/keri/app/cli/commands/did/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/did/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3450 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/did/generate.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.892638 keri-1.2.0.dev2/src/keri/app/cli/commands/ends/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ends/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4679 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ends/add.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2873 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ends/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2566 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ends/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6291 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/escrow.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3744 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7156 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5479 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/init.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4897 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/interact.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.893724 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6651 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/admit.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      531 2024-04-30 21:46:50.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/agree.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      472 2024-04-30 21:46:50.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/apply.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6996 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/grant.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9834 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/join.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10073 2024-04-30 21:46:50.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      566 2024-04-30 21:46:50.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/offer.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5584 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/spurn.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3371 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/kevers.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1402 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.893945 keri-1.2.0.dev2/src/keri/app/cli/commands/local/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/local/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9105 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/local/watch.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.894337 keri-1.2.0.dev2/src/keri/app/cli/commands/mailbox/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/mailbox/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4555 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/mailbox/debug.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2554 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/mailbox/update.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.894865 keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1938 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1785 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/run.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1806 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/show.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6153 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/migrate.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.896336 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3045 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/continue.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      735 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/demo.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6698 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5619 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/interact.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    30790 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/join.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5227 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/notice.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10190 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/rotate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9500 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/shell.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4891 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/update.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      442 2024-04-30 21:46:50.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/nonce.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.896772 keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1975 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/clean.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3120 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3716 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/resolve.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.897186 keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      662 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1521 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/remove.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2549 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/set.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3559 2024-05-02 01:19:02.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/query.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2161 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/rename.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4044 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/rollback.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8964 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/rotate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1051 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/saidify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      519 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/salt.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2140 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/sign.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.897379 keri-1.2.0.dev2/src/keri/app/cli/commands/ssh/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ssh/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3392 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/ssh/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2284 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/status.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      414 2024-04-05 21:44:00.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/time.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.898001 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10874 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/create.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5966 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6251 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.898488 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7267 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1764 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3683 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/status.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7517 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/vc/revoke.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2940 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/verify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1251 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/version.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.898763 keri-1.2.0.dev2/src/keri/app/cli/commands/watcher/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       78 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/watcher/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4507 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/watcher/add.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.899448 keri-1.2.0.dev2/src/keri/app/cli/commands/witness/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/witness/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4187 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/witness/authenticate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3047 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/witness/demo.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4836 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/witness/start.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4655 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/commands/witness/submit.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.900487 keri-1.2.0.dev2/src/keri/app/cli/common/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/common/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/common/config.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3887 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/common/displaying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3357 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/cli/common/existing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1783 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/cli/common/incepting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1208 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/common/rotating.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      415 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/cli/common/terming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      728 2024-04-22 16:39:31.000000 keri-1.2.0.dev2/src/keri/app/cli/kli.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8151 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/configing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7632 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/connecting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10242 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/delegating.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    24676 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/directing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    18769 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/forwarding.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    26643 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/grouping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   124689 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/app/habbing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8702 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/httping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    41828 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/app/indirecting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    73656 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/app/keeping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    13938 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/notifying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    26860 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/app/oobiing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4471 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/querying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8400 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/signaling.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5908 2024-04-05 21:44:00.000000 keri-1.2.0.dev2/src/keri/app/signing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1837 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/app/specing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9669 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/app/storing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.902315 keri-1.2.0.dev2/src/keri/core/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      507 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/core/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   201749 2024-05-02 01:21:52.000000 keri-1.2.0.dev2/src/keri/core/coring.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    38577 2024-05-02 01:21:52.000000 keri-1.2.0.dev2/src/keri/core/counting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   306428 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/core/eventing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    34501 2024-05-02 01:21:52.000000 keri-1.2.0.dev2/src/keri/core/indexing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    58321 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/core/parsing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    26820 2024-04-29 23:03:37.000000 keri-1.2.0.dev2/src/keri/core/routing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    12848 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/core/scheming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    82877 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/core/serdering.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    35338 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/core/signing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    15364 2024-05-02 01:21:52.000000 keri-1.2.0.dev2/src/keri/core/streaming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    25641 2024-05-02 01:21:52.000000 keri-1.2.0.dev2/src/keri/core/structing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.903615 keri-1.2.0.dev2/src/keri/db/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       55 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/db/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   127858 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/db/basing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    77257 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/db/dbing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9246 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/db/escrowing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    30476 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/db/koming.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.903848 keri-1.2.0.dev2/src/keri/db/migrations/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/db/migrations/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2861 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/db/migrations/rekey_habs.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    59458 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/db/subing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.904643 keri-1.2.0.dev2/src/keri/demo/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       59 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/demo/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2790 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/demo/demo_bob.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2806 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/demo/demo_eve.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      932 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/demo/demo_kev.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2831 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/demo/demo_sam.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    16437 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/demo/demoing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.905087 keri-1.2.0.dev2/src/keri/end/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       73 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/end/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    25038 2024-05-02 01:46:06.000000 keri-1.2.0.dev2/src/keri/end/ending.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1322 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/end/priming.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.905329 keri-1.2.0.dev2/src/keri/help/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      619 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/help/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    12484 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/help/helping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    27254 2024-05-02 01:21:52.000000 keri-1.2.0.dev2/src/keri/kering.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.905527 keri-1.2.0.dev2/src/keri/peer/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/peer/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    19698 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/peer/exchanging.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.906195 keri-1.2.0.dev2/src/keri/vc/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       56 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/vc/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10278 2024-04-05 21:44:00.000000 keri-1.2.0.dev2/src/keri/vc/protocoling.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2528 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/vc/proving.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3749 2024-03-12 23:12:35.000000 keri-1.2.0.dev2/src/keri/vc/walleting.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.906953 keri-1.2.0.dev2/src/keri/vdr/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      120 2023-03-20 02:45:25.000000 keri-1.2.0.dev2/src/keri/vdr/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    34327 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/vdr/credentialing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    84698 2024-04-30 21:46:50.000000 keri-1.2.0.dev2/src/keri/vdr/eventing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    14424 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/vdr/verifying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    35856 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/src/keri/vdr/viring.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.907459 keri-1.2.0.dev2/src/keri.egg-info/
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1594 2024-05-02 02:06:53.000000 keri-1.2.0.dev2/src/keri.egg-info/PKG-INFO
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6046 2024-05-02 02:06:53.000000 keri-1.2.0.dev2/src/keri.egg-info/SOURCES.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2024-05-02 02:06:53.000000 keri-1.2.0.dev2/src/keri.egg-info/dependency_links.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)      181 2024-05-02 02:06:53.000000 keri-1.2.0.dev2/src/keri.egg-info/entry_points.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2023-03-20 03:44:29.000000 keri-1.2.0.dev2/src/keri.egg-info/not-zip-safe
--rw-r--r--   0 pfeairheller   (501) staff       (20)      314 2024-05-02 02:06:53.000000 keri-1.2.0.dev2/src/keri.egg-info/requires.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        5 2024-05-02 02:06:53.000000 keri-1.2.0.dev2/src/keri.egg-info/top_level.txt
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-02 02:06:53.907088 keri-1.2.0.dev2/tests/
--rw-r--r--   0 pfeairheller   (501) staff       (20)    28418 2024-04-25 20:01:20.000000 keri-1.2.0.dev2/tests/test_kering.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.691207 keri-1.2.0.dev3/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    11357 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/LICENSE
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1594 2024-05-18 21:02:18.690889 keri-1.2.0.dev3/PKG-INFO
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2457 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/README.md
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       38 2024-05-18 21:02:18.691253 keri-1.2.0.dev3/setup.cfg
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4061 2024-05-18 21:00:07.000000 keri-1.2.0.dev3/setup.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.654579 keri-1.2.0.dev3/src/
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.657395 keri-1.2.0.dev3/src/keri/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       83 2024-05-18 21:00:08.000000 keri-1.2.0.dev3/src/keri/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.664834 keri-1.2.0.dev3/src/keri/app/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       58 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    37921 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/agenting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2780 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/apping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1648 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/challenging.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.666496 keri-1.2.0.dev3/src/keri/app/cli/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       62 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.671115 keri-1.2.0.dev3/src/keri/app/cli/commands/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.671864 keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1529 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4353 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/respond.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5565 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/verify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1847 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/clean.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.672145 keri-1.2.0.dev3/src/keri/app/cli/commands/contacts/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/contacts/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2662 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/contacts/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2074 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/decrypt.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.672577 keri-1.2.0.dev3/src/keri/app/cli/commands/delegate/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/delegate/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9099 2024-05-18 20:59:33.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/delegate/confirm.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4076 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/delegate/request.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.672801 keri-1.2.0.dev3/src/keri/app/cli/commands/did/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/did/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3450 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/did/generate.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.673325 keri-1.2.0.dev3/src/keri/app/cli/commands/ends/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ends/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4679 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ends/add.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2873 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ends/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2566 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ends/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6291 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/escrow.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3744 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7158 2024-05-18 20:59:33.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5479 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/init.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4897 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/interact.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.674814 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6651 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/admit.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      531 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/agree.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      472 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/apply.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6996 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/grant.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9834 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/join.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10073 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      566 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/offer.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5584 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/spurn.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3371 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/kevers.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1402 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/list.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.675074 keri-1.2.0.dev3/src/keri/app/cli/commands/local/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/local/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9105 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/local/watch.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.675492 keri-1.2.0.dev3/src/keri/app/cli/commands/mailbox/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/mailbox/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4555 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/mailbox/debug.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2554 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/mailbox/update.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.675984 keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1938 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1785 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/run.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1806 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/show.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6153 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/migrate.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.677576 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3045 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/continue.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      735 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/demo.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6698 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5619 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/interact.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    31512 2024-05-18 15:25:02.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/join.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5227 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/notice.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10166 2024-05-18 15:25:02.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/rotate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9500 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/shell.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4891 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/update.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      442 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/nonce.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.678186 keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1975 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/clean.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3120 2024-05-18 15:25:13.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3716 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/resolve.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.678847 keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      662 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1521 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/remove.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2549 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/set.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3559 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/query.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2161 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/rename.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4044 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/rollback.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8964 2024-05-18 20:59:33.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/rotate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1051 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/saidify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      519 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/salt.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2140 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/sign.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.679058 keri-1.2.0.dev3/src/keri/app/cli/commands/ssh/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ssh/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3392 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ssh/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2284 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/status.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      414 2024-04-05 21:44:00.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/time.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.679783 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10874 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/create.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5966 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6251 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/list.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.680321 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7267 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1764 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3683 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/status.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7517 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/revoke.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2940 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/verify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1251 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/version.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.680587 keri-1.2.0.dev3/src/keri/app/cli/commands/watcher/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       78 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/watcher/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4507 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/watcher/add.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.681283 keri-1.2.0.dev3/src/keri/app/cli/commands/witness/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/witness/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4187 2024-05-18 15:25:13.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/witness/authenticate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3047 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/witness/demo.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4836 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/witness/start.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4655 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/witness/submit.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.682549 keri-1.2.0.dev3/src/keri/app/cli/common/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/common/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/common/config.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3887 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/common/displaying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3357 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/common/existing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1783 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/cli/common/incepting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1208 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/common/rotating.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      415 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/common/terming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      728 2024-04-22 16:39:31.000000 keri-1.2.0.dev3/src/keri/app/cli/kli.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8151 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/configing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7632 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/connecting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10593 2024-05-18 20:59:33.000000 keri-1.2.0.dev3/src/keri/app/delegating.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    24676 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/directing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    18769 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/forwarding.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26489 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/grouping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   124689 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/habbing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8702 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/httping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    41828 2024-05-18 15:25:13.000000 keri-1.2.0.dev3/src/keri/app/indirecting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    73656 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/keeping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    13938 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/notifying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26860 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/oobiing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4471 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/querying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8400 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/signaling.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5908 2024-04-05 21:44:00.000000 keri-1.2.0.dev3/src/keri/app/signing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1837 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/specing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9669 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/storing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.684687 keri-1.2.0.dev3/src/keri/core/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      468 2024-05-08 02:11:51.000000 keri-1.2.0.dev3/src/keri/core/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   201749 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/core/coring.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    38577 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/core/counting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   304791 2024-05-18 20:59:33.000000 keri-1.2.0.dev3/src/keri/core/eventing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    34501 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/core/indexing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    58336 2024-05-18 20:59:33.000000 keri-1.2.0.dev3/src/keri/core/parsing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26820 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/core/routing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    12848 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/core/scheming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    82877 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/core/serdering.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    33908 2024-05-08 02:11:51.000000 keri-1.2.0.dev3/src/keri/core/signing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    15364 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/core/streaming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    25641 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/core/structing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.685954 keri-1.2.0.dev3/src/keri/db/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       55 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/db/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   127640 2024-05-18 20:59:33.000000 keri-1.2.0.dev3/src/keri/db/basing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    77257 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/db/dbing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9246 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/db/escrowing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    30476 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/db/koming.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.686219 keri-1.2.0.dev3/src/keri/db/migrations/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/db/migrations/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2861 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/db/migrations/rekey_habs.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    59458 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/db/subing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.687187 keri-1.2.0.dev3/src/keri/demo/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       59 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/demo/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2790 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/demo/demo_bob.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2806 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/demo/demo_eve.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      932 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/demo/demo_kev.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2831 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/demo/demo_sam.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    16437 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/demo/demoing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.687785 keri-1.2.0.dev3/src/keri/end/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       73 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/end/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    25038 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/end/ending.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1322 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/end/priming.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.688029 keri-1.2.0.dev3/src/keri/help/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      619 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/help/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    12484 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/help/helping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    27254 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/kering.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.688340 keri-1.2.0.dev3/src/keri/peer/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/peer/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    19698 2024-05-18 15:25:13.000000 keri-1.2.0.dev3/src/keri/peer/exchanging.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.689229 keri-1.2.0.dev3/src/keri/vc/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       56 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/vc/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10278 2024-04-05 21:44:00.000000 keri-1.2.0.dev3/src/keri/vc/protocoling.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2528 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/vc/proving.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3749 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/vc/walleting.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.690143 keri-1.2.0.dev3/src/keri/vdr/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      120 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/vdr/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    34327 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/vdr/credentialing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    84698 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/vdr/eventing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    14424 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/vdr/verifying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    35856 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/vdr/viring.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.690509 keri-1.2.0.dev3/src/keri.egg-info/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1594 2024-05-18 21:02:18.000000 keri-1.2.0.dev3/src/keri.egg-info/PKG-INFO
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6046 2024-05-18 21:02:18.000000 keri-1.2.0.dev3/src/keri.egg-info/SOURCES.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2024-05-18 21:02:18.000000 keri-1.2.0.dev3/src/keri.egg-info/dependency_links.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      181 2024-05-18 21:02:18.000000 keri-1.2.0.dev3/src/keri.egg-info/entry_points.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2023-03-20 03:44:29.000000 keri-1.2.0.dev3/src/keri.egg-info/not-zip-safe
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      314 2024-05-18 21:02:18.000000 keri-1.2.0.dev3/src/keri.egg-info/requires.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        5 2024-05-18 21:02:18.000000 keri-1.2.0.dev3/src/keri.egg-info/top_level.txt
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.690319 keri-1.2.0.dev3/tests/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    28418 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/tests/test_kering.py
```

### Comparing `keri-1.2.0.dev2/LICENSE` & `keri-1.2.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/PKG-INFO` & `keri-1.2.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keri
-Version: 1.2.0.dev2
+Version: 1.2.0.dev3
 Summary: Key Event Receipt Infrastructure
 Home-page: https://github.com/WebOfTrust/keripy
 Author: Samuel M. Smith
 Author-email: smith.samuel.m@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://keri.readthedocs.io/
 Project-URL: Changelog, https://keri.readthedocs.io/en/latest/changelog.html
```

### Comparing `keri-1.2.0.dev2/README.md` & `keri-1.2.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/setup.py` & `keri-1.2.0.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from glob import glob
 from os.path import basename
 from os.path import splitext
 
 from setuptools import find_packages, setup
 setup(
     name='keri',
-    version='1.2.0-dev2',  # also change in src/keri/__init__.py
+    version='1.2.0-dev3',  # also change in src/keri/__init__.py
     license='Apache Software License 2.0',
     description='Key Event Receipt Infrastructure',
     long_description="KERI Decentralized Key Management Infrastructure",
     author='Samuel M. Smith',
     author_email='smith.samuel.m@gmail.com',
     url='https://github.com/WebOfTrust/keripy',
     packages=find_packages('src'),
```

### Comparing `keri-1.2.0.dev2/src/keri/app/agenting.py` & `keri-1.2.0.dev3/src/keri/app/agenting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/apping.py` & `keri-1.2.0.dev3/src/keri/app/apping.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/challenging.py` & `keri-1.2.0.dev3/src/keri/app/challenging.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/generate.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/respond.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/respond.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/challenge/verify.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/verify.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/clean.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/clean.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/contacts/list.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/contacts/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/decrypt.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/decrypt.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/delegate/confirm.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/delegate/confirm.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,17 +92,16 @@
         # enter context
         self.wind(tymth)
         self.tock = tock
         _ = (yield self.tock)
 
         while True:
             esc = self.escrowed()
-            for ekey, edig in esc:
-                pre, sn = dbing.splitKeySN(ekey)  # get pre and sn from escrow item
-                dgkey = dbing.dgKey(pre, bytes(edig))
+            for pre, sn, edig in esc:
+                dgkey = dbing.dgKey(pre, edig)
                 eraw = self.hby.db.getEvt(dgkey)
                 if eraw is None:
                     continue
                 eserder = serdering.SerderKERI(raw=bytes(eraw))  # escrowed event
 
                 ilk = eserder.sad["t"]
                 if ilk in (coring.Ilks.dip,):
@@ -200,25 +199,20 @@
                             self.witq.query(src=hab.pre, pre=eserder.pre, sn=eserder.sn, wits=wits)
 
                             while eserder.pre not in self.hby.kevers:
                                 yield self.tock
 
                             print(f"Delegate {eserder.pre} {typ} event committed.")
 
+                        self.hby.db.delegables.rem(keys=(pre, sn))
                         self.remove(self.toRemove)
                         return True
 
                 yield self.tock
 
             yield self.tock
 
     def escrowed(self):
         esc = []
-        key = ekey = b''  # both start same. when not same means escrows found
-        while True:  # break when done
-            for ekey, edig in self.hby.db.getPseItemsNextIter(key=key):
-                esc.append((ekey, edig))
-            if ekey == key:  # still same so no escrows found on last while iteration
-                break
-            key = ekey  # setup next while iteration, with key after ekey
-
+        for (pre, sn), edig in self.hby.db.delegables.getItemIter():
+            esc.append((pre, sn, edig))
         return esc
```

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/delegate/request.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/delegate/request.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/did/generate.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/did/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/ends/add.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/ends/add.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/ends/export.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/ends/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/ends/list.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/ends/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/escrow.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/escrow.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/export.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/incept.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/incept.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,24 +133,23 @@
                                     base="",
                                     headDirPath=cnfg,
                                     temp=False,
                                     reopen=True,
                                     clear=False)
         self.endpoint = endpoint
         self.proxy = proxy
-        hby = existing.setupHby(name=name, base=base, bran=bran, cf=cf)
-        self.hbyDoer = habbing.HaberyDoer(habery=hby)  # setup doer
-        self.swain = delegating.Anchorer(hby=hby)
-        self.postman = forwarding.Poster(hby=hby)
-        self.mbx = indirecting.MailboxDirector(hby=hby, topics=['/receipt', "/replay", "/reply"])
+        self.hby = existing.setupHby(name=name, base=base, bran=bran, cf=cf)
+        self.hbyDoer = habbing.HaberyDoer(habery=self.hby)  # setup doer
+        self.swain = delegating.Anchorer(hby=self.hby, proxy=self.hby.habByName(self.proxy))
+        self.postman = forwarding.Poster(hby=self.hby)
+        self.mbx = indirecting.MailboxDirector(hby=self.hby, topics=['/receipt', "/replay", "/reply"])
         doers = [self.hbyDoer, self.postman, self.mbx, self.swain, doing.doify(self.inceptDo)]
 
         self.inits = kwa
         self.alias = alias
-        self.hby = hby
         super(InceptDoer, self).__init__(doers=doers)
 
     def inceptDo(self, tymth, tock=0.0):
         """
         Parameters:
             tymth (function): injected function wrapper closure returned by .tymen() of
                 Tymist instance. Calling tymth() returns associated Tymist .tyme.
@@ -165,15 +164,15 @@
 
         hab = self.hby.makeHab(name=self.alias, **self.inits)
         witDoer = agenting.WitnessReceiptor(hby=self.hby)
         receiptor = agenting.Receiptor(hby=self.hby)
         self.extend([witDoer, receiptor])
 
         if hab.kever.delpre:
-            self.swain.delegation(pre=hab.pre, sn=0, proxy=self.hby.habByName(self.proxy))
+            self.swain.delegation(pre=hab.pre, sn=0)
             print("Waiting for delegation approval...")
             while not self.swain.complete(hab.kever.prefixer, coring.Seqner(sn=hab.kever.sn)):
                 yield self.tock
 
         elif hab.kever.wits:
             print("Waiting for witness receipts...")
             if self.endpoint:
```

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/init.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/interact.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/interact.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/admit.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/admit.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/agree.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/agree.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/grant.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/grant.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/join.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/join.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/list.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/offer.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/offer.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/ipex/spurn.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/spurn.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/kevers.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/kevers.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/list.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/local/watch.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/local/watch.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/mailbox/debug.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/mailbox/debug.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/mailbox/update.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/mailbox/update.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/list.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/run.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/run.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/migrate/show.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/show.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/migrate.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/continue.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/continue.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/demo.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/demo.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/incept.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/incept.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/interact.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/interact.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/join.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/join.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,55 +17,60 @@
 from keri.core import coring, eventing, scheming, parsing, routing, serdering
 from keri.peer import exchanging
 from keri.vdr import verifying, credentialing
 
 logger = help.ogler.getLogger()
 
 parser = argparse.ArgumentParser(description='Join group multisig inception, rotation or interaction event.')
-parser.set_defaults(handler=lambda args: confirm(args))
+parser.set_defaults(handler=lambda args: join(args))
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
+parser.add_argument('--group', '-a', help='human-readable name for the multisig group identifier prefix', required=False, default=None)
 parser.add_argument('--passcode', '-p', help='21 character encryption passcode for keystore (is not saved)',
                     dest="bran", default=None)  # passcode => bran
 parser.add_argument("--auto", "-Y", help="auto approve any delegation request non-interactively", action="store_true")
 
 
-def confirm(args):
-    """  Wait for and provide interactive confirmation of group multisig inception, rotation or interaction events
+def join(args):
+    """ Wait for and provide interactive confirmation of group multisig inception, rotation or interaction events
 
     Parameters:
-        args(Namespace): parsed arguements namespace object
+        args(Namespace): parsed arguments namespace object
 
     """
     name = args.name
     base = args.base
     bran = args.bran
     auto = args.auto
+    group = args.group
 
-    confirmDoer = ConfirmDoer(name=name, base=base, bran=bran, auto=auto)
+    joinDoer = JoinDoer(name=name, base=base, bran=bran, group=group, auto=auto)
 
-    doers = [confirmDoer]
+    doers = [joinDoer]
     return doers
 
 
-class ConfirmDoer(doing.DoDoer):
-    """  Doist doer capable of polling for group multisig events and prompting user for action
+class JoinDoer(doing.DoDoer):
+    """ Doist doer capable of polling for group multisig events and prompting user for action
 
     """
 
-    def __init__(self, name, base, bran, auto=False):
+    def __init__(self, name, base, bran, group, auto=False):
         """ Create doer for polling for group multisig events and either approve automatically or prompt user
 
         Parameters:
             name (str): database environment name
             base (str): database directory prefix
             bran (str): passcode to unlock keystore
-
+            group (str): human-readable name for the multisig identifier prefix
+            auto (bool): non-interactively auto approve any inception, rotation, interaction, or other event
+                         while using the default group of "default-group"
         """
+        self.group = group
         self.hby = existing.setupHby(name=name, base=base, bran=bran)
         self.rgy = credentialing.Regery(hby=self.hby, name=name, base=base)
         self.hbyDoer = habbing.HaberyDoer(habery=self.hby)  # setup doer
         self.witq = agenting.WitnessInquisitor(hby=self.hby)
         self.org = connecting.Organizer(hby=self.hby)
         self.notifier = notifying.Notifier(hby=self.hby)
         self.exc = exchanging.Exchanger(hby=self.hby, handlers=[])
@@ -84,19 +89,19 @@
 
         self.mbx = indirecting.MailboxDirector(hby=self.hby, exc=self.exc, topics=['/receipt', '/multisig', '/replay',
                                                                                    '/delegate'])
         self.postman = forwarding.Poster(hby=self.hby)
 
         doers = [self.hbyDoer, self.witq,  self.mbx, self.counselor, self.registrar, self.credentialer, self.postman]
         self.toRemove = list(doers)
-        doers.extend([doing.doify(self.confirmDo)])
+        doers.extend([doing.doify(self.joinDo)])
         self.auto = auto
-        super(ConfirmDoer, self).__init__(doers=doers)
+        super(JoinDoer, self).__init__(doers=doers)
 
-    def confirmDo(self, tymth, tock=0.0):
+    def joinDo(self, tymth, tock=0.0):
         """
         Parameters:
             tymth (function): injected function wrapper closure returned by .tymen() of
                 Tymist instance. Calling tymth() returns associated Tymist .tyme.
             tock (float): injected initial tock value
 
         Returns:  doifiable Doist compatible generator method
@@ -142,15 +147,15 @@
                     self.notifier.noter.notes.rem(keys=keys)
 
             yield self.tock
 
         self.remove(self.toRemove)
 
     def incept(self, attrs):
-        """ Incept group multisig
+        """ Join a group multisig inception event
 
         """
         said = attrs["d"]
         exn, pathed = exchanging.cloneMessage(self.hby, said=said)
         payload = exn.ked['a']
 
         smids = payload["smids"]
@@ -173,16 +178,16 @@
         #original icp
         embeds = exn.ked['e']
         oicp = serdering.SerderKERI(sad=embeds["icp"])
 
         inits["isith"] = oicp.ked["kt"]
         inits["nsith"] = oicp.ked["nt"]
 
-        inits["estOnly"] = eventing.TraitCodex.EstOnly in oicp.ked["c"]
-        inits["DnD"] = eventing.TraitCodex.DoNotDelegate in oicp.ked["c"]
+        inits["estOnly"] = kering.TraitCodex.EstOnly in oicp.ked["c"]
+        inits["DnD"] = kering.TraitCodex.DoNotDelegate in oicp.ked["c"]
 
         inits["toad"] = oicp.ked["bt"]
         inits["wits"] = oicp.ked["b"]
         inits["delpre"] = oicp.ked["di"] if "di" in ked else None
 
         print()
         print("Group Multisig Inception proposed:")
@@ -192,25 +197,28 @@
             approve = True
         else:
             yn = input(f"\nJoin [Y|n]? ")
             approve = yn in ('', 'y', 'Y')
 
         if approve:
             if self.auto:
-                alias = "test alias"
+                if self.group is None:
+                    group = "default-group"
+                else:
+                    group = self.group
             else:
                 while True:
-                    alias = input(f"\nEnter alias for new AID: ")
-                    if self.hby.habByName(alias) is not None:
-                        print(f"AID alias {alias} is already in use, please try again")
+                    group = input(f"\nEnter group name for new AID: ")
+                    if self.hby.habByName(group) is not None:
+                        print(f"AID group name {group} is already in use, please try again")
                     else:
                         break
 
             try:
-                ghab = self.hby.makeGroupHab(group=alias, mhab=mhab,
+                ghab = self.hby.makeGroupHab(group=group, mhab=mhab,
                                              smids=smids, rmids=rmids, **inits)
             except ValueError as e:
                 return False
 
             icp = ghab.makeOwnInception(allowPartiallySigned=True)
 
             exn, ims = grouping.multisigInceptExn(ghab.mhab,
@@ -389,27 +397,30 @@
 
         if approve:
             pre = orot.ked['i']
             if pre in self.hby.habs:
                 ghab = self.hby.habs[pre]
             else:
                 if self.auto:
-                    alias = "test alias"
+                    if self.group is None:
+                        group = "default-group"
+                    else:
+                        group = self.group
                 else:
                     while True:
-                        alias = input(f"\nEnter alias for new AID: ")
-                        if self.hby.habByName(alias) is not None:
-                            print(f"AID alias {alias} is already in use, please try again")
+                        group = input(f"\nEnter group name for new AID: ")
+                        if self.hby.habByName(group) is not None:
+                            print(f"AID group name {group} is already in use, please try again")
                         else:
                             break
 
-                ghab = self.hby.joinGroupHab(pre, group=alias, mhab=mhab, smids=smids, rmids=rmids)
+                ghab = self.hby.joinGroupHab(pre, group=group, mhab=mhab, smids=smids, rmids=rmids)
 
             try:
-                ghab.rotate(serder=orot)
+                ghab.rotate(serder=orot, smids=smids, rmids=rmids)
             except ValueError:
                 return False
 
             rot = ghab.makeOwnEvent(allowPartiallySigned=True, sn=orot.sn)
 
             exn, ims = grouping.multisigRotateExn(ghab,
                                                   smids=ghab.smids,
```

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/notice.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/notice.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/rotate.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/rotate.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,47 +49,47 @@
 
     Parameters:
         args (parseargs):  command line parameters
 
     """
 
     data = config.parseData(args.data) if args.data is not None else None
-
-    rotDoer = GroupMultisigRotate(name=args.name, base=args.base, alias=args.alias, smids=args.smids, rmids=args.rmids,
-                                  bran=args.bran, wits=args.witnesses, cuts=args.cuts, adds=args.witness_add,
+    hby = existing.setupHby(name=args.name, base=args.base, bran=args.bran)
+    rotDoer = GroupMultisigRotate(hby=hby, alias=args.alias, smids=args.smids, rmids=args.rmids,
+                                  wits=args.witnesses, cuts=args.cuts, adds=args.witness_add,
                                   isith=args.isith, nsith=args.nsith, toad=args.toad, data=data)
 
     doers = [rotDoer]
     return doers
 
 
 class GroupMultisigRotate(doing.DoDoer):
     """
     Command line DoDoer to launch the needed coroutines to run launch Multisig rotation.
        This DoDoer will remove the multisig coroutine and exit when it recieves a message
        that the multisig coroutine has successfully completed a cooperative rotation.
 
     """
 
-    def __init__(self, name, base, bran, alias, smids=None, rmids=None, isith=None, nsith=None,
+    def __init__(self, hby, alias, smids=None, rmids=None, isith=None, nsith=None,
                  toad=None, wits=None, cuts=None, adds=None, data: list = None):
 
         self.alias = alias
         self.isith = isith
         self.nsith = nsith
         self.toad = toad
         self.smids = smids
         self.rmids = rmids
         self.data = data
+        self.hby = hby
 
         self.wits = wits if wits is not None else []
         self.cuts = cuts if cuts is not None else []
         self.adds = adds if adds is not None else []
 
-        self.hby = existing.setupHby(name=name, base=base, bran=bran)
         self.hbyDoer = habbing.HaberyDoer(habery=self.hby)  # setup doer
         notifier = Notifier(self.hby)
         mux = grouping.Multiplexor(self.hby, notifier=notifier)
         exc = exchanging.Exchanger(hby=self.hby, handlers=[])
         grouping.loadHandlers(exc, mux)
 
         mbd = indirecting.MailboxDirector(hby=self.hby, topics=['/receipt', '/multisig', '/replay'], exc=exc)
```

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/shell.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/shell.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/multisig/update.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/update.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/clean.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/clean.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/generate.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/oobi/resolve.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/resolve.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/generate.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/remove.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/remove.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/passcode/set.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/set.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/query.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/rename.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/rename.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/rollback.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/rollback.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/rotate.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/rotate.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
         self.wits = wits if wits is not None else []
         self.cuts = cuts if cuts is not None else []
         self.adds = adds if adds is not None else []
 
         self.hby = existing.setupHby(name=name, base=base, bran=bran)
         self.hbyDoer = habbing.HaberyDoer(habery=self.hby)  # setup doer
-        self.swain = delegating.Anchorer(hby=self.hby)
+        self.swain = delegating.Anchorer(hby=self.hby, proxy=self.hby.habByName(self.proxy))
         self.postman = forwarding.Poster(hby=self.hby)
         self.mbx = indirecting.MailboxDirector(hby=self.hby, topics=['/receipt', "/replay", "/reply"])
         doers = [self.hbyDoer, self.mbx, self.swain, self.postman, doing.doify(self.rotateDo)]
 
         super(RotateDoer, self).__init__(doers=doers)
 
     def rotateDo(self, tymth, tock=0.0):
@@ -194,15 +194,15 @@
         auths = {}
         if self.authenticate:
             for wit in hab.kever.wits:
                 code = input(f"Entire code for {wit}: ")
                 auths[wit] = f"{code}#{helping.nowIso8601()}"
 
         if hab.kever.delpre:
-            self.swain.delegation(pre=hab.pre, sn=hab.kever.sn, proxy=self.hby.habByName(self.proxy))
+            self.swain.delegation(pre=hab.pre, sn=hab.kever.sn)
             print("Waiting for delegation approval...")
             while not self.swain.complete(hab.kever.prefixer, coring.Seqner(sn=hab.kever.sn)):
                 yield self.tock
 
         elif hab.kever.wits:
             if self.endpoint:
                 yield from receiptor.receipt(hab.pre, sn=hab.kever.sn, auths=auths)
```

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/saidify.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/saidify.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/salt.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/salt.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/sign.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/sign.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/ssh/export.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/ssh/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/status.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/vc/create.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/vc/create.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/vc/export.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/vc/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/vc/list.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/vc/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/incept.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/incept.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/list.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/vc/registry/status.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/status.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/vc/revoke.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/vc/revoke.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/verify.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/verify.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/version.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/watcher/add.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/watcher/add.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/witness/authenticate.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/witness/authenticate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/witness/demo.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/witness/demo.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/witness/start.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/witness/start.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/commands/witness/submit.py` & `keri-1.2.0.dev3/src/keri/app/cli/commands/witness/submit.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/common/config.py` & `keri-1.2.0.dev3/src/keri/app/cli/common/config.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/common/displaying.py` & `keri-1.2.0.dev3/src/keri/app/cli/common/displaying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/common/existing.py` & `keri-1.2.0.dev3/src/keri/app/cli/common/existing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/common/incepting.py` & `keri-1.2.0.dev3/src/keri/app/cli/common/incepting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/common/rotating.py` & `keri-1.2.0.dev3/src/keri/app/cli/common/rotating.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/cli/kli.py` & `keri-1.2.0.dev3/src/keri/app/cli/kli.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/configing.py` & `keri-1.2.0.dev3/src/keri/app/configing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/connecting.py` & `keri-1.2.0.dev3/src/keri/app/connecting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/delegating.py` & `keri-1.2.0.dev3/src/keri/app/delegating.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,58 +43,38 @@
         self.hby = hby
         self.postman = forwarding.Poster(hby=hby)
         self.witq = agenting.WitnessInquisitor(hby=hby)
         self.witDoer = agenting.Receiptor(hby=self.hby)
         self.proxy = proxy
 
         super(Anchorer, self).__init__(doers=[self.witq, self.witDoer, self.postman, doing.doify(self.escrowDo)],
-                                     **kwa)
+                                       **kwa)
 
     def delegation(self, pre, sn=None, proxy=None):
         if pre not in self.hby.habs:
             raise kering.ValidationError(f"{pre} is not a valid local AID for delegation")
 
+        if proxy is not None:
+            self.proxy = proxy
+
         # load the hab of the delegated identifier to anchor
         hab = self.hby.habs[pre]
         delpre = hab.kever.delpre  # get the delegator identifier
         if delpre not in hab.kevers:
             raise kering.ValidationError(f"delegator {delpre} not found, unable to process delegation")
 
-        dkever = hab.kevers[delpre]  # and the delegator's kever
         sn = sn if sn is not None else hab.kever.sner.num
 
         # load the event and signatures
         evt = hab.makeOwnEvent(sn=sn)
 
-        smids = []
-        if isinstance(hab, GroupHab):
-            phab = hab.mhab
-            smids = hab.smids
-        elif proxy is not None:
-            phab = proxy
-        elif hab.kever.sn > 0:
-            phab = hab
-        elif self.proxy is not None:
-            phab = self.proxy
-        else:
-            raise kering.ValidationError("no proxy to send messages for delegation")
-
         # Send exn message for notification purposes
-        exn, atc = delegateRequestExn(phab, delpre=delpre, evt=bytes(evt), aids=smids)
-
-        self.postman.send(hab=phab, dest=hab.kever.delpre, topic="delegate", serder=exn, attachment=atc)
-
         srdr = serdering.SerderKERI(raw=evt)
-        del evt[:srdr.size]
-        self.postman.send(hab=phab, dest=delpre, topic="delegate", serder=srdr, attachment=evt)
-
-        seal = dict(i=srdr.pre, s=srdr.snh, d=srdr.said)
-        self.witq.query(hab=phab, pre=dkever.prefixer.qb64, anchor=seal)
-
-        self.hby.db.dune.pin(keys=(srdr.pre, srdr.said), val=srdr)
+        self.witDoer.msgs.append(dict(pre=pre, sn=srdr.sn))
+        self.hby.db.dpwe.pin(keys=(srdr.pre, srdr.said), val=srdr)
 
     def complete(self, prefixer, seqner, saider=None):
         """ Check for completed delegation protocol for the specific event
 
         Parameters:
             prefixer (Prefixer): qb64 identifier prefix of event to check
             seqner (Seqner): sequence number of event to check
@@ -135,16 +115,16 @@
         _ = (yield self.tock)
 
         while True:
             self.processEscrows()
             yield 0.5
 
     def processEscrows(self):
-        self.processUnanchoredEscrow()
         self.processPartialWitnessEscrow()
+        self.processUnanchoredEscrow()
 
     def processUnanchoredEscrow(self):
         """
         Process escrow of partially signed multisig group KEL events.  Message
         processing will send this local controllers signature to all other participants
         then this escrow waits for signatures from all other participants
 
@@ -155,19 +135,18 @@
 
             seal = dict(i=serder.pre, s=serder.snh, d=serder.said)
             if dserder := self.hby.db.findAnchoringSealEvent(dkever.prefixer.qb64, seal=seal):
                 seqner = coring.Seqner(sn=dserder.sn)
                 couple = seqner.qb64b + dserder.saidb
                 dgkey = dbing.dgKey(kever.prefixer.qb64b, kever.serder.saidb)
                 self.hby.db.setAes(dgkey, couple)  # authorizer event seal (delegator/issuer)
-                self.witDoer.msgs.append(dict(pre=pre, sn=serder.sn))
 
                 # Move to escrow waiting for witness receipts
-                logger.info(f"Waiting for fully signed witness receipts for {serder.sn}")
-                self.hby.db.dpwe.pin(keys=(pre, said), val=serder)
+                logger.info(f"Delegation approval received, {serder.pre} confirmed")
+                self.hby.db.cdel.put(keys=(pre, coring.Seqner(sn=serder.sn).qb64), val=coring.Saider(qb64=serder.said))
                 self.hby.db.dune.rem(keys=(pre, said))
 
     def processPartialWitnessEscrow(self):
         """
         Process escrow of delegated events that do not have a full compliment of receipts
         from witnesses yet.  When receipting is complete, remove from escrow and cue up a message
         that the event is complete.
@@ -184,17 +163,41 @@
                 if len(kever.wits) > 0:
                     witnessed = False
                     for cue in self.witDoer.cues:
                         if cue["pre"] == serder.pre and cue["sn"] == seqner.sn:
                             witnessed = True
                     if not witnessed:
                         continue
-                logger.info(f"Witness receipts complete, {pre} confirmed.")
+                logger.info(f"Witness receipts complete, waiting for delegation approval.")
+                hab = self.hby.habs[pre]
+                delpre = hab.kever.delpre  # get the delegator identifier
+                dkever = hab.kevers[delpre]  # and the delegator's kever
+                smids = []
+                if isinstance(hab, GroupHab):
+                    phab = hab.mhab
+                    smids = hab.smids
+                elif self.proxy is not None:
+                    phab = self.proxy
+                else:
+                    raise kering.ValidationError("no proxy to send messages for delegation")
+
+                evt = hab.db.cloneEvtMsg(pre=serder.pre, fn=0, dig=serder.said)
+                exn, atc = delegateRequestExn(phab, delpre=delpre, evt=bytes(evt), aids=smids)
+
+                self.postman.send(hab=phab, dest=hab.kever.delpre, topic="delegate", serder=exn, attachment=atc)
+
+                srdr = serdering.SerderKERI(raw=evt)
+                del evt[:srdr.size]
+                self.postman.send(hab=phab, dest=delpre, topic="delegate", serder=srdr, attachment=evt)
+
+                seal = dict(i=srdr.pre, s=srdr.snh, d=srdr.said)
+                self.witq.query(hab=phab, pre=dkever.prefixer.qb64, anchor=seal)
+
                 self.hby.db.dpwe.rem(keys=(pre, said))
-                self.hby.db.cdel.put(keys=(pre, seqner.qb64), val=coring.Saider(qb64=serder.said))
+                self.hby.db.dune.pin(keys=(srdr.pre, srdr.said), val=srdr)
 
 
 def loadHandlers(hby, exc, notifier):
     """ Load handlers for the peer-to-peer delegation protocols
 
     Parameters:
         hby (Habery): Database and keystore for environment
```

### Comparing `keri-1.2.0.dev2/src/keri/app/directing.py` & `keri-1.2.0.dev3/src/keri/app/directing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/forwarding.py` & `keri-1.2.0.dev3/src/keri/app/forwarding.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/grouping.py` & `keri-1.2.0.dev3/src/keri/app/grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,19 +43,15 @@
 
             ghab (Hab): group Habitat
             prefixer (Prefixer): prefixer of group identifier
             seqner (Seqner): seqner of event of group identifier
             saider (Saider): saider of event of group identifier
 
         """
-        evt = ghab.makeOwnEvent(sn=seqner.sn, allowPartiallySigned=True)
-        serder = serdering.SerderKERI(raw=evt)
-        del evt[:serder.size]
-
-        logger.info(f"Waiting for other signatures for {serder.pre}:{seqner.sn}...")
+        print(f"Waiting for other signatures for {prefixer.qb64}:{seqner.sn}...")
         return self.hby.db.gpse.add(keys=(prefixer.qb64,), val=(seqner, saider))
 
     def complete(self, prefixer, seqner, saider=None):
         """ Check for completed multsig protocol for the specific event
 
         Parameters:
             prefixer (Prefixer): qb64 identifier prefix of event to check
```

### Comparing `keri-1.2.0.dev2/src/keri/app/habbing.py` & `keri-1.2.0.dev3/src/keri/app/habbing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/httping.py` & `keri-1.2.0.dev3/src/keri/app/httping.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/indirecting.py` & `keri-1.2.0.dev3/src/keri/app/indirecting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/keeping.py` & `keri-1.2.0.dev3/src/keri/app/keeping.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/notifying.py` & `keri-1.2.0.dev3/src/keri/app/notifying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/oobiing.py` & `keri-1.2.0.dev3/src/keri/app/oobiing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/querying.py` & `keri-1.2.0.dev3/src/keri/app/querying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/signaling.py` & `keri-1.2.0.dev3/src/keri/app/signaling.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/signing.py` & `keri-1.2.0.dev3/src/keri/app/signing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/specing.py` & `keri-1.2.0.dev3/src/keri/app/specing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/app/storing.py` & `keri-1.2.0.dev3/src/keri/app/storing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/core/coring.py` & `keri-1.2.0.dev3/src/keri/core/coring.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/core/counting.py` & `keri-1.2.0.dev3/src/keri/core/counting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/core/eventing.py` & `keri-1.2.0.dev3/src/keri/core/eventing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1705,41 +1705,32 @@
 
         """
         # assumes stale group membership is taken care of by presence of groups
         # i.e where once a local member but no more.
         pre = pre if pre is not None else self.prefixer.qb64
         return pre in self.groups  # groups
 
-
     def locallyContributedIndices(self, verfers: list[Verfer]):
         """Returns list of indices of public keys contributed by local members
         to the KEL with current signing keys represented by verfers
 
         Using the pubs index to find members of a signing group
 
         Parameters:
             verfers (list[Verfer]): instance for each current signing key
 
         Returns:
             indices list[int]: list of indices of keys contributed by local members
 
         """
-        indices = []
-
-        for i, verfer in enumerate(verfers):
-            if (couples := self.pubs.get(keys=(verfer.qb64,))) is None:
-                continue
-
-            for (prefixer, seqner) in couples:
-                if self.locallyOwned(prefixer.qb64):  # only member not group aid
-                    indices.append(i)
-                    break  # only need one local member to exclude signature
-
-        return indices
+        habord = self.db.habs.get(keys=(self.prefixer.qb64,))
+        kever = self.kevers[habord.mid]
 
+        idx = [verfer.qb64 for verfer in verfers].index(kever.verfers[0].qb64)
+        return [idx]
 
     def reload(self, state):
         """
         Reload Kever attributes (aka its state) from state (KeyStateRecord)
 
         Parameters:
             state (KeyStateRecord | None): instance for key state notice
@@ -2223,21 +2214,23 @@
                                             serder.ked))
 
         # Filters sigers to remove any signatures from locally membered groups
         # when not local (remote) event source. So that attacker can't source
         # compromised signature remotely to satisfy threshold.
 
         if not local and self.locallyMembered():  # is this Kever's pre a local group
-            if (indices := self.locallyContributedIndices(verfers)):
+            if indices := self.locallyContributedIndices(verfers):
                 for siger in list(sigers):  # copy so clean del on original elements
                     if siger.index in indices:
-                        del sigers[siger.index]
-                        self.cues.push(dict(kin="remoteMemberedSig",
-                                            serder=serder,
-                                              index=siger.index))
+                        sigers.remove(siger)
+                        if self.cues:
+                            self.cues.push(dict(kin="remoteMemberedSig",
+                                                serder=serder,
+                                                index=siger.index))
+
 
         # get unique verified sigers and indices lists from sigers list
         sigers, indices = verifySigs(raw=serder.raw, sigers=sigers, verfers=verfers)
         # sigers  now have .verfer assigned
 
         # check if minimally signed in order to continue processing
         if not indices:  # must have a least one verified sig
@@ -2251,29 +2244,29 @@
                  self.locallyWitnessed(wits=wits))):
             self.escrowMFEvent(serder=serder, sigers=sigers, wigers=wigers,
                                    seqner=delseqner, saider=delsaider, local=local)
             raise MisfitEventSourceError(f"Nonlocal source for locally owned"
                                              f"or locally witnessed event"
                                                  f" = {serder.ked}.")
 
-
         werfers = [Verfer(qb64=wit) for wit in wits]  # get witness public key verifiers
         # get unique verified wigers and windices lists from wigers list
         wigers, windices = verifySigs(raw=serder.raw, sigers=wigers, verfers=werfers)
         # each wiger now has added to it a werfer of its wit in its .verfer property
 
         # escrow if not fully signed vs signing threshold
         if not tholder.satisfy(indices):  # at least one but not enough
             self.escrowPSEvent(serder=serder, sigers=sigers, wigers=wigers, local=local)
             if delseqner and delsaider:
                 self.escrowPACouple(serder=serder, seqner=delseqner, saider=delsaider)
             raise MissingSignatureError(f"Failure satisfying sith = {tholder.sith}"
                                         f" on sigs for {[siger.qb64 for siger in sigers]}"
                                         f" for evt = {serder.ked}.")
 
+
         # escrow if not fully signed vs prior next rotation threshold
         if serder.ilk in (Ilks.rot, Ilks.drt):  # rotation so check prior next threshold
             # prior next threshold in .ntholder and digers in .ndigers
             ondices = self.exposeds(sigers)
             if not self.ntholder.satisfy(indices=ondices):
                 self.escrowPSEvent(serder=serder, sigers=sigers, wigers=wigers, local=local)
                 if delseqner and delsaider:  # save in case not attached later
@@ -2302,15 +2295,15 @@
                                seqner=delseqner, saider=delsaider, local=local)
             raise MisfitEventSourceError(f"Nonlocal source  for locally"
                                                  f" delegated by {delpre} of"
                                                  f"event = {serder.ked}.")
 
         # short circuit witness validation when either locallyOwned or locallyWitnessed
         # otherwise must validate fully witnessed
-        if not (self.locallyOwned() or self.locallyWitnessed(wits=wits)):
+        if not (self.locallyOwned() or self.locallyMembered() or self.locallyWitnessed(wits=wits)):
             if wits:  # is witnessed
                 if toader.num < 1 or toader.num > len(wits):  # out of bounds toad
                     raise ValidationError(f"Invalid toad = {toader.num} for wits = {wits}")
             else:  # not witnessed
                 if toader.num != 0:  # invalid toad
                     raise ValidationError(f"Invalid toad = {toader.num} for wits = {wits}")
 
@@ -2635,46 +2628,24 @@
                 # promote to local and reprocess event before we get to here
                 self.escrowDelegableEvent(serder=serder, sigers=sigers,
                                           wigers=wigers,local=local)
                 raise MissingDelegableApprovalError(f"Missing approval for "
                                                     f" delegation by {delpre} of"
                                                          f"event = {serder.ked}.")
 
-                # ToDo XXXX This logic moves to the Delegable escrow processing
-                # ToDo XXXX create process escrow for delegable events "dees."
-                #in order to get delegator approval
-                # any virtual delegation or sandboxing logic happens there
-                # create virtual anchor seal so local delegator can evaluate
-                # superseding logic with provisional virtual seal
-                #dkever = self.kevers[delpre]
-                #dseal = SealEvent(i=serder.pre, s=serder.snh, d=serder.said)
-                #dserder = interact(pre=dkever.prefixer.qb64,
-                                           #dig=dkever.serder.said,
-                                           #sn=dkever.sner.num + 1,
-                                           #data=[dseal._asdict()])
-                #delseqner = coring.Seqner(snh=dserder.snh)
-                #delsaider = coring.Saider(qb64=dserder.said)
-                # ToDo XXXX  need to cue task here  to approve delegation by generating
-                # an anchoring SealEvent of serder in delegators KEL
-                # may include MFA and or business logic for the delegator i.e. is local
-                # event that designates this controller as delegator triggers
-                # this cue to approave delegation
                 #self.cues.push(dict(kin="approveDelegation",
                                         #delegator=kever.delpre,
                                         #serder=serder))
 
-
             else:  # not local delegator so escrow
                 self.escrowPSEvent(serder=serder, sigers=sigers, wigers=wigers, local=local)
                 raise MissingDelegationError(f"No delegation seal for delegator "
                                          "{delpre} of evt = {serder.ked}.")
 
-        #ssn = validateSN(sn=delseqner.snh, inceptive=False)  # delseqner Number should already do this
         ssn = Number(num=delseqner.sn).validate(inceptive=False).sn
-        #ssn = sner.num sner is Number seqner is Seqner
         # ToDo XXXX need to replace Seqners with Numbers
 
         # get the dig of the delegating event. Using getKeLast ensures delegating
         #  event has not already been superceded
         key = snKey(pre=delpre, sn=ssn)  # database key
         raw = self.db.getKeLast(key)  # get dig of delegating event
```

### Comparing `keri-1.2.0.dev2/src/keri/core/indexing.py` & `keri-1.2.0.dev3/src/keri/core/indexing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/core/parsing.py` & `keri-1.2.0.dev3/src/keri/core/parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -990,18 +990,18 @@
                                      delsaider=delsaider,
                                      firner=firner,
                                      dater=dater,
                                      local=local)
 
                     if cigars:
                         kvy.processAttachedReceiptCouples(serder, cigars,
-                                                    firner=firner, local=local)
+                                                          firner=firner, local=local)
                     if trqs:
                         kvy.processAttachedReceiptQuadruples(serder, trqs,
-                                                    firner=firner, local=local)
+                                                             firner=firner, local=local)
 
                 except AttributeError as ex:
                     raise kering.ValidationError("No kevery to process so dropped msg"
                                                  "= {}.".format(serder.pretty())) from ex
 
             elif ilk in [Ilks.rct]:  # event receipt msg (nontransferable)
                 if not (cigars or wigers or tsgs):
```

### Comparing `keri-1.2.0.dev2/src/keri/core/routing.py` & `keri-1.2.0.dev3/src/keri/core/routing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/core/scheming.py` & `keri-1.2.0.dev3/src/keri/core/scheming.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/core/serdering.py` & `keri-1.2.0.dev3/src/keri/core/serdering.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/core/signing.py` & `keri-1.2.0.dev3/src/keri/core/signing.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,52 +21,14 @@
 
 
 DSS_SIG_MODE = "fips-186-3"
 ECDSA_256r1_SEEDBYTES = 32
 ECDSA_256k1_SEEDBYTES = 32
 
 
-# deprecated use Salter.signers instead
-def generateSigners(raw=None, count=8, transferable=True):
-    """Returns list of Signers for Ed25519
-
-    Deprecated, use Salter.signers instead.
-
-    Use this when simply need valid AIDs but not when need valid controller
-    contexts. In the latter case use openHby or openHab which create databases.
-
-    Parameters:
-        raw (bytes):  16 byte long salt cryptomatter from which seeds
-            for Signers in list are derived
-            random salt created if not provided
-        count is number of signers in list
-        transferable is boolean true means signer.verfer code is transferable
-                                non-transferable otherwise
-    """
-    if not raw:
-        raw = pysodium.randombytes(pysodium.crypto_pwhash_SALTBYTES)
-
-    signers = []
-    for i in range(count):
-        path = f"{i:x}"
-        # algorithm default is argon2id
-        seed = pysodium.crypto_pwhash(outlen=32,
-                                      passwd=path,
-                                      salt=raw,
-                                      opslimit=2,  # pysodium.crypto_pwhash_OPSLIMIT_INTERACTIVE,
-                                      memlimit=67108864,  # pysodium.crypto_pwhash_MEMLIMIT_INTERACTIVE,
-                                      alg=pysodium.crypto_pwhash_ALG_ARGON2ID13)
-
-        signers.append(Signer(raw=seed, transferable=transferable))
-
-    return signers
-
-
-
-
 class Signer(Matter):
     """
     Signer is Matter subclass with method to create signature of serialization
     using:
         .raw as signing (private) key seed,
         .code as cipher suite for signing
         .verfer whose property .raw is public key for signing.
```

### Comparing `keri-1.2.0.dev2/src/keri/core/streaming.py` & `keri-1.2.0.dev3/src/keri/core/streaming.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/core/structing.py` & `keri-1.2.0.dev3/src/keri/core/structing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/db/basing.py` & `keri-1.2.0.dev3/src/keri/db/basing.py`

 * *Files 0% similar despite different names*

```diff
@@ -945,15 +945,15 @@
                                    schema=EventSourceRecord,
                                    subkey='esrs.')
 
         # misfit escrows whose processing may change the .esrs event source record
         self.misfits = subing.IoSetSuber(db=self, subkey='mfes.')
 
         # delegable events escrows. events with local delegator that need approval
-        self.delegables = subing.CesrIoSetSuber(db=self, subkey='dees.', klas=coring.Diger)
+        self.delegables = subing.IoSetSuber(db=self, subkey='dees.')
 
         # events as ordered by first seen ordinals
         self.fons = subing.CesrSuber(db=self, subkey='fons.', klas=core.Number)
         # Kever state made of KeyStateRecord key states
         # TODO: clean
         self.states = koming.Komer(db=self,
                                    schema=KeyStateRecord,
@@ -1496,17 +1496,14 @@
 
         # add authorizer (delegator/issuer) source seal event couple to attachments
         couple = self.getAes(dgkey)
         if couple is not None:
             atc.extend(coring.Counter(code=coring.CtrDex.SealSourceCouples,
                                       count=1).qb64b)
             atc.extend(couple)
-        elif self.kevers[pre].delegated:
-            if coring.SerderKERI(raw=raw).estive:
-                raise kering.MissingEntryError("Missing delegator anchor seal for dig={}.".format(dig))
 
         # add trans endorsement quadruples to attachments not controller
         # may have been originally key event attachments or receipted endorsements
         if quads := self.getVrcs(key=dgkey):
             atc.extend(coring.Counter(code=coring.CtrDex.TransReceiptQuadruples,
                                       count=len(quads)).qb64b)
             for quad in quads:
```

### Comparing `keri-1.2.0.dev2/src/keri/db/dbing.py` & `keri-1.2.0.dev3/src/keri/db/dbing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/db/escrowing.py` & `keri-1.2.0.dev3/src/keri/db/escrowing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/db/koming.py` & `keri-1.2.0.dev3/src/keri/db/koming.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/db/migrations/rekey_habs.py` & `keri-1.2.0.dev3/src/keri/db/migrations/rekey_habs.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/db/subing.py` & `keri-1.2.0.dev3/src/keri/db/subing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/demo/demo_bob.py` & `keri-1.2.0.dev3/src/keri/demo/demo_bob.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/demo/demo_eve.py` & `keri-1.2.0.dev3/src/keri/demo/demo_eve.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/demo/demo_kev.py` & `keri-1.2.0.dev3/src/keri/demo/demo_kev.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/demo/demo_sam.py` & `keri-1.2.0.dev3/src/keri/demo/demo_sam.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/demo/demoing.py` & `keri-1.2.0.dev3/src/keri/demo/demoing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/end/ending.py` & `keri-1.2.0.dev3/src/keri/end/ending.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/end/priming.py` & `keri-1.2.0.dev3/src/keri/end/priming.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/help/__init__.py` & `keri-1.2.0.dev3/src/keri/help/__init__.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/help/helping.py` & `keri-1.2.0.dev3/src/keri/help/helping.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/kering.py` & `keri-1.2.0.dev3/src/keri/kering.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/peer/exchanging.py` & `keri-1.2.0.dev3/src/keri/peer/exchanging.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/vc/protocoling.py` & `keri-1.2.0.dev3/src/keri/vc/protocoling.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/vc/proving.py` & `keri-1.2.0.dev3/src/keri/vc/proving.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/vc/walleting.py` & `keri-1.2.0.dev3/src/keri/vc/walleting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/vdr/credentialing.py` & `keri-1.2.0.dev3/src/keri/vdr/credentialing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/vdr/eventing.py` & `keri-1.2.0.dev3/src/keri/vdr/eventing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/vdr/verifying.py` & `keri-1.2.0.dev3/src/keri/vdr/verifying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri/vdr/viring.py` & `keri-1.2.0.dev3/src/keri/vdr/viring.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/src/keri.egg-info/PKG-INFO` & `keri-1.2.0.dev3/src/keri.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keri
-Version: 1.2.0.dev2
+Version: 1.2.0.dev3
 Summary: Key Event Receipt Infrastructure
 Home-page: https://github.com/WebOfTrust/keripy
 Author: Samuel M. Smith
 Author-email: smith.samuel.m@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://keri.readthedocs.io/
 Project-URL: Changelog, https://keri.readthedocs.io/en/latest/changelog.html
```

### Comparing `keri-1.2.0.dev2/src/keri.egg-info/SOURCES.txt` & `keri-1.2.0.dev3/src/keri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev2/tests/test_kering.py` & `keri-1.2.0.dev3/tests/test_kering.py`

 * *Files identical despite different names*

