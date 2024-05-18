# Comparing `tmp/SimplHDL-0.0.4.tar.gz` & `tmp/simplhdl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimplHDL-0.0.4.tar", last modified: Thu Apr 11 13:40:01 2024, max compression
+gzip compressed data, was "simplhdl-0.0.5.tar", last modified: Sat May 18 15:34:33 2024, max compression
```

## Comparing `SimplHDL-0.0.4.tar` & `simplhdl-0.0.5.tar`

### file list

```diff
@@ -1,228 +1,229 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.193458 SimplHDL-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.201458 SimplHDL-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.201458 SimplHDL-0.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.201458 SimplHDL-0.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    50717 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/_static/simplhdl_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)   111558 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/_static/simplhdl_light.png
--rw-r--r--   0 runner    (1001) docker     (127)    38948 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/_static/simplhdl_light_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20233 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/drawing.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/docs/flows/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows/ghdl.rst
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows/icarus.rst
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows/quartus.rst
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows/questasim.rst
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows/vcs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows/vivado.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows/xsim.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows.rst
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/intel-ips.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/hdl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/adder/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/adder.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/adder/hdl/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/hdl/adder.sv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/adder/sim/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/sim/testbench.sv
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/sim/testbench.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/adder/syn/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/syn/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/syn/placement.xdc
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/syn/timing.xdc
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/syn/top.sv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/alu/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/alu.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/alu/hdl/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/hdl/add.sv
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/hdl/alu.sv
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/hdl/mul.sv
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/hdl/sub.sv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/hdl/alu/sim/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/aluif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/sequenceitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/sequencer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/clock_vip/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/clock_vip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/clock_vip/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/clock_vip/clockif.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/pyuvm.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/test/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/test/seq_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/testbench.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/agent.svh
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/alu_vip.sv
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/alu_vip.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/driver.svh
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/env.svh
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/monitor.svh
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/sequence_item.svh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/seq_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/seq_lib/add_seq.svh
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/seq_lib/base_seq.svh
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/tb_env.sv
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/tb_env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/test/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/test/base_test.svh
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/test/test_add.svh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testbench/
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testbench/alu_if.sv
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testbench/testbench.sv
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testbench/testbench.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testcases/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testcases/test_add/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testcases/test_add/test_add.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.213458 SimplHDL-0.0.4/examples/hdl/alu/syn/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/syn/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/syn/placement.xdc
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/syn/timing.xdc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.213458 SimplHDL-0.0.4/examples/hdl/hello/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/hello/build.sbt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/hello/hello.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/hdl/hello/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/hdl/hello/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.213458 SimplHDL-0.0.4/examples/hdl/hello/src/main/scala/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/hello/src/main/scala/Hello.scala
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.213458 SimplHDL-0.0.4/examples/hdl/hello/syn/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/hello/syn/build.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.213458 SimplHDL-0.0.4/examples/plugins/simple_parser/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/plugins/simple_parser/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/plugins/simple_parser/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.213458 SimplHDL-0.0.4/examples/plugins/simple_parser/src/simple_parser/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/plugins/simple_parser/src/simple_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/plugins/simple_parser/src/simple_parser/simple_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/src/SimplHDL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-11 13:40:01.000000 SimplHDL-0.0.4/src/SimplHDL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-04-11 13:40:01.000000 SimplHDL-0.0.4/src/SimplHDL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:40:01.000000 SimplHDL-0.0.4/src/SimplHDL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 13:40:01.000000 SimplHDL-0.0.4/src/SimplHDL.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-11 13:40:01.000000 SimplHDL-0.0.4/src/SimplHDL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 13:40:01.000000 SimplHDL-0.0.4/src/SimplHDL.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/cocotb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/flows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/implementationflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/modelsimflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/quartusflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/flows/questasim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/questasim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/questasim/questasimflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/flows/rivierapro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/rivierapro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/rivierapro/rivieraproflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/simulationflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/flows/vcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/vcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/vcs/vcsflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/vivadoflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/flows/xsim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/xsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/xsim/xsimflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/generators/chisel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/generators/ipxact.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/generators/spd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/generators/systemrdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/parsers/fusesocparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/parsers/simplhdlparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.221458 SimplHDL-0.0.4/src/simplhdl/pyedaa/
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/pyedaa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/pyedaa/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/pyedaa/design.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/pyedaa/fileset.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/pyedaa/filetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/pyedaa/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/pyedaa/vhdllibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.221458 SimplHDL-0.0.4/src/simplhdl/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.221458 SimplHDL-0.0.4/src/simplhdl/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.221458 SimplHDL-0.0.4/src/simplhdl/resources/templates/quartus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/quartus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/quartus/project.tcl.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/quartus/run.tcl.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.221458 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/Makefile.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/cocotb.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/dependencies.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/files.j2
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/fileset.j2
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/project.mk.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.221458 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/Makefile.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/cocotb.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/dependencies.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/files.j2
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/fileset.j2
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/project.mk.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/Makefile.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/cocotb.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/dependencies.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/files.j2
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/fileset.j2
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/pli.tab.j2
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/project.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/synopsys_sim.setup.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/launch_run.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/project.tcl.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/run.tcl.j2
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/steps.tcl.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/Makefile.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/cocotb.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/dependencies.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/files.j2
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/fileset.j2
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/project.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/simplhdl.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/tests/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.080980 simplhdl-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.040980 simplhdl-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.048980 simplhdl-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-18 15:34:28.000000 simplhdl-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-18 15:34:28.000000 simplhdl-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-18 15:34:28.000000 simplhdl-0.0.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-18 15:34:28.000000 simplhdl-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-18 15:34:33.080980 simplhdl-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-18 15:34:28.000000 simplhdl-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.048980 simplhdl-0.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.048980 simplhdl-0.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    50717 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/_static/simplhdl_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111558 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/_static/simplhdl_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38948 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/_static/simplhdl_light_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20233 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/drawing.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.052980 simplhdl-0.0.5/docs/flows/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/flows/ghdl.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/flows/icarus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/flows/quartus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/flows/questasim.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/flows/vcs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/flows/vivado.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/flows/xsim.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/flows.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/intel-ips.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-18 15:34:28.000000 simplhdl-0.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.044980 simplhdl-0.0.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.044980 simplhdl-0.0.5/examples/hdl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.052980 simplhdl-0.0.5/examples/hdl/adder/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/adder/adder.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.052980 simplhdl-0.0.5/examples/hdl/adder/hdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/adder/hdl/adder.sv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.052980 simplhdl-0.0.5/examples/hdl/adder/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/adder/sim/testbench.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/adder/sim/testbench.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.052980 simplhdl-0.0.5/examples/hdl/adder/syn/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/adder/syn/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/adder/syn/placement.xdc
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/adder/syn/timing.xdc
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/adder/syn/top.sv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.052980 simplhdl-0.0.5/examples/hdl/alu/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/alu.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.052980 simplhdl-0.0.5/examples/hdl/alu/hdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/hdl/add.sv
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/hdl/alu.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/hdl/mul.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/hdl/sub.sv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.040980 simplhdl-0.0.5/examples/hdl/alu/sim/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.052980 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.056980 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/alu_vip/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/alu_vip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/alu_vip/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/alu_vip/aluif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/alu_vip/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/alu_vip/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/alu_vip/sequenceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/alu_vip/sequencer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.056980 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/clock_vip/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/clock_vip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/clock_vip/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/clock_vip/clockif.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/pyuvm.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.056980 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/test/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/test/seq_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/testbench.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.044980 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.056980 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/alu_vip/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/alu_vip/agent.svh
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/alu_vip/alu_vip.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/alu_vip/alu_vip.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/alu_vip/driver.svh
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/alu_vip/env.svh
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/alu_vip/monitor.svh
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/alu_vip/sequence_item.svh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.060980 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/tb_env/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.060980 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/tb_env/seq_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/tb_env/seq_lib/add_seq.svh
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/tb_env/seq_lib/base_seq.svh
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/tb_env/tb_env.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/tb_env/tb_env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.060980 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/tb_env/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/tb_env/test/base_test.svh
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/tb_env/test/test_add.svh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.060980 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/testbench/
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/testbench/alu_if.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/testbench/testbench.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/testbench/testbench.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.044980 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/testcases/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.060980 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/testcases/test_add/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/sim/uvm/testcases/test_add/test_add.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.060980 simplhdl-0.0.5/examples/hdl/alu/syn/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/syn/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/syn/placement.xdc
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/alu/syn/timing.xdc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.060980 simplhdl-0.0.5/examples/hdl/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/hello/build.sbt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/hello/hello.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.044980 simplhdl-0.0.5/examples/hdl/hello/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.044980 simplhdl-0.0.5/examples/hdl/hello/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.060980 simplhdl-0.0.5/examples/hdl/hello/src/main/scala/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/hello/src/main/scala/Hello.scala
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.060980 simplhdl-0.0.5/examples/hdl/hello/syn/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/hdl/hello/syn/build.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.044980 simplhdl-0.0.5/examples/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.060980 simplhdl-0.0.5/examples/plugins/simple_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/plugins/simple_parser/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.044980 simplhdl-0.0.5/examples/plugins/simple_parser/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.060980 simplhdl-0.0.5/examples/plugins/simple_parser/src/simple_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/plugins/simple_parser/src/simple_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-18 15:34:28.000000 simplhdl-0.0.5/examples/plugins/simple_parser/src/simple_parser/simple_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-18 15:34:28.000000 simplhdl-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:34:33.080980 simplhdl-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.044980 simplhdl-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.076980 simplhdl-0.0.5/src/SimplHDL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-18 15:34:32.000000 simplhdl-0.0.5/src/SimplHDL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-18 15:34:33.000000 simplhdl-0.0.5/src/SimplHDL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:34:32.000000 simplhdl-0.0.5/src/SimplHDL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-18 15:34:32.000000 simplhdl-0.0.5/src/SimplHDL.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-18 15:34:32.000000 simplhdl-0.0.5/src/SimplHDL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 15:34:32.000000 simplhdl-0.0.5/src/SimplHDL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.064980 simplhdl-0.0.5/src/simplhdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/cocotb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.064980 simplhdl-0.0.5/src/simplhdl/flows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flows/implementationflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flows/modelsimflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flows/quartusflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.068980 simplhdl-0.0.5/src/simplhdl/flows/questasim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flows/questasim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flows/questasim/questasimflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.068980 simplhdl-0.0.5/src/simplhdl/flows/rivierapro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flows/rivierapro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flows/rivierapro/rivieraproflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flows/simulationflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.068980 simplhdl-0.0.5/src/simplhdl/flows/vcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flows/vcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7878 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flows/vcs/vcsflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flows/vivadoflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.068980 simplhdl-0.0.5/src/simplhdl/flows/xsim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flows/xsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/flows/xsim/xsimflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.068980 simplhdl-0.0.5/src/simplhdl/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/generators/chisel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/generators/ipxact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/generators/spd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/generators/systemrdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.068980 simplhdl-0.0.5/src/simplhdl/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/parsers/fusesocparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/parsers/simplhdlparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.072980 simplhdl-0.0.5/src/simplhdl/pyedaa/
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/pyedaa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/pyedaa/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/pyedaa/design.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/pyedaa/fileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/pyedaa/filetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/pyedaa/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/pyedaa/vhdllibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.072980 simplhdl-0.0.5/src/simplhdl/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.072980 simplhdl-0.0.5/src/simplhdl/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.072980 simplhdl-0.0.5/src/simplhdl/resources/templates/quartus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/quartus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/quartus/project.tcl.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/quartus/run.tcl.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.072980 simplhdl-0.0.5/src/simplhdl/resources/templates/questasim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/questasim/Makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/questasim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/questasim/cocotb.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/questasim/dependencies.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/questasim/files.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/questasim/fileset.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/questasim/project.mk.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.072980 simplhdl-0.0.5/src/simplhdl/resources/templates/rivierapro/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/rivierapro/Makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/rivierapro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/rivierapro/cocotb.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/rivierapro/dependencies.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/rivierapro/files.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/rivierapro/fileset.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/rivierapro/project.mk.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.076980 simplhdl-0.0.5/src/simplhdl/resources/templates/vcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vcs/Makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vcs/cocotb.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vcs/dependencies.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vcs/files.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vcs/fileset.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vcs/pli.tab.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vcs/project.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vcs/synopsys_sim.setup.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vcs/vcs.parameters.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.076980 simplhdl-0.0.5/src/simplhdl/resources/templates/vivado/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vivado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vivado/launch_run.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vivado/project.tcl.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vivado/run.tcl.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/vivado/steps.tcl.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.076980 simplhdl-0.0.5/src/simplhdl/resources/templates/xsim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/xsim/Makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/xsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/xsim/cocotb.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/xsim/dependencies.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/xsim/files.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/xsim/fileset.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/resources/templates/xsim/project.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/simplhdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-18 15:34:28.000000 simplhdl-0.0.5/src/simplhdl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:34:33.076980 simplhdl-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-18 15:34:28.000000 simplhdl-0.0.5/tests/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-18 15:34:28.000000 simplhdl-0.0.5/tox.ini
```

### Comparing `SimplHDL-0.0.4/.github/workflows/publish.yml` & `simplhdl-0.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/.gitignore` & `simplhdl-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/.readthedocs.yaml` & `simplhdl-0.0.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/LICENSE` & `simplhdl-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/PKG-INFO` & `simplhdl-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimplHDL
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework for simulating and implementing HDL designs
 Author-email: Rasmus Grøndahl Olsen <simplhdl@gmail.com>
 Maintainer-email: Rasmus Grøndahl Olsen <simplhdl@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 SimplHDL
         
@@ -47,14 +47,15 @@
 Requires-Dist: pySVModel==0.3.5
 Requires-Dist: pyEDAA.ProjectModel==0.4.3
 Requires-Dist: pyyaml
 Requires-Dist: types-PyYAML
 Requires-Dist: argcomplete
 Requires-Dist: jinja2
 Requires-Dist: GitPython
+Requires-Dist: rich
 
 ## Introduction
 
 SimplHDL is a plugin-based command-line application for simplifying FPGA and
 ASIC development regardless of EDA tools and flows.
 
 The goal is to embrase structured and reusable designs by creating a generic
```

### Comparing `SimplHDL-0.0.4/README.md` & `simplhdl-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/docs/_static/simplhdl_dark.png` & `simplhdl-0.0.5/docs/_static/simplhdl_dark.png`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/docs/_static/simplhdl_light.png` & `simplhdl-0.0.5/docs/_static/simplhdl_light.png`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/docs/_static/simplhdl_light_1.png` & `simplhdl-0.0.5/docs/_static/simplhdl_light_1.png`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/docs/conf.py` & `simplhdl-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/docs/drawing.svg` & `simplhdl-0.0.5/docs/drawing.svg`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/docs/flows/vivado.rst` & `simplhdl-0.0.5/docs/flows/vivado.rst`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/docs/index.rst` & `simplhdl-0.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/docs/intel-ips.md` & `simplhdl-0.0.5/docs/intel-ips.md`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/docs/plugins.rst` & `simplhdl-0.0.5/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/docs/requirements.txt` & `simplhdl-0.0.5/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/adder/syn/placement.xdc` & `simplhdl-0.0.5/examples/hdl/adder/syn/placement.xdc`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/hdl/alu.sv` & `simplhdl-0.0.5/examples/hdl/alu/hdl/alu.sv`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/agent.py` & `simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/alu_vip/agent.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/driver.py` & `simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/alu_vip/driver.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/monitor.py` & `simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/alu_vip/monitor.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/sequenceitem.py` & `simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/alu_vip/sequenceitem.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/clock_vip/agent.py` & `simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/clock_vip/agent.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/test/seq_lib.py` & `simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/test/seq_lib.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/test/test.py` & `simplhdl-0.0.5/examples/hdl/alu/sim/pyuvm/test/test.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/agent.svh` & `simplhdl-0.0.5/examples/hdl/alu/sim/uvm/alu_vip/agent.svh`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/driver.svh` & `simplhdl-0.0.5/examples/hdl/alu/sim/uvm/alu_vip/driver.svh`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/monitor.svh` & `simplhdl-0.0.5/examples/hdl/alu/sim/uvm/alu_vip/monitor.svh`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/sequence_item.svh` & `simplhdl-0.0.5/examples/hdl/alu/sim/uvm/alu_vip/sequence_item.svh`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/seq_lib/base_seq.svh` & `simplhdl-0.0.5/examples/hdl/alu/sim/uvm/tb_env/seq_lib/base_seq.svh`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/test/base_test.svh` & `simplhdl-0.0.5/examples/hdl/alu/sim/uvm/tb_env/test/base_test.svh`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/test/test_add.svh` & `simplhdl-0.0.5/examples/hdl/alu/sim/uvm/tb_env/test/test_add.svh`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testbench/alu_if.sv` & `simplhdl-0.0.5/examples/hdl/alu/sim/uvm/testbench/alu_if.sv`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testbench/testbench.sv` & `simplhdl-0.0.5/examples/hdl/alu/sim/uvm/testbench/testbench.sv`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/alu/syn/placement.xdc` & `simplhdl-0.0.5/examples/hdl/alu/syn/placement.xdc`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/hdl/hello/src/main/scala/Hello.scala` & `simplhdl-0.0.5/examples/hdl/hello/src/main/scala/Hello.scala`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/examples/plugins/simple_parser/src/simple_parser/simple_parser.py` & `simplhdl-0.0.5/examples/plugins/simple_parser/src/simple_parser/simple_parser.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/pyproject.toml` & `simplhdl-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "pySVModel==0.3.5",
     "pyEDAA.ProjectModel==0.4.3",
     "pyyaml",
     "types-PyYAML",
     "argcomplete",
     "jinja2",
     "GitPython",
+    "rich",
 ]
 requires-python = ">=3.8"
 authors = [
   {name = "Rasmus Grøndahl Olsen", email = "simplhdl@gmail.com"},
 ]
 maintainers = [
   {name = "Rasmus Grøndahl Olsen", email = "simplhdl@gmail.com"},
```

### Comparing `SimplHDL-0.0.4/src/SimplHDL.egg-info/PKG-INFO` & `simplhdl-0.0.5/src/SimplHDL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimplHDL
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework for simulating and implementing HDL designs
 Author-email: Rasmus Grøndahl Olsen <simplhdl@gmail.com>
 Maintainer-email: Rasmus Grøndahl Olsen <simplhdl@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 SimplHDL
         
@@ -47,14 +47,15 @@
 Requires-Dist: pySVModel==0.3.5
 Requires-Dist: pyEDAA.ProjectModel==0.4.3
 Requires-Dist: pyyaml
 Requires-Dist: types-PyYAML
 Requires-Dist: argcomplete
 Requires-Dist: jinja2
 Requires-Dist: GitPython
+Requires-Dist: rich
 
 ## Introduction
 
 SimplHDL is a plugin-based command-line application for simplifying FPGA and
 ASIC development regardless of EDA tools and flows.
 
 The goal is to embrase structured and reusable designs by creating a generic
```

### Comparing `SimplHDL-0.0.4/src/SimplHDL.egg-info/SOURCES.txt` & `simplhdl-0.0.5/src/SimplHDL.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,15 @@
 src/simplhdl/resources/templates/vcs/cocotb.mk.j2
 src/simplhdl/resources/templates/vcs/dependencies.mk.j2
 src/simplhdl/resources/templates/vcs/files.j2
 src/simplhdl/resources/templates/vcs/fileset.j2
 src/simplhdl/resources/templates/vcs/pli.tab.j2
 src/simplhdl/resources/templates/vcs/project.mk.j2
 src/simplhdl/resources/templates/vcs/synopsys_sim.setup.j2
+src/simplhdl/resources/templates/vcs/vcs.parameters.j2
 src/simplhdl/resources/templates/vivado/__init__.py
 src/simplhdl/resources/templates/vivado/launch_run.sh.j2
 src/simplhdl/resources/templates/vivado/project.tcl.j2
 src/simplhdl/resources/templates/vivado/run.tcl.j2
 src/simplhdl/resources/templates/vivado/steps.tcl.j2
 src/simplhdl/resources/templates/xsim/Makefile.j2
 src/simplhdl/resources/templates/xsim/__init__.py
```

### Comparing `SimplHDL-0.0.4/src/simplhdl/__main__.py` & `simplhdl-0.0.5/src/simplhdl/__main__.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/cocotb.py` & `simplhdl-0.0.5/src/simplhdl/cocotb.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/flow.py` & `simplhdl-0.0.5/src/simplhdl/flow.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/flows/modelsimflow.py` & `simplhdl-0.0.5/src/simplhdl/flows/modelsimflow.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/flows/quartusflow.py` & `simplhdl-0.0.5/src/simplhdl/flows/quartusflow.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/flows/questasim/questasimflow.py` & `simplhdl-0.0.5/src/simplhdl/flows/rivierapro/rivieraproflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from typing import Any, List, Dict
 from argparse import Namespace
 from jinja2 import Template
 from simplhdl.pyedaa.project import Project
 from simplhdl.pyedaa.fileset import FileSet
 from simplhdl.utils import sh
 from simplhdl.flow import FlowFactory, FlowTools
-from simplhdl.resources.templates import questasim as questasimtemplates
+from simplhdl.resources.templates import rivierapro as rivieraprotemplates
 from simplhdl.flows.simulationflow import SimulationFlow
 
 logger = logging.getLogger(__name__)
 
 
-@FlowFactory.register('questasim')
-class QuestaSimFlow(SimulationFlow):
+@FlowFactory.register('rivierapro')
+class RivieraProFlow(SimulationFlow):
 
     @classmethod
     def parse_args(self, subparsers) -> None:
-        parser = subparsers.add_parser('questasim', help='QuestaSim HDL Simulation Flow')
+        parser = subparsers.add_parser('rivierapro', help='Riviera PRO HDL Simulation Flow')
         parser.add_argument(
             '--step',
             action='store',
             choices=['compile', 'elaborate', 'simulate'],
             default='simulate',
             help="flow step to run"
         )
@@ -34,80 +34,80 @@
             '--wave',
             action='store_true',
             help="Dump waveforms"
         )
         parser.add_argument(
             '--gui',
             action='store_true',
-            help="Open project in QuestaSim GUI"
+            help="Open project in Riviera PRO GUI"
         )
         parser.add_argument(
             '--vsim-args',
             default='',
             action='store',
-            metavar='ARGS',
-            help="Extra arguments for QuestaSim vsim command"
+            metavar='args',
+            help="Extra args for Riviera PRO vsim command"
         )
         parser.add_argument(
             '--vopt-args',
             default='',
             action='store',
-            metavar='ARGS',
-            help="Extra arguments for QuestaSim vopt command"
+            metavar='args',
+            help="Extra args for Riviera PRO vopt command"
         )
         parser.add_argument(
             '--vmap-args',
             default='',
             action='store',
-            metavar='ARGS',
-            help="Extra arguments for QuestaSim vmap command"
+            metavar='args',
+            help="Extra args for Riviera PRO vmap command"
         )
         parser.add_argument(
             '--vcom-args',
             default='',
             action='store',
-            metavar='ARGS',
-            help="Extra arguments for QuestaSim vcom command"
+            metavar='args',
+            help="Extra args for Riviera PRO vcom command"
         )
         parser.add_argument(
             '--vlog-args',
             default='',
             action='store',
-            metavar='ARGS',
-            help="Extra arguments for QuestaSim vlog command"
+            metavar='args',
+            help="Extra args for Riviera PRO vlog command"
         )
         parser.add_argument(
             '--seed',
-            type=int,
             default=1,
             action='store',
             help="Seed to initialize random generator"
         )
         parser.add_argument(
             '--random-seed',
+            default=1,
             action='store_true',
             help="Generate a random seed to initialize random generator"
         )
         parser.add_argument(
             '--do',
             metavar='COMMAND',
             action='store',
             help="Do command to start simulation"
         )
         parser.add_argument(
             '--timescale',
             default='1ns/1ps',
             action='store',
-            help="Set the simulator timescale for QuestaSim"
+            help="Set the simulator timescale for Riviera PRO"
         )
 
     def __init__(self, name, args: Namespace, project: Project, builddir: Path):
         super().__init__(name, args, project, builddir)
-        self.templates = questasimtemplates
-        self.tools.add(FlowTools.QUESTASIM)
+        self.templates = rivieraprotemplates
+        self.tools.add(FlowTools.RIVIERAPRO)
 
     def get_globals(self) -> Dict[str, Any]:
         globals = super().get_globals()
         globals['vlog_args'] = self.vlog_args()
         globals['vcom_args'] = self.vcom_args()
         globals['vopt_args'] = self.vopt_args()
         globals['vsim_args'] = self.vsim_args()
@@ -129,67 +129,81 @@
 
     def fileset_verilog_args(self, fileset: FileSet) -> str:
         library = fileset.VHDLLibrary
         return f"-work {library.Name}"
 
     def fileset_systemverilog_args(self, fileset: FileSet) -> str:
         library = fileset.VHDLLibrary
-        return f"-sv -work {library.Name}"
+        return f"-sv2k17 -work {library.Name}"
 
     def fileset_vhdl_args(self, fileset: FileSet) -> str:
         library = fileset.VHDLLibrary
         return f"-2008 -work {library.Name}"
 
     def vlog_args(self) -> str:
         args = set()
         if self.args.verbose == 0:
             args.add('-quiet')
+        if self.args.timescale:
+            args.add(f"-timescale {self.args.timescale}")
         for name in self.get_libraries().keys():
-            args.add(f"-L {name}")
+            args.add(f"-l {name}")
+        if self.args.gui:
+            args.add('-dbg')
         for name, value in self.project.Defines.items():
             args.add(f"+define+{name}={value}")
         return ' '.join(list(args) + [self.args.vlog_args])
 
     def vcom_args(self) -> str:
         args = set()
         if self.args.verbose == 0:
             args.add('-quiet')
+        if self.args.gui:
+            args.add('-dbg')
         return ' '.join(list(args) + [self.args.vcom_args])
 
     def vmap_args(self) -> str:
         args = set()
         return ' '.join(list(args) + [self.args.vmap_args])
 
     def vopt_args(self) -> str:
+        return ""
+
+    def vsim_args(self) -> str:
         args = set()
         if self.args.verbose == 0:
             args.add('-quiet')
         for name in self.get_libraries().keys():
             args.add(f"-L {name}")
-        if self.args.timescale:
-            args.add(f"-timescale {self.args.timescale}")
         for name, value in self.project.Generics.items():
             args.add(f"-g{name}={value}")
         for name, value in self.project.Parameters.items():
             args.add(f"-g{name}={value}")
-        if self.args.gui or self.cocotb.enabled:
-            args.add('+acc=npr')
-        return ' '.join(list(args) + [self.args.vopt_args])
-
-    def vsim_args(self) -> str:
-        args = set()
-        args.add(f"-sv_seed {self.args.seed}")
-        if self.args.verbose == 0:
-            args.add('-quiet')
         for name, value in self.project.PlusArgs.items():
             args.add(f"+{name}={value}")
         if self.args.gui:
-            args.add('-onfinish final')
-        else:
-            args.add('-onfinish exit')
+            args.add('-dbg +access +r')
+        if self.cocotb.enabled:
+            args.add('+access +w_nets+p+*')
+            # args.add('+access +w')
+        args.add(f"-sv_seed {self.args.seed}")
+        args.add(f"-random_seed {self.args.random_seed}")
+        return ' '.join(list(args) + [self.args.vopt_args])
+
+#    def vsim_args(self) -> str:
+#        args = set()
+#        args.add(f"-sv_seed {self.args.seed}")
+#        if self.args.verbose == 0:
+#            args.add('-quiet')
+#        for name, value in self.project.PlusArgs.items():
+#            args.add(f"+{name}={value}")
+#        if self.args.gui:
+#            args.add('-onfinish final')
+#        else:
+#            args.add('-onfinish exit')
 
         return ' '.join(list(args) + [self.args.vsim_args])
 
     def get_library(self, fileset: FileSet) -> str:
         try:
             library = fileset.VHDLLibrary.Name
         except AttributeError:
@@ -230,21 +244,21 @@
 
     def is_tool_setup(self) -> None:
         if (shutil.which('vlog') is None or
                 shutil.which('vsim') is None or
                 shutil.which('vcom') is None or
                 shutil.which('vlib') is None or
                 shutil.which('vmap') is None):
-            raise Exception("QuestaSim is not setup correctly")
-        # NOTE: If questasim's bin directory is appended to the PATH variable,
+            raise Exception("Riviera PRO is not setup correctly")
+        # NOTE: If rivierapro's bin directory is appended to the PATH variable,
         #       the vdir command is found in /bin/vdir which is not the
-        #       QuestaSim vdir command
+        #       Riviera PRO vdir command
         vdir = Path(shutil.which('vdir'))
         vsim = Path(shutil.which('vsim'))
         if vdir.parent != vsim.parent:
             logger.warning(
-                "QuestaSim is not setup correctly. "
+                "Riviera PRO is not setup correctly. "
                 f"The 'vdir' command is pointing to {vdir}, which "
-                "is not part of the QuestaSim installation. Try to "
-                "prepend Questa to the PATH environment variable."
+                "is not part of the Riviera PRO installation. Try to "
+                "prepend Riviera PRO to the PATH environment variable."
             )
             os.environ['PATH'] = f"{vsim.parent}:{os.environ['PATH']}"
```

### Comparing `SimplHDL-0.0.4/src/simplhdl/flows/rivierapro/rivieraproflow.py` & `simplhdl-0.0.5/src/simplhdl/flows/questasim/questasimflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import os
 import logging
 import shutil
 
 from pathlib import Path
-from typing import Any, List, Dict
+from typing import Any, List, Dict, Optional
 from argparse import Namespace
 from jinja2 import Template
 from simplhdl.pyedaa.project import Project
 from simplhdl.pyedaa.fileset import FileSet
 from simplhdl.utils import sh
 from simplhdl.flow import FlowFactory, FlowTools
-from simplhdl.resources.templates import rivierapro as rivieraprotemplates
+from simplhdl.resources.templates import questasim as questasimtemplates
 from simplhdl.flows.simulationflow import SimulationFlow
 
 logger = logging.getLogger(__name__)
 
 
-@FlowFactory.register('rivierapro')
-class RivieraProFlow(SimulationFlow):
+@FlowFactory.register('questasim')
+class QuestaSimFlow(SimulationFlow):
 
     @classmethod
     def parse_args(self, subparsers) -> None:
-        parser = subparsers.add_parser('rivierapro', help='Riviera PRO HDL Simulation Flow')
+        parser = subparsers.add_parser('questasim', help='QuestaSim HDL Simulation Flow')
         parser.add_argument(
             '--step',
             action='store',
             choices=['compile', 'elaborate', 'simulate'],
             default='simulate',
             help="flow step to run"
         )
@@ -34,80 +34,80 @@
             '--wave',
             action='store_true',
             help="Dump waveforms"
         )
         parser.add_argument(
             '--gui',
             action='store_true',
-            help="Open project in Riviera PRO GUI"
+            help="Open project in QuestaSim GUI"
         )
         parser.add_argument(
             '--vsim-args',
             default='',
             action='store',
-            metavar='args',
-            help="Extra args for Riviera PRO vsim command"
+            metavar='ARGS',
+            help="Extra arguments for QuestaSim vsim command"
         )
         parser.add_argument(
             '--vopt-args',
             default='',
             action='store',
-            metavar='args',
-            help="Extra args for Riviera PRO vopt command"
+            metavar='ARGS',
+            help="Extra arguments for QuestaSim vopt command"
         )
         parser.add_argument(
             '--vmap-args',
             default='',
             action='store',
-            metavar='args',
-            help="Extra args for Riviera PRO vmap command"
+            metavar='ARGS',
+            help="Extra arguments for QuestaSim vmap command"
         )
         parser.add_argument(
             '--vcom-args',
             default='',
             action='store',
-            metavar='args',
-            help="Extra args for Riviera PRO vcom command"
+            metavar='ARGS',
+            help="Extra arguments for QuestaSim vcom command"
         )
         parser.add_argument(
             '--vlog-args',
             default='',
             action='store',
-            metavar='args',
-            help="Extra args for Riviera PRO vlog command"
+            metavar='ARGS',
+            help="Extra arguments for QuestaSim vlog command"
         )
         parser.add_argument(
             '--seed',
+            type=int,
             default=1,
             action='store',
             help="Seed to initialize random generator"
         )
         parser.add_argument(
             '--random-seed',
-            default=1,
             action='store_true',
             help="Generate a random seed to initialize random generator"
         )
         parser.add_argument(
             '--do',
             metavar='COMMAND',
             action='store',
             help="Do command to start simulation"
         )
         parser.add_argument(
             '--timescale',
             default='1ns/1ps',
             action='store',
-            help="Set the simulator timescale for Riviera PRO"
+            help="Set the simulator timescale for QuestaSim"
         )
 
     def __init__(self, name, args: Namespace, project: Project, builddir: Path):
         super().__init__(name, args, project, builddir)
-        self.templates = rivieraprotemplates
-        self.tools.add(FlowTools.RIVIERAPRO)
+        self.templates = questasimtemplates
+        self.tools.add(FlowTools.QUESTASIM)
 
     def get_globals(self) -> Dict[str, Any]:
         globals = super().get_globals()
         globals['vlog_args'] = self.vlog_args()
         globals['vcom_args'] = self.vcom_args()
         globals['vopt_args'] = self.vopt_args()
         globals['vsim_args'] = self.vsim_args()
@@ -129,81 +129,68 @@
 
     def fileset_verilog_args(self, fileset: FileSet) -> str:
         library = fileset.VHDLLibrary
         return f"-work {library.Name}"
 
     def fileset_systemverilog_args(self, fileset: FileSet) -> str:
         library = fileset.VHDLLibrary
-        return f"-sv2k17 -work {library.Name}"
+        return f"-sv -work {library.Name}"
 
     def fileset_vhdl_args(self, fileset: FileSet) -> str:
         library = fileset.VHDLLibrary
         return f"-2008 -work {library.Name}"
 
     def vlog_args(self) -> str:
         args = set()
         if self.args.verbose == 0:
             args.add('-quiet')
-        if self.args.timescale:
-            args.add(f"-timescale {self.args.timescale}")
-        for name in self.get_libraries().keys():
-            args.add(f"-l {name}")
-        if self.args.gui:
-            args.add('-dbg')
         for name, value in self.project.Defines.items():
             args.add(f"+define+{name}={value}")
         return ' '.join(list(args) + [self.args.vlog_args])
 
     def vcom_args(self) -> str:
         args = set()
         if self.args.verbose == 0:
             args.add('-quiet')
-        if self.args.gui:
-            args.add('-dbg')
         return ' '.join(list(args) + [self.args.vcom_args])
 
     def vmap_args(self) -> str:
         args = set()
         return ' '.join(list(args) + [self.args.vmap_args])
 
     def vopt_args(self) -> str:
-        return ""
-
-    def vsim_args(self) -> str:
         args = set()
         if self.args.verbose == 0:
             args.add('-quiet')
         for name in self.get_libraries().keys():
             args.add(f"-L {name}")
+        if self.args.timescale:
+            args.add(f"-timescale {self.args.timescale}")
         for name, value in self.project.Generics.items():
             args.add(f"-g{name}={value}")
         for name, value in self.project.Parameters.items():
             args.add(f"-g{name}={value}")
+        if self.args.gui or self.args.do or self.args.wave or self.cocotb.enabled:
+            args.add('+acc=npr')
+        return ' '.join(list(args) + [self.args.vopt_args])
+
+    def vsim_args(self) -> str:
+        args = set()
+        args.add(f"-sv_seed {self.args.seed}")
+        timescale = self.timescale()
+        if timescale:
+            args.add(timescale)
+        if self.args.verbose == 0:
+            args.add('-quiet')
         for name, value in self.project.PlusArgs.items():
             args.add(f"+{name}={value}")
         if self.args.gui:
-            args.add('-dbg +access +r')
-        if self.cocotb.enabled:
-            args.add('+access +w_nets+p+*')
-            # args.add('+access +w')
-        args.add(f"-sv_seed {self.args.seed}")
-        args.add(f"-random_seed {self.args.random_seed}")
-        return ' '.join(list(args) + [self.args.vopt_args])
-
-#    def vsim_args(self) -> str:
-#        args = set()
-#        args.add(f"-sv_seed {self.args.seed}")
-#        if self.args.verbose == 0:
-#            args.add('-quiet')
-#        for name, value in self.project.PlusArgs.items():
-#            args.add(f"+{name}={value}")
-#        if self.args.gui:
-#            args.add('-onfinish final')
-#        else:
-#            args.add('-onfinish exit')
+            args.add('-onfinish final')
+        else:
+            args.add('-onfinish exit')
 
         return ' '.join(list(args) + [self.args.vsim_args])
 
     def get_library(self, fileset: FileSet) -> str:
         try:
             library = fileset.VHDLLibrary.Name
         except AttributeError:
@@ -238,27 +225,37 @@
             for command in self.project.Hooks[name]:
                 logger.info(f"Running {name} hook: {command}")
                 sh(command.split(), cwd=self.builddir, output=True)
         except KeyError:
             # NOTE: Continue if no hook is registret
             pass
 
+    def timescale(self) -> Optional[str]:
+        """
+        Sets the timescale for VHDL based on the Verilog timescale
+        resolution.
+        """
+        if self.args.timescale.endswith('ps'):
+            return "-t ps"
+        elif self.args.timescale.endswith('fs'):
+            return "-t fs"
+
     def is_tool_setup(self) -> None:
         if (shutil.which('vlog') is None or
                 shutil.which('vsim') is None or
                 shutil.which('vcom') is None or
                 shutil.which('vlib') is None or
                 shutil.which('vmap') is None):
-            raise Exception("Riviera PRO is not setup correctly")
-        # NOTE: If rivierapro's bin directory is appended to the PATH variable,
+            raise Exception("QuestaSim is not setup correctly")
+        # NOTE: If questasim's bin directory is appended to the PATH variable,
         #       the vdir command is found in /bin/vdir which is not the
-        #       Riviera PRO vdir command
+        #       QuestaSim vdir command
         vdir = Path(shutil.which('vdir'))
         vsim = Path(shutil.which('vsim'))
         if vdir.parent != vsim.parent:
             logger.warning(
-                "Riviera PRO is not setup correctly. "
+                "QuestaSim is not setup correctly. "
                 f"The 'vdir' command is pointing to {vdir}, which "
-                "is not part of the Riviera PRO installation. Try to "
-                "prepend Riviera PRO to the PATH environment variable."
+                "is not part of the QuestaSim installation. Try to "
+                "prepend Questa to the PATH environment variable."
             )
             os.environ['PATH'] = f"{vsim.parent}:{os.environ['PATH']}"
```

### Comparing `SimplHDL-0.0.4/src/simplhdl/flows/simulationflow.py` & `simplhdl-0.0.5/src/simplhdl/flows/simulationflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         """
         walker = FileSetWalker()
         rules: Dict[str, List[str]] = dict()
         for fileset in walker.walk(self.project.DefaultDesign.DefaultFileSet, reverse=False):
             name = md5sum(fileset.Name)
             dependencies = []
             for language_fileset in [f for f in filelist if f.stem.startswith(name)]:
-                for child in fileset.FileSets.values():
+                for child in fileset.Dependencies(usedin='simulation'):
                     child_name = md5sum(child.Name)
                     dependencies += [append_suffix(f, '.com').name for f in filelist
                                      if f.stem.startswith(child_name)]
                     if dependencies:
                         rules[append_suffix(language_fileset, '.com').name] = dependencies
         return rules
```

### Comparing `SimplHDL-0.0.4/src/simplhdl/flows/vcs/vcsflow.py` & `simplhdl-0.0.5/src/simplhdl/flows/xsim/xsimflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-from argparse import Namespace
 import os
 import logging
-from pathlib import Path
 import shutil
 
-from typing import Dict, Any, List
+from argparse import Namespace
+from pathlib import Path
+from typing import List, Dict, Any
 from jinja2 import Template
-from simplhdl.pyedaa.fileset import FileSet
 from simplhdl.pyedaa.project import Project
+from simplhdl.pyedaa.fileset import FileSet
 from simplhdl.utils import sh
 from simplhdl.flow import FlowFactory, FlowTools
-from simplhdl.resources.templates import vcs as vcstemplates
-from ..simulationflow import SimulationFlow
-
+from simplhdl.resources.templates import xsim as xsimtemplates
+from simplhdl.flows.simulationflow import SimulationFlow
 
 logger = logging.getLogger(__name__)
 
 
-@FlowFactory.register('vcs')
-class VcsFlow(SimulationFlow):
+@FlowFactory.register('xsim')
+class XsimFlow(SimulationFlow):
 
     @classmethod
     def parse_args(self, subparsers) -> None:
-        parser = subparsers.add_parser('vcs', help='Vcs HDL Simulation Flow')
+        parser = subparsers.add_parser('xsim', help='Xilinx Xsim HDL Simulation Flow')
         parser.add_argument(
             '-s',
             '--step',
             action='store',
             choices=['compile', 'elaborate', 'simulate'],
             default='simulate',
             help="flow step to run"
@@ -36,39 +35,39 @@
             '--wave',
             action='store_true',
             help="Dump waveforms"
         )
         parser.add_argument(
             '--gui',
             action='store_true',
-            help="Open project in DVE or Verdi GUI"
+            help="Open project in GUI"
         )
         parser.add_argument(
-            '--simv-args',
+            '--xsim-args',
             default='',
             action='store',
-            help="Extra args for Vcs simv command"
+            help="Extra args for Xsim xsim command"
         )
         parser.add_argument(
-            '--vcs-args',
+            '--xelab-args',
             default='',
             action='store',
-            help="Extra args for Vcs vcs command"
+            help="Extra args for Xsim xelab command"
         )
         parser.add_argument(
-            '--vhdlan-args',
+            '--xvhdl-args',
             default='',
             action='store',
-            help="Extra args for Vcs vhdlan command"
+            help="Extra args for Xsim xvhdl command"
         )
         parser.add_argument(
-            '--vlogan-args',
+            '--xvlog-args',
             default='',
             action='store',
-            help="Extra args for Vcs vlogan command"
+            help="Extra args for Xsim xvlog command"
         )
         parser.add_argument(
             '--seed',
             default='1',
             action='store',
             help="Seed to initialize random generator"
         )
@@ -77,124 +76,109 @@
             action='store_true',
             help="Generate a random seed to initialize random generator"
         )
         parser.add_argument(
             '--timescale',
             default='1ns/1ps',
             action='store',
-            help="Set the simulator timescale for Verilog"
+            help="Set the simulator timescale for Xsim"
         )
 
     def __init__(self, name, args: Namespace, project: Project, builddir: Path):
         super().__init__(name, args, project, builddir)
-        self.templates = vcstemplates
-        self.tools.add(FlowTools.VCS)
+        self.templates = xsimtemplates
+        self.tools.add(FlowTools.XSIM)
+
+    def configure(self):
+        super().configure()
+        if self.cocotb.enabled:
+            os.environ['MODULE'] = self.cocotb.module()
+            raise NotImplementedError("Xsim currently doesn't support cocotb")
 
     def get_globals(self) -> Dict[str, Any]:
         globals = super().get_globals()
-        globals['vlogan_args'] = self.vlogan_args()
-        globals['vhdlan_args'] = self.vhdlan_args()
-        globals['vcs_args'] = self.vcs_args()
-        globals['simv_args'] = self.simv_args()
+        globals['xvlog_args'] = self.xvlog_args()
+        globals['xvhdl_args'] = self.xvhdl_args()
+        globals['xelab_args'] = self.xelab_args()
+        globals['xsim_args'] = self.xsim_args()
         return globals
 
     def get_project_templates(self, environment) -> List[Template]:
         return [
             environment.get_template('Makefile.j2'),
-            environment.get_template('synopsys_sim.setup.j2'),
             environment.get_template('project.mk.j2')
         ]
 
     def get_cocotb_templates(self, environment):
         if self.cocotb.enabled:
             return [
-                environment.get_template('cocotb.mk.j2'),
-                environment.get_template('pli.tab.j2')
+                environment.get_template('cocotb.mk.j2')
             ]
         else:
             return list()
 
     def fileset_verilog_args(self, fileset: FileSet) -> str:
         library = fileset.VHDLLibrary
-        return f"+v2k -work {library.Name}"
+        return f"-work {library.Name}"
 
     def fileset_systemverilog_args(self, fileset: FileSet) -> str:
         library = fileset.VHDLLibrary
-        return f"-sverilog -work {library.Name}"
+        return f"-sv -work {library.Name}"
 
     def fileset_vhdl_args(self, fileset: FileSet) -> str:
         library = fileset.VHDLLibrary
-        return f"-vhdl08 -work {library.Name}"
+        return f"--2008 -work {library.Name}"
 
-    def vlogan_args(self) -> str:
+    def xvlog_args(self) -> str:
         args = set()
+        args.add(f"-v {self.args.verbose if self.args.verbose < 2 else 2}")
         for name, value in self.project.Defines.items():
-            args.add(f"+define+{name}={value}")
-        if self.args.verbose == 0:
-            args.add('-q')
-        elif self.args.verbose > 1:
-            args.add('-V')
-        if self.is_uvm():
-            args.add('-ntb_opts uvm')
-        if self.is_verdi():
-            args.add('-kdb')
-        return ' '.join(list(args) + [self.args.vlogan_args]).strip()
+            args.add(f"-d {name}={value}")
+        return ' '.join(list(args) + [self.args.xvlog_args]).strip()
 
-    def vhdlan_args(self) -> str:
+    def xvhdl_args(self) -> str:
         args = set()
-        if self.args.verbose == 0:
-            args.add('-q')
-        elif self.args.verbose > 1:
-            args.add('-verbose')
-        if self.args.gui and self.is_verdi():
-            args.add('-kdb')
-        return ' '.join(list(args) + [self.args.vhdlan_args]).strip()
+        args.add(f"-v {self.args.verbose if self.args.verbose < 2 else 2}")
+        return ' '.join(list(args) + [self.args.xvhdl_args])
 
-    def vcs_args(self) -> str:
+    def xelab_args(self) -> str:
         args = set()
-        if self.args.verbose == 0:
-            args.add('-q')
+        verbosity = f"-v {self.args.verbose if self.args.verbose < 2 else 2}"
+        args.add(verbosity)
         if self.args.timescale:
-            args.add(f"-timescale={self.args.timescale}")
-        if self.is_uvm():
-            args.add('-ntb_opts uvm')
-        if self.args.gui:
-            args.add('-debug_access+all')
-            if self.is_verdi():
-                args.add('-kdb')
+            args.add(f"--timescale={self.args.timescale}")
         for name, value in self.project.Generics.items():
-            args.add(f"-pvalue+{name}={value}")
+            args.add(f"--generic_top {name}={value}")
         for name, value in self.project.Parameters.items():
-            args.add(f"-pvalue+{name}={value}")
-        return ' '.join(list(args) + [self.args.vcs_args])
+            args.add(f"--generic_top {name}={value}")
+        return ' '.join(list(args) + [self.args.xelab_args])
 
-    def simv_args(self) -> str:
+    def xsim_args(self) -> str:
         args = set()
-        if self.args.seed != '1':
-            args.add(f"+ntb_random_seed={self.args.seed}")
+        args.add(f"-sv_seed {self.args.seed}")
+        if self.cocotb.enabled:
+            # xsim currently doesn't work with cocotb
+            pass
         for name, value in self.project.PlusArgs.items():
-            args.add(f"+{name}={value}")
-        return ' '.join(list(args) + [self.args.simv_args])
-
-    def get_library(self, fileset: FileSet) -> str:
-        try:
-            library = fileset.VHDLLibrary.Name
-        except AttributeError:
-            # TODO: This is a workaround The default fileset is FileSet
-            #       which is bugged. Because it is empty we don't need it
-            #       anyway and can just ignore it.
-            library = ''
-        return library
+            args.add(f"--testplusarg {name}={value}")
+        return ' '.join(list(args) + [self.args.xsim_args])
 
     def execute(self, step: str) -> None:
         self.run_hooks('pre')
         sh(['make', 'compile'], cwd=self.builddir, output=True)
         if step == 'compile':
             return
 
+        if self.cocotb.enabled:
+            for toplevel in [t for t in self.project.DefaultDesign.TopLevel.split() if t != self.cocotb.module()]:
+                # TODO: what should happend in Vcs?
+                # self.hdl_language = get_hdl_language(toplevel, directory=self.builddir)
+                # os.environ['SIMPLHDL_LANGUAGE'] = self.hdl_language
+                pass
+
         if self.args.gui:
             command = ['make', 'gui']
         else:
             command = ['make', step]
         sh(command, cwd=self.builddir, output=True)
         if step == 'simulate':
             self.run_hooks('post')
@@ -205,15 +189,30 @@
                 logger.info(f"Running {name} hook: {command}")
                 sh(command.split(), cwd=self.builddir, output=True)
         except KeyError:
             # NOTE: Continue if no hook is registret
             pass
 
     def is_tool_setup(self) -> None:
-        if (shutil.which('vlogan') is None or
-                shutil.which('vhdlan') is None or
-                shutil.which('vcs') is None):
-            raise Exception("Vcs is not setup correctly")
-
-    def is_verdi(self) -> bool:
-        return (os.environ.get('SNPS_SIM_DEFAULT_GUI') == 'verdi' or
-                os.environ.get('VERDI_HOME'))
+        if (shutil.which('xvlog') is None or
+                shutil.which('xvhdl') is None or
+                shutil.which('xsim') is None):
+            raise Exception("Xsim is not setup correctly")
+
+
+def get_hdl_language(name: str, directory: Path = Path.cwd()) -> str:
+    """Get language of HDL module by inspecting the compiled libraries
+
+    Args:
+        name (str): Module/Entity name
+        directory (Path): Directory of library locations
+
+    Returns:
+        str: Verilog or VHDL
+    """
+    info = sh(['vdir', '-prop', 'top', name], cwd=directory)
+    if info.startswith('ENTITY'):
+        return "vhdl"
+    elif info.startswith('MODULE'):
+        return "verilog"
+    else:
+        raise Exception(f"Unknow info: {info}")
```

### Comparing `SimplHDL-0.0.4/src/simplhdl/flows/vivadoflow.py` & `simplhdl-0.0.5/src/simplhdl/flows/vivadoflow.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/flows/xsim/xsimflow.py` & `simplhdl-0.0.5/src/simplhdl/flows/vcs/vcsflow.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,33 @@
+from argparse import Namespace
 import os
 import logging
+from pathlib import Path
 import shutil
+import re
 
-from argparse import Namespace
-from pathlib import Path
-from typing import List, Dict, Any
+from typing import Dict, Any, List
 from jinja2 import Template
-from simplhdl.pyedaa.project import Project
 from simplhdl.pyedaa.fileset import FileSet
+from simplhdl.pyedaa.project import Project
 from simplhdl.utils import sh
 from simplhdl.flow import FlowFactory, FlowTools
-from simplhdl.resources.templates import xsim as xsimtemplates
-from simplhdl.flows.simulationflow import SimulationFlow
+from simplhdl.resources.templates import vcs as vcstemplates
+from ..simulationflow import SimulationFlow
+
 
 logger = logging.getLogger(__name__)
 
 
-@FlowFactory.register('xsim')
-class XsimFlow(SimulationFlow):
+@FlowFactory.register('vcs')
+class VcsFlow(SimulationFlow):
 
     @classmethod
     def parse_args(self, subparsers) -> None:
-        parser = subparsers.add_parser('xsim', help='Xilinx Xsim HDL Simulation Flow')
+        parser = subparsers.add_parser('vcs', help='Vcs HDL Simulation Flow')
         parser.add_argument(
             '-s',
             '--step',
             action='store',
             choices=['compile', 'elaborate', 'simulate'],
             default='simulate',
             help="flow step to run"
@@ -35,39 +37,39 @@
             '--wave',
             action='store_true',
             help="Dump waveforms"
         )
         parser.add_argument(
             '--gui',
             action='store_true',
-            help="Open project in GUI"
+            help="Open project in DVE or Verdi GUI"
         )
         parser.add_argument(
-            '--xsim-args',
+            '--simv-args',
             default='',
             action='store',
-            help="Extra args for Xsim xsim command"
+            help="Extra args for Vcs simv command"
         )
         parser.add_argument(
-            '--xelab-args',
+            '--vcs-args',
             default='',
             action='store',
-            help="Extra args for Xsim xelab command"
+            help="Extra args for Vcs vcs command"
         )
         parser.add_argument(
-            '--xvhdl-args',
+            '--vhdlan-args',
             default='',
             action='store',
-            help="Extra args for Xsim xvhdl command"
+            help="Extra args for Vcs vhdlan command"
         )
         parser.add_argument(
-            '--xvlog-args',
+            '--vlogan-args',
             default='',
             action='store',
-            help="Extra args for Xsim xvlog command"
+            help="Extra args for Vcs vlogan command"
         )
         parser.add_argument(
             '--seed',
             default='1',
             action='store',
             help="Seed to initialize random generator"
         )
@@ -76,109 +78,145 @@
             action='store_true',
             help="Generate a random seed to initialize random generator"
         )
         parser.add_argument(
             '--timescale',
             default='1ns/1ps',
             action='store',
-            help="Set the simulator timescale for Xsim"
+            help="Set the simulator timescale for Verilog"
         )
 
     def __init__(self, name, args: Namespace, project: Project, builddir: Path):
         super().__init__(name, args, project, builddir)
-        self.templates = xsimtemplates
-        self.tools.add(FlowTools.XSIM)
-
-    def configure(self):
-        super().configure()
-        if self.cocotb.enabled:
-            os.environ['MODULE'] = self.cocotb.module()
-            raise NotImplementedError("Xsim currently doesn't support cocotb")
+        self.templates = vcstemplates
+        self.tools.add(FlowTools.VCS)
 
     def get_globals(self) -> Dict[str, Any]:
         globals = super().get_globals()
-        globals['xvlog_args'] = self.xvlog_args()
-        globals['xvhdl_args'] = self.xvhdl_args()
-        globals['xelab_args'] = self.xelab_args()
-        globals['xsim_args'] = self.xsim_args()
+        globals['vlogan_args'] = self.vlogan_args()
+        globals['vhdlan_args'] = self.vhdlan_args()
+        globals['vcs_args'] = self.vcs_args()
+        globals['simv_args'] = self.simv_args()
+        globals['parameters'] = {**self.project.Generics, **self.project.Parameters}
+        globals['format'] = self.format
         return globals
 
+    def format(self, value: str) -> str:
+        """
+        Format the parameter value in relation to it's type.
+        """
+        isformat_a = re.compile(r"^\d+#[0-9a-gA-G]+#")
+        isformat_b = re.compile(r"^\d*'(h|d|b)[0-9a-fA-F]+")
+        isformat_c = re.compile(r"^\d+\.\d+")
+
+        if (
+            value.isnumeric() or
+            isformat_a.match(value) or
+            isformat_b.match(value) or
+            isformat_c.match(value)
+        ):
+            return value
+        else:
+            return f'"{value}"'
+
     def get_project_templates(self, environment) -> List[Template]:
         return [
             environment.get_template('Makefile.j2'),
-            environment.get_template('project.mk.j2')
+            environment.get_template('synopsys_sim.setup.j2'),
+            environment.get_template('project.mk.j2'),
+            environment.get_template('vcs.parameters.j2'),
         ]
 
     def get_cocotb_templates(self, environment):
         if self.cocotb.enabled:
             return [
-                environment.get_template('cocotb.mk.j2')
+                environment.get_template('cocotb.mk.j2'),
+                environment.get_template('pli.tab.j2')
             ]
         else:
             return list()
 
     def fileset_verilog_args(self, fileset: FileSet) -> str:
         library = fileset.VHDLLibrary
-        return f"-work {library.Name}"
+        return f"+v2k -work {library.Name}"
 
     def fileset_systemverilog_args(self, fileset: FileSet) -> str:
         library = fileset.VHDLLibrary
-        return f"-sv -work {library.Name}"
+        return f"-sverilog -work {library.Name}"
 
     def fileset_vhdl_args(self, fileset: FileSet) -> str:
         library = fileset.VHDLLibrary
-        return f"--2008 -work {library.Name}"
+        return f"-vhdl08 -work {library.Name}"
 
-    def xvlog_args(self) -> str:
+    def vlogan_args(self) -> str:
         args = set()
-        args.add(f"-v {self.args.verbose if self.args.verbose < 2 else 2}")
         for name, value in self.project.Defines.items():
-            args.add(f"-d {name}={value}")
-        return ' '.join(list(args) + [self.args.xvlog_args]).strip()
+            args.add(f"+define+{name}={value}")
+        if self.args.verbose == 0:
+            args.add('-q')
+        elif self.args.verbose > 1:
+            args.add('-V')
+        if self.is_uvm():
+            args.add('-ntb_opts uvm')
+        if self.is_verdi():
+            args.add('-kdb')
+        return ' '.join(list(args) + [self.args.vlogan_args]).strip()
 
-    def xvhdl_args(self) -> str:
+    def vhdlan_args(self) -> str:
         args = set()
-        args.add(f"-v {self.args.verbose if self.args.verbose < 2 else 2}")
-        return ' '.join(list(args) + [self.args.xvhdl_args])
+        if self.args.verbose == 0:
+            args.add('-q')
+        elif self.args.verbose > 1:
+            args.add('-verbose')
+        if self.args.gui and self.is_verdi():
+            args.add('-kdb')
+        return ' '.join(list(args) + [self.args.vhdlan_args]).strip()
 
-    def xelab_args(self) -> str:
+    def vcs_args(self) -> str:
         args = set()
-        verbosity = f"-v {self.args.verbose if self.args.verbose < 2 else 2}"
-        args.add(verbosity)
+        if self.args.verbose == 0:
+            args.add('-q')
         if self.args.timescale:
-            args.add(f"--timescale={self.args.timescale}")
-        for name, value in self.project.Generics.items():
-            args.add(f"--generic_top {name}={value}")
-        for name, value in self.project.Parameters.items():
-            args.add(f"--generic_top {name}={value}")
-        return ' '.join(list(args) + [self.args.xelab_args])
+            args.add(f"-timescale={self.args.timescale}")
+        if self.is_uvm():
+            args.add('-ntb_opts uvm')
+        if self.args.gui:
+            args.add('-debug_access+all')
+            if self.is_verdi():
+                args.add('-kdb')
+        parameters = {**self.project.Generics, **self.project.Parameters}
+        if parameters:
+            args.add('-gfile vcs.parameters -lca')
+
+        return ' '.join(list(args) + [self.args.vcs_args])
 
-    def xsim_args(self) -> str:
+    def simv_args(self) -> str:
         args = set()
-        args.add(f"-sv_seed {self.args.seed}")
-        if self.cocotb.enabled:
-            # xsim currently doesn't work with cocotb
-            pass
+        if self.args.seed != '1':
+            args.add(f"+ntb_random_seed={self.args.seed}")
         for name, value in self.project.PlusArgs.items():
-            args.add(f"--testplusarg {name}={value}")
-        return ' '.join(list(args) + [self.args.xsim_args])
+            args.add(f"+{name}={value}")
+        return ' '.join(list(args) + [self.args.simv_args])
+
+    def get_library(self, fileset: FileSet) -> str:
+        try:
+            library = fileset.VHDLLibrary.Name
+        except AttributeError:
+            # TODO: This is a workaround The default fileset is FileSet
+            #       which is bugged. Because it is empty we don't need it
+            #       anyway and can just ignore it.
+            library = ''
+        return library
 
     def execute(self, step: str) -> None:
         self.run_hooks('pre')
         sh(['make', 'compile'], cwd=self.builddir, output=True)
         if step == 'compile':
             return
 
-        if self.cocotb.enabled:
-            for toplevel in [t for t in self.project.DefaultDesign.TopLevel.split() if t != self.cocotb.module()]:
-                # TODO: what should happend in Vcs?
-                # self.hdl_language = get_hdl_language(toplevel, directory=self.builddir)
-                # os.environ['SIMPLHDL_LANGUAGE'] = self.hdl_language
-                pass
-
         if self.args.gui:
             command = ['make', 'gui']
         else:
             command = ['make', step]
         sh(command, cwd=self.builddir, output=True)
         if step == 'simulate':
             self.run_hooks('post')
@@ -189,30 +227,15 @@
                 logger.info(f"Running {name} hook: {command}")
                 sh(command.split(), cwd=self.builddir, output=True)
         except KeyError:
             # NOTE: Continue if no hook is registret
             pass
 
     def is_tool_setup(self) -> None:
-        if (shutil.which('xvlog') is None or
-                shutil.which('xvhdl') is None or
-                shutil.which('xsim') is None):
-            raise Exception("Xsim is not setup correctly")
-
-
-def get_hdl_language(name: str, directory: Path = Path.cwd()) -> str:
-    """Get language of HDL module by inspecting the compiled libraries
-
-    Args:
-        name (str): Module/Entity name
-        directory (Path): Directory of library locations
-
-    Returns:
-        str: Verilog or VHDL
-    """
-    info = sh(['vdir', '-prop', 'top', name], cwd=directory)
-    if info.startswith('ENTITY'):
-        return "vhdl"
-    elif info.startswith('MODULE'):
-        return "verilog"
-    else:
-        raise Exception(f"Unknow info: {info}")
+        if (shutil.which('vlogan') is None or
+                shutil.which('vhdlan') is None or
+                shutil.which('vcs') is None):
+            raise Exception("Vcs is not setup correctly")
+
+    def is_verdi(self) -> bool:
+        return (os.environ.get('SNPS_SIM_DEFAULT_GUI') == 'verdi' or
+                os.environ.get('VERDI_HOME'))
```

### Comparing `SimplHDL-0.0.4/src/simplhdl/generator.py` & `simplhdl-0.0.5/src/simplhdl/generator.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/generators/chisel.py` & `simplhdl-0.0.5/src/simplhdl/generators/chisel.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/generators/ipxact.py` & `simplhdl-0.0.5/src/simplhdl/generators/ipxact.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/generators/spd.py` & `simplhdl-0.0.5/src/simplhdl/generators/spd.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/generators/systemrdl.py` & `simplhdl-0.0.5/src/simplhdl/generators/systemrdl.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/parser.py` & `simplhdl-0.0.5/src/simplhdl/parser.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/parsers/fusesocparser.py` & `simplhdl-0.0.5/src/simplhdl/parsers/fusesocparser.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/parsers/simplhdlparser.py` & `simplhdl-0.0.5/src/simplhdl/parsers/simplhdlparser.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/plugins.py` & `simplhdl-0.0.5/src/simplhdl/plugins.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/pyedaa/__init__.py` & `simplhdl-0.0.5/src/simplhdl/pyedaa/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,18 @@
 
     def _registerAttributes(self):
         super()._registerAttributes()
         FileMixIn._registerAttributes(self)
 
     @property
     def Library(self) -> HDLLibrary:
-        return self._library
+        if self._library is not None:
+            return self._library
+        elif self.FileSet.VHDLLibrary is not None:
+            return self.FileSet.VHDLLibrary
 
     @Library.setter
     def Library(self, value) -> None:
         self._library = value
 
 
 class VerilogIncludeFile(HDLIncludeFile, pm.HumanReadableContent):
```

### Comparing `SimplHDL-0.0.4/src/simplhdl/pyedaa/design.py` & `simplhdl-0.0.5/src/simplhdl/pyedaa/design.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/pyedaa/project.py` & `simplhdl-0.0.5/src/simplhdl/pyedaa/project.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/pyedaa/vhdllibrary.py` & `simplhdl-0.0.5/src/simplhdl/pyedaa/vhdllibrary.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/repo.py` & `simplhdl-0.0.5/src/simplhdl/repo.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/resources/templates/quartus/project.tcl.j2` & `simplhdl-0.0.5/src/simplhdl/resources/templates/quartus/project.tcl.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/resources/templates/quartus/run.tcl.j2` & `simplhdl-0.0.5/src/simplhdl/resources/templates/quartus/run.tcl.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/Makefile.j2` & `simplhdl-0.0.5/src/simplhdl/resources/templates/questasim/Makefile.j2`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 VMAP := vmap
 VCOM := vcom
 VLOG := vlog
 VOPT := vopt
 VSIM := vsim
 
 VLIB_FLAGS :=
-VMAP_FLAGS := {{vmap_args}}
-VCOM_FLAGS := {{vcom_args}}
-VLOG_FLAGS := {{vlog_args}}
-VOPT_FLAGS := {{vopt_args}}
-VSIM_FLAGS := {{vsim_args}}
+VMAP_FLAGS := {{vmap_args|replace('#', '\#')}}
+VCOM_FLAGS := {{vcom_args|replace('#', '\#')}}
+VLOG_FLAGS := {{vlog_args|replace('#', '\#')}}
+VOPT_FLAGS := {{vopt_args|replace('#', '\#')}}
+VSIM_FLAGS := {{vsim_args|replace('#', '\#')}}
 
 VOPT_DESIGN ?= simvopt
 
 
 include project.mk
 -include cocotb.mk
 
@@ -25,14 +25,16 @@
 else
 GUI_DO_CMD := $(DO_CMD)
 endif
 
 simulate: $(VOPT_DESIGN)
 	$(VSIM) $(VSIM_FLAGS) $< -c $(DO_CMD)
 
+elaborate: $(VOPT_DESIGN)
+
 $(VOPT_DESIGN): compile
 	$(VOPT) $(VOPT_FLAGS) $(TOPLEVELS) -o $@
 
 gui: $(VOPT_DESIGN)
 	$(VSIM) $(VSIM_FLAGS) $< $(GUI_DO_CMD)
```

### Comparing `SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/cocotb.mk.j2` & `simplhdl-0.0.5/src/simplhdl/resources/templates/questasim/cocotb.mk.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/project.mk.j2` & `simplhdl-0.0.5/src/simplhdl/resources/templates/questasim/project.mk.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/Makefile.j2` & `simplhdl-0.0.5/src/simplhdl/resources/templates/rivierapro/Makefile.j2`

 * *Files 18% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 VMAP := vmap
 VCOM := vcom
 VLOG := vlog
 VOPT := :
 VSIM := vsim
 
 VLIB_FLAGS :=
-VMAP_FLAGS := {{vmap_args}}
-VCOM_FLAGS := {{vcom_args}}
-VLOG_FLAGS := {{vlog_args}}
-VOPT_FLAGS := {{vopt_args}}
-VSIM_FLAGS := {{vsim_args}}
+VMAP_FLAGS := {{vmap_args|replace('#', '\#')}}
+VCOM_FLAGS := {{vcom_args|replace('#', '\#')}}
+VLOG_FLAGS := {{vlog_args|replace('#', '\#')}}
+VOPT_FLAGS := {{vopt_args|replace('#', '\#')}}
+VSIM_FLAGS := {{vsim_args|replace('#', '\#')}}
 
 VOPT_DESIGN ?= simvopt
 
 
 include project.mk
 -include cocotb.mk
```

### Comparing `SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/cocotb.mk.j2` & `simplhdl-0.0.5/src/simplhdl/resources/templates/rivierapro/cocotb.mk.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/project.mk.j2` & `simplhdl-0.0.5/src/simplhdl/resources/templates/rivierapro/project.mk.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/Makefile.j2` & `simplhdl-0.0.5/src/simplhdl/resources/templates/vcs/Makefile.j2`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 SIMV := ./simv
 {% if uvm %}
 UVM := uvm.com
 {% else %}
 UVM :=
 {% endif %}
 
-VLOGAN_FLAGS := -full64 +warn=noLNX_OS_VERUN {{vlogan_args}}
-VHDLAN_FLAGS := -full64 {{vhdlan_args}}
-VCS_FLAGS := -full64 -licqueue +warn=noLINX_KRNL {{vcs_args}}
-SIMV_FLAGS := -licqueue {{simv_args}}
+VLOGAN_FLAGS := -full64 +warn=noLNX_OS_VERUN {{vlogan_args|replace('#', '\#')}}
+VHDLAN_FLAGS := -full64 {{vhdlan_args|replace('#', '\#')}}
+VCS_FLAGS := -full64 -licqueue +warn=noLINX_KRNL {{vcs_args|replace('#', '\#')}}
+SIMV_FLAGS := -licqueue {{simv_args|replace('#', '\#')}}
 
 include project.mk
 -include cocotb.mk
 
 .PHONY: clean compile elaborate simulate gui
```

### Comparing `SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/project.tcl.j2` & `simplhdl-0.0.5/src/simplhdl/resources/templates/vivado/project.tcl.j2`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 {% if file.FileType == VerilogIncludeFile %}
 add_files "{{file.Path}}"
 {% elif file.FileType == SystemVerilogSourceFile %}
 read_verilog -sv "{{file.Path}}"
 {% elif file.FileType == VerilogSourceFile %}
 read_verilog "{{file.Path}}"
 {% elif file.FileType == VHDLSourceFile %}
-read_vhdl -vhdl2008 "{{file.Path}}"
+read_vhdl -vhdl2008 -library {{file.Library}} "{{file.Path}}"
 {% elif file.FileType == ConstraintFile %}
 read_xdc "{{file.Path}}"
 {% elif file.FileType == VivadoIPSpecificationFile %}
 {% if file.Path.suffix == '.xcix' %}
 read_ip "{{file.Path}}"
 {% else %}
 import_ip "{{file.Path}}"
```

### Comparing `SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/run.tcl.j2` & `simplhdl-0.0.5/src/simplhdl/resources/templates/vivado/run.tcl.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/Makefile.j2` & `simplhdl-0.0.5/src/simplhdl/resources/templates/xsim/Makefile.j2`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 XVLOG := xvlog
 XVHDL := xvhdl
 XELAB := xelab
 XSIM := xsim
 
-XVLOG_FLAGS := {{xvlog_args}}
-XVHDL_FLAGS := {{xvhdl_args}}
-XELAB_FLAGS := {{xelab_args}}
-XSIM_FLAGS := {{xsim_args}}
+XVLOG_FLAGS := {{xvlog_args|replace('#', '\#')}}
+XVHDL_FLAGS := {{xvhdl_args|replace('#', '\#')}}
+XELAB_FLAGS := {{xelab_args|replace('#', '\#')}}
+XSIM_FLAGS := {{xsim_args|replace('#', '\#')}}
 
 include project.mk
 -include cocotb.mk
 
 .PHONY: clean compile elaborate simulate gui
```

### Comparing `SimplHDL-0.0.4/src/simplhdl/simplhdl.py` & `simplhdl-0.0.5/src/simplhdl/simplhdl.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/src/simplhdl/utils.py` & `simplhdl-0.0.5/src/simplhdl/utils.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.4/tox.ini` & `simplhdl-0.0.5/tox.ini`

 * *Files identical despite different names*

