# Comparing `tmp/tinyrl-0.4.2.tar.gz` & `tmp/tinyrl-0.4.3.tar.gz`

## Comparing `tinyrl-0.4.2.tar` & `tinyrl-0.4.3.tar`

### file list

```diff
@@ -1,301 +1,311 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/__init__.py
--rw-r--r--   0        0        0    10546 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers.h
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/version.h
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_mkl.h
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h
--rw-r--r--   0        0        0    13873 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h
--rw-r--r--   0        0        0    36524 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/generic.h
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h
--rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/nn.h
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu.h
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_blas.h
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mkl.h
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_openblas.h
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cuda.h
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/operations_dummy.h
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/operations_generic.h
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/persist.h
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/layers.h
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu.h
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_blas.h
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_mkl.h
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_openblas.h
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cuda.h
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_dummy.h
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_generic.h
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu.h
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h
--rw-r--r--   0        0        0    11380 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h
--rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_dummy.h
--rw-r--r--   0        0        0    18598 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h
--rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h
--rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/operations_generic.h
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/adam.h
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h
--rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/operations_generic.h
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_cuda.h
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/models.h
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cpu.h
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cuda.h
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_dummy.h
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_generic.h
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist.h
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist_code.h
--rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cpu.h
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cuda.h
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_dummy.h
--rw-r--r--   0        0        0    21585 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist_code.h
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_cpu.h
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/network.h
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_cpu.h
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h
--rw-r--r--   0        0        0    12469 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/uniform_random/model.h
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/uniform_random/operations_generic.h
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_2.h
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_3.h
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_2.h
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_3.h
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_3.h
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_3.h
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_3.h
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_3.h
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_2.h
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_3.h
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_3.h
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_3.h
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/persist/code.h
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/random/operations_cpu.h
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/random/operations_cuda.h
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/operations_generic.h
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/rl.h
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/algorithms.h
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu.h
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu_mkl.h
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_generic.h
--rw-r--r--   0        0        0    21211 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h
--rw-r--r--   0        0        0    17856 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h
--rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h
--rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mkl.h
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mux.h
--rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h
--rw-r--r--   0        0        0    37045 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h
--rw-r--r--   0        0        0     8221 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h
--rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h
--rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mkl.h
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mux.h
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h
--rw-r--r--   0        0        0    21928 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h
--rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/components.h
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu.h
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_mkl.h
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_generic.h
--rw-r--r--   0        0        0     8533 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h
--rw-r--r--   0        0        0    10600 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h
--rw-r--r--   0        0        0    16980 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h
--rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h
--rw-r--r--   0        0        0    12764 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h
--rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_cpu.h
--rw-r--r--   0        0        0     8285 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h
--rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/environments.h
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_cpu.h
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h
--rw-r--r--   0        0        0    11982 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h
--rw-r--r--   0        0        0    10667 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h
--rw-r--r--   0        0        0    68731 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h
--rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/README.MD
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h
--rw-r--r--   0        0        0    30495 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h
--rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_cpu.h
--rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/loop/loop.h
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/config.h
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h
--rw-r--r--   0        0        0     8951 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h
--rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h
--rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/client.h
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/assert/declarations_cpu.h
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/generic/memcpy.h
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/interface/algorithms/ppo/template.h
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/interface/algorithms/sac/template.h
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/interface/algorithms/td3/template.h
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/interface/inference/inference.cpp
--rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/interface/python_environment/operations_cpu.h
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/interface/python_environment/python_environment.h
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/interface/training/training.cpp
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/src/__init__.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/src/accelerate.py
--rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/src/compile.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/src/link_accelerate.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/src/link_blas.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/src/link_mkl.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/src/load_checkpoint.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/src/load_module.py
--rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/src/ppo.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/src/render.py
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/src/sac.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/src/td3.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/src/training.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 tinyrl-0.4.2/tinyrl/src/utils.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tinyrl-0.4.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 tinyrl-0.4.2/LICENSE
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 tinyrl-0.4.2/README.md
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 tinyrl-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 tinyrl-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/__init__.py
+-rw-r--r--   0        0        0    10546 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers.h
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/version.h
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h
+-rw-r--r--   0        0        0    13873 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h
+-rw-r--r--   0        0        0    36763 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/generic.h
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h
+-rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h
+-rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/nn.h
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu.h
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_blas.h
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_openblas.h
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cuda.h
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/operations_dummy.h
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/operations_generic.h
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/persist.h
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/persist_code.h
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/capability/capability.h
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/capability/persist_code.h
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/layers.h
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu.h
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_blas.h
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_mkl.h
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_openblas.h
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cuda.h
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_dummy.h
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_generic.h
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h
+-rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu.h
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h
+-rw-r--r--   0        0        0    25323 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_dummy.h
+-rw-r--r--   0        0        0    18594 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h
+-rw-r--r--   0        0        0     9746 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h
+-rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/sample_and_squash/layer.h
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/sample_and_squash/operations_generic.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/operations_generic.h
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/adam.h
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h
+-rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/operations_generic.h
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_cuda.h
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/models.h
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cpu.h
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cuda.h
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_dummy.h
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_generic.h
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist.h
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist_code.h
+-rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cpu.h
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cuda.h
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_dummy.h
+-rw-r--r--   0        0        0    21316 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist_code.h
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_cpu.h
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/network.h
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_cpu.h
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/random_uniform/model.h
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/random_uniform/operations_generic.h
+-rw-r--r--   0        0        0     7423 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h
+-rw-r--r--   0        0        0    12633 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_2.h
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_3.h
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_2.h
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_3.h
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_3.h
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_3.h
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_3.h
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_3.h
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_2.h
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_3.h
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_3.h
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_3.h
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/persist/code.h
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/random/operations_cpu.h
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/random/operations_cuda.h
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/operations_generic.h
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/rl.h
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/algorithms.h
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu.h
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu_mkl.h
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_generic.h
+-rw-r--r--   0        0        0    21130 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h
+-rw-r--r--   0        0        0    17856 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h
+-rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mux.h
+-rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h
+-rw-r--r--   0        0        0    37266 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h
+-rw-r--r--   0        0        0     8221 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h
+-rw-r--r--   0        0        0    10559 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h
+-rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mux.h
+-rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h
+-rw-r--r--   0        0        0    21944 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h
+-rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h
+-rw-r--r--   0        0        0     9991 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h
+-rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/components.h
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu.h
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_mkl.h
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_generic.h
+-rw-r--r--   0        0        0     8634 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h
+-rw-r--r--   0        0        0    10972 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h
+-rw-r--r--   0        0        0    17112 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h
+-rw-r--r--   0        0        0     8069 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h
+-rw-r--r--   0        0        0    12764 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h
+-rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_cpu.h
+-rw-r--r--   0        0        0     8285 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/environments.h
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_cpu.h
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h
+-rw-r--r--   0        0        0    11982 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h
+-rw-r--r--   0        0        0    10667 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h
+-rw-r--r--   0        0        0    68731 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h
+-rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/README.MD
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h
+-rw-r--r--   0        0        0    30495 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h
+-rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_cpu.h
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/loop.h
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/checkpoint/config.h
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/checkpoint/operations_cpu.h
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/checkpoint/state.h
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/extrack/config.h
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/extrack/operations_cpu.h
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/extrack/state.h
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/config.h
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h
+-rw-r--r--   0        0        0     8951 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h
+-rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h
+-rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/client.h
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/assert/declarations_cpu.h
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/generic/memcpy.h
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/interface/algorithms/ppo/template.h
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/interface/algorithms/sac/template.h
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/interface/algorithms/td3/template.h
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/interface/inference/inference.cpp
+-rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/interface/python_environment/operations_cpu.h
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/interface/python_environment/python_environment.h
+-rw-r--r--   0        0        0     7371 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/interface/training/training.cpp
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/src/__init__.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/src/accelerate.py
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/src/compile.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/src/link_accelerate.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/src/link_blas.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/src/link_mkl.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/src/load_checkpoint.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/src/load_module.py
+-rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/src/ppo.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/src/render.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/src/sac.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/src/td3.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/src/training.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 tinyrl-0.4.3/tinyrl/src/utils.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tinyrl-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 tinyrl-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 tinyrl-0.4.3/README.md
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 tinyrl-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 tinyrl-0.4.3/PKG-INFO
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/version.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/version.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_mkl.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h`

 * *Files 1% similar despite different names*

```diff
@@ -82,23 +82,31 @@
     }
     template<typename DEVICE, typename SPEC>
     void free(DEVICE& device, MatrixDynamic<SPEC>& matrix){
         using TI = typename DEVICE::index_t;
 #ifdef RL_TOOLS_DEBUG_CONTAINER_CHECK_MALLOC
         utils::assert_exit(device, matrix._data != nullptr, "Matrix has not been allocated");
 #endif
+#ifndef RL_TOOLS_DISABLE_ALIGNED_MEMORY_ALLOCATIONS
         char* aligned_byte_pointer = reinterpret_cast<char*>(matrix._data);
         static constexpr TI POINTER_SIZE = sizeof(void*);
         char* original_pointer_storage = aligned_byte_pointer - POINTER_SIZE;
-#ifdef RL_TOOLS_CONTAINERS_USE_MALLOC
-        void* original_pointer = *((void**)original_pointer_storage);
-        ::free(original_pointer);
+    #ifdef RL_TOOLS_CONTAINERS_USE_MALLOC
+            void* original_pointer = *((void**)original_pointer_storage);
+            ::free(original_pointer);
+    #else
+            char* original_pointer = *((char**)original_pointer_storage);
+            delete original_pointer;
+    #endif
 #else
-        char* original_pointer = *((char**)original_pointer_storage);
-        delete original_pointer;
+        #ifdef RL_TOOLS_CONTAINERS_USE_MALLOC
+            ::free(matrix._data);
+        #else
+            delete matrix._data;
+        #endif
 #endif
         matrix._data = nullptr;
     }
 #endif
 
     template<typename SPEC>
     RL_TOOLS_FUNCTION_PLACEMENT constexpr typename SPEC::TI rows(const Matrix<SPEC>& m){
@@ -435,20 +443,20 @@
         return acc;
     }
     template<typename DEVICE, typename SPEC>
     typename SPEC::T mean_of_squares(DEVICE& device, const Matrix<SPEC>& m){
         return sum_of_squares(device, m) / (SPEC::ROWS * SPEC::COLS);
     }
     template<typename DEVICE, typename SPEC>
-    [[deprecated("Note: math::isnan might be optimized out by the compiler when using e.g. fast-math")]]
+//    [[deprecated("Note: math::isnan might be optimized out by the compiler when using e.g. fast-math")]]
     bool is_nan(DEVICE& device, const Matrix<SPEC>& m){
         return reduce_unary<DEVICE, SPEC, bool, containers::vectorization::operators::is_nan<typename DEVICE::SPEC::MATH, typename SPEC::T>>(device, m, false);
     }
     template<typename DEVICE, typename SPEC>
-    [[deprecated("Note: math::isfinite might be optimized out by the compiler when using e.g. fast-math")]]
+//    [[deprecated("Note: math::isfinite might be optimized out by the compiler when using e.g. fast-math")]]
     bool is_finite(DEVICE& device, const Matrix<SPEC>& m){
         return reduce_unary<DEVICE, SPEC, bool, containers::vectorization::operators::is_finite<typename DEVICE::SPEC::MATH, typename SPEC::T>>(device, m, true);
     }
     template<typename DEVICE, typename SPEC>
     typename SPEC::T max(DEVICE& device, const Matrix<SPEC>& m){
         static_assert(SPEC::ROWS > 0 && SPEC::COLS > 0);
         using T = typename SPEC::T;
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h`

 * *Files 9% similar despite different names*

```diff
@@ -53,25 +53,26 @@
         static_assert(sizeof(T) % sizeof(containers::persist::STORAGE_TYPE) == 0);
         std::stringstream indent_ss;
         for(TI i=0; i < indent; i++){
             indent_ss << "    ";
         }
         std::string ind = indent_ss.str();
         std::stringstream ss_header;
+        ss_header << "// NOTE: This code export assumes that the endianness of the target platform is the same as the endianness of the source platform\n";
         ss_header << "#include <rl_tools/containers.h>\n";
         std::stringstream ss;
         ss << ind << "namespace " << name << " {\n";
         ss << ind << "    static_assert(sizeof(" << containers::persist::get_type_string<containers::persist::STORAGE_TYPE>() << ") == 1);\n";
         ss << ind << "    alignas(" << containers::persist::get_type_string<T>() << ") " << (const_declaration ? "const " : "") << containers::persist::get_type_string<containers::persist::STORAGE_TYPE>() << " memory[] = {";
         bool first = true;
         for(TI i=0; i < SPEC::ROWS; i++){
             for(TI j=0; j < SPEC::COLS; j++){
                 auto value = get(m, i, j);
                 auto* ptr = reinterpret_cast<containers::persist::STORAGE_TYPE*>(&value);
-                for(int k=0; k < sizeof(T); k++){
+                for(TI k=0; k < sizeof(T); k++){
                     if(!first){
                         ss << ", ";
                     }
                     ss << (int)ptr[k];
                     first = false;
                 }
             }
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 #if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_DEVICES_CPU_ACCELERATE_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
 #define RL_TOOLS_DEVICES_CPU_ACCELERATE_H
 
 #include "../utils/generic/typing.h"
 #include "devices.h"
 
+#define ACCELERATE_NEW_LAPACK
+#define ACCELERATE_LAPACK_ILP64
 #include "cpu_blas.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools::devices{
     template <typename T_SPEC>
     struct CPU_ACCELERATE: CPU_BLAS<T_SPEC>{
         static constexpr DeviceId DEVICE_ID = DeviceId::CPU_ACCELERATE;
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h`

 * *Files 5% similar despite different names*

```diff
@@ -21,28 +21,23 @@
             if(!logger.topic_frequency_dict.count(key)){
                 logger.topic_frequency_dict.insert({key, 0});
             }
             logger.topic_frequency_dict[key] += 1;
         }
     }
     template <typename DEVICE, typename SPEC>
-    void init(DEVICE& device, devices::logging::CPU_TENSORBOARD<SPEC>& logger){
+    void init(DEVICE& device, devices::logging::CPU_TENSORBOARD<SPEC>& logger, std::filesystem::path run_dir){
         // the path is passed through the (CPU) device since the CPU device always supports the stdlib with std::string etc.
         utils::assert_exit(device, device.initialized, "CPU Device not initialized, can't init tensorboard logger");
-        std::filesystem::path runs_dir = std::filesystem::path(device.runs_path);
-        if(!std::filesystem::is_directory(runs_dir) || !std::filesystem::exists(runs_dir)) {
-            std::filesystem::create_directory(runs_dir);
-        }
-        std::filesystem::path run_dir = std::filesystem::path(device.run_path);
         if (!std::filesystem::is_directory(run_dir) || !std::filesystem::exists(run_dir)) {
-            std::filesystem::create_directory(run_dir);
+            std::filesystem::create_directories(run_dir);
         }
 
         auto log_file = run_dir / std::string("logs.tfevents");
-        std::cout << "Logging to " << log_file.string() << std::endl;
+        std::cerr << "Tensorboard Logger logging to: " << log_file.string() << std::endl;
         TensorBoardLoggerOptions opts;
         opts.flush_period_s(1);
         logger.tb = new TensorBoardLogger(log_file.string(), opts);
     }
     template <typename DEVICE, typename SPEC>
     void free(DEVICE& device, devices::logging::CPU_TENSORBOARD<SPEC>& logger){
         delete logger.tb;
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h`

 * *Files 4% similar despite different names*

```diff
@@ -33,32 +33,32 @@
         static constexpr bool ENFORCE_FLOATING_POINT_TYPE = T_ENFORCE_FLOATING_POINT_TYPE;
         using MEMORY_LAYOUT = T_MEMORY_LAYOUT;
         // Summary
         static constexpr auto NUM_WEIGHTS = CONSTANT_DIM;
     };
 
     template<typename T_SPEC>
-    struct Layer {
+    struct LayerForward{
         using SPEC = T_SPEC;
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         static constexpr TI INPUT_DIM = SPEC::INPUT_DIM;
         static constexpr TI CONSTANT_DIM = SPEC::CONSTANT_DIM;
         static constexpr TI OUTPUT_DIM = SPEC::OUTPUT_DIM;
         static constexpr TI NUM_WEIGHTS = SPEC::NUM_WEIGHTS;
         using WEIGHTS_CONTAINER_SPEC = matrix::Specification<T, TI, 1, CONSTANT_DIM, typename SPEC::MEMORY_LAYOUT>;
         using WEIGHTS_CONTAINER_TYPE = typename SPEC::CONTAINER_TYPE_TAG::template type<WEIGHTS_CONTAINER_SPEC>;
         typename SPEC::PARAMETER_TYPE::template instance<WEIGHTS_CONTAINER_TYPE> constants;
     };
     template<typename SPEC>
-    struct LayerBackward : public Layer<SPEC> {
+    struct LayerBackward : public LayerForward<SPEC> {
         static constexpr typename SPEC::TI BATCH_SIZE = SPEC::BATCH_SIZE;
     };
     template<typename SPEC>
-    struct LayerBackwardGradient : public LayerBackward<SPEC> {
+    struct LayerGradient : public LayerBackward<SPEC> {
         // This layer supports backpropagation wrt its input but including its weights (for this it stores the intermediate outputs in addition to the pre_activations because they determine the gradient wrt the weights of the following layer)
         using OUTPUT_CONTAINER_SPEC = matrix::Specification<typename SPEC::T, typename SPEC::TI, SPEC::BATCH_SIZE, SPEC::OUTPUT_DIM, typename SPEC::MEMORY_LAYOUT>;
         using OUTPUT_CONTAINER_TYPE = typename SPEC::CONTAINER_TYPE_TAG::template type<OUTPUT_CONTAINER_SPEC>;
         OUTPUT_CONTAINER_TYPE output;
     };
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #include "layer.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    void evaluate(DEVICE& device, const nn::layers::concat_constant::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+    void evaluate(DEVICE& device, const nn::layers::concat_constant::LayerForward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         static_assert(nn::layers::concat_constant::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         // Warning do not use the same buffer for input and output!
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using TI = typename DEVICE::index_t;
         auto input_target_view = view(device, output, matrix::ViewSpec<BATCH_SIZE, LAYER_SPEC::INPUT_DIM>{});
         auto constant_target_view = view(device, output, matrix::ViewSpec<BATCH_SIZE, LAYER_SPEC::INPUT_DIM>{}, 0, LAYER_SPEC::INPUT_DIM);
         copy(device, device, input, input_target_view);
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_LAYERS_DENSE_LAYER_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
 #define RL_TOOLS_NN_LAYERS_DENSE_LAYER_H
 #include "../../../nn/activation_functions.h"
 #include "../../../utils/generic/typing.h"
 #include "../../../containers.h"
 
+#include "../../../nn/nn.h"
 #include "../../../nn/parameters/parameters.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools::nn::layers::dense {
     template <typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
     constexpr bool check_input_output_f(){
         static_assert(INPUT_SPEC::COLS == LAYER_SPEC::INPUT_DIM);
@@ -18,42 +19,46 @@
         static_assert(OUTPUT_SPEC::COLS == LAYER_SPEC::OUTPUT_DIM);
         static_assert(!LAYER_SPEC::ENFORCE_FLOATING_POINT_TYPE || utils::typing::is_same_v<typename LAYER_SPEC::T, typename INPUT_SPEC::T>);
         static_assert(!LAYER_SPEC::ENFORCE_FLOATING_POINT_TYPE || utils::typing::is_same_v<typename INPUT_SPEC::T, typename OUTPUT_SPEC::T>);
         return true;
     }
     template <typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
     constexpr bool check_input_output = check_input_output_f<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>();
-    template<typename T_T, typename T_TI, T_TI T_INPUT_DIM, T_TI T_OUTPUT_DIM, nn::activation_functions::ActivationFunction T_ACTIVATION_FUNCTION, typename T_PARAMETER_TYPE, T_TI T_BATCH_SIZE=1, typename T_PARAMETER_GROUP=parameters::groups::Normal, typename T_CONTAINER_TYPE_TAG = MatrixDynamicTag, bool T_ENFORCE_FLOATING_POINT_TYPE=true, typename T_MEMORY_LAYOUT = matrix::layouts::RowMajorAlignmentOptimized<T_TI>>
+    template<typename T_T, typename T_TI, T_TI T_INPUT_DIM, T_TI T_OUTPUT_DIM, nn::activation_functions::ActivationFunction T_ACTIVATION_FUNCTION, T_TI T_BATCH_SIZE=1, typename T_PARAMETER_GROUP=parameters::groups::Normal, typename T_CONTAINER_TYPE_TAG = MatrixDynamicTag, bool T_ENFORCE_FLOATING_POINT_TYPE=true, typename T_MEMORY_LAYOUT = matrix::layouts::RowMajorAlignmentOptimized<T_TI>>
     struct Specification {
         using T = T_T;
         using TI = T_TI;
         static constexpr auto INPUT_DIM = T_INPUT_DIM;
         static constexpr auto OUTPUT_DIM = T_OUTPUT_DIM;
         static constexpr nn::activation_functions::ActivationFunction ACTIVATION_FUNCTION = T_ACTIVATION_FUNCTION;
-        using PARAMETER_TYPE = T_PARAMETER_TYPE;
         using PARAMETER_GROUP = T_PARAMETER_GROUP;
         static constexpr auto BATCH_SIZE = T_BATCH_SIZE;
         using CONTAINER_TYPE_TAG = T_CONTAINER_TYPE_TAG;
         static constexpr bool ENFORCE_FLOATING_POINT_TYPE = T_ENFORCE_FLOATING_POINT_TYPE;
         using MEMORY_LAYOUT = T_MEMORY_LAYOUT;
         // Summary
         static constexpr auto NUM_WEIGHTS = OUTPUT_DIM * INPUT_DIM + OUTPUT_DIM;
     };
+    template <typename T_CAPABILITY, typename T_SPEC>
+    struct CapabilitySpecification: T_SPEC{
+        using CAPABILITY = T_CAPABILITY;
+        using PARAMETER_TYPE = typename CAPABILITY::PARAMETER_TYPE;
+    };
     template<typename SPEC_1, typename SPEC_2>
     constexpr bool check_spec_memory =
             utils::typing::is_same_v<typename SPEC_1::T, typename SPEC_2::T>
             && SPEC_1::INPUT_DIM == SPEC_2::INPUT_DIM
             && SPEC_1::OUTPUT_DIM == SPEC_2::OUTPUT_DIM;
     template<typename SPEC_1, typename SPEC_2>
     constexpr bool check_spec =
         check_spec_memory<SPEC_1, SPEC_2>
         && SPEC_1::ACTIVATION_FUNCTION == SPEC_2::ACTIVATION_FUNCTION;
 
     template<typename T_SPEC>
-    struct Layer {
+    struct LayerForward {
         using SPEC = T_SPEC;
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         using CONTAINER_TYPE_TAG = typename SPEC::CONTAINER_TYPE_TAG;
         static constexpr TI INPUT_DIM = SPEC::INPUT_DIM;
         static constexpr TI OUTPUT_DIM = SPEC::OUTPUT_DIM;
         static constexpr TI NUM_WEIGHTS = SPEC::NUM_WEIGHTS;
@@ -64,25 +69,39 @@
 
         using BIASES_CONTAINER_SPEC = matrix::Specification<T, TI, 1, OUTPUT_DIM, typename SPEC::MEMORY_LAYOUT>;
         using BIASES_CONTAINER_TYPE = typename SPEC::CONTAINER_TYPE_TAG::template type<BIASES_CONTAINER_SPEC>;
         using BIASES_PARAMETER_SPEC = typename SPEC::PARAMETER_TYPE::template spec<BIASES_CONTAINER_TYPE, typename SPEC::PARAMETER_GROUP, nn::parameters::categories::Biases>;
         typename SPEC::PARAMETER_TYPE::template instance<BIASES_PARAMETER_SPEC> biases;
     };
     template<typename SPEC>
-    struct LayerBackward : public Layer<SPEC> {
+    struct LayerBackward: public LayerForward<SPEC> {
         static constexpr typename SPEC::TI BATCH_SIZE = SPEC::BATCH_SIZE;
         // This layer supports backpropagation wrt its input but not its weights (for this it stores the intermediate pre_activations)
         using PRE_ACTIVATIONS_CONTAINER_SPEC = matrix::Specification<typename SPEC::T, typename SPEC::TI, SPEC::BATCH_SIZE, SPEC::OUTPUT_DIM>;
         using PRE_ACTIVATIONS_CONTAINER_TYPE = typename SPEC::CONTAINER_TYPE_TAG::template type<PRE_ACTIVATIONS_CONTAINER_SPEC>;
         PRE_ACTIVATIONS_CONTAINER_TYPE pre_activations;
     };
     template<typename SPEC>
-    struct LayerBackwardGradient : public LayerBackward<SPEC> {
+    struct LayerGradient: public LayerBackward<SPEC> {
         // This layer supports backpropagation wrt its input but including its weights (for this it stores the intermediate outputs in addition to the pre_activations because they determine the gradient wrt the weights of the following layer)
         using OUTPUT_CONTAINER_SPEC = matrix::Specification<typename SPEC::T, typename SPEC::TI, SPEC::BATCH_SIZE, SPEC::OUTPUT_DIM, typename SPEC::MEMORY_LAYOUT>;
         using OUTPUT_CONTAINER_TYPE = typename SPEC::CONTAINER_TYPE_TAG::template type<OUTPUT_CONTAINER_SPEC>;
         OUTPUT_CONTAINER_TYPE output;
     };
+    template<typename CAPABILITY, typename SPEC>
+    using Layer =
+        typename utils::typing::conditional_t<CAPABILITY::TAG == nn::LayerCapability::Forward,
+            LayerForward<CapabilitySpecification<CAPABILITY, SPEC>>,
+        typename utils::typing::conditional_t<CAPABILITY::TAG == nn::LayerCapability::Backward,
+            LayerBackward<CapabilitySpecification<CAPABILITY, SPEC>>,
+        typename utils::typing::conditional_t<CAPABILITY::TAG == nn::LayerCapability::Gradient,
+            LayerGradient<CapabilitySpecification<CAPABILITY, SPEC>>, void>>>;
+
+    template <typename T_SPEC>
+    struct BindSpecification{
+        template <typename CAPABILITY>
+        using Layer = nn::layers::dense::Layer<CAPABILITY, T_SPEC>;
+    };
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 #include <Accelerate/Accelerate.h>
 #include "operations_cpu_blas.h"
 #include "../../../devices/cpu_accelerate.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    RL_TOOLS_FUNCTION_PLACEMENT void evaluate(devices::CPU_ACCELERATE<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+    RL_TOOLS_FUNCTION_PLACEMENT void evaluate(devices::CPU_ACCELERATE<DEV_SPEC>& device, const nn::layers::dense::LayerForward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         evaluate((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output, rng);
     }
 
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
     RL_TOOLS_FUNCTION_PLACEMENT void forward(devices::CPU_ACCELERATE<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         forward((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output, rng);
     }
 
     template<typename DEV_SPEC, typename LAYER_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void backward_input(devices::CPU_ACCELERATE<DEV_SPEC>& device, const nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
+    RL_TOOLS_FUNCTION_PLACEMENT void backward_input(devices::CPU_ACCELERATE<DEV_SPEC>& device, const nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         backward_input((devices::CPU_BLAS<DEV_SPEC> &) device, layer, d_output, d_input);
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void backward_param(devices::CPU_ACCELERATE<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output) {
+    RL_TOOLS_FUNCTION_PLACEMENT void backward_param(devices::CPU_ACCELERATE<DEV_SPEC>& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output) {
         backward_param((devices::CPU_BLAS<DEV_SPEC> &) device, layer, input, d_output);
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void backward(devices::CPU_ACCELERATE<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
+    RL_TOOLS_FUNCTION_PLACEMENT void backward(devices::CPU_ACCELERATE<DEV_SPEC>& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         backward((devices::CPU_BLAS<DEV_SPEC> &) device, layer, input, d_output, d_input);
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //     void cblas_sgemm(const enum CBLAS_ORDER Order, const enum CBLAS_TRANSPOSE TransA, const enum CBLAS_TRANSPOSE TransB, const int M, const int N, const int K, const float alpha, const float *A, const int lda, const float *B, const int ldb, const float beta, float *C, const int ldc);
 //     void cblas_dgemm(const enum CBLAS_ORDER Order, const enum CBLAS_TRANSPOSE TransA, const enum CBLAS_TRANSPOSE TransB, const int M, const int N, const int K, const double alpha, const double *A, const int lda, const double *B, const int ldb, const double beta, double *C, const int ldc);
 // }
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    void evaluate(devices::CPU_BLAS<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+    void evaluate(devices::CPU_BLAS<DEV_SPEC>& device, const nn::layers::dense::LayerForward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
 
         // Warning do not use the same buffer for input and output!
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using DEVICE = devices::CPU_BLAS<DEV_SPEC>;
         using T = typename LAYER_SPEC::T;
         using TI = typename DEVICE::index_t;
@@ -97,15 +97,15 @@
             for(TI output_i = 0; output_i < OUTPUT_DIM; output_i++) {
                 T d_pre_activation = d_activation_d_x<typename DEV_SPEC::MATH, T, LAYER_SPEC::ACTIVATION_FUNCTION>(get(layer.pre_activations, batch_i, output_i)) * get(d_output, batch_i, output_i);
                 set(d_pre_activations, batch_i, output_i, d_pre_activation);
             }
         }
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC>
-    void backward_param(devices::CPU_BLAS<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output) {
+    void backward_param(devices::CPU_BLAS<DEV_SPEC>& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output) {
         // Warning do not reuse d_output as d_output is used as a temporary buffer
         // todo: create sparate function that does not set d_input (to save cost on backward pass for the first layer)
         // todo: think about storing gradient in column major order to avoid iterating over the minor dimension
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, D_OUTPUT_SPEC>);
         constexpr auto OUTPUT_DIM = LAYER_SPEC::OUTPUT_DIM;
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using T = typename LAYER_SPEC::T;
@@ -169,15 +169,15 @@
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
     void backward_input(devices::CPU_BLAS<DEV_SPEC>& device, const nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         backward_pre_activations(device, layer, d_output, d_output);
         backward_input_additional(device, layer, d_output, d_input);
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
-    void backward(devices::CPU_BLAS<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
+    void backward(devices::CPU_BLAS<DEV_SPEC>& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         backward_param(device, layer, input, d_output);
         backward_input_additional(device, layer, d_output, d_input);
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h`

 * *Files 3% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 
 #include "operations_cpu_blas.h"
 #include "../../../devices/cpu_mkl.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    RL_TOOLS_FUNCTION_PLACEMENT void evaluate(devices::CPU_MKL<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng){
+    RL_TOOLS_FUNCTION_PLACEMENT void evaluate(devices::CPU_MKL<DEV_SPEC>& device, const nn::layers::dense::LayerForward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng){
         evaluate((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output, rng);
     }
 
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
     RL_TOOLS_FUNCTION_PLACEMENT void forward(devices::CPU_MKL<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng){
         forward((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output, rng);
     }
 
     template<typename DEV_SPEC, typename LAYER_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void backward_input(devices::CPU_MKL<DEV_SPEC>& device, const nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
+    RL_TOOLS_FUNCTION_PLACEMENT void backward_input(devices::CPU_MKL<DEV_SPEC>& device, const nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         backward_input((devices::CPU_BLAS<DEV_SPEC> &) device, layer, d_output, d_input);
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void backward_param(devices::CPU_MKL<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output) {
+    RL_TOOLS_FUNCTION_PLACEMENT void backward_param(devices::CPU_MKL<DEV_SPEC>& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output) {
         backward_param((devices::CPU_BLAS<DEV_SPEC> &) device, layer, input, d_output);
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void backward(devices::CPU_MKL<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
+    RL_TOOLS_FUNCTION_PLACEMENT void backward(devices::CPU_MKL<DEV_SPEC>& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         backward((devices::CPU_BLAS<DEV_SPEC> &) device, layer, input, d_output, d_input);
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h`

 * *Files 6% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 
 #include "operations_cpu_blas.h"
 #include "../../../devices/cpu_openblas.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    RL_TOOLS_FUNCTION_PLACEMENT void evaluate(devices::CPU_OPENBLAS<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+    RL_TOOLS_FUNCTION_PLACEMENT void evaluate(devices::CPU_OPENBLAS<DEV_SPEC>& device, const nn::layers::dense::LayerForward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         evaluate((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output, rng);
     }
 
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
     RL_TOOLS_FUNCTION_PLACEMENT void forward(devices::CPU_OPENBLAS<DEV_SPEC>& device, nn::layers::dense::LayerBackward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         forward((devices::CPU_BLAS<DEV_SPEC>&) device, layer, input, output, rng);
     }
 
     template<typename DEV_SPEC, typename LAYER_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void backward_input(devices::CPU_OPENBLAS<DEV_SPEC>& device, const nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
+    RL_TOOLS_FUNCTION_PLACEMENT void backward_input(devices::CPU_OPENBLAS<DEV_SPEC>& device, const nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         backward_input((devices::CPU_BLAS<DEV_SPEC> &) device, layer, d_output, d_input);
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void backward_param(devices::CPU_OPENBLAS<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output) {
+    RL_TOOLS_FUNCTION_PLACEMENT void backward_param(devices::CPU_OPENBLAS<DEV_SPEC>& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output) {
         backward_param((devices::CPU_BLAS<DEV_SPEC> &) device, layer, input, d_output);
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
-    RL_TOOLS_FUNCTION_PLACEMENT void backward(devices::CPU_OPENBLAS<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
+    RL_TOOLS_FUNCTION_PLACEMENT void backward(devices::CPU_OPENBLAS<DEV_SPEC>& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         backward((devices::CPU_BLAS<DEV_SPEC> &) device, layer, input, d_output, d_input);
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #include <cublas_v2.h>
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     namespace nn::dense::cuda{
         template<typename DEV_SPEC, typename SPEC, typename OUTPUT_SPEC>
         __global__ void
-        set_biases_kernel(devices::CUDA<DEV_SPEC> device, const nn::layers::dense::Layer<SPEC> layer, Matrix<OUTPUT_SPEC> output) {
+        set_biases_kernel(devices::CUDA<DEV_SPEC> device, const nn::layers::dense::LayerForward<SPEC> layer, Matrix<OUTPUT_SPEC> output) {
             using T = typename SPEC::T;
             using TI = typename devices::CUDA<DEV_SPEC>::index_t;
             constexpr TI INPUT_DIM = SPEC::INPUT_DIM;
             constexpr TI OUTPUT_DIM = SPEC::OUTPUT_DIM;
             constexpr TI BATCH_SIZE = OUTPUT_SPEC::ROWS;
 
             TI output_pos = blockIdx.x * blockDim.x + threadIdx.x;
@@ -27,42 +27,42 @@
                 T bias = get(layer.biases.parameters, 0, output_pos);
                 for(TI batch_i = 0; batch_i < BATCH_SIZE; batch_i++){
                     set(output, batch_i, output_pos, bias);
                 }
             }
         }
         template<typename DEV_SPEC, typename SPEC, typename OUTPUT_SPEC>
-        void set_biases(devices::CUDA<DEV_SPEC>& device, const nn::layers::dense::Layer<SPEC>& layer, Matrix<OUTPUT_SPEC>& output) {
+        void set_biases(devices::CUDA<DEV_SPEC>& device, const nn::layers::dense::LayerForward<SPEC>& layer, Matrix<OUTPUT_SPEC>& output) {
             using DEVICE = devices::CUDA<DEV_SPEC>;
             constexpr typename devices::CUDA<DEV_SPEC>::index_t BLOCKSIZE_BIAS = 32;
             constexpr typename devices::CUDA<DEV_SPEC>::index_t N_BLOCKS_BIAS = RL_TOOLS_DEVICES_CUDA_CEIL(SPEC::OUTPUT_DIM, BLOCKSIZE_BIAS);
             dim3 bias_grid(N_BLOCKS_BIAS);
             dim3 bias_block(BLOCKSIZE_BIAS);
             devices::cuda::TAG<DEVICE, true> tag_device{};
             nn::dense::cuda::set_biases_kernel<<<bias_grid, bias_block, 0, device.stream>>>(tag_device, layer, output);
             check_status(device);
         }
         template<typename DEV_SPEC, typename SPEC, typename PRE_ACTIVATIONS_SPEC, typename OUTPUT_SPEC>
         __global__ void
-        activation_kernel(devices::CUDA<DEV_SPEC> device, const nn::layers::dense::Layer<SPEC>& layer, Matrix<PRE_ACTIVATIONS_SPEC> pre_activations, Matrix<OUTPUT_SPEC> output) {
+        activation_kernel(devices::CUDA<DEV_SPEC> device, const nn::layers::dense::LayerForward<SPEC>& layer, Matrix<PRE_ACTIVATIONS_SPEC> pre_activations, Matrix<OUTPUT_SPEC> output) {
             using T = typename SPEC::T;
             using TI = typename devices::CUDA<DEV_SPEC>::index_t;
             static_assert(PRE_ACTIVATIONS_SPEC::ROWS == OUTPUT_SPEC::ROWS);
             constexpr TI INPUT_DIM = SPEC::INPUT_DIM;
             constexpr TI OUTPUT_DIM = SPEC::OUTPUT_DIM;
             constexpr TI BATCH_SIZE = PRE_ACTIVATIONS_SPEC::ROWS;
 
             TI output_pos_x = blockIdx.x * blockDim.x + threadIdx.x;
             TI output_pos_y = blockIdx.y * blockDim.y + threadIdx.y;
             if(output_pos_x < OUTPUT_DIM && output_pos_y < BATCH_SIZE){
                 set(output, output_pos_y, output_pos_x, rl_tools::activation<typename DEV_SPEC::MATH, T, SPEC::ACTIVATION_FUNCTION>(get(pre_activations, output_pos_y, output_pos_x)));
             }
         }
         template<typename DEV_SPEC, typename SPEC, typename PRE_ACTIVATIONS_SPEC, typename OUTPUT_SPEC>
-        void activation(devices::CUDA<DEV_SPEC>& device, const nn::layers::dense::Layer<SPEC>& layer, Matrix<PRE_ACTIVATIONS_SPEC>& pre_activations, Matrix<OUTPUT_SPEC>& output){
+        void activation(devices::CUDA<DEV_SPEC>& device, const nn::layers::dense::LayerForward<SPEC>& layer, Matrix<PRE_ACTIVATIONS_SPEC>& pre_activations, Matrix<OUTPUT_SPEC>& output){
             using DEVICE = devices::CUDA<DEV_SPEC>;
             using T = typename SPEC::T;
             using TI = typename DEVICE::index_t;
             static_assert(PRE_ACTIVATIONS_SPEC::ROWS == OUTPUT_SPEC::ROWS);
             constexpr TI BATCH_SIZE = PRE_ACTIVATIONS_SPEC::ROWS;
             constexpr typename devices::CUDA<DEV_SPEC>::index_t BLOCKSIZE_ACTIVATION_BATCH = 32;
             constexpr typename devices::CUDA<DEV_SPEC>::index_t BLOCKSIZE_ACTIVATION_OUTPUT = 32;
@@ -72,15 +72,15 @@
             dim3 activation_block(BLOCKSIZE_ACTIVATION_OUTPUT, BLOCKSIZE_ACTIVATION_BATCH);
             devices::cuda::TAG<DEVICE, true> tag_device{};
             nn::dense::cuda::activation_kernel<<<activation_grid, activation_block, 0, device.stream>>>(tag_device, layer, pre_activations, output);
             check_status(device);
         }
         template<typename DEV_SPEC, typename SPEC, typename PRE_ACTIVATIONS_SPEC, typename D_OUTPUT_SPEC, typename D_PRE_ACTIVATIONS_SPEC>
         __global__ void
-        d_activation_kernel(devices::CUDA<DEV_SPEC> device, const nn::layers::dense::Layer<SPEC> layer, Matrix<PRE_ACTIVATIONS_SPEC> pre_activations, Matrix<D_OUTPUT_SPEC> d_output, Matrix<D_PRE_ACTIVATIONS_SPEC> d_pre_activations) {
+        d_activation_kernel(devices::CUDA<DEV_SPEC> device, const nn::layers::dense::LayerForward<SPEC> layer, Matrix<PRE_ACTIVATIONS_SPEC> pre_activations, Matrix<D_OUTPUT_SPEC> d_output, Matrix<D_PRE_ACTIVATIONS_SPEC> d_pre_activations) {
             using T = typename SPEC::T;
             using TI = typename devices::CUDA<DEV_SPEC>::index_t;
             constexpr TI OUTPUT_DIM = SPEC::OUTPUT_DIM;
             static_assert(containers::check_structure<PRE_ACTIVATIONS_SPEC, D_OUTPUT_SPEC>);
             static_assert(containers::check_structure<D_OUTPUT_SPEC, D_PRE_ACTIVATIONS_SPEC>);
             constexpr TI BATCH_SIZE = PRE_ACTIVATIONS_SPEC::ROWS;
 
@@ -91,27 +91,27 @@
                     T d_pre_activation_temp = d_activation_d_x<typename DEV_SPEC::MATH, T, SPEC::ACTIVATION_FUNCTION>(get(pre_activations, batch_i, output_i)) * get(d_output, batch_i, output_i);
                     set(d_pre_activations, batch_i, output_i, d_pre_activation_temp);
                     acc += d_pre_activation_temp;
                 }
             }
         }
         template<typename DEV_SPEC, typename SPEC, typename PRE_ACTIVATIONS_SPEC, typename D_OUTPUT_SPEC, typename D_PRE_ACTIVATIONS_SPEC>
-        void d_activation(devices::CUDA<DEV_SPEC>& device, const nn::layers::dense::Layer<SPEC>& layer, Matrix<PRE_ACTIVATIONS_SPEC>& pre_activations, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_PRE_ACTIVATIONS_SPEC>& d_pre_activations) {
+        void d_activation(devices::CUDA<DEV_SPEC>& device, const nn::layers::dense::LayerForward<SPEC>& layer, Matrix<PRE_ACTIVATIONS_SPEC>& pre_activations, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_PRE_ACTIVATIONS_SPEC>& d_pre_activations) {
             using DEVICE = devices::CUDA<DEV_SPEC>;
             constexpr typename devices::CUDA<DEV_SPEC>::index_t BLOCKSIZE_ACTIVATION_OUTPUT = 32;
             constexpr typename devices::CUDA<DEV_SPEC>::index_t N_BLOCKS_ACTIVATION_OUTPUT = RL_TOOLS_DEVICES_CUDA_CEIL(SPEC::OUTPUT_DIM, BLOCKSIZE_ACTIVATION_OUTPUT);
             dim3 activation_grid(N_BLOCKS_ACTIVATION_OUTPUT);
             dim3 activation_block(BLOCKSIZE_ACTIVATION_OUTPUT);
             devices::cuda::TAG<DEVICE, true> tag_device{};
             nn::dense::cuda::d_activation_kernel<<<activation_grid, activation_block, 0, device.stream>>>(tag_device, layer, pre_activations, d_output, d_pre_activations);
             check_status(device);
         }
         template<typename DEV_SPEC, typename SPEC, typename PRE_ACTIVATIONS_SPEC, typename D_OUTPUT_SPEC, typename D_BIASES_SPEC, typename D_PRE_ACTIVATIONS_SPEC>
         __global__ void
-        d_activation_accumulate_bias_gradient_kernel(devices::CUDA<DEV_SPEC> device, const nn::layers::dense::Layer<SPEC> layer, Matrix<PRE_ACTIVATIONS_SPEC> pre_activations, Matrix<D_OUTPUT_SPEC> d_output, Matrix<D_BIASES_SPEC> d_biases, Matrix<D_PRE_ACTIVATIONS_SPEC> d_pre_activations) {
+        d_activation_accumulate_bias_gradient_kernel(devices::CUDA<DEV_SPEC> device, const nn::layers::dense::LayerForward<SPEC> layer, Matrix<PRE_ACTIVATIONS_SPEC> pre_activations, Matrix<D_OUTPUT_SPEC> d_output, Matrix<D_BIASES_SPEC> d_biases, Matrix<D_PRE_ACTIVATIONS_SPEC> d_pre_activations) {
             using T = typename SPEC::T;
             using TI = typename devices::CUDA<DEV_SPEC>::index_t;
             constexpr TI OUTPUT_DIM = SPEC::OUTPUT_DIM;
             static_assert(containers::check_structure<PRE_ACTIVATIONS_SPEC, D_OUTPUT_SPEC>);
             static_assert(containers::check_structure<D_OUTPUT_SPEC, D_PRE_ACTIVATIONS_SPEC>);
             constexpr TI BATCH_SIZE = PRE_ACTIVATIONS_SPEC::ROWS;
             static_assert(PRE_ACTIVATIONS_SPEC::COLS == D_BIASES_SPEC::COLS);
@@ -124,27 +124,27 @@
                     set(d_pre_activations, batch_i, output_i, d_pre_activation_temp);
                     acc += d_pre_activation_temp;
                 }
                 increment(d_biases, 0, output_i, acc);
             }
         }
         template<typename DEV_SPEC, typename SPEC, typename PRE_ACTIVATIONS_SPEC, typename D_OUTPUT_SPEC, typename D_BIASES_SPEC, typename D_PRE_ACTIVATIONS_SPEC>
-        void d_activation_accumulate_bias_gradient(devices::CUDA<DEV_SPEC>& device, const nn::layers::dense::Layer<SPEC>& layer, Matrix<PRE_ACTIVATIONS_SPEC>& pre_activations, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_BIASES_SPEC>& d_biases, Matrix<D_PRE_ACTIVATIONS_SPEC>& d_pre_activations) {
+        void d_activation_accumulate_bias_gradient(devices::CUDA<DEV_SPEC>& device, const nn::layers::dense::LayerForward<SPEC>& layer, Matrix<PRE_ACTIVATIONS_SPEC>& pre_activations, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_BIASES_SPEC>& d_biases, Matrix<D_PRE_ACTIVATIONS_SPEC>& d_pre_activations) {
             using DEVICE = devices::CUDA<DEV_SPEC>;
             constexpr typename devices::CUDA<DEV_SPEC>::index_t BLOCKSIZE_ACTIVATION_OUTPUT = 32;
             constexpr typename devices::CUDA<DEV_SPEC>::index_t N_BLOCKS_ACTIVATION_OUTPUT = RL_TOOLS_DEVICES_CUDA_CEIL(SPEC::OUTPUT_DIM, BLOCKSIZE_ACTIVATION_OUTPUT);
             dim3 activation_grid(N_BLOCKS_ACTIVATION_OUTPUT);
             dim3 activation_block(BLOCKSIZE_ACTIVATION_OUTPUT);
             devices::cuda::TAG<DEVICE, true> tag_device{};
             nn::dense::cuda::d_activation_accumulate_bias_gradient_kernel<<<activation_grid, activation_block, 0, device.stream>>>(tag_device, layer, pre_activations, d_output, d_biases, d_pre_activations);
             check_status(device);
         }
         template<typename DEV_SPEC, typename SPEC, typename PARAMETERS>
         __global__
-        void update_kernel(devices::CUDA<DEV_SPEC> device, nn::layers::dense::LayerBackwardGradient<SPEC> layer, nn::optimizers::Adam<PARAMETERS> optimizer) {
+        void update_kernel(devices::CUDA<DEV_SPEC> device, nn::layers::dense::LayerGradient<SPEC> layer, nn::optimizers::Adam<PARAMETERS> optimizer) {
             // fully fused adam update
             using DEVICE = devices::CUDA<DEV_SPEC>;
             using T = typename SPEC::T;
             using TI = typename DEVICE::index_t;
             constexpr TI INPUT_DIM = SPEC::INPUT_DIM;
             constexpr TI OUTPUT_DIM = SPEC::OUTPUT_DIM;
 
@@ -168,15 +168,15 @@
                 T weight_update = optimizer.parameters.alpha * optimizer.first_order_moment_bias_correction * d_weight_first_order_moment / (math::sqrt(typename DEVICE::SPEC::MATH_DEVICE_ACCURATE(), d_weight_second_order_moment * optimizer.second_order_moment_bias_correction) + optimizer.parameters.epsilon);
                 increment(layer.weights.parameters, output_i, input_i, -weight_update);
             }
         }
     }
 
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    void evaluate(devices::CUDA<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng){
+    void evaluate(devices::CUDA<DEV_SPEC>& device, const nn::layers::dense::LayerForward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng){
         // Warning do not use the same buffer for input and output!
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         static_assert(INPUT_SPEC::COL_PITCH == 1);
         static_assert(OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.parameters)::COL_PITCH == 1);
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using DEVICE = devices::CUDA<DEV_SPEC>;
@@ -242,15 +242,15 @@
 
         copy(device, device, output, layer.pre_activations);
 
         nn::dense::cuda::activation(device, layer, output, output);
     }
 
     template<typename DEV_SPEC, typename LAYER_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
-    void backward_input_additional(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
+    void backward_input_additional(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, D_INPUT_SPEC, D_OUTPUT_SPEC>);
         static_assert(D_OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(D_INPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.gradient)::COL_PITCH == 1);
 
         constexpr auto INPUT_DIM = LAYER_SPEC::INPUT_DIM;
         constexpr auto OUTPUT_DIM = LAYER_SPEC::OUTPUT_DIM;
@@ -278,15 +278,15 @@
             }
             if(stat != CUBLAS_STATUS_SUCCESS){
                 std::cout << "CUBLAS ERROR: " << cublasGetStatusString(stat) << std::endl;
             }
         }
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC>
-    void backward_param(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output) {
+    void backward_param(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output) {
         // Warning do not reuse d_output as d_output is used as a temporary buffer
         // todo: create sparate function that does not set d_input (to save cost on backward pass for the first layer)
         // todo: think about storing gradient in column major order to avoid iterating over the minor dimension
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, D_OUTPUT_SPEC>);
         static_assert(INPUT_SPEC::COL_PITCH == 1);
         static_assert(D_OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.gradient)::COL_PITCH == 1);
@@ -320,45 +320,45 @@
             }
             if(stat != CUBLAS_STATUS_SUCCESS){
                 std::cout << "CUBLAS ERROR: " << cublasGetStatusString(stat) << std::endl;
             }
         }
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
-    void backward(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
+    void backward(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         backward_param(device, layer, input, d_output);
         backward_input_additional(device, layer, d_output, d_input);
     }
     template<typename DEV_SPEC, typename LAYER_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
-    void backward_input(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
+    void backward_input(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         nn::dense::cuda::d_activation(device, layer, layer.pre_activations, d_output, d_output);
         backward_input_additional(device, layer, d_output, d_input);
     }
 
     template<typename DEV_SPEC, typename SPEC>
-    void zero_gradient(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<SPEC>& layer) {
+    void zero_gradient(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerGradient<SPEC>& layer) {
         cudaMemset(layer.weights.gradient._data, 0, decltype(layer.weights.gradient)::SPEC::SIZE_BYTES);
         check_status(device);
         cudaMemset(layer.biases.gradient._data, 0, decltype(layer.biases.gradient)::SPEC::SIZE_BYTES);
         check_status(device);
     }
     template<typename DEV_SPEC, typename SPEC, typename PARAMETERS>
-    void _reset_optimizer_state(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<SPEC>& layer, nn::optimizers::Adam<PARAMETERS>& optimizer) {
+    void _reset_optimizer_state(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerGradient<SPEC>& layer, nn::optimizers::Adam<PARAMETERS>& optimizer) {
         cudaMemset(layer.weights.gradient_first_order_moment._data, 0, decltype(layer.weights.gradient_first_order_moment)::SPEC::SIZE_BYTES);
         check_status(device);
         cudaMemset(layer.weights.gradient_second_order_moment._data, 0, decltype(layer.weights.gradient_second_order_moment)::SPEC::SIZE_BYTES);
         check_status(device);
         cudaMemset(layer.biases.gradient_first_order_moment._data, 0, decltype(layer.biases.gradient_first_order_moment)::SPEC::SIZE_BYTES);
         check_status(device);
         cudaMemset(layer.biases.gradient_second_order_moment._data, 0, decltype(layer.biases.gradient_second_order_moment)::SPEC::SIZE_BYTES);
         check_status(device);
     }
 
     template<typename DEV_SPEC, typename SPEC, typename PARAMETERS>
-    void update(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerBackwardGradient<SPEC>& layer, nn::optimizers::Adam<PARAMETERS>& optimizer) {
+    void update(devices::CUDA<DEV_SPEC>& device, nn::layers::dense::LayerGradient<SPEC>& layer, nn::optimizers::Adam<PARAMETERS>& optimizer) {
         using DEVICE = devices::CUDA<DEV_SPEC>;
         constexpr typename devices::CUDA<DEV_SPEC>::index_t BLOCKSIZE_ACTIVATION_OUTPUT = 32;
         constexpr typename devices::CUDA<DEV_SPEC>::index_t BLOCKSIZE_ACTIVATION_INPUT = 32;
         constexpr typename devices::CUDA<DEV_SPEC>::index_t N_BLOCKS_ACTIVATION_OUTPUT = RL_TOOLS_DEVICES_CUDA_CEIL(SPEC::OUTPUT_DIM, BLOCKSIZE_ACTIVATION_OUTPUT);
         constexpr typename devices::CUDA<DEV_SPEC>::index_t N_BLOCKS_ACTIVATION_INPUT = RL_TOOLS_DEVICES_CUDA_CEIL(SPEC::INPUT_DIM, BLOCKSIZE_ACTIVATION_INPUT);
         dim3 activation_grid(N_BLOCKS_ACTIVATION_INPUT, N_BLOCKS_ACTIVATION_OUTPUT);
         dim3 activation_block(BLOCKSIZE_ACTIVATION_INPUT, BLOCKSIZE_ACTIVATION_OUTPUT);
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h`

 * *Files 3% similar despite different names*

```diff
@@ -10,46 +10,46 @@
 #ifndef RL_TOOLS_FUNCTION_PLACEMENT
 #define RL_TOOLS_FUNCTION_PLACEMENT
 #endif
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template<typename DEVICE, typename SPEC>
-    void malloc(DEVICE& device, nn::layers::dense::Layer<SPEC>& layer) {
+    void malloc(DEVICE& device, nn::layers::dense::LayerForward<SPEC>& layer) {
         malloc(device, layer.weights);
         malloc(device, layer.biases);
     }
     template<typename DEVICE, typename SPEC>
-    void free(DEVICE& device, nn::layers::dense::Layer<SPEC>& layer) {
+    void free(DEVICE& device, nn::layers::dense::LayerForward<SPEC>& layer) {
         free(device, layer.weights);
         free(device, layer.biases);
     }
     template<typename DEVICE, typename SPEC>
     void malloc(DEVICE& device, nn::layers::dense::LayerBackward<SPEC>& layer) {
-        malloc(device, (nn::layers::dense::Layer<SPEC>&) layer);
+        malloc(device, (nn::layers::dense::LayerForward<SPEC>&) layer);
         malloc(device, layer.pre_activations);
     }
     template<typename DEVICE, typename SPEC>
     void free(DEVICE& device, nn::layers::dense::LayerBackward<SPEC>& layer) {
-        free(device, (nn::layers::dense::Layer<SPEC>&) layer);
+        free(device, (nn::layers::dense::LayerForward<SPEC>&) layer);
         free(device, layer.pre_activations);
     }
     template<typename DEVICE, typename SPEC>
-    void malloc(DEVICE& device, nn::layers::dense::LayerBackwardGradient<SPEC>& layer) {
+    void malloc(DEVICE& device, nn::layers::dense::LayerGradient<SPEC>& layer) {
         malloc(device, (nn::layers::dense::LayerBackward<SPEC>&) layer);
         malloc(device, layer.output);
     }
     template<typename DEVICE, typename SPEC>
-    void free(DEVICE& device, nn::layers::dense::LayerBackwardGradient<SPEC>& layer) {
+    void free(DEVICE& device, nn::layers::dense::LayerGradient<SPEC>& layer) {
         free(device, (nn::layers::dense::LayerBackward<SPEC>&) layer);
         free(device, layer.output);
     }
 
     template<typename DEVICE, typename SPEC, typename RNG>
-    void init_kaiming(DEVICE& device, nn::layers::dense::Layer<SPEC>& layer, RNG& rng) {
+    void init_kaiming(DEVICE& device, nn::layers::dense::LayerForward<SPEC>& layer, RNG& rng) {
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         T negative_slope = math::sqrt(device.math, (T)5);
         T gain = math::sqrt(device.math, (T)2.0 / (1 + negative_slope * negative_slope));
         T fan = SPEC::INPUT_DIM;
         T std = gain / math::sqrt(device.math, fan);
         T weight_bound = math::sqrt(device.math, (T)3.0) * std;
@@ -58,21 +58,21 @@
             set(layer.biases.parameters, 0, i, (T)random::uniform_real_distribution(typename DEVICE::SPEC::RANDOM(), -bias_bound, bias_bound, rng));
             for(TI j = 0; j < SPEC::INPUT_DIM; j++) {
                 set(layer.weights.parameters, i, j, random::uniform_real_distribution(typename DEVICE::SPEC::RANDOM(), -weight_bound, weight_bound, rng));
             }
         }
     }
     template<typename DEVICE, typename SPEC, typename RNG>
-    void init_weights(DEVICE& device, nn::layers::dense::Layer<SPEC>& layer, RNG& rng) {
+    void init_weights(DEVICE& device, nn::layers::dense::LayerForward<SPEC>& layer, RNG& rng) {
         init_kaiming(device, layer, rng);
     }
 
 #ifndef RL_TOOLS_NN_DISABLE_GENERIC_FORWARD_BACKWARD
     template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    void evaluate(DEVICE& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+    void evaluate(DEVICE& device, const nn::layers::dense::LayerForward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         // Warning do not use the same buffer for input and output!
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using TI = typename DEVICE::index_t;
         for(TI batch_i=0; batch_i < BATCH_SIZE; batch_i++){
             for(TI output_i = 0; output_i < LAYER_SPEC::OUTPUT_DIM; output_i++) {
                 set(output, batch_i, output_i, get(layer.biases.parameters, 0, output_i));
@@ -101,20 +101,20 @@
                 set(output, batch_i, i, activation<typename DEVICE::SPEC::MATH, T, LAYER_SPEC::ACTIVATION_FUNCTION>(get(layer.pre_activations, batch_i, i)));
             }
         }
     }
 #endif
 
     template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename RNG>
-    void forward(DEVICE& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, RNG& rng) {
+    void forward(DEVICE& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, RNG& rng) {
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, typename decltype(layer.output)::SPEC>);
         forward(device, (nn::layers::dense::LayerBackward<LAYER_SPEC>&)layer, input, layer.output, rng);
     }
     template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    void forward(DEVICE& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+    void forward(DEVICE& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         // compile time warning if used
         forward(device, layer, input, rng);
         copy(device, device, layer.output, output);
     }
 
 #ifndef RL_TOOLS_NN_DISABLE_GENERIC_FORWARD_BACKWARD
@@ -137,15 +137,15 @@
                 }
             }
         }
     }
 
 
     template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC>
-    void backward_param(DEVICE& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output) {
+    void backward_param(DEVICE& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output) {
         // todo: create sparate function that does not set d_input (to save cost on backward pass for the first layer)
         // todo: think about storing gradient in column major order to avoid iterating over the minor dimension
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, D_OUTPUT_SPEC>);
         constexpr auto INPUT_DIM = LAYER_SPEC::INPUT_DIM;
         constexpr auto OUTPUT_DIM = LAYER_SPEC::OUTPUT_DIM;
         constexpr auto BATCH_SIZE = D_OUTPUT_SPEC::ROWS;
         using T = typename LAYER_SPEC::T;
@@ -159,15 +159,15 @@
                     increment(layer.weights.gradient, output_i, input_i, d_pre_activation * get(input, batch_i, input_i));
                 }
             }
         }
     }
 
     template<typename DEVICE, typename LAYER_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC>
-    void backward(DEVICE& device, nn::layers::dense::LayerBackwardGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
+    void backward(DEVICE& device, nn::layers::dense::LayerGradient<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input) {
         // todo: create sparate function that does not set d_input (to save cost on backward pass for the first layer)
         // todo: think about storing gradient in column major order to avoid iterating over the minor dimension
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, D_INPUT_SPEC, D_OUTPUT_SPEC>);
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, D_OUTPUT_SPEC>);
         constexpr auto INPUT_DIM = LAYER_SPEC::INPUT_DIM;
         constexpr auto OUTPUT_DIM = LAYER_SPEC::OUTPUT_DIM;
         constexpr auto BATCH_SIZE = D_OUTPUT_SPEC::ROWS;
@@ -187,118 +187,118 @@
                 }
             }
         }
     }
 
 #endif
     template<typename DEVICE, typename SPEC>
-    void zero_gradient(DEVICE& device, nn::layers::dense::LayerBackwardGradient<SPEC>& layer) {
+    void zero_gradient(DEVICE& device, nn::layers::dense::LayerGradient<SPEC>& layer) {
         zero_gradient(device, layer.weights);
         zero_gradient(device, layer.biases);
     }
     template<typename DEVICE, typename SPEC, typename OPTIMIZER>
-    void update(DEVICE& device, nn::layers::dense::LayerBackwardGradient<SPEC>& layer, OPTIMIZER& optimizer){
+    void update(DEVICE& device, nn::layers::dense::LayerGradient<SPEC>& layer, OPTIMIZER& optimizer){
         update(device, layer.weights, optimizer);
         update(device, layer.biases, optimizer);
     }
 
     template<typename DEVICE, typename SPEC, typename OPTIMIZER>
-    void _reset_optimizer_state(DEVICE& device, nn::layers::dense::LayerBackwardGradient<SPEC>& layer, OPTIMIZER& optimizer) {
+    void _reset_optimizer_state(DEVICE& device, nn::layers::dense::LayerGradient<SPEC>& layer, OPTIMIZER& optimizer) {
         _reset_optimizer_state(device, layer.weights, optimizer);
         _reset_optimizer_state(device, layer.biases, optimizer);
     }
 
     template<typename SOURCE_DEVICE, typename TARGET_DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
-    void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, const  nn::layers::dense::Layer<SOURCE_SPEC>& source, nn::layers::dense::Layer<TARGET_SPEC>& target){
+    void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, const  nn::layers::dense::LayerForward<SOURCE_SPEC>& source, nn::layers::dense::LayerForward<TARGET_SPEC>& target){
         static_assert(nn::layers::dense::check_spec_memory<SOURCE_SPEC, TARGET_SPEC>);
         copy(source_device, target_device, source.weights, target.weights);
         copy(source_device, target_device, source.biases, target.biases);
     }
     template<typename SOURCE_DEVICE, typename TARGET_DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
     void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, const nn::layers::dense::LayerBackward<SOURCE_SPEC>& source, nn::layers::dense::LayerBackward<TARGET_SPEC>& target){
         static_assert(nn::layers::dense::check_spec_memory<SOURCE_SPEC, TARGET_SPEC>);
-        copy(source_device, target_device, (nn::layers::dense::Layer<SOURCE_SPEC>&) source, (nn::layers::dense::Layer<TARGET_SPEC>&) target);
+        copy(source_device, target_device, (nn::layers::dense::LayerForward<SOURCE_SPEC>&) source, (nn::layers::dense::LayerForward<TARGET_SPEC>&) target);
         copy(source_device, target_device, source.pre_activations, target.pre_activations);
     }
     template<typename SOURCE_DEVICE, typename TARGET_DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
-    void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, const nn::layers::dense::LayerBackwardGradient<SOURCE_SPEC>& source, nn::layers::dense::LayerBackwardGradient<TARGET_SPEC>& target){
+    void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, const nn::layers::dense::LayerGradient<SOURCE_SPEC>& source, nn::layers::dense::LayerGradient<TARGET_SPEC>& target){
         static_assert(nn::layers::dense::check_spec_memory<SOURCE_SPEC, TARGET_SPEC>);
         copy(source_device, target_device, (nn::layers::dense::LayerBackward<SOURCE_SPEC>&)source, (nn::layers::dense::LayerBackward<TARGET_SPEC>&)target);
         copy(source_device, target_device, source.output, target.output);
 
     }
     template <typename DEVICE, typename SPEC_1, typename SPEC_2>
-    typename SPEC_1::T abs_diff(DEVICE& device, const rl_tools::nn::layers::dense::Layer<SPEC_1>* l1, const rl_tools::nn::layers::dense::Layer<SPEC_2>* l2) {
+    typename SPEC_1::T abs_diff(DEVICE& device, const rl_tools::nn::layers::dense::LayerForward<SPEC_1>* l1, const rl_tools::nn::layers::dense::LayerForward<SPEC_2>* l2) {
         static_assert(nn::layers::dense::check_spec_memory<SPEC_1, SPEC_2>);
         using T = typename SPEC_1::T;
         T acc = 0;
         acc += abs_diff(device, l1->weights, l2->weights);
         acc += abs_diff(device, l1->biases, l2->biases);
         return acc;
     }
     template <typename DEVICE, typename SPEC_1, typename SPEC_2>
-    typename SPEC_1::T abs_diff(DEVICE& device, const rl_tools::nn::layers::dense::Layer<SPEC_1>& l1, const rl_tools::nn::layers::dense::Layer<SPEC_2>& l2) {
+    typename SPEC_1::T abs_diff(DEVICE& device, const rl_tools::nn::layers::dense::LayerForward<SPEC_1>& l1, const rl_tools::nn::layers::dense::LayerForward<SPEC_2>& l2) {
         static_assert(nn::layers::dense::check_spec_memory<SPEC_1, SPEC_2>);
         return abs_diff(device, &l1, &l2);
     }
     template <typename DEVICE, typename SPEC_1, typename SPEC_2>
     typename SPEC_1::T abs_diff(DEVICE& device, const rl_tools::nn::layers::dense::LayerBackward<SPEC_1>* l1, const rl_tools::nn::layers::dense::LayerBackward<SPEC_2>* l2) {
         static_assert(nn::layers::dense::check_spec_memory<SPEC_1, SPEC_2>);
         using T = typename SPEC_1::T;
-        T acc = abs_diff(device, (rl_tools::nn::layers::dense::Layer<SPEC_1>*) l1, (rl_tools::nn::layers::dense::Layer<SPEC_2>*) l2);
+        T acc = abs_diff(device, (rl_tools::nn::layers::dense::LayerForward<SPEC_1>*) l1, (rl_tools::nn::layers::dense::LayerForward<SPEC_2>*) l2);
         acc += abs_diff(device, l1->pre_activations, l2->pre_activations);
         return acc;
     }
     template <typename DEVICE, typename SPEC_1, typename SPEC_2>
     typename SPEC_1::T abs_diff(DEVICE& device, const rl_tools::nn::layers::dense::LayerBackward<SPEC_1>& l1, const rl_tools::nn::layers::dense::LayerBackward<SPEC_2>& l2) {
         static_assert(nn::layers::dense::check_spec_memory<SPEC_1, SPEC_2>);
         return abs_diff(device, &l1, &l2);
     }
     template <typename DEVICE, typename SPEC_1, typename SPEC_2>
-    typename SPEC_1::T abs_diff(DEVICE& device, const rl_tools::nn::layers::dense::LayerBackwardGradient<SPEC_1>* l1, const rl_tools::nn::layers::dense::LayerBackwardGradient<SPEC_2>* l2) {
+    typename SPEC_1::T abs_diff(DEVICE& device, const rl_tools::nn::layers::dense::LayerGradient<SPEC_1>* l1, const rl_tools::nn::layers::dense::LayerGradient<SPEC_2>* l2) {
         static_assert(nn::layers::dense::check_spec_memory<SPEC_1, SPEC_2>);
         using T = typename SPEC_1::T;
         T acc = abs_diff(device, (rl_tools::nn::layers::dense::LayerBackward<SPEC_1>*) l1, (rl_tools::nn::layers::dense::LayerBackward<SPEC_2>*) l2);
         acc += abs_diff(device, l1->output, l2->output);
         return acc;
     }
     template <typename DEVICE, typename SPEC_1, typename SPEC_2>
-    typename SPEC_1::T abs_diff(DEVICE& device, const rl_tools::nn::layers::dense::LayerBackwardGradient<SPEC_1>& l1, const rl_tools::nn::layers::dense::LayerBackwardGradient<SPEC_2>& l2) {
+    typename SPEC_1::T abs_diff(DEVICE& device, const rl_tools::nn::layers::dense::LayerGradient<SPEC_1>& l1, const rl_tools::nn::layers::dense::LayerGradient<SPEC_2>& l2) {
         static_assert(nn::layers::dense::check_spec_memory<SPEC_1, SPEC_2>);
         return abs_diff(device, &l1, &l2);
     }
     template <typename DEVICE, typename SPEC>
     void reset_forward_state(DEVICE& device, rl_tools::nn::layers::dense::LayerBackward<SPEC>* l) {
         set_all(device, l->pre_activations, 0);
     }
     template <typename DEVICE, typename SPEC>
     void reset_forward_state(DEVICE& device, rl_tools::nn::layers::dense::LayerBackward<SPEC>& l) {
-        reset_forward_state(device, (rl_tools::nn::layers::dense::Layer<SPEC>*) l);
+        reset_forward_state(device, (rl_tools::nn::layers::dense::LayerForward<SPEC>*) l);
     }
     template <typename DEVICE, typename SPEC>
-    void reset_forward_state(DEVICE& device, rl_tools::nn::layers::dense::LayerBackwardGradient<SPEC>* l) {
+    void reset_forward_state(DEVICE& device, rl_tools::nn::layers::dense::LayerGradient<SPEC>* l) {
         reset_forward_state(device, (rl_tools::nn::layers::dense::LayerBackward<SPEC>*) l);
         set_all(device, l->output, 0);
     }
     template <typename DEVICE, typename SPEC>
-    void reset_forward_state(DEVICE& device, rl_tools::nn::layers::dense::LayerBackwardGradient<SPEC>& l) {
+    void reset_forward_state(DEVICE& device, rl_tools::nn::layers::dense::LayerGradient<SPEC>& l) {
         reset_forward_state(device, &l);
     }
     template <typename DEVICE, typename SPEC>
-    bool is_nan(DEVICE& device, const rl_tools::nn::layers::dense::Layer<SPEC>& l) {
+    bool is_nan(DEVICE& device, const rl_tools::nn::layers::dense::LayerForward<SPEC>& l) {
         return is_nan(device, l.weights) || is_nan(device, l.biases);
     }
     template <typename DEVICE, typename SPEC>
     bool is_nan(DEVICE& device, const rl_tools::nn::layers::dense::LayerBackward<SPEC>& l) {
         return
-                is_nan(device, (rl_tools::nn::layers::dense::Layer<SPEC>&) l) ||
+                is_nan(device, (rl_tools::nn::layers::dense::LayerForward<SPEC>&) l) ||
                 is_nan(device, l.pre_activations);
     }
     template <typename DEVICE, typename SPEC>
-    bool is_nan(DEVICE& device, const rl_tools::nn::layers::dense::LayerBackwardGradient<SPEC>& l) {
+    bool is_nan(DEVICE& device, const rl_tools::nn::layers::dense::LayerGradient<SPEC>& l) {
         return
             is_nan(device, (rl_tools::nn::layers::dense::LayerBackward<SPEC>&) l) ||
             is_nan(device, l.output);
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h`

 * *Files 21% similar despite different names*

```diff
@@ -5,38 +5,44 @@
 #include "../../../containers/persist.h"
 #include "layer.h"
 #include "../../../utils/persist.h"
 #include <iostream>
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools {
     template<typename DEVICE, typename SPEC>
-    void save(DEVICE& device, nn::layers::dense::Layer<SPEC>& layer, HighFive::Group group) {
+    void save(DEVICE& device, nn::layers::dense::LayerForward<SPEC>& layer, HighFive::Group group) {
         // todo: forward implementation to Parameter struct
         save(device, layer.weights, group.createGroup("weights"));
         save(device, layer.biases, group.createGroup("biases"));
     }
     template<typename DEVICE, typename SPEC>
     void save(DEVICE& device, nn::layers::dense::LayerBackward<SPEC>& layer, HighFive::Group group) {
-        save(device, (nn::layers::dense::Layer<SPEC>&)layer, group);
+        save(device, (nn::layers::dense::LayerForward<SPEC>&)layer, group);
         save(device, layer.pre_activations, group, "pre_activations");
     }
     template<typename DEVICE, typename SPEC>
-    void save(DEVICE& device, nn::layers::dense::LayerBackwardGradient<SPEC>& layer, HighFive::Group group) {
+    void save(DEVICE& device, nn::layers::dense::LayerGradient<SPEC>& layer, HighFive::Group group) {
         save(device, (nn::layers::dense::LayerBackward<SPEC>&)layer, group);
         save(device, layer.output, group, "output");
     }
     template<typename DEVICE, typename SPEC>
-    void load(DEVICE& device, nn::layers::dense::Layer<SPEC>& layer, HighFive::Group group) {
+    void load(DEVICE& device, nn::layers::dense::LayerForward<SPEC>& layer, HighFive::Group group) {
         load(device, layer.weights, group.getGroup("weights"));
         load(device, layer.biases, group.getGroup("biases"));
     }
     template<typename DEVICE, typename SPEC>
     void load(DEVICE& device, nn::layers::dense::LayerBackward<SPEC>& layer, HighFive::Group group) {
-        load(device, (nn::layers::dense::Layer<SPEC>&)layer, group);
+        load(device, (nn::layers::dense::LayerForward<SPEC>&)layer, group);
+        if(group.exist("pre_activations")){
+            load(device, layer.pre_activations, group, "pre_activations");
+        }
     }
     template<typename DEVICE, typename SPEC>
-    void load(DEVICE& device, nn::layers::dense::LayerBackwardGradient<SPEC>& layer, HighFive::Group group) {
+    void load(DEVICE& device, nn::layers::dense::LayerGradient<SPEC>& layer, HighFive::Group group) {
         load(device, (nn::layers::dense::LayerBackward<SPEC>&)layer, group);
+        if(group.exist("output")){
+            load(device, layer.output, group, "output");
+        }
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,98 @@
-#include "../../../version.h"
-#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_LAYERS_DENSE_PERSIST_CODE_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
+#include "../../version.h"
+#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_PARAMETERS_PERSIST_CODE_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
-#define RL_TOOLS_NN_LAYERS_DENSE_PERSIST_CODE_H
-#include "layer.h"
-#include "../../../containers/persist_code.h"
+#define RL_TOOLS_NN_PARAMETERS_PERSIST_CODE_H
+#include "../../containers/persist_code.h"
+#include "parameters.h"
 #include <sstream>
-#include "../../../persist/code.h"
-#include "../../../containers/persist_code.h"
-
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools {
-    namespace nn::layers::dense::persist{
-        template<nn::activation_functions::ActivationFunction ACTIVATION_FUNCTION>
-        auto get_activation_function_string(){
-            static_assert(ACTIVATION_FUNCTION == nn::activation_functions::ActivationFunction::IDENTITY ||
-                          ACTIVATION_FUNCTION == nn::activation_functions::ActivationFunction::RELU ||
-                          ACTIVATION_FUNCTION == nn::activation_functions::ActivationFunction::GELU ||
-                          ACTIVATION_FUNCTION == nn::activation_functions::ActivationFunction::TANH ||
-                          ACTIVATION_FUNCTION == nn::activation_functions::ActivationFunction::FAST_TANH ||
-                          ACTIVATION_FUNCTION == nn::activation_functions::ActivationFunction::SIGMOID);
-
-            if constexpr (ACTIVATION_FUNCTION == nn::activation_functions::ActivationFunction::IDENTITY){
-                return "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::activation_functions::ActivationFunction::IDENTITY";
-            } else if constexpr (ACTIVATION_FUNCTION == nn::activation_functions::ActivationFunction::RELU){
-                return "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::activation_functions::ActivationFunction::RELU";
-            } else if constexpr (ACTIVATION_FUNCTION == nn::activation_functions::ActivationFunction::TANH){
-                return "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::activation_functions::ActivationFunction::TANH";
-            } else if constexpr (ACTIVATION_FUNCTION == nn::activation_functions::ActivationFunction::FAST_TANH){
-                return "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::activation_functions::ActivationFunction::FAST_TANH";
-            } else if constexpr (ACTIVATION_FUNCTION == nn::activation_functions::ActivationFunction::SIGMOID){
-                return "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::activation_functions::ActivationFunction::SIGMOID";
-            }
-        }
+
+    std::string get_type_string(nn::parameters::Plain p){
+        return "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::parameters::Plain";
+    }
+    std::string get_type_string(nn::parameters::Gradient p){
+        return "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::parameters::Gradient";
+    }
+
+    template <typename DEVICE>
+    std::string get_type_string_tag(const DEVICE&, const nn::parameters::categories::Weights){
+        return "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::parameters::categories::Weights";
+    }
+
+    template <typename DEVICE>
+    std::string get_type_string_tag(const DEVICE&, const nn::parameters::categories::Biases){
+        return "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::parameters::categories::Biases";
     }
 
-    template<typename DEVICE, typename SPEC>
-    persist::Code save_split(DEVICE& device, nn::layers::dense::Layer <SPEC> &layer, std::string name, bool const_declaration=false, typename DEVICE::index_t indent=0){
+    template <typename DEVICE>
+    std::string get_type_string_tag(const DEVICE&, const nn::parameters::groups::Normal){
+        return "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::parameters::groups::Normal";
+    }
+
+    template <typename DEVICE>
+    std::string get_type_string_tag(const DEVICE&, const nn::parameters::groups::Input){
+        return "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::parameters::groups::Input";
+    }
+
+    template <typename DEVICE>
+    std::string get_type_string_tag(const DEVICE&, const nn::parameters::groups::Output){
+        return "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::parameters::groups::Output";
+    }
+
+    template<typename DEVICE, typename CONTAINER>
+    persist::Code save_split(DEVICE& device, nn::parameters::Plain::instance<CONTAINER>& parameter, std::string name, bool const_declaration=false, typename DEVICE::index_t indent=0, bool output_memory_only=false){
         using TI = typename DEVICE::index_t;
         std::stringstream indent_ss;
         for(TI i=0; i < indent; i++){
             indent_ss << "    ";
         }
         std::string ind = indent_ss.str();
-        using TI = typename DEVICE::index_t;
-        std::stringstream ss_header;
-        ss_header << "#include <rl_tools/nn/layers/dense/layer.h>\n";
-        std::stringstream ss;
+        std::stringstream ss, ss_header;
         ss << ind << "namespace " << name << " {\n";
-        auto weights = save_split(device, layer.weights, "weights", const_declaration, indent+1);
-        ss_header << weights.header;
-        ss << weights.body;
-        auto biases = save_split(device, layer.biases, "biases", const_declaration, indent+1);
-        ss_header << biases.header;
-        ss << biases.body;
-        ss << ind << "    using SPEC = " << "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::layers::dense::Specification<"
-            << containers::persist::get_type_string<typename SPEC::T>() << ", "
-            << containers::persist::get_type_string<typename SPEC::TI>() << ", "
-            << SPEC::INPUT_DIM << ", "
-            << SPEC::OUTPUT_DIM << ", "
-            << nn::layers::dense::persist::get_activation_function_string<SPEC::ACTIVATION_FUNCTION>() << ", "
-            << get_type_string(typename SPEC::PARAMETER_TYPE{}) << ", "
-            << 1 << ", "
-            << get_type_string_tag(device, typename SPEC::PARAMETER_GROUP{}) << ", "
-            << "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::MatrixDynamicTag" << ", "
-            << "true, "
-            << "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::matrix::layouts::RowMajorAlignment<" << containers::persist::get_type_string<TI>() << ", 1>"
-            << ">; \n";
-        ss << ind << "    " << "using TYPE = RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::layers::dense::Layer<SPEC>;";
-        ss << ind << "    " << (const_declaration ? "const " : "") << "TYPE layer = {weights::parameters, biases::parameters};\n";
+        auto container = save_split(device, parameter.parameters, "parameters_memory", const_declaration, indent+1);
+        ss_header << container.header;
+        ss_header << "#include <rl_tools/nn/parameters/parameters.h>\n";
+        ss << container.body;
+        if(!output_memory_only){
+            ss << ind << "    " << "using PARAMETER_SPEC = " << "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::parameters::Plain::spec<parameters_memory::CONTAINER_TYPE, "
+            << get_type_string_tag(device, typename CONTAINER::GROUP_TAG{})
+            << ", "
+            << get_type_string_tag(device, typename CONTAINER::CATEGORY_TAG{})
+            << ">;\n";
+            ss << ind << "    " << (const_declaration ? "const " : "") << "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::parameters::Plain::instance<PARAMETER_SPEC> parameters = {parameters_memory::container};\n";
+        }
         ss << ind << "}\n";
-
         return {ss_header.str(), ss.str()};
     }
-    template<typename DEVICE, typename SPEC>
-    std::string save_code(DEVICE& device, nn::layers::dense::Layer <SPEC> &layer, std::string name, bool const_declaration=false, typename DEVICE::index_t indent=0){
-        auto code = save_split(device, layer, name, const_declaration, indent);
-        return code.header + code.body;
+
+    template<typename DEVICE, typename CONTAINER>
+    persist::Code save_split(DEVICE& device, nn::parameters::Gradient::instance<CONTAINER>& parameter, std::string name, bool const_declaration=false, typename DEVICE::index_t indent=0, bool output_memory_only=false){
+        using TI = typename DEVICE::index_t;
+        std::stringstream indent_ss;
+        for(TI i=0; i < indent; i++){
+            indent_ss << "    ";
+        }
+        std::string ind = indent_ss.str();
+        std::stringstream ss, ss_header;
+        ss_header << "#include <rl_tools/utils/generic/typing.h>\n";
+        auto plain = save_split(device, (nn::parameters::Plain::instance<CONTAINER>&) parameter, name, const_declaration, indent, true);
+        ss_header << plain.header;
+        ss << plain.body;
+        ss << ind << "namespace " << name << " {\n";
+        auto gradient = save_split(device, parameter.gradient, "gradient_memory", const_declaration, indent+1);
+        ss_header << gradient.header;
+        ss << gradient.body;
+        if(!output_memory_only){
+            ss << ind << "    " << "static_assert(RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::utils::typing::is_same_v<parameters_memory::CONTAINER_TYPE, gradient_memory::CONTAINER_TYPE>);\n";
+            ss << ind << "    " << "using PARAMETER_SPEC = " << "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::parameters::Gradient::spec<parameters_memory::CONTAINER_TYPE, " << get_type_string_tag(device, typename CONTAINER::CATEGORY_TAG{}) << ">;\n";
+            ss << ind << "    " << (const_declaration ? "const " : "") << "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::parameters::Gradient::instance<parameters_memory::CONTAINER_TYPE> parameters = {parameters_memory::container, gradient_memory::container};\n";
+        }
+        ss << ind << "}\n";
+        return {ss_header.str(), ss.str()};
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
-#endif
+
+#endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 template<typename DEV_SPEC, typename SPEC, typename devices::CUDA<DEV_SPEC>::index_t BATCH_SIZE, typename devices::CUDA<DEV_SPEC>::index_t BLOCK_SIZE>
 __global__ void
-evaluate_batch_kernel(devices::CUDA<DEV_SPEC>& device, const nn::layers::dense::Layer<SPEC> layer, const typename SPEC::T* input, typename SPEC::T* output) {
+evaluate_batch_kernel(devices::CUDA<DEV_SPEC>& device, const nn::layers::dense::LayerForward<SPEC> layer, const typename SPEC::T* input, typename SPEC::T* output) {
     using T = typename SPEC::T;
     using TI = typename devices::CUDA<DEV_SPEC>::index_t;
     constexpr TI INPUT_DIM = SPEC::INPUT_DIM;
     constexpr TI OUTPUT_DIM = SPEC::OUTPUT_DIM;
 
     __shared__ T shared_input[BLOCK_SIZE * BLOCK_SIZE];
     __shared__ T shared_weights[BLOCK_SIZE * BLOCK_SIZE];
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 //#include "../../../../utils/generic/memcpy.h"
 #include "../../../../devices/arm.h"
 #include "arm_math.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    void evaluate(devices::arm::DSP<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+    void evaluate(devices::arm::DSP<DEV_SPEC>& device, const nn::layers::dense::LayerForward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         static_assert(INPUT_SPEC::ROW_PITCH == INPUT_SPEC::COLS);
         static_assert(INPUT_SPEC::COL_PITCH == 1);
         static_assert(OUTPUT_SPEC::ROW_PITCH == OUTPUT_SPEC::COLS);
         static_assert(OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.parameters)::ROW_PITCH == INPUT_SPEC::COLS);
         static_assert(decltype(layer.weights.parameters)::COL_PITCH == 1);
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #include "../../../../nn/layers/dense/operations_generic.h"
 //#include "../../../../utils/generic/memcpy.h"
 #include "../../../../devices/arm.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    void evaluate(devices::arm::OPT<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+    void evaluate(devices::arm::OPT<DEV_SPEC>& device, const nn::layers::dense::LayerForward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         // For performance reasons: restricted to dense row-major matrices (row-pitch is allowed)
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         static_assert(INPUT_SPEC::COL_PITCH == 1);
         static_assert(OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.parameters)::COL_PITCH == 1);
         static_assert(decltype(layer.biases.parameters)::COL_PITCH == 1);
 //        static_assert(utils::typing::is_same_v<typename LAYER_SPEC::T, float>);
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #include "../../../../nn/layers/dense/layer.h"
 
 #include "esp_dsp.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    void evaluate(devices::esp32::DSP<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+    void evaluate(devices::esp32::DSP<DEV_SPEC>& device, const nn::layers::dense::LayerForward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         // For performance reasons: restricted to dense row-major matrices (row-pitch is allowed)
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         static_assert(INPUT_SPEC::ROWS == 1); // only supporting batch size of 1 for now
         static_assert(INPUT_SPEC::COL_PITCH == 1);
         static_assert(OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.parameters)::COL_PITCH == 1);
         static_assert(decltype(layer.biases.parameters)::COL_PITCH == 1);
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 #include "../../../../devices/esp32.h"
 #include "../../../../nn/layers/dense/layer.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    void evaluate(devices::esp32::OPT<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+    void evaluate(devices::esp32::OPT<DEV_SPEC>& device, const nn::layers::dense::LayerForward<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         // For performance reasons: restricted to dense row-major matrices (row-pitch is allowed)
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         static_assert(INPUT_SPEC::COL_PITCH == 1);
         static_assert(OUTPUT_SPEC::COL_PITCH == 1);
         static_assert(decltype(layer.weights.parameters)::COL_PITCH == 1);
         static_assert(decltype(layer.biases.parameters)::COL_PITCH == 1);
 //        static_assert(utils::typing::is_same_v<typename LAYER_SPEC::T, float>);
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/adam.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/adam.h`

 * *Files 4% similar despite different names*

```diff
@@ -11,33 +11,36 @@
         template<typename T_T>
         struct Parameters{
             using T = T_T;
             T alpha;
             T beta_1;
             T beta_2;
             T epsilon;
+            T epsilon_sqrt;
             T weight_decay;
             T weight_decay_input;
             T weight_decay_output;
             T bias_lr_factor;
         };
         template <typename T>
         struct DEFAULT_PARAMETERS_TENSORFLOW{
             static constexpr T ALPHA = 0.001;
             static constexpr T BETA_1 = 0.9;
             static constexpr T BETA_2 = 0.999;
             static constexpr T EPSILON = 1e-7;
+            static constexpr T EPSILON_SQRT = 1e-7;
             static constexpr T WEIGHT_DECAY = 0;
             static constexpr T WEIGHT_DECAY_INPUT = 0;
             static constexpr T WEIGHT_DECAY_OUTPUT = 0;
             static constexpr T BIAS_LR_FACTOR = 1;
         };
         template <typename T>
         struct DEFAULT_PARAMETERS_PYTORCH: DEFAULT_PARAMETERS_TENSORFLOW<T>{
             static constexpr T EPSILON = 1e-8;
+            static constexpr T EPSILON_SQRT = 1e-8;
         };
         template <typename T_T, typename T_TI, typename T_DEFAULT_PARAMETERS=DEFAULT_PARAMETERS_TENSORFLOW<T_T>, bool T_ENABLE_WEIGHT_DECAY = false, bool T_ENABLE_BIAS_LR_FACTOR = false>
         struct Specification{
             using T = T_T;
             using TI = T_TI;
             using DEFAULT_PARAMETERS = T_DEFAULT_PARAMETERS;
             static constexpr bool ENABLE_WEIGHT_DECAY = T_ENABLE_WEIGHT_DECAY;
@@ -51,14 +54,15 @@
         using TI = typename SPEC::TI;
         using DEFAULT_PARAMETERS = typename SPEC::DEFAULT_PARAMETERS;
         adam::Parameters<T> parameters = {
             DEFAULT_PARAMETERS::ALPHA,
             DEFAULT_PARAMETERS::BETA_1,
             DEFAULT_PARAMETERS::BETA_2,
             DEFAULT_PARAMETERS::EPSILON,
+            DEFAULT_PARAMETERS::EPSILON_SQRT,
             DEFAULT_PARAMETERS::WEIGHT_DECAY,
             DEFAULT_PARAMETERS::WEIGHT_DECAY_INPUT,
             DEFAULT_PARAMETERS::WEIGHT_DECAY_OUTPUT,
             DEFAULT_PARAMETERS::BIAS_LR_FACTOR
         };
         T first_order_moment_bias_correction;
         T second_order_moment_bias_correction;
@@ -66,15 +70,15 @@
     };
 
 
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools::nn::parameters {
-    struct Adam: Gradient{
+    struct Adam{
         template <typename T_CONTAINER, typename T_GROUP_TAG, typename T_CATEGORY_TAG>
         struct spec {
             using CONTAINER = T_CONTAINER;
             using GROUP_TAG = T_GROUP_TAG;
             using CATEGORY_TAG = T_CATEGORY_TAG;
         };
         template <typename T_SPEC>
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "adam.h"
+#include "operations_generic.h"
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools {
     namespace nn::optimizers::adam::cuda {
         template<typename DEV_SPEC, typename PARAMETER_SPEC, typename SPEC>
         __global__
         void update_kernel(devices::CUDA<DEV_SPEC>& device, nn::parameters::Adam::instance<PARAMETER_SPEC> parameter, nn::optimizers::Adam<SPEC> optimizer) {
             // fully fused adam update
@@ -14,15 +15,17 @@
             TI row_i = blockIdx.y * blockDim.y + threadIdx.y;
             if(col_i < PARAMETER_SPEC::CONTAINER::COLS && row_i < PARAMETER_SPEC::CONTAINER::ROWS){
                 T d_weight = get(parameter.gradient, row_i, col_i);
                 T d_weight_first_order_moment = optimizer.parameters.beta_1 * get(parameter.gradient_first_order_moment, row_i, col_i) + (1 - optimizer.parameters.beta_1) * d_weight;
                 set(parameter.gradient_first_order_moment, row_i, col_i, d_weight_first_order_moment);
                 T d_weight_second_order_moment = optimizer.parameters.beta_2 * get(parameter.gradient_second_order_moment, row_i, col_i) + (1 - optimizer.parameters.beta_2) * d_weight * d_weight;
                 set(parameter.gradient_second_order_moment, row_i, col_i, d_weight_second_order_moment);
-                T parameter_update = optimizer.parameters.alpha * optimizer.first_order_moment_bias_correction * d_weight_first_order_moment / (math::sqrt(typename DEVICE::SPEC::MATH_DEVICE_ACCURATE(), d_weight_second_order_moment * optimizer.second_order_moment_bias_correction) + optimizer.parameters.epsilon);
+                T pre_sqrt_term = d_weight_second_order_moment * optimizer.second_order_moment_bias_correction;
+                pre_sqrt_term = math::max(device.math, pre_sqrt_term, (T)optimizer.parameters.epsilon_sqrt);
+                T parameter_update = optimizer.parameters.alpha * optimizer.first_order_moment_bias_correction * d_weight_first_order_moment / (math::sqrt(typename DEVICE::SPEC::MATH_DEVICE_ACCURATE(), pre_sqrt_term) + optimizer.parameters.epsilon);
                 if constexpr(utils::typing::is_same_v<typename PARAMETER_SPEC::CATEGORY_TAG, nn::parameters::categories::Biases> && SPEC::ENABLE_BIAS_LR_FACTOR){
                     parameter_update *= optimizer.parameters.bias_lr_factor;
                 }
                 if constexpr(utils::typing::is_same_v<typename PARAMETER_SPEC::CATEGORY_TAG, nn::parameters::categories::Weights>){
                     if constexpr(utils::typing::is_same_v<typename PARAMETER_SPEC::GROUP_TAG, nn::parameters::groups::Normal> && SPEC::ENABLE_WEIGHT_DECAY){
                         parameter_update += get(parameter.parameters, row_i, col_i) * optimizer.parameters.weight_decay / 2;
                     }
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,21 @@
         utils::polyak::update(device, parameter.gradient, parameter.gradient_first_order_moment, optimizer.parameters.beta_1);
         utils::polyak::update_squared(device, parameter.gradient, parameter.gradient_second_order_moment, optimizer.parameters.beta_2);
         gradient_descent(device, parameter, optimizer);
     }
 
     template<typename DEVICE, typename SPEC, typename PARAMETER_SPEC>
     void gradient_descent(DEVICE& device, nn::parameters::Adam::instance<PARAMETER_SPEC>& parameter, nn::optimizers::Adam<SPEC>& optimizer){
-        for(typename DEVICE::index_t row_i = 0; row_i < PARAMETER_SPEC::CONTAINER::ROWS; row_i++) {
-            for(typename DEVICE::index_t col_i = 0; col_i < PARAMETER_SPEC::CONTAINER::COLS; col_i++) {
-                typename PARAMETER_SPEC::CONTAINER::T parameter_update = optimizer.parameters.alpha * optimizer.first_order_moment_bias_correction * get(parameter.gradient_first_order_moment, row_i, col_i) / (math::sqrt(device.math, get(parameter.gradient_second_order_moment, row_i, col_i) * optimizer.second_order_moment_bias_correction) + optimizer.parameters.epsilon);
+        using TI = typename DEVICE::index_t;
+        using T = typename PARAMETER_SPEC::CONTAINER::T;
+        for(TI row_i = 0; row_i < PARAMETER_SPEC::CONTAINER::ROWS; row_i++) {
+            for(TI col_i = 0; col_i < PARAMETER_SPEC::CONTAINER::COLS; col_i++) {
+                T pre_sqrt_term = get(parameter.gradient_second_order_moment, row_i, col_i) * optimizer.second_order_moment_bias_correction;
+                pre_sqrt_term = math::max(device.math, pre_sqrt_term, (T)optimizer.parameters.epsilon_sqrt);
+                T parameter_update = optimizer.parameters.alpha * optimizer.first_order_moment_bias_correction * get(parameter.gradient_first_order_moment, row_i, col_i) / (math::sqrt(device.math, pre_sqrt_term) + optimizer.parameters.epsilon);
                 if constexpr(utils::typing::is_same_v<typename PARAMETER_SPEC::CATEGORY_TAG, nn::parameters::categories::Biases> && SPEC::ENABLE_BIAS_LR_FACTOR){
                     parameter_update *= optimizer.parameters.bias_lr_factor;
                 }
                 if constexpr(utils::typing::is_same_v<typename PARAMETER_SPEC::CATEGORY_TAG, nn::parameters::categories::Weights>){
                     if constexpr(utils::typing::is_same_v<typename PARAMETER_SPEC::GROUP_TAG, nn::parameters::groups::Normal> && SPEC::ENABLE_WEIGHT_DECAY){
                         parameter_update += get(parameter.parameters, row_i, col_i) * optimizer.parameters.weight_decay / 2;
                     }
@@ -74,14 +78,16 @@
     }
 //    template<typename DEVICE, typename SPEC, typename OPTIMIZER>
 //    void _reset_optimizer_state(DEVICE& device, nn::parameters::Adam::instance<SPEC>& p1, OPTIMIZER& optimizer) {
 //        set_all(device, p1.gradient_first_order_moment, 0);
 //        set_all(device, p1.gradient_second_order_moment, 0);
 //    }
     template<typename DEVICE, typename SPEC, typename MODEL>
+    void _reset_optimizer_state(DEVICE& device, nn::optimizers::Adam<SPEC>& optimizer, MODEL& model);
+    template<typename DEVICE, typename SPEC, typename MODEL>
     void reset_optimizer_state(DEVICE& device, nn::optimizers::Adam<SPEC>& optimizer, MODEL& model) {
         optimizer.age = 1;
         _reset_optimizer_state(device, model, optimizer);
     }
 
     template<typename DEVICE, typename SPEC, typename MODEL>
     void step(DEVICE& device, nn::optimizers::Adam<SPEC>& optimizer, MODEL& model) {
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             ss << ind << "    " << "static_assert(rl_tools::utils::typing::is_same_v<gradient_memory::CONTAINER_TYPE, gradient_first_order_moment_memory::CONTAINER_TYPE>);\n";
             ss << ind << "    " << "static_assert(rl_tools::utils::typing::is_same_v<gradient_memory::CONTAINER_TYPE, gradient_second_order_moment_memory::CONTAINER_TYPE>);\n";
             ss << ind << "    " << "using PARAMETER_SPEC = " << "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn::parameters::Adam::spec<parameters_memory::CONTAINER_TYPE, "
                << get_type_string_tag(device, typename CONTAINER::GROUP_TAG{})
                << ", "
                << get_type_string_tag(device, typename CONTAINER::CATEGORY_TAG{})
                << ">;\n";
-            ss << ind << "    " << (const_declaration ? "const " : "") << "rl_tools::nn::parameters::Adam::instance<PARAMETER_SPEC> parameters = {parameters_memory::container, gradient_memory::container, gradient_first_order_moment_memory::container, gradient_second_order_moment_memory::container, };\n";
+            ss << ind << "    " << (const_declaration ? "const " : "") << "rl_tools::nn::parameters::Adam::instance<PARAMETER_SPEC> parameters = {{{parameters_memory::container}, gradient_memory::container}, gradient_first_order_moment_memory::container, gradient_second_order_moment_memory::container};\n";
         }
         ss << ind << "}\n";
         return {ss_header.str(), ss.str()};
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         static constexpr T ALPHA = 0.001;
     };
 
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools::nn::parameters{
-    struct SGD: Gradient{
+    struct SGD{
         template <typename T_SPEC>
         struct instance: Gradient::instance<T_SPEC>{};
     };
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,21 @@
         template <typename T_SPEC>
         struct instance{
             using SPEC = T_SPEC;
             using CONTAINER = typename SPEC::CONTAINER;
             CONTAINER parameters;
         };
     };
-    struct Gradient: Plain{
+    struct Gradient{
+        template <typename T_CONTAINER, typename T_GROUP_TAG, typename T_CATEGORY_TAG>
+        struct spec {
+            using CONTAINER = T_CONTAINER;
+            using GROUP_TAG = T_GROUP_TAG;
+            using CATEGORY_TAG = T_CATEGORY_TAG;
+        };
         template <typename T_SPEC>
         struct instance: Plain::instance<T_SPEC>{
             using SPEC = T_SPEC;
             using CONTAINER = typename SPEC::CONTAINER;
             CONTAINER gradient;
         };
     };
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,165 +1,149 @@
-#include "../../version.h"
-#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_MODELS_MLP_NETWORK_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
+#include "../../../../../version.h"
+#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_RL_ALGORITHMS_SAC_LOOP_CORE_CONFIG_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
-#define RL_TOOLS_NN_MODELS_MLP_NETWORK_H
+#define RL_TOOLS_RL_ALGORITHMS_SAC_LOOP_CORE_CONFIG_H
 
-#include "../../nn/nn.h"
-#include "../../nn/parameters/parameters.h"
-#include "../../nn/optimizers/sgd/sgd.h"
-#include "../../nn/optimizers/adam/adam.h"
-#include "../../utils/generic/typing.h"
-#include "../../containers.h"
+#include "../../../../../nn_models/sequential/model.h"
+#include "../../../../../nn_models/mlp/network.h"
+#include "../../../../../nn_models/random_uniform/model.h"
+#include "../../../../../rl/algorithms/sac/sac.h"
+#include "../../../../../nn/optimizers/adam/adam.h"
+#include "state.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
-namespace rl_tools::nn_models::mlp {
-    template <typename T_T, typename T_TI, T_TI T_INPUT_DIM, T_TI T_OUTPUT_DIM, T_TI T_NUM_LAYERS, T_TI T_HIDDEN_DIM, nn::activation_functions::ActivationFunction T_HIDDEN_ACTIVATION_FUNCTION, nn::activation_functions::ActivationFunction T_OUTPUT_ACTIVATION_FUNCTION, T_TI T_BATCH_SIZE=1, typename T_CONTAINER_TYPE_TAG = MatrixDynamicTag, bool T_ENFORCE_FLOATING_POINT_TYPE=true, typename T_MEMORY_LAYOUT = matrix::layouts::RowMajorAlignmentOptimized<T_TI>>
-    struct StructureSpecification{
-        using T = T_T;
-        using TI = T_TI;
-        static constexpr T_TI INPUT_DIM = T_INPUT_DIM;
-        static constexpr T_TI OUTPUT_DIM = T_OUTPUT_DIM;
-        static constexpr T_TI NUM_LAYERS = T_NUM_LAYERS; // The input and output layers count towards the total number of layers
-        static constexpr T_TI HIDDEN_DIM = T_HIDDEN_DIM;
-        static constexpr auto HIDDEN_ACTIVATION_FUNCTION = T_HIDDEN_ACTIVATION_FUNCTION;
-        static constexpr auto OUTPUT_ACTIVATION_FUNCTION = T_OUTPUT_ACTIVATION_FUNCTION;
-        static constexpr T_TI BATCH_SIZE = T_BATCH_SIZE;
-
-        using CONTAINER_TYPE_TAG = T_CONTAINER_TYPE_TAG;
-        static constexpr bool ENFORCE_FLOATING_POINT_TYPE = T_ENFORCE_FLOATING_POINT_TYPE;
-        using MEMORY_LAYOUT = T_MEMORY_LAYOUT;
-    };
-    template<typename SPEC_1, typename SPEC_2>
-    constexpr bool check_spec_memory =
-            utils::typing::is_same_v<typename SPEC_1::T, typename SPEC_2::T>
-            && SPEC_1::INPUT_DIM == SPEC_2::INPUT_DIM
-            && SPEC_1::OUTPUT_DIM == SPEC_2::OUTPUT_DIM
-            && SPEC_1::NUM_LAYERS == SPEC_2::NUM_LAYERS
-            && SPEC_1::HIDDEN_DIM == SPEC_2::HIDDEN_DIM;
-    template<typename SPEC_1, typename SPEC_2>
-    constexpr bool check_spec =
-            check_spec_memory<SPEC_1, SPEC_2>
-            && SPEC_1::HIDDEN_ACTIVATION_FUNCTION == SPEC_2::HIDDEN_ACTIVATION_FUNCTION
-            && SPEC_1::OUTPUT_ACTIVATION_FUNCTION == SPEC_2::OUTPUT_ACTIVATION_FUNCTION;
-
-
-    template <typename T_STRUCTURE_SPEC, typename T_PARAMETER_TYPE>
-    struct Specification{
-        using STRUCTURE_SPEC = T_STRUCTURE_SPEC;
-        using S = STRUCTURE_SPEC;
-        using PARAMETER_TYPE = T_PARAMETER_TYPE;
-        using T = typename S::T;
-        using TI = typename S::TI;
-        static constexpr TI NUM_HIDDEN_LAYERS = STRUCTURE_SPEC::NUM_LAYERS - 2;
-        static constexpr TI INPUT_DIM = S::INPUT_DIM;
-        static constexpr TI HIDDEN_DIM = S::HIDDEN_DIM;
-        static constexpr TI OUTPUT_DIM = S::OUTPUT_DIM;
-        static constexpr TI BATCH_SIZE = S::BATCH_SIZE;
-        using CONTAINER_TYPE_TAG = typename S::CONTAINER_TYPE_TAG;
-        static constexpr bool ENFORCE_FLOATING_POINT_TYPE = S::ENFORCE_FLOATING_POINT_TYPE;
-        using MEMORY_LAYOUT = typename S::MEMORY_LAYOUT;
-
-        using INPUT_LAYER_SPEC  = nn::layers::dense::Specification<T, TI, INPUT_DIM , HIDDEN_DIM, S::HIDDEN_ACTIVATION_FUNCTION, PARAMETER_TYPE, BATCH_SIZE, nn::parameters::groups::Input , CONTAINER_TYPE_TAG, ENFORCE_FLOATING_POINT_TYPE, MEMORY_LAYOUT>;
-        using HIDDEN_LAYER_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, HIDDEN_DIM, S::HIDDEN_ACTIVATION_FUNCTION, PARAMETER_TYPE, BATCH_SIZE, nn::parameters::groups::Normal, CONTAINER_TYPE_TAG, ENFORCE_FLOATING_POINT_TYPE, MEMORY_LAYOUT>;
-        using OUTPUT_LAYER_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, OUTPUT_DIM, S::OUTPUT_ACTIVATION_FUNCTION, PARAMETER_TYPE, BATCH_SIZE, nn::parameters::groups::Output, CONTAINER_TYPE_TAG, ENFORCE_FLOATING_POINT_TYPE, MEMORY_LAYOUT>;
+namespace rl_tools::rl::algorithms::sac::loop::core{
+    // Config State (Init/Step)
+    template<typename T, typename TI, typename ENVIRONMENT>
+    struct DefaultParameters{
+        using SAC_PARAMETERS = rl::algorithms::sac::DefaultParameters<T, TI, ENVIRONMENT::ACTION_DIM>;
+        static constexpr TI N_ENVIRONMENTS = 1;
+        static constexpr TI N_WARMUP_STEPS = 100;
+        static_assert(N_WARMUP_STEPS >= SAC_PARAMETERS::ACTOR_BATCH_SIZE);
+        static constexpr TI STEP_LIMIT = 10000;
+        static constexpr TI REPLAY_BUFFER_CAP = STEP_LIMIT; // Note: when inheriting from this class for overwriting the default STEP_LIMIT you need to set the REPLAY_BUFFER_CAP as well otherwise it will be the default step limit
+        static constexpr TI EPISODE_STEP_LIMIT = 200;
+
+        static constexpr TI ACTOR_HIDDEN_DIM = 64;
+        static constexpr TI ACTOR_NUM_LAYERS = 3;
+        static constexpr auto ACTOR_ACTIVATION_FUNCTION = nn::activation_functions::ActivationFunction::RELU;
+        static constexpr TI CRITIC_HIDDEN_DIM = 64;
+        static constexpr TI CRITIC_NUM_LAYERS = 3;
+        static constexpr auto CRITIC_ACTIVATION_FUNCTION = nn::activation_functions::ActivationFunction::RELU;
+
+        static constexpr bool COLLECT_EPISODE_STATS = true;
+        static constexpr TI EPISODE_STATS_BUFFER_SIZE = 1000;
+
+        static constexpr bool SHARED_BATCH = true;
+
+        using OPTIMIZER_PARAMETERS = nn::optimizers::adam::DEFAULT_PARAMETERS_TENSORFLOW<T>;
+    };
+
+    // The approximator config sets up any types that support the usual rl_tools::forward and rl_tools::backward operations (can be custom as well)
+    // We provide approximators based on the sequential and mlp models. The latter (mlp) allows for a variable number of layers, but is restricted to a uniform hidden layer size while the former allows for arbitrary layers to be combined in a sequential manner. Both support compile-time autodiff
+    template<typename T, typename TI, typename ENVIRONMENT, typename PARAMETERS, typename CONTAINER_TYPE_TAG>
+    struct ConfigApproximatorsSequential{
+        template <typename CAPABILITY>
+        struct ACTOR{
+            static constexpr TI HIDDEN_DIM = PARAMETERS::ACTOR_HIDDEN_DIM;
+            static constexpr TI BATCH_SIZE = PARAMETERS::SAC_PARAMETERS::ACTOR_BATCH_SIZE;
+            static constexpr auto ACTIVATION_FUNCTION = PARAMETERS::ACTOR_ACTIVATION_FUNCTION;
+            using LAYER_1_SPEC = nn::layers::dense::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, BATCH_SIZE, nn::parameters::groups::Input, CONTAINER_TYPE_TAG>;
+            using LAYER_1 = nn::layers::dense::BindSpecification<LAYER_1_SPEC>;
+            using LAYER_2_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, BATCH_SIZE, nn::parameters::groups::Normal, CONTAINER_TYPE_TAG>;
+            using LAYER_2 = nn::layers::dense::BindSpecification<LAYER_2_SPEC>;
+            static constexpr TI ACTOR_OUTPUT_DIM = ENVIRONMENT::ACTION_DIM * 2; // to express mean and log_std for each action
+            using LAYER_3_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, ACTOR_OUTPUT_DIM, nn::activation_functions::ActivationFunction::IDENTITY, BATCH_SIZE, nn::parameters::groups::Output, CONTAINER_TYPE_TAG>; // note the output activation should be identity because we want to sample from a gaussian and then squash afterwards (taking into account the squashing in the distribution)
+            using LAYER_3 = nn::layers::dense::BindSpecification<LAYER_3_SPEC>;
+
+            using IF = nn_models::sequential::Interface<CAPABILITY>;
+            using MODEL = typename IF::template Module<LAYER_1::template Layer, typename IF::template Module<LAYER_2::template Layer, typename IF::template Module<LAYER_3::template Layer>>>;
+        };
+
+        template <typename CAPABILITY>
+        struct CRITIC{
+            static constexpr TI HIDDEN_DIM = PARAMETERS::CRITIC_HIDDEN_DIM;
+            static constexpr TI BATCH_SIZE = PARAMETERS::SAC_PARAMETERS::CRITIC_BATCH_SIZE;
+            static constexpr auto ACTIVATION_FUNCTION = PARAMETERS::CRITIC_ACTIVATION_FUNCTION;
+
+            using LAYER_1_SPEC = nn::layers::dense::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM + ENVIRONMENT::ACTION_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, BATCH_SIZE, nn::parameters::groups::Input, CONTAINER_TYPE_TAG>;
+            using LAYER_1 = nn::layers::dense::BindSpecification<LAYER_1_SPEC>;
+            using LAYER_2_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, BATCH_SIZE, nn::parameters::groups::Normal, CONTAINER_TYPE_TAG>;
+            using LAYER_2 = nn::layers::dense::BindSpecification<LAYER_2_SPEC>;
+            using LAYER_3_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, 1, nn::activation_functions::ActivationFunction::IDENTITY, BATCH_SIZE, nn::parameters::groups::Output, CONTAINER_TYPE_TAG>;
+            using LAYER_3 = nn::layers::dense::BindSpecification<LAYER_3_SPEC>;
+
+            using IF = nn_models::sequential::Interface<CAPABILITY>;
+            using MODEL = typename IF::template Module<LAYER_1::template Layer, typename IF::template Module<LAYER_2::template Layer, typename IF::template Module<LAYER_3::template Layer>>>;
+        };
+
+        using OPTIMIZER_SPEC = nn::optimizers::adam::Specification<T, TI, typename PARAMETERS::OPTIMIZER_PARAMETERS>;
+
+        using OPTIMIZER = nn::optimizers::Adam<OPTIMIZER_SPEC>;
+
+        using ACTOR_TYPE = typename ACTOR<nn::layer_capability::Gradient<nn::parameters::Adam>>::MODEL;
+        using CRITIC_TYPE = typename CRITIC<nn::layer_capability::Gradient<nn::parameters::Adam>>::MODEL;
+        using CRITIC_TARGET_TYPE = typename CRITIC<nn::layer_capability::Forward>::MODEL;
     };
 
-    template <typename T_STRUCTURE_SPEC>
-    struct InferenceSpecification: Specification<T_STRUCTURE_SPEC, nn::parameters::Plain>{
-        using SUPER = Specification<T_STRUCTURE_SPEC, nn::parameters::Plain>;
-        using  INPUT_LAYER = nn::layers::dense::Layer<typename SUPER::INPUT_LAYER_SPEC >;
-        using HIDDEN_LAYER = nn::layers::dense::Layer<typename SUPER::HIDDEN_LAYER_SPEC>;
-        using OUTPUT_LAYER = nn::layers::dense::Layer<typename SUPER::OUTPUT_LAYER_SPEC>;
-    };
+    template<typename T, typename TI, typename ENVIRONMENT, typename PARAMETERS, typename T_CONTAINER_TYPE_TAG>
+    struct ConfigApproximatorsMLP{
+        using CONTAINER_TYPE_TAG = T_CONTAINER_TYPE_TAG;
+        using ACTOR_SPEC = nn_models::mlp::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM, 2*ENVIRONMENT::ACTION_DIM, PARAMETERS::ACTOR_NUM_LAYERS, PARAMETERS::ACTOR_HIDDEN_DIM, PARAMETERS::ACTOR_ACTIVATION_FUNCTION, nn::activation_functions::IDENTITY, PARAMETERS::SAC_PARAMETERS::ACTOR_BATCH_SIZE, CONTAINER_TYPE_TAG>;
+        using CRITIC_SPEC = nn_models::mlp::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM + ENVIRONMENT::ACTION_DIM, 1, PARAMETERS::CRITIC_NUM_LAYERS, PARAMETERS::CRITIC_HIDDEN_DIM, PARAMETERS::CRITIC_ACTIVATION_FUNCTION, nn::activation_functions::IDENTITY, PARAMETERS::SAC_PARAMETERS::CRITIC_BATCH_SIZE, CONTAINER_TYPE_TAG>;
+        using OPTIMIZER_SPEC = typename nn::optimizers::adam::Specification<T, TI, typename PARAMETERS::OPTIMIZER_PARAMETERS>;
+        using OPTIMIZER = nn::optimizers::Adam<OPTIMIZER_SPEC>;
 
-    template <typename T_STRUCTURE_SPEC>
-    struct InferenceBackwardSpecification: Specification<T_STRUCTURE_SPEC, nn::parameters::Plain>{
-        using SUPER = Specification<T_STRUCTURE_SPEC, nn::parameters::Plain>;
-        using  INPUT_LAYER = nn::layers::dense::LayerBackward<typename SUPER::INPUT_LAYER_SPEC>;
-        using HIDDEN_LAYER = nn::layers::dense::LayerBackward<typename SUPER::HIDDEN_LAYER_SPEC>;
-        using OUTPUT_LAYER = nn::layers::dense::LayerBackward<typename SUPER::OUTPUT_LAYER_SPEC>;
-    };
+        using CAPABILITY_LEARNING = nn::layer_capability::Gradient<nn::parameters::Adam>;
+        using ACTOR_TYPE = nn_models::mlp::NeuralNetwork<CAPABILITY_LEARNING, ACTOR_SPEC>;
 
-    template <typename T_STRUCTURE_SPEC>
-    struct BackwardGradientSpecification: Specification<T_STRUCTURE_SPEC, nn::parameters::Gradient>{
-        using SUPER = Specification<T_STRUCTURE_SPEC, nn::parameters::Gradient>;
-        using  INPUT_LAYER = nn::layers::dense::LayerBackwardGradient<typename SUPER::INPUT_LAYER_SPEC>;
-        using HIDDEN_LAYER = nn::layers::dense::LayerBackwardGradient<typename SUPER::HIDDEN_LAYER_SPEC>;
-        using OUTPUT_LAYER = nn::layers::dense::LayerBackwardGradient<typename SUPER::OUTPUT_LAYER_SPEC>;
+        using CRITIC_TYPE = nn_models::mlp::NeuralNetwork<CAPABILITY_LEARNING, CRITIC_SPEC>;
+        using CRITIC_TARGET_TYPE = nn_models::mlp::NeuralNetwork<nn::layer_capability::Forward, CRITIC_SPEC>;
     };
 
-    template<typename T_STRUCTURE_SPEC>
-    struct SGDSpecification: Specification<T_STRUCTURE_SPEC, nn::parameters::SGD>{
-        using SUPER = Specification<T_STRUCTURE_SPEC, nn::parameters::SGD>;
-        using  INPUT_LAYER = nn::layers::dense::LayerBackwardGradient<typename SUPER::INPUT_LAYER_SPEC>;
-        using HIDDEN_LAYER = nn::layers::dense::LayerBackwardGradient<typename SUPER::HIDDEN_LAYER_SPEC>;
-        using OUTPUT_LAYER = nn::layers::dense::LayerBackwardGradient<typename SUPER::OUTPUT_LAYER_SPEC>;
-    };
-
-    template<typename T_STRUCTURE_SPEC>
-    struct AdamSpecification: Specification<T_STRUCTURE_SPEC, nn::parameters::Adam>{
-        using SUPER = Specification<T_STRUCTURE_SPEC, nn::parameters::Adam>;
-        using  INPUT_LAYER = nn::layers::dense::LayerBackwardGradient<typename SUPER::INPUT_LAYER_SPEC>;
-        using HIDDEN_LAYER = nn::layers::dense::LayerBackwardGradient<typename SUPER::HIDDEN_LAYER_SPEC>;
-        using OUTPUT_LAYER = nn::layers::dense::LayerBackwardGradient<typename SUPER::OUTPUT_LAYER_SPEC>;
-    };
-
-    template<typename T_SPEC, typename T_SPEC::TI T_BATCH_SIZE, typename T_CONTAINER_TYPE_TAG = MatrixDynamicTag>
-    struct NeuralNetworkBuffersSpecification{
-        using SPEC = T_SPEC;
-        using TI = typename SPEC::TI;
-        static constexpr TI BATCH_SIZE = T_BATCH_SIZE;
+    template<typename T_T, typename T_TI, typename T_RNG, typename T_ENVIRONMENT, typename T_PARAMETERS = DefaultParameters<T_T, T_TI, T_ENVIRONMENT>, template<typename, typename, typename, typename, typename> class APPROXIMATOR_CONFIG=ConfigApproximatorsSequential, typename T_CONTAINER_TYPE_TAG = MatrixDynamicTag>
+    struct Config{
+        using T = T_T;
+        using TI = T_TI;
+        using RNG = T_RNG;
+        using ENVIRONMENT = T_ENVIRONMENT;
+        using ENVIRONMENT_EVALUATION = T_ENVIRONMENT;
+        using CORE_PARAMETERS = T_PARAMETERS;
         using CONTAINER_TYPE_TAG = T_CONTAINER_TYPE_TAG;
-        static constexpr TI DIM = SPEC::HIDDEN_DIM;
-    };
-
-    template<typename T_BUFFER_SPEC>
-    struct NeuralNetworkBuffers{
-        using BUFFER_SPEC = T_BUFFER_SPEC;
-        using SPEC = typename BUFFER_SPEC::SPEC;
-        using T = typename SPEC::T;
-        using TI = typename SPEC::TI;
-        static constexpr TI BATCH_SIZE = T_BUFFER_SPEC::BATCH_SIZE;
-        using TICK_TOCK_CONTAINER_SPEC = matrix::Specification<T, TI, BATCH_SIZE, BUFFER_SPEC::DIM, typename SPEC::MEMORY_LAYOUT>;
-        using TICK_TOCK_CONTAINER_TYPE = typename BUFFER_SPEC::CONTAINER_TYPE_TAG::template type<TICK_TOCK_CONTAINER_SPEC>;
-        TICK_TOCK_CONTAINER_TYPE tick;
-        TICK_TOCK_CONTAINER_TYPE tock;
-    };
 
-    template<typename T_SPEC>
-    struct NeuralNetwork{
-        using SPEC = T_SPEC;
-        using T = typename SPEC::T;
-        using TI = typename SPEC::TI;
-        template<TI BUFFER_BATCH_SIZE = SPEC::BATCH_SIZE, typename T_CONTAINER_TYPE_TAG = typename T_SPEC::CONTAINER_TYPE_TAG>
-        using Buffer = NeuralNetworkBuffers<NeuralNetworkBuffersSpecification<SPEC, BUFFER_BATCH_SIZE, T_CONTAINER_TYPE_TAG>>;
-
-        // Convenience
-        static_assert(SPEC::STRUCTURE_SPEC::NUM_LAYERS >= 2); // At least input and output layer are required
-        static constexpr TI NUM_HIDDEN_LAYERS = SPEC::STRUCTURE_SPEC::NUM_LAYERS - 2;
-        static_assert(SPEC::NUM_HIDDEN_LAYERS == NUM_HIDDEN_LAYERS);
-
-        // Interface
-        static constexpr TI  INPUT_DIM = SPEC::INPUT_LAYER ::SPEC::INPUT_DIM;
-        static constexpr TI OUTPUT_DIM = SPEC::OUTPUT_LAYER::SPEC::OUTPUT_DIM;
-        static constexpr TI NUM_WEIGHTS = SPEC::INPUT_LAYER::NUM_WEIGHTS + SPEC::HIDDEN_LAYER::NUM_WEIGHTS * NUM_HIDDEN_LAYERS + SPEC::OUTPUT_LAYER::NUM_WEIGHTS;
-
-
-        // Storage
-        typename SPEC:: INPUT_LAYER input_layer;
-        typename SPEC::HIDDEN_LAYER hidden_layers[NUM_HIDDEN_LAYERS];
-        typename SPEC::OUTPUT_LAYER output_layer;
-    };
+        using NN = APPROXIMATOR_CONFIG<T, TI, T_ENVIRONMENT, CORE_PARAMETERS, CONTAINER_TYPE_TAG>;
+//        using NN = ConfigApproximatorsMLP<T, TI, T_ENVIRONMENT, T_PARAMETERS>;
 
-    template<typename SPEC>
-    struct NeuralNetworkBackward: public NeuralNetwork<SPEC>{};
-    template<typename SPEC>
-    struct NeuralNetworkBackwardGradient: public NeuralNetworkBackward<SPEC>{};
-    template<typename SPEC>
-    struct NeuralNetworkSGD: public NeuralNetworkBackwardGradient<SPEC>{};
-    template<typename SPEC>
-    struct NeuralNetworkAdam: public NeuralNetworkBackwardGradient<SPEC>{};
+        using EXPLORATION_POLICY_SPEC = nn_models::random_uniform::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM, ENVIRONMENT::ACTION_DIM, nn_models::random_uniform::Range::MINUS_ONE_TO_ONE>;
+        using EXPLORATION_POLICY = nn_models::RandomUniform<EXPLORATION_POLICY_SPEC>;
 
+        using ALPHA_PARAMETER_TYPE = nn::parameters::Adam;
+        using ALPHA_OPTIMIZER = nn::optimizers::Adam<typename NN::OPTIMIZER_SPEC>;
 
+        using ACTOR_CRITIC_SPEC = rl::algorithms::sac::Specification<T, TI, ENVIRONMENT, typename NN::ACTOR_TYPE, typename NN::CRITIC_TYPE, typename NN::CRITIC_TARGET_TYPE, ALPHA_PARAMETER_TYPE, typename NN::OPTIMIZER, typename NN::OPTIMIZER, ALPHA_OPTIMIZER, typename CORE_PARAMETERS::SAC_PARAMETERS, CONTAINER_TYPE_TAG>;
+        using ACTOR_CRITIC_TYPE = rl::algorithms::sac::ActorCritic<ACTOR_CRITIC_SPEC>;
+
+        struct OFF_POLICY_RUNNER_PARAMETERS{
+            static constexpr TI N_ENVIRONMENTS = CORE_PARAMETERS::N_ENVIRONMENTS;
+            static constexpr bool ASYMMETRIC_OBSERVATIONS = false;
+            static constexpr TI REPLAY_BUFFER_CAPACITY = CORE_PARAMETERS::REPLAY_BUFFER_CAP;
+            static constexpr TI EPISODE_STEP_LIMIT = CORE_PARAMETERS::EPISODE_STEP_LIMIT;
+            static constexpr bool STOCHASTIC_POLICY = true;
+            static constexpr bool COLLECT_EPISODE_STATS = CORE_PARAMETERS::COLLECT_EPISODE_STATS;
+            static constexpr TI EPISODE_STATS_BUFFER_SIZE = CORE_PARAMETERS::EPISODE_STATS_BUFFER_SIZE;
+            static constexpr T EXPLORATION_NOISE = 0.1;
+        };
+
+        using OFF_POLICY_RUNNER_SPEC = rl::components::off_policy_runner::Specification<
+                T,
+                TI,
+                ENVIRONMENT,
+                OFF_POLICY_RUNNER_PARAMETERS
+        >;
+        static_assert(ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::ACTOR_BATCH_SIZE == ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::CRITIC_BATCH_SIZE);
+        template <typename CONFIG>
+        using State = State<CONFIG>;
+    };
 }
-RL_TOOLS_NAMESPACE_WRAPPER_END
+
 #endif
+
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h`

 * *Files 11% similar despite different names*

```diff
@@ -2,55 +2,54 @@
 #if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_MODELS_MLP_OPERATIONS_GENERIC_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
 #define RL_TOOLS_NN_MODELS_MLP_OPERATIONS_GENERIC_H
 
 #include "../../nn_models/mlp/network.h"
 #include "../../nn/operations_generic.h"
 #include "../../nn/parameters/operations_generic.h"
-#include "../../nn/optimizers/adam/operations_generic.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools {
     template<typename DEVICE, typename SPEC>
-    void malloc(DEVICE& device, nn_models::mlp::NeuralNetwork<SPEC>& network) {
+    void malloc(DEVICE& device, nn_models::mlp::NeuralNetworkForward<SPEC>& network) {
         malloc(device, network.input_layer);
         for (typename DEVICE::index_t layer_i = 0; layer_i < SPEC::NUM_HIDDEN_LAYERS; layer_i++){
             malloc(device, network.hidden_layers[layer_i]);
         }
         malloc(device, network.output_layer);
     }
     template<typename DEVICE, typename BUFFER_SPEC>
     void malloc(DEVICE& device, nn_models::mlp::NeuralNetworkBuffers<BUFFER_SPEC>& buffers) {
         malloc(device, buffers.tick);
         malloc(device, buffers.tock);
     }
     template<typename DEVICE, typename SPEC>
-    void free(DEVICE& device, nn_models::mlp::NeuralNetwork<SPEC>& network) {
+    void free(DEVICE& device, nn_models::mlp::NeuralNetworkForward<SPEC>& network) {
         free(device, network.input_layer);
         for (typename DEVICE::index_t layer_i = 0; layer_i < SPEC::NUM_HIDDEN_LAYERS; layer_i++){
             free(device, network.hidden_layers[layer_i]);
         }
         free(device, network.output_layer);
     }
     template<typename DEVICE, typename SPEC>
     void free(DEVICE& device, nn_models::mlp::NeuralNetworkBuffers<SPEC>& buffers) {
         free(device, buffers.tick);
         free(device, buffers.tock);
     }
     template<typename DEVICE, typename SPEC, typename RNG>
-    void init_weights(DEVICE& device, nn_models::mlp::NeuralNetwork<SPEC>& network, RNG& rng) {
+    void init_weights(DEVICE& device, nn_models::mlp::NeuralNetworkForward<SPEC>& network, RNG& rng) {
         init_weights(device, network.input_layer, rng);
         for (typename DEVICE::index_t layer_i = 0; layer_i < SPEC::NUM_HIDDEN_LAYERS; layer_i++){
             init_weights(device, network.hidden_layers[layer_i], rng);
         }
         init_weights(device, network.output_layer, rng);
     }
 
     template <typename SPEC>
-    constexpr auto& output(nn_models::mlp::NeuralNetwork<SPEC>& m){
+    constexpr auto& output(nn_models::mlp::NeuralNetworkForward<SPEC>& m){
         return m.output_layer.output;
     }
 
     // evaluate does not set intermediate outputs and hence can also be called from stateless layers, for register efficiency use forward when working with "Backward" compatible layers
 
     namespace nn_models::mlp{
         template <typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
@@ -62,15 +61,15 @@
             static_assert(!MODEL_SPEC::ENFORCE_FLOATING_POINT_TYPE || utils::typing::is_same_v<typename INPUT_SPEC::T, typename OUTPUT_SPEC::T>);
             return true;
         }
         template <typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
         constexpr bool check_input_output = check_input_output_f<MODEL_SPEC, INPUT_SPEC, OUTPUT_SPEC>();
     }
     template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename TEMP_SPEC, typename RNG>
-    void evaluate_memless(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, Matrix<TEMP_SPEC>& layer_output_tick, Matrix<TEMP_SPEC>& layer_output_tock, RNG& rng){
+    void evaluate_memless(DEVICE& device, const nn_models::mlp::NeuralNetworkForward<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, Matrix<TEMP_SPEC>& layer_output_tick, Matrix<TEMP_SPEC>& layer_output_tock, RNG& rng){
         static_assert(nn_models::mlp::check_input_output<MODEL_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         static_assert(TEMP_SPEC::ROWS >= BATCH_SIZE);
         static_assert(TEMP_SPEC::COLS >= MODEL_SPEC::HIDDEN_DIM);
         evaluate(device, network.input_layer, input, layer_output_tick, rng);
         for (typename DEVICE::index_t layer_i = 0; layer_i < MODEL_SPEC::NUM_HIDDEN_LAYERS; layer_i++){
             if(layer_i % 2 == 0){
@@ -82,23 +81,23 @@
         if constexpr(MODEL_SPEC::NUM_HIDDEN_LAYERS % 2 == 0){
             evaluate(device, network.output_layer, layer_output_tick, output, rng);
         } else {
             evaluate(device, network.output_layer, layer_output_tock, output, rng);
         }
     }
     template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename BUFFER_MODEL_SPEC, typename RNG>
-    void evaluate(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, nn_models::mlp::NeuralNetworkBuffers<BUFFER_MODEL_SPEC>& buffers, RNG& rng){
+    void evaluate(DEVICE& device, const nn_models::mlp::NeuralNetworkForward<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, nn_models::mlp::NeuralNetworkBuffers<BUFFER_MODEL_SPEC>& buffers, RNG& rng){
         static_assert(BUFFER_MODEL_SPEC::BATCH_SIZE >= OUTPUT_SPEC::ROWS);
         static_assert(BUFFER_MODEL_SPEC::SPEC::HIDDEN_DIM == MODEL_SPEC::HIDDEN_DIM);
         auto tick = view(device, buffers.tick, matrix::ViewSpec<OUTPUT_SPEC::ROWS, BUFFER_MODEL_SPEC::SPEC::HIDDEN_DIM>{});
         auto tock = view(device, buffers.tock, matrix::ViewSpec<OUTPUT_SPEC::ROWS, BUFFER_MODEL_SPEC::SPEC::HIDDEN_DIM>{});
         evaluate_memless(device, network, input, output, tick, tock, rng);
     }
     template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    void evaluate(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng){
+    void evaluate(DEVICE& device, const nn_models::mlp::NeuralNetworkForward<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng){
         static_assert(nn_models::mlp::check_input_output<MODEL_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using T = typename MODEL_SPEC::T;
         using TICK_TOCK_SPEC = matrix::Specification<T, typename DEVICE::index_t, BATCH_SIZE, MODEL_SPEC::HIDDEN_DIM>;
 #ifndef RL_TOOLS_DISABLE_DYNAMIC_MEMORY_ALLOCATIONS
         MatrixDynamic<TICK_TOCK_SPEC> layer_output_tick;
         MatrixDynamic<TICK_TOCK_SPEC> layer_output_tock;
@@ -111,15 +110,15 @@
         evaluate_memless(device, network, input, output, layer_output_tick, layer_output_tock, rng);
         free(device, layer_output_tick);
         free(device, layer_output_tock);
     }
 
     // forward modifies intermediate outputs and pre activations to facilitate backward pass
     template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename TEMP_SPEC, typename RNG>
-    void forward_memless(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, Matrix<TEMP_SPEC>& layer_output_tick, Matrix<TEMP_SPEC>& layer_output_tock, RNG& rng){
+    void forward_memless(DEVICE& device, const nn_models::mlp::NeuralNetworkForward<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, Matrix<TEMP_SPEC>& layer_output_tick, Matrix<TEMP_SPEC>& layer_output_tock, RNG& rng){
         static_assert(nn_models::mlp::check_input_output<MODEL_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         static_assert(TEMP_SPEC::ROWS == BATCH_SIZE);
         static_assert(TEMP_SPEC::COLS == MODEL_SPEC::HIDDEN_DIM);
 
         forward(network.input_layer, input, layer_output_tick, rng);
         for (typename DEVICE::index_t layer_i = 0; layer_i < MODEL_SPEC::NUM_HIDDEN_LAYERS; layer_i++){
@@ -132,38 +131,38 @@
         if constexpr(MODEL_SPEC::NUM_HIDDEN_LAYERS % 2 == 0){
             forward(network.output_layer, layer_output_tick, output, rng);
         } else {
             forward(network.output_layer, layer_output_tock, output, rng);
         }
     }
     template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename BUFFER_MODEL_SPEC, typename RNG>
-    void forward(DEVICE& device, const nn_models::mlp::NeuralNetwork<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, nn_models::mlp::NeuralNetworkBuffers<BUFFER_MODEL_SPEC> buffers, RNG& rng){
+    void forward(DEVICE& device, const nn_models::mlp::NeuralNetworkForward<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, nn_models::mlp::NeuralNetworkBuffers<BUFFER_MODEL_SPEC> buffers, RNG& rng){
         static_assert(BUFFER_MODEL_SPEC::BATCH_SIZE == OUTPUT_SPEC::ROWS);
         forward_memless(device, network, input, output, buffers.tick, buffers.tock);
     }
     template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename RNG>
-    void forward(DEVICE& device, nn_models::mlp::NeuralNetworkBackwardGradient<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, RNG& rng) {
+    void forward(DEVICE& device, nn_models::mlp::NeuralNetworkGradient<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, RNG& rng) {
         forward(device, network.input_layer, input, rng);
 
         auto current_output = network.input_layer.output;
         for (typename DEVICE::index_t layer_i = 0; layer_i < MODEL_SPEC::NUM_HIDDEN_LAYERS; layer_i++){
             forward(device, network.hidden_layers[layer_i], current_output, rng);
             current_output = network.hidden_layers[layer_i].output;
         }
         forward(device, network.output_layer, current_output, rng);
     }
     template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    void forward(DEVICE& device, nn_models::mlp::NeuralNetworkBackwardGradient<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
+    void forward(DEVICE& device, nn_models::mlp::NeuralNetworkGradient<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, RNG& rng) {
         static_assert(nn_models::mlp::check_input_output<MODEL_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         forward(device, network, input, rng);
         copy(device, device, network.output_layer.output, output);
     }
 
     template<typename DEVICE, typename SPEC>
-    void zero_gradient(DEVICE& device, nn_models::mlp::NeuralNetwork<SPEC>& network) {
+    void zero_gradient(DEVICE& device, nn_models::mlp::NeuralNetworkGradient<SPEC>& network) {
         zero_gradient(device, network.input_layer);
         for(typename DEVICE::index_t i = 0; i < SPEC::NUM_HIDDEN_LAYERS; i++){
             zero_gradient(device, network.hidden_layers[i]);
         }
         zero_gradient(device, network.output_layer);
     }
     template<typename DEVICE, typename MODEL_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC, typename BUFFER_MODEL_SPEC>
@@ -186,15 +185,15 @@
             }
         }
         auto& target_d_output_buffer = (MODEL_SPEC::NUM_HIDDEN_LAYERS % 2 == 0) ? buffers.tick : buffers.tock;
         backward_input(device, network.input_layer, target_d_output_buffer, d_input);
     }
 
     template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC, typename BUFFER_MODEL_SPEC, typename D_INPUT_SPEC>
-    void backward_full(DEVICE& device, nn_models::mlp::NeuralNetworkBackwardGradient<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input, nn_models::mlp::NeuralNetworkBuffers<BUFFER_MODEL_SPEC> buffer) {
+    void backward_full(DEVICE& device, nn_models::mlp::NeuralNetworkGradient<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input, nn_models::mlp::NeuralNetworkBuffers<BUFFER_MODEL_SPEC> buffer) {
         // ATTENTION: this modifies d_output (uses it as a buffer for the d_pre_activations
         static_assert(nn_models::mlp::check_input_output<MODEL_SPEC, D_INPUT_SPEC, D_OUTPUT_SPEC>);
         static_assert(nn_models::mlp::check_input_output<MODEL_SPEC, INPUT_SPEC, D_OUTPUT_SPEC>);
         constexpr auto BATCH_SIZE = D_INPUT_SPEC::ROWS;
         static_assert(BUFFER_MODEL_SPEC::BATCH_SIZE == BATCH_SIZE);
         static_assert(BUFFER_MODEL_SPEC::DIM >= MODEL_SPEC::HIDDEN_DIM);
 
@@ -212,15 +211,15 @@
         if constexpr(MODEL_SPEC::NUM_HIDDEN_LAYERS % 2 == 0){
             backward(device, network.input_layer, input, buffer.tick, d_input);
         } else {
             backward(device, network.input_layer, input, buffer.tock, d_input);
         }
     }
     template<typename DEVICE, typename MODEL_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC, typename BUFFER_MODEL_SPEC>
-    void backward(DEVICE& device, nn_models::mlp::NeuralNetworkBackwardGradient<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, nn_models::mlp::NeuralNetworkBuffers<BUFFER_MODEL_SPEC> buffer) {
+    void backward(DEVICE& device, nn_models::mlp::NeuralNetworkGradient<MODEL_SPEC>& network, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, nn_models::mlp::NeuralNetworkBuffers<BUFFER_MODEL_SPEC> buffer) {
         // ATTENTION: this modifies d_output (uses it as a buffer for the d_pre_activations
         static_assert(nn_models::mlp::check_input_output<MODEL_SPEC, INPUT_SPEC, D_OUTPUT_SPEC>);
         constexpr auto BATCH_SIZE = D_OUTPUT_SPEC::ROWS;
         static_assert(BUFFER_MODEL_SPEC::BATCH_SIZE == BATCH_SIZE);
         static_assert(BUFFER_MODEL_SPEC::DIM >= MODEL_SPEC::HIDDEN_DIM);
 
         auto previous_output = MODEL_SPEC::NUM_HIDDEN_LAYERS > 0 ? network.hidden_layers[MODEL_SPEC::NUM_HIDDEN_LAYERS - 1].output : network.input_layer.output;
@@ -238,77 +237,73 @@
             backward_param(device, network.input_layer, input, buffer.tick);
         } else {
             backward_param(device, network.input_layer, input, buffer.tock);
         }
     }
 
     template<typename DEVICE, typename SPEC, typename ADAM_PARAMETERS>
-    void update(DEVICE& device, nn_models::mlp::NeuralNetworkBackwardGradient<SPEC>& network, nn::optimizers::Adam<ADAM_PARAMETERS>& optimizer) {
+    void update(DEVICE& device, nn_models::mlp::NeuralNetworkGradient<SPEC>& network, nn::optimizers::Adam<ADAM_PARAMETERS>& optimizer) {
         using T = typename SPEC::T;
         update(device, network.input_layer, optimizer);
         for(typename DEVICE::index_t layer_i = 0; layer_i < SPEC::NUM_HIDDEN_LAYERS; layer_i++){
             update(device, network.hidden_layers[layer_i], optimizer);
         }
         update(device, network.output_layer, optimizer);
     }
 
-    template<typename DEVICE, typename SPEC>
-    void _reset_optimizer_state(DEVICE& device, nn_models::mlp::NeuralNetworkSGD<SPEC>& network) {
-    }
-
     template<typename DEVICE, typename SPEC, typename OPTIMIZER>
-    void _reset_optimizer_state(DEVICE& device, nn_models::mlp::NeuralNetworkBackwardGradient<SPEC>& network, OPTIMIZER& optimizer) {
+    void _reset_optimizer_state(DEVICE& device, nn_models::mlp::NeuralNetworkGradient<SPEC>& network, OPTIMIZER& optimizer) {
         // this function is marked with a underscore because it should usually be called from the reset_optimizer_state function of the optimizer to have one coherent entrypoint for resetting the optimizer state in the optimizer and in the model
         _reset_optimizer_state(device, network.input_layer, optimizer);
         for(typename DEVICE::index_t layer_i = 0; layer_i < SPEC::NUM_HIDDEN_LAYERS; layer_i++){
             _reset_optimizer_state(device, network.hidden_layers[layer_i], optimizer);
         }
         _reset_optimizer_state(device, network.output_layer, optimizer);
     }
 
     // The following copy operators are more powerful than the default copy assignment operator in that they can e.g. copy between networks with different activation functions
     template<typename SOURCE_DEVICE, typename TARGET_DEVICE,  typename SOURCE_SPEC, typename TARGET_SPEC>
-    void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, const  nn_models::mlp::NeuralNetwork<SOURCE_SPEC>& source, nn_models::mlp::NeuralNetwork<TARGET_SPEC>& target){
-        static_assert(rl_tools::nn_models::mlp::check_spec_memory<typename SOURCE_SPEC::STRUCTURE_SPEC, typename TARGET_SPEC::STRUCTURE_SPEC>, "The source and target network must have the same structure");
+    void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, const  nn_models::mlp::NeuralNetworkForward<SOURCE_SPEC>& source, nn_models::mlp::NeuralNetworkForward<TARGET_SPEC>& target){
+        static_assert(rl_tools::nn_models::mlp::check_spec_memory<SOURCE_SPEC, TARGET_SPEC>, "The source and target network must have the same structure");
         copy(source_device, target_device, source.input_layer, target.input_layer);
         for(typename SOURCE_SPEC::TI layer_i = 0; layer_i <  SOURCE_SPEC::NUM_HIDDEN_LAYERS; layer_i++){
             copy(source_device, target_device, source.hidden_layers[layer_i], target.hidden_layers[layer_i]);
         }
         copy(source_device, target_device, source.output_layer, target.output_layer);
     }
 
-    template<typename SOURCE_DEVICE, typename TARGET_DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
-    void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, const  nn_models::mlp::NeuralNetworkAdam<SOURCE_SPEC>& source, nn_models::mlp::NeuralNetworkAdam<TARGET_SPEC>& target){
-        static_assert(rl_tools::nn_models::mlp::check_spec_memory<typename SOURCE_SPEC::STRUCTURE_SPEC, typename TARGET_SPEC::STRUCTURE_SPEC>, "The source and target network must have the same structure");
-        copy(source_device, target_device, (nn_models::mlp::NeuralNetwork<SOURCE_SPEC>&)source, (nn_models::mlp::NeuralNetwork<TARGET_SPEC>&)target);
-    }
+//    template<typename SOURCE_DEVICE, typename TARGET_DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
+//    void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, const  nn_models::mlp::NeuralNetworkAdam<SOURCE_SPEC>& source, nn_models::mlp::NeuralNetworkAdam<TARGET_SPEC>& target){
+//        static_assert(rl_tools::nn_models::mlp::check_spec_memory<SOURCE_SPEC, TARGET_SPEC>, "The source and target network must have the same structure");
+//        copy(source_device, target_device, (nn_models::mlp::NeuralNetworkForward<SOURCE_SPEC>&)source, (nn_models::mlp::NeuralNetworkForward<TARGET_SPEC>&)target);
+//    }
 
     template<typename DEVICE, typename SPEC>
-    void reset_forward_state(DEVICE& device, nn_models::mlp::NeuralNetwork<SPEC>& n){
+    void reset_forward_state(DEVICE& device, nn_models::mlp::NeuralNetworkForward<SPEC>& n){
         reset_forward_state(device, n.input_layer);
         for(typename DEVICE::index_t layer_i = 0; layer_i <  SPEC::NUM_HIDDEN_LAYERS; layer_i++){
             reset_forward_state(device, n.hidden_layers[layer_i]);
         }
         reset_forward_state(device, n.output_layer);
     }
 
     template<typename DEVICE, typename SPEC_1, typename SPEC_2>
-    typename SPEC_1::T abs_diff(DEVICE& device, nn_models::mlp::NeuralNetwork<SPEC_1>& n1, const nn_models::mlp::NeuralNetwork<SPEC_2>& n2){
-        static_assert(rl_tools::nn_models::mlp::check_spec_memory<typename SPEC_1::STRUCTURE_SPEC, typename SPEC_2::STRUCTURE_SPEC>, "The source and target network must have the same structure");
+    typename SPEC_1::T abs_diff(DEVICE& device, nn_models::mlp::NeuralNetworkForward<SPEC_1>& n1, const nn_models::mlp::NeuralNetworkForward<SPEC_2>& n2){
+        static_assert(rl_tools::nn_models::mlp::check_spec_memory<SPEC_1, SPEC_2>, "The source and target network must have the same structure");
         typename SPEC_1::T acc = 0;
 
         acc += abs_diff(device, n1.output_layer, n2.output_layer);
         for(typename DEVICE::index_t layer_i = 0; layer_i < SPEC_1::NUM_HIDDEN_LAYERS; layer_i++){
             acc += abs_diff(device, n1.hidden_layers[layer_i], n2.hidden_layers[layer_i]);
         }
         acc += abs_diff(device, n1.input_layer, n2.input_layer);
         return acc;
     }
     template <typename DEVICE, typename SPEC>
-    bool is_nan(DEVICE& device, const rl_tools::nn_models::mlp::NeuralNetwork<SPEC>& n) {
+    bool is_nan(DEVICE& device, const rl_tools::nn_models::mlp::NeuralNetworkForward<SPEC>& n) {
         bool found_nan = false;
         found_nan = found_nan || is_nan(device, n.input_layer);
         for(typename DEVICE::index_t layer_i = 0; layer_i < SPEC::NUM_HIDDEN_LAYERS; layer_i++){
             found_nan = found_nan || is_nan(device, n.hidden_layers[layer_i]);
         }
         found_nan = found_nan || is_nan(device, n.output_layer);
         return found_nan;
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h`

 * *Files 4% similar despite different names*

```diff
@@ -8,36 +8,32 @@
 #include "network.h"
 
 #include <highfive/H5Group.hpp>
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template<typename DEVICE, typename SPEC>
-    void save(DEVICE& device, nn_models::mlp::NeuralNetwork<SPEC>& network, HighFive::Group group) {
+    void save(DEVICE& device, nn_models::mlp::NeuralNetworkForward<SPEC>& network, HighFive::Group group) {
         using NetworkType = typename utils::typing::remove_reference<decltype(network)>::type;
         save(device, network.input_layer, group.createGroup("input_layer"));
         for(typename DEVICE::index_t layer_i = 0; layer_i < NetworkType::NUM_HIDDEN_LAYERS; layer_i++) {
             save(device, network.hidden_layers[layer_i], group.createGroup("hidden_layer_" + std::to_string(layer_i)));
         }
         save(device, network.output_layer, group.createGroup("output_layer"));
     }
     template<typename DEVICE, typename SPEC>
-    void save(DEVICE& device, nn_models::mlp::NeuralNetworkAdam<SPEC>& network, HighFive::Group group) {
-        save(device, (nn_models::mlp::NeuralNetwork<SPEC>&)network, group);
-    }
-    template<typename DEVICE, typename SPEC>
-    void load(DEVICE& device, nn_models::mlp::NeuralNetwork<SPEC>& network, HighFive::Group group){
+    void load(DEVICE& device, nn_models::mlp::NeuralNetworkForward<SPEC>& network, HighFive::Group group){
         using NetworkType = typename utils::typing::remove_reference<decltype(network)>::type;
         load(device, network.input_layer, group.getGroup("input_layer"));
         for(typename DEVICE::index_t layer_i = 0; layer_i < NetworkType::NUM_HIDDEN_LAYERS; layer_i++) {
             load(device, network.hidden_layers[layer_i], group.getGroup("hidden_layer_" + std::to_string(layer_i)));
         }
         load(device, network.output_layer, group.getGroup("output_layer"));
     }
     template<typename DEVICE, typename SPEC>
-    void load(DEVICE& device, nn_models::mlp::NeuralNetwork<SPEC>& network, std::string file_path){
+    void load(DEVICE& device, nn_models::mlp::NeuralNetworkForward<SPEC>& network, std::string file_path){
         auto file = HighFive::File(file_path, HighFive::File::ReadOnly);
         load(device, network, file.getGroup("mlp"));
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,55 @@
+#include "../../version.h"
+#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_MODELS_MLP_UNCONDITIONAL_STDDEV_OPERATIONS_GENERIC_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
+#pragma once
+#define RL_TOOLS_NN_MODELS_MLP_UNCONDITIONAL_STDDEV_OPERATIONS_GENERIC_H
+
 #include "network.h"
 #include "../../nn_models/mlp/operations_generic.h"
 
 
+
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
-    template <typename DEVICE, typename SPEC>
-    void malloc(DEVICE& device, nn_models::mlp_unconditional_stddev::NeuralNetworkAdam<SPEC>& m){
-        malloc(device, (nn_models::mlp::NeuralNetworkAdam<SPEC>&)m);
+    template <typename DEVICE, typename SPEC, template <typename> typename BASE>
+    void malloc(DEVICE& device, nn_models::mlp_unconditional_stddev::NeuralNetworkForward<SPEC, BASE>& m){
+        malloc(device, (nn_models::mlp::NeuralNetworkForward<SPEC>&)m);
         malloc(device, m.log_std);
     }
-    template <typename DEVICE, typename SPEC>
-    void free(DEVICE& device, nn_models::mlp_unconditional_stddev::NeuralNetworkAdam<SPEC>& m){
-        free(device, (nn_models::mlp::NeuralNetworkAdam<SPEC>&)m);
+    template <typename DEVICE, typename SPEC, template <typename> typename BASE>
+    void free(DEVICE& device, nn_models::mlp_unconditional_stddev::NeuralNetworkForward<SPEC, BASE>& m){
+        free(device, (nn_models::mlp::NeuralNetworkForward<SPEC>&)m);
         free(device, m.log_std);
     }
-    template <typename DEVICE, typename SPEC, typename RNG>
-    void init_weights(DEVICE& device, nn_models::mlp_unconditional_stddev::NeuralNetworkAdam<SPEC>& m, RNG& rng){
-        init_weights(device, (nn_models::mlp::NeuralNetworkAdam<SPEC>&)m, rng);
+    template <typename DEVICE, typename SPEC, template <typename> typename BASE, typename RNG>
+    void init_weights(DEVICE& device, nn_models::mlp_unconditional_stddev::NeuralNetworkForward<SPEC, BASE>& m, RNG& rng){
+        init_weights(device, (nn_models::mlp::NeuralNetworkForward<SPEC>&)m, rng);
         set_all(device, m.log_std.parameters, 0);
     }
-    template<typename DEVICE, typename SPEC, typename ADAM_PARAMETERS>
-    void update(DEVICE& device, nn_models::mlp_unconditional_stddev::NeuralNetworkAdam<SPEC>& network, nn::optimizers::Adam<ADAM_PARAMETERS>& optimizer) {
+    template<typename DEVICE, typename SPEC, template <typename> typename BASE, typename ADAM_PARAMETERS>
+    void update(DEVICE& device, nn_models::mlp_unconditional_stddev::NeuralNetworkGradient<SPEC, BASE>& network, nn::optimizers::Adam<ADAM_PARAMETERS>& optimizer) {
         using T = typename SPEC::T;
         update(device, network.log_std, optimizer);
-        update(device, (nn_models::mlp::NeuralNetworkAdam<SPEC>&)network, optimizer);
+        update(device, (nn_models::mlp::NeuralNetworkGradient<SPEC>&)network, optimizer);
     }
-    template<typename DEVICE, typename SPEC>
-    void zero_gradient(DEVICE& device, nn_models::mlp_unconditional_stddev::NeuralNetworkAdam<SPEC>& network) {
-        zero_gradient(device, (nn_models::mlp::NeuralNetworkAdam<SPEC>&)network);
+    template<typename DEVICE, typename SPEC, template <typename> typename BASE>
+    void zero_gradient(DEVICE& device, nn_models::mlp_unconditional_stddev::NeuralNetworkGradient<SPEC, BASE>& network) {
+        zero_gradient(device, (nn_models::mlp::NeuralNetworkGradient<SPEC>&)network);
         zero_gradient(device, network.log_std);
     }
 
-    template<typename DEVICE, typename SPEC, typename OPTIMIZER>
-    void _reset_optimizer_state(DEVICE& device, nn_models::mlp_unconditional_stddev::NeuralNetworkAdam<SPEC>& network, OPTIMIZER& optimizer) {
-        _reset_optimizer_state(device, (nn_models::mlp::NeuralNetworkAdam<SPEC>&)network, optimizer);
+    template<typename DEVICE, typename SPEC, template <typename> typename BASE, typename OPTIMIZER>
+    void _reset_optimizer_state(DEVICE& device, nn_models::mlp_unconditional_stddev::NeuralNetworkGradient<SPEC, BASE>& network, OPTIMIZER& optimizer) {
+        _reset_optimizer_state(device, (nn_models::mlp::NeuralNetworkGradient<SPEC>&)network, optimizer);
         _reset_optimizer_state(device, network.log_std, optimizer);
     }
 
-    template<typename SOURCE_DEVICE, typename TARGET_DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
-    void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, const  nn_models::mlp_unconditional_stddev::NeuralNetworkAdam<SOURCE_SPEC>& source, nn_models::mlp_unconditional_stddev::NeuralNetworkAdam<TARGET_SPEC>& target){
-        static_assert(rl_tools::nn_models::mlp::check_spec_memory<typename SOURCE_SPEC::STRUCTURE_SPEC, typename TARGET_SPEC::STRUCTURE_SPEC>, "The source and target network must have the same structure");
-        copy(source_device, target_device, (nn_models::mlp::NeuralNetworkAdam<SOURCE_SPEC>&)source, (nn_models::mlp::NeuralNetworkAdam<TARGET_SPEC>&)target);
+    template<typename SOURCE_DEVICE, typename TARGET_DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC, template <typename> typename SOURCE_BASE, template <typename> typename TARGET_BASE>
+    void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, const  nn_models::mlp_unconditional_stddev::NeuralNetworkForward<SOURCE_SPEC, SOURCE_BASE>& source, nn_models::mlp_unconditional_stddev::NeuralNetworkForward<TARGET_SPEC, TARGET_BASE>& target){
+        static_assert(rl_tools::nn_models::mlp::check_spec_memory<SOURCE_SPEC, TARGET_SPEC>, "The source and target network must have the same structure");
+        copy(source_device, target_device, (nn_models::mlp::NeuralNetworkForward<SOURCE_SPEC>&)source, (nn_models::mlp::NeuralNetworkForward<TARGET_SPEC>&)target);
         copy(source_device, target_device, source.log_std, target.log_std);
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
+
+#endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 #include "../../version.h"
 #if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_MODELS_SEQUENTIAL_MODEL_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
 #define RL_TOOLS_NN_MODELS_SEQUENTIAL_MODEL_H
 
 #include "../../utils/generic/typing.h"
+#include "../../nn/nn.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools::nn_models::sequential{
     struct OutputModule{
         struct CONTENT{
             static constexpr auto INPUT_DIM = 0;
             static constexpr auto BATCH_SIZE = 0;
         };
+        template <typename>
+        using CHANGE_CAPABILITY = OutputModule;
     };
 
     // Required fields on CONTENT:
     // compile-time types
     //     T
     //     TI
     // compile-time constants
@@ -41,15 +44,15 @@
     }
     template <typename TI, typename SPEC>
     constexpr auto find_max_hiddend_dim(TI current_max = 0){
         current_max = current_max > SPEC::CONTENT::OUTPUT_DIM ? current_max : SPEC::CONTENT::OUTPUT_DIM;
         if constexpr (utils::typing::is_same_v<typename SPEC::NEXT_MODULE, OutputModule>){
             return 0;
         } else {
-            auto max_downstream = find_max_hiddend_dim<TI, typename SPEC::NEXT_MODULE>();
+            TI max_downstream = find_max_hiddend_dim<TI, typename SPEC::NEXT_MODULE>();
             return max_downstream > current_max ? max_downstream : current_max;
         }
     }
     template <typename MODULE>
     constexpr bool check_batch_size_consistency_f(){
         if constexpr (utils::typing::is_same_v<typename MODULE::NEXT_MODULE, OutputModule>){
             return true;
@@ -85,14 +88,20 @@
         using CONTAINER_TYPE_TAG = typename CONTENT::CONTAINER_TYPE_TAG;
         static constexpr TI INPUT_DIM = CONTENT::INPUT_DIM;
         static constexpr TI OUTPUT_DIM = find_output_dim<Specification<T_CONTENT, T_NEXT_MODULE>>();
         static constexpr TI MAX_HIDDEN_DIM = find_max_hiddend_dim<typename CONTENT::TI, Specification<T_CONTENT, T_NEXT_MODULE>>();
         static_assert(utils::typing::is_same_v<NEXT_MODULE, OutputModule> || CONTENT::OUTPUT_DIM == NEXT_MODULE::CONTENT::INPUT_DIM);
     };
 
+    template <typename T_CAPABILITY, typename T_SPEC>
+    struct CapabilitySpecification: T_SPEC{
+        using CAPABILITY = T_CAPABILITY;
+        using PARAMETER_TYPE = typename CAPABILITY::PARAMETER_TYPE;
+    };
+
     template <typename T_SPEC, typename T_SPEC::TI T_BATCH_SIZE, typename T_CONTAINER_TYPE_TAG, typename T_MEMORY_LAYOUT>
     struct ModuleBufferSpecification {
         using SPEC = T_SPEC;
         using TI = typename SPEC::TI;
         static constexpr TI BATCH_SIZE = T_BATCH_SIZE;
         using CONTAINER_TYPE_TAG = T_CONTAINER_TYPE_TAG;
         using MEMORY_LAYOUT = T_MEMORY_LAYOUT;
@@ -106,15 +115,15 @@
         static constexpr TI BATCH_SIZE = T_BUFFER_SPEC::BATCH_SIZE;
         using TICK_TOCK_CONTAINER_SPEC = matrix::Specification<T, TI, BATCH_SIZE, SPEC::MAX_HIDDEN_DIM, typename BUFFER_SPEC::MEMORY_LAYOUT>;
         using TICK_TOCK_CONTAINER_TYPE = typename BUFFER_SPEC::CONTAINER_TYPE_TAG::template type<TICK_TOCK_CONTAINER_SPEC>;
         TICK_TOCK_CONTAINER_TYPE tick;
         TICK_TOCK_CONTAINER_TYPE tock;
     };
     template <typename T_SPEC>
-    struct Module{
+    struct ModuleForward{
         using SPEC = T_SPEC;
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         using CONTENT = typename SPEC::CONTENT;
         using NEXT_MODULE = typename SPEC::NEXT_MODULE;
         CONTENT content;
         NEXT_MODULE next_module;
@@ -122,16 +131,37 @@
         static constexpr auto INPUT_DIM = SPEC::INPUT_DIM;
         static constexpr auto OUTPUT_DIM = SPEC::OUTPUT_DIM;
 
         template <typename SPEC::TI BATCH_SIZE, typename CONTAINER_TYPE_TAG=typename SPEC::CONTAINER_TYPE_TAG, typename MEMORY_LAYOUT = matrix::layouts::DEFAULT<typename SPEC::TI>>
         using Buffer = ModuleBuffer<ModuleBufferSpecification<SPEC, BATCH_SIZE, CONTAINER_TYPE_TAG, MEMORY_LAYOUT>>;
     };
 
-    namespace interface{
-        template <typename T_CONTENT, typename T_NEXT_MODULE = OutputModule>
-        struct Module: rl_tools::nn_models::sequential::Module<Specification<T_CONTENT, T_NEXT_MODULE>>{};
-    }
+    template <typename T_SPEC>
+    struct ModuleBackward: public ModuleForward<T_SPEC>{};
+    template <typename T_SPEC>
+    struct ModuleGradient: public ModuleBackward<T_SPEC>{};
+
+    template <typename CAPABILITY, template <typename> typename CONTENT, typename NEXT_MODULE>
+    using _Module =
+        utils::typing::conditional_t<CAPABILITY::TAG == nn::LayerCapability::Forward,
+                ModuleForward<CapabilitySpecification<CAPABILITY, Specification<CONTENT<CAPABILITY>, NEXT_MODULE>>>,
+        utils::typing::conditional_t<CAPABILITY::TAG == nn::LayerCapability::Backward,
+                ModuleBackward<CapabilitySpecification<CAPABILITY, Specification<CONTENT<CAPABILITY>, NEXT_MODULE>>>,
+        utils::typing::conditional_t<CAPABILITY::TAG == nn::LayerCapability::Gradient,
+                ModuleGradient<CapabilitySpecification<CAPABILITY, Specification<CONTENT<CAPABILITY>, NEXT_MODULE>>>, void>>>;
+
+    template <typename T_CAPABILITY, template <typename> typename T_CONTENT, typename T_NEXT_MODULE = OutputModule>
+    struct Module: _Module<T_CAPABILITY, T_CONTENT, T_NEXT_MODULE>{
+        template <typename TT_CAPABILITY>
+        using CHANGE_CAPABILITY = Module<TT_CAPABILITY, T_CONTENT, typename T_NEXT_MODULE::template CHANGE_CAPABILITY<TT_CAPABILITY>>;
+    };
+
+    template <typename T_CAPABILITY>
+    struct Interface{
+        template <template <typename> typename T_CONTENT, typename T_NEXT_MODULE = OutputModule>
+        using Module = sequential::Module<T_CAPABILITY, T_CONTENT, T_NEXT_MODULE>;
+    };
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
 
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 #define RL_TOOLS_NN_MODELS_SEQUENTIAL_OPERATIONS_GENERIC_H
 
 #include "model.h"
 #include "../../utils/generic/typing.h"
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template <typename DEVICE, typename MODULE_SPEC>
-    void malloc(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& module){
+    void malloc(DEVICE& device, nn_models::sequential::ModuleForward<MODULE_SPEC>& module){
         using namespace nn_models::sequential;
         malloc(device, module.content);
         if constexpr(!utils::typing::is_same_v<typename MODULE_SPEC::NEXT_MODULE, OutputModule>){
             malloc(device, module.next_module);
         }
     }
     template <typename DEVICE, typename MODULE_SPEC>
-    void free(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& module){
+    void free(DEVICE& device, nn_models::sequential::ModuleForward<MODULE_SPEC>& module){
         using namespace nn_models::sequential;
         free(device, module.content);
         if constexpr(!utils::typing::is_same_v<typename MODULE_SPEC::NEXT_MODULE, OutputModule>){
             free(device, module.next_module);
         }
     }
     template <typename DEVICE, typename BUFFER_SPEC>
@@ -32,41 +32,41 @@
     template <typename DEVICE, typename BUFFER_SPEC>
     void free(DEVICE& device, nn_models::sequential::ModuleBuffer<BUFFER_SPEC>& buffers){
         using namespace nn_models::sequential;
         free(device, buffers.tick);
         free(device, buffers.tock);
     }
     template <typename DEVICE, typename MODULE_SPEC, typename RNG>
-    void init_weights(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& module, RNG& rng){
+    void init_weights(DEVICE& device, nn_models::sequential::ModuleForward<MODULE_SPEC>& module, RNG& rng){
         using namespace nn_models::sequential;
         init_weights(device, module.content, rng);
         if constexpr(!utils::typing::is_same_v<typename MODULE_SPEC::NEXT_MODULE, OutputModule>){
             init_weights(device, module.next_module, rng);
         }
     }
     template <typename SPEC>
-    constexpr typename SPEC::TI num_layers(nn_models::sequential::Module<SPEC>){
+    constexpr typename SPEC::TI num_layers(nn_models::sequential::ModuleForward<SPEC>){
         if constexpr(!utils::typing::is_same_v<typename SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             return num_layers(typename SPEC::NEXT_MODULE{}) + 1;
         }
         else{
             return 1;
         }
     }
     template <typename SPEC>
-    constexpr auto& output(nn_models::sequential::Module<SPEC>& m){
+    constexpr auto& output(nn_models::sequential::ModuleGradient<SPEC>& m){
         if constexpr (utils::typing::is_same_v<typename SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             return m.content.output;
         } else {
             return output(m.next_module);
         }
     }
     // Evaluate is like a forward pass but without saving intermediate activations (so a backward pass is not possible). Hence we can reuse the memory of the intermediate outputs and just require a double buffer where each buffer has to be able to contain the maximum hidden dimension of the module
     template<bool TICK = true, typename DEVICE, typename MODULE_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename BUFFER_SPEC, typename RNG>
-    void evaluate(DEVICE& device, const nn_models::sequential::Module<MODULE_SPEC>& model, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, nn_models::sequential::ModuleBuffer<BUFFER_SPEC>& buffers, RNG& rng){
+    void evaluate(DEVICE& device, const nn_models::sequential::ModuleForward<MODULE_SPEC>& model, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, nn_models::sequential::ModuleBuffer<BUFFER_SPEC>& buffers, RNG& rng){
         static_assert(nn_models::sequential::buffer_compatible<BUFFER_SPEC, MODULE_SPEC>);
         static_assert(BUFFER_SPEC::BATCH_SIZE == OUTPUT_SPEC::ROWS);
         static_assert(nn_models::sequential::check_input_output<MODULE_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
         constexpr auto BATCH_SIZE = INPUT_SPEC::ROWS;
         using DOUBLE_BUFFER_TYPE = decltype(buffers.tick);
 
         if constexpr(utils::typing::is_same_v<typename MODULE_SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
@@ -76,48 +76,48 @@
             DOUBLE_BUFFER_TYPE& output_buffer = TICK ? buffers.tick : buffers.tock;
             auto output_buffer_view = view(device, output_buffer, matrix::ViewSpec<BATCH_SIZE, MODULE_SPEC::CONTENT::OUTPUT_DIM>{});
             evaluate(device, model.content, input, output_buffer_view, rng);
             evaluate<!TICK>(device, model.next_module, output_buffer_view, output, buffers, rng);
         }
     }
     template <typename DEVICE, typename MODULE_SPEC, typename INPUT, typename RNG>
-    void forward(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& module, INPUT& input, RNG& rng){
+    void forward(DEVICE& device, nn_models::sequential::ModuleGradient<MODULE_SPEC>& module, INPUT& input, RNG& rng){
         forward(device, module.content, input, rng);
         if constexpr(!utils::typing::is_same_v<typename MODULE_SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             forward(device, module.next_module, module.content.output, rng);
         }
     }
     template <typename DEVICE, typename MODULE_SPEC, typename INPUT, typename OUTPUT, typename RNG>
-    void forward(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& module, INPUT& input, OUTPUT& output, RNG& rng){
+    void forward(DEVICE& device, nn_models::sequential::ModuleGradient<MODULE_SPEC>& module, INPUT& input, OUTPUT& output, RNG& rng){
         forward(device, module, input, rng);
         copy(device, device, rl_tools::output(module), output);
     }
     template <typename DEVICE, typename MODULE_SPEC>
-    void zero_gradient(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& module){
+    void zero_gradient(DEVICE& device, nn_models::sequential::ModuleGradient<MODULE_SPEC>& module){
         zero_gradient(device, module.content);
         if constexpr(!utils::typing::is_same_v<typename MODULE_SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             zero_gradient(device, module.next_module);
         }
     }
     template<typename DEVICE, typename SPEC, typename OPTIMIZER>
-    void _reset_optimizer_state(DEVICE& device, nn_models::sequential::Module<SPEC>& module, OPTIMIZER& optimizer) {
+    void _reset_optimizer_state(DEVICE& device, nn_models::sequential::ModuleGradient<SPEC>& module, OPTIMIZER& optimizer) {
         _reset_optimizer_state(device, module.content, optimizer);
         if constexpr(!utils::typing::is_same_v<typename SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             _reset_optimizer_state(device, module.next_module, optimizer);
         }
     }
     template<typename DEVICE, typename SPEC>
-    void reset_forward_state(DEVICE& device, nn_models::sequential::Module<SPEC>& module) {
+    void reset_forward_state(DEVICE& device, nn_models::sequential::ModuleGradient<SPEC>& module) {
         reset_forward_state(device, module.content);
         if constexpr(!utils::typing::is_same_v<typename SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             reset_forward_state(device, module.next_module);
         }
     }
     template<typename DEVICE, typename MODULE_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC, typename BUFFER_SPEC, bool TICK = true>
-    void backward_full(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& model, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input, nn_models::sequential::ModuleBuffer<BUFFER_SPEC> buffers) {
+    void backward_full(DEVICE& device, nn_models::sequential::ModuleGradient<MODULE_SPEC>& model, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input, nn_models::sequential::ModuleBuffer<BUFFER_SPEC> buffers) {
         static_assert(nn_models::sequential::check_input_output<MODULE_SPEC, INPUT_SPEC, D_OUTPUT_SPEC>);
         static_assert(nn_models::sequential::check_input_output<MODULE_SPEC, D_INPUT_SPEC, D_OUTPUT_SPEC>);
         static_assert(nn_models::sequential::buffer_compatible<BUFFER_SPEC, MODULE_SPEC>);
         using DOUBLE_BUFFER_TYPE = decltype(buffers.tick);
 
         if constexpr(utils::typing::is_same_v<typename MODULE_SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             backward(device, model.content, input, d_output, d_input);
@@ -125,72 +125,72 @@
         else{
             DOUBLE_BUFFER_TYPE& current_d_output_buffer = TICK ? buffers.tick : buffers.tock;
             backward_full<DEVICE, typename MODULE_SPEC::NEXT_MODULE::SPEC, typename decltype(model.content.output)::SPEC, D_OUTPUT_SPEC, typename DOUBLE_BUFFER_TYPE::SPEC, BUFFER_SPEC, !TICK>(device, model.next_module, model.content.output, d_output, current_d_output_buffer, buffers);
             backward(device, model.content, input, current_d_output_buffer, d_input);
         }
     }
     template<typename DEVICE, typename MODULE_SPEC, typename D_OUTPUT_SPEC, typename D_INPUT_SPEC, typename BUFFER_SPEC, bool TICK = true>
-    void backward_input(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& model, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input, nn_models::sequential::ModuleBuffer<BUFFER_SPEC> buffers) {
+    void backward_input(DEVICE& device, nn_models::sequential::ModuleBackward<MODULE_SPEC>& model, Matrix<D_OUTPUT_SPEC>& d_output, Matrix<D_INPUT_SPEC>& d_input, nn_models::sequential::ModuleBuffer<BUFFER_SPEC> buffers) {
         static_assert(nn_models::sequential::check_input_output<MODULE_SPEC, D_INPUT_SPEC, D_OUTPUT_SPEC>);
         static_assert(nn_models::sequential::buffer_compatible<BUFFER_SPEC, MODULE_SPEC>);
         using DOUBLE_BUFFER_TYPE = decltype(buffers.tick);
 
         if constexpr(utils::typing::is_same_v<typename MODULE_SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             backward_input(device, model.content, d_output, d_input);
         }
         else{
             DOUBLE_BUFFER_TYPE& current_d_output_buffer = TICK ? buffers.tick : buffers.tock;
             backward_input<DEVICE, typename MODULE_SPEC::NEXT_MODULE::SPEC, D_OUTPUT_SPEC, typename DOUBLE_BUFFER_TYPE::SPEC, BUFFER_SPEC, !TICK>(device, model.next_module, d_output, current_d_output_buffer, buffers);
             backward_input(device, model.content, current_d_output_buffer, d_input);
         }
     }
     template<typename DEVICE, typename MODULE_SPEC, typename INPUT_SPEC, typename D_OUTPUT_SPEC, typename BUFFER_SPEC>
-    void backward(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& model, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, nn_models::sequential::ModuleBuffer<BUFFER_SPEC> buffers) {
+    void backward(DEVICE& device, nn_models::sequential::ModuleGradient<MODULE_SPEC>& model, const Matrix<INPUT_SPEC>& input, Matrix<D_OUTPUT_SPEC>& d_output, nn_models::sequential::ModuleBuffer<BUFFER_SPEC> buffers) {
         static_assert(!utils::typing::is_same_v<typename MODULE_SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>);
         backward_full<DEVICE, typename MODULE_SPEC::NEXT_MODULE::SPEC, typename decltype(model.content.output)::SPEC, D_OUTPUT_SPEC, typename decltype(buffers.tick)::SPEC, BUFFER_SPEC, false>(device, model.next_module, model.content.output, d_output, buffers.tick, buffers);
         backward_param(device, model.content, input, buffers.tick);
     }
     template<typename DEVICE, typename SPEC, typename OPTIMIZER>
-    void update(DEVICE& device, nn_models::sequential::Module<SPEC>& model, OPTIMIZER& optimizer) {
+    void update(DEVICE& device, nn_models::sequential::ModuleGradient<SPEC>& model, OPTIMIZER& optimizer) {
         update(device, model.content, optimizer);
         if constexpr(!utils::typing::is_same_v<typename SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             update(device, model.next_module, optimizer);
         }
     }
     template<typename SOURCE_DEVICE, typename TARGET_DEVICE,  typename SOURCE_SPEC, typename TARGET_SPEC>
-    void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, const  nn_models::sequential::Module<SOURCE_SPEC>& source, nn_models::sequential::Module<TARGET_SPEC>& target){
+    void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, const  nn_models::sequential::ModuleForward<SOURCE_SPEC>& source, nn_models::sequential::ModuleForward<TARGET_SPEC>& target){
         copy(source_device, target_device, source.content, target.content);
         if constexpr(!utils::typing::is_same_v<typename TARGET_SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             copy(source_device, target_device, source.next_module, target.next_module);
         }
     }
 
     template<typename DEVICE, typename SPEC_A, typename SPEC_B>
-    typename SPEC_A::T abs_diff(DEVICE& device, nn_models::sequential::Module<SPEC_A>& a, const nn_models::sequential::Module<SPEC_B>& b){
+    typename SPEC_A::T abs_diff(DEVICE& device, nn_models::sequential::ModuleForward<SPEC_A>& a, const nn_models::sequential::ModuleForward<SPEC_B>& b){
         auto diff = abs_diff(device, a.content, b.content);
         if constexpr(!utils::typing::is_same_v<typename SPEC_A::NEXT_MODULE, nn_models::sequential::OutputModule>){
             diff += abs_diff(device, a.next_module, b.next_module);
         }
         return diff;
     }
 
     template<typename DEVICE, typename MODULE_SPEC, auto LAYER_I>
-    constexpr auto& get_layer(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& model, Constant<LAYER_I>){
+    constexpr auto& get_layer(DEVICE& device, nn_models::sequential::ModuleForward<MODULE_SPEC>& model, Constant<LAYER_I>){
         static_assert(LAYER_I >= 0);
-        static_assert(LAYER_I < num_layers(nn_models::sequential::Module<MODULE_SPEC>{}));
+        static_assert(LAYER_I < num_layers(nn_models::sequential::ModuleForward<MODULE_SPEC>{}));
         if constexpr(LAYER_I == 0){
             return model.content;
         }
         else{
             return get_layer(device, model.next_module, Constant<LAYER_I - 1>{});
         }
     }
 
     template<typename DEVICE, typename MODULE_SPEC>
-    bool is_nan(DEVICE& device, nn_models::sequential::Module<MODULE_SPEC>& model){
+    bool is_nan(DEVICE& device, nn_models::sequential::ModuleForward<MODULE_SPEC>& model){
         bool current_module_nan = is_nan(device, model.content);
         if constexpr(!utils::typing::is_same_v<typename MODULE_SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             current_module_nan = current_module_nan || is_nan(device, model.next_module);
         }
         return current_module_nan;
     }
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h`

 * *Files 9% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 
 #include <highfive/H5Group.hpp>
 #include <string>
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
         template<typename DEVICE, typename SPEC>
-        void save(DEVICE& device, nn_models::sequential::Module<SPEC>& model, HighFive::Group group, typename DEVICE::index_t layer_i = 0) {
+        void save(DEVICE& device, nn_models::sequential::ModuleForward<SPEC>& model, HighFive::Group group, typename DEVICE::index_t layer_i = 0) {
             if(layer_i == 0){
                 group = group.createGroup("layers");
             }
             save(device, model.content, group.createGroup(std::to_string(layer_i)));
             if constexpr (!utils::typing::is_same_v<typename SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
                 save(device, model.next_module, group, layer_i + 1);
             }
         }
     template<typename DEVICE, typename SPEC>
-    void load(DEVICE& device, nn_models::sequential::Module<SPEC>& model, HighFive::Group group, typename DEVICE::index_t layer_i = 0) {
+    void load(DEVICE& device, nn_models::sequential::ModuleForward<SPEC>& model, HighFive::Group group, typename DEVICE::index_t layer_i = 0) {
         if(layer_i == 0){
             group = group.getGroup("layers");
         }
         load(device, model.content, group.getGroup(std::to_string(layer_i)));
         if constexpr (!utils::typing::is_same_v<typename SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             load(device, model.next_module, group, layer_i + 1);
         }
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 #include "../../version.h"
 #if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_MODELS_SEQUENTIAL_PERSIST_CODE_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
 #define RL_TOOLS_NN_MODELS_SEQUENTIAL_PERSIST_CODE_H
 #include "../../containers/persist_code.h"
 #include "../../persist/code.h"
+#include "../../nn/persist_code.h"
 #include "model.h"
 
 #include <string>
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template<typename DEVICE, typename SPEC>
-    persist::Code save_code_split(DEVICE& device, nn_models::sequential::Module<SPEC>& model, std::string name, bool const_declaration=false, typename DEVICE::index_t indent = 0, typename DEVICE::index_t layer_i = 0) {
+    persist::Code save_code_split(DEVICE& device, nn_models::sequential::ModuleForward<SPEC>& model, std::string name, bool const_declaration=false, typename DEVICE::index_t indent = 0, typename DEVICE::index_t layer_i = 0) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         std::stringstream indent_ss;
         for(TI i=0; i < indent; i++){
             indent_ss << "    ";
         }
         std::string ind = indent_ss.str();
-        std::stringstream ss_header;
-        std::stringstream ss;
+        std::stringstream ss, ss_header;
+        auto layer_output = save_split(device, model.content, "layer_" + std::to_string(layer_i), const_declaration, indent+1);
+        ss_header << layer_output.header;
+        ss_header << "#include <rl_tools/nn_models/sequential/model.h>\n";
         if(layer_i == 0){
-            ss_header << "#include <rl_tools/nn_models/sequential/model.h>\n";
             ss << ind << "namespace " << name << " {\n";
         }
-        auto layer_output = save_split(device, model.content, "layer_" + std::to_string(layer_i), const_declaration, indent+1);
-        ss_header << layer_output.header;
         ss << layer_output.body;
         if constexpr(!utils::typing::is_same_v<typename SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
             auto downstream_output = save_code_split(device, model.next_module, name, const_declaration, indent, layer_i+1);
             ss_header << downstream_output.header;
             ss << downstream_output.body;
         }
         if(layer_i == 0){
             ss << ind << "    " << "namespace model_definition {\n";
-            ss << ind << "    " << "    " << "using namespace RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn_models::sequential::interface;\n";
-            ss << ind << "    " << "    " << "using MODEL = Module<";
+//            ss << ind << "    " << "    " << "using namespace RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn_models::sequential::interface;\n";
+//            std::string capability = "Forward";
+            ss << ind << "    " << "    " << "using CAPABILITY = " << to_string(typename SPEC::CAPABILITY{}) << "; \n";
+            ss << ind << "    " << "    " << "using IF = RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn_models::sequential::Interface<CAPABILITY>;\n";
+            ss << ind << "    " << "    " << "using MODEL = IF::Module<";
             for(TI layer_i = 0; layer_i < num_layers(model); layer_i++){
-                ss << "layer_" << layer_i << "::TYPE";
+                ss << "layer_" << layer_i << "::TEMPLATE";
                 if(layer_i < num_layers(model)-1){
-                    ss << ", Module<";
+                    ss << ", IF::Module<";
                 }
             }
             for(TI layer_i = 0; layer_i < num_layers(model); layer_i++){
                 ss << ">";
             }
             ss << ind << ";\n";
             ss << ind << "    " << "}\n";
@@ -52,25 +55,26 @@
             ss << ind << "    " << (const_declaration ? "const " : "") << "MODEL model = {";
             for(TI layer_i = 0; layer_i < num_layers(model); layer_i++){
                 ss << "layer_" << layer_i << "::layer";
                 if(layer_i < num_layers(model)-1){
                     ss << ", {";
                 }
             }
+            ss << ", {}";
             for(TI layer_i = 0; layer_i < num_layers(model); layer_i++){
                 ss << "}";
             }
             ss << ";\n";
 
 //            ss << ind << "    " << (const_declaration ? "const " : "") << "RL_TOOLS""_NAMESPACE_WRAPPER ::rl_tools::nn_models::sequential::Module<" << layer_i << "> module = {layer_0::container, " << get_type_string<typename SPEC::NEXT_MODULE>() << "::module, };\n";
             ss << ind << "}";
         }
         return {ss_header.str(), ss.str()};
     }
     template<typename DEVICE, typename SPEC>
-    std::string save_code(DEVICE& device, nn_models::sequential::Module<SPEC>& network, std::string name, bool const_declaration = false, typename DEVICE::index_t indent = 0) {
+    std::string save_code(DEVICE& device, nn_models::sequential::ModuleForward<SPEC>& network, std::string name, bool const_declaration = false, typename DEVICE::index_t indent = 0) {
         auto code = save_code_split(device, network, name, const_declaration, indent);
         return code.header + code.body;
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/uniform_random/model.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/random_uniform/model.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #include "../../version.h"
-#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_MODELS_UNIFORM_RANDOM_MODEL_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
+#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_MODELS_RANDOM_UNIFORM_MODEL_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
-#define RL_TOOLS_NN_MODELS_UNIFORM_RANDOM_MODEL_H
+#define RL_TOOLS_NN_MODELS_RANDOM_UNIFORM_MODEL_H
 RL_TOOLS_NAMESPACE_WRAPPER_START
 RL_TOOLS_NAMESPACE_WRAPPER_START
-namespace rl_tools::nn_models::uniform_random{
+namespace rl_tools::nn_models::random_uniform{
     enum class Range{
         MINUS_ONE_TO_ONE,
         ZERO_TO_ONE
     };
     template <typename T_T, typename T_TI, T_TI T_INPUT_DIM, T_TI T_OUTPUT_DIM, Range T_RANGE>
     struct Specification{
         using T = T_T;
@@ -18,20 +18,20 @@
         static constexpr Range RANGE = T_RANGE;
     };
     struct Buffer{};
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 namespace rl_tools::nn_models{
     template <typename T_SPEC>
-    struct UniformRandom{
+    struct RandomUniform{
         using SPEC = T_SPEC;
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         static constexpr TI INPUT_DIM = SPEC::INPUT_DIM;
         static constexpr TI OUTPUT_DIM = SPEC::OUTPUT_DIM;
 
         template <TI BATCH_SIZE=1>
-        using Buffer = typename rl_tools::nn_models::uniform_random::Buffer;
+        using Buffer = typename random_uniform::Buffer;
     };
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/nn_models/uniform_random/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/nn_models/random_uniform/operations_generic.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #include "../../version.h"
-#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_MODELS_UNIFORM_RANDOM_OPERATIONS_GENERIC_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
+#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_NN_MODELS_RANDOM_UNIFORM_OPERATIONS_GENERIC_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
-#define RL_TOOLS_NN_MODELS_UNIFORM_RANDOM_OPERATIONS_GENERIC_H
+#define RL_TOOLS_NN_MODELS_RANDOM_UNIFORM_OPERATIONS_GENERIC_H
 #include "model.h"
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template <typename DEVICE, typename SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC, typename RNG>
-    void evaluate(const DEVICE& device, nn_models::UniformRandom<SPEC>, Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, nn_models::uniform_random::Buffer, RNG& rng){
+    void evaluate(const DEVICE& device, nn_models::RandomUniform<SPEC>, Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output, nn_models::random_uniform::Buffer, RNG& rng){
         static_assert(SPEC::OUTPUT_DIM == OUTPUT_SPEC::COLS, "Output dimension mismatch");
         static_assert(SPEC::INPUT_DIM == INPUT_SPEC::COLS, "Input dimension mismatch");
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         for(TI row_i = 0; row_i < OUTPUT_SPEC::ROWS; row_i++){
             for(TI col_i = 0; col_i < OUTPUT_SPEC::COLS; col_i++){
                 T value = 0;
-                if(SPEC::RANGE == nn_models::uniform_random::Range::MINUS_ONE_TO_ONE){
+                if(SPEC::RANGE == nn_models::random_uniform::Range::MINUS_ONE_TO_ONE){
                     value = random::uniform_real_distribution(device.random, (T)-1, (T)1, rng);
-                }else if(SPEC::RANGE == nn_models::uniform_random::Range::ZERO_TO_ONE){
+                }else if(SPEC::RANGE == nn_models::random_uniform::Range::ZERO_TO_ONE){
                     value = random::uniform_real_distribution(device.random, (T)0, (T)1, rng);
                 }
                 set(output, row_i, col_i, value);
             }
         }
     }
 }
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/persist/code.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/persist/code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/random/operations_cpu.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/random/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/random/operations_cuda.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/random/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h`

 * *Files 2% similar despite different names*

```diff
@@ -61,22 +61,21 @@
             T previous_advantage = 0;
             for(TI step_forward_i = 0; step_forward_i < STEPS_PER_ENV; step_forward_i++){
                 TI step_backward_i = (STEPS_PER_ENV - 1 - step_forward_i);
                 TI pos = step_backward_i * OPR_SPEC::N_ENVIRONMENTS + env_i;
                 bool terminated = get(dataset.terminated, pos, 0);
                 bool truncated = get(dataset.truncated, pos, 0);
 #ifdef RL_TOOLS_DEBUG_RL_ALGORITHMS_PPO_GAE_CHECK_TERMINATED_TRUNCATED
-                utils::assert_exit(device, !terminated || terminated && truncated, "terminationn should imply truncation");
+                utils::assert_exit(device, !terminated || (terminated && truncated), "terminationn should imply truncation");
 #endif
                 T current_step_value = get(dataset.values, pos, 0);
-//                T next_step_value = terminated || truncated ? 0 : previous_value;
-                T next_step_value = terminated && !PPO_PARAMETERS::IGNORE_TERMINATION ? 0 : previous_value;
+                bool terminated_actual = terminated && !PPO_PARAMETERS::IGNORE_TERMINATION;
+                T next_step_value = terminated_actual ? 0 : previous_value;
 
                 T td_error = get(dataset.rewards, pos, 0) + PPO_PARAMETERS::GAMMA * next_step_value - current_step_value;
-//                previous_advantage = terminated || truncated ? 0 : previous_advantage;
                 if(truncated){
                     if(!terminated){ // e.g. time limited or random truncation
                         td_error = 0;
                     }
                     previous_advantage = 0;
                 }
                 T advantage = PPO_PARAMETERS::LAMBDA * PPO_PARAMETERS::GAMMA * previous_advantage + td_error;
@@ -153,15 +152,15 @@
                     for (TI batch_step_i = 0; batch_step_i < BATCH_SIZE; batch_step_i++) {
                         T advantage = get(batch_advantages, batch_step_i, 0);
                         advantage_mean += advantage;
                         advantage_std += advantage * advantage;
                     }
                     advantage_mean /= BATCH_SIZE;
                     advantage_std /= BATCH_SIZE;
-                    advantage_std = math::sqrt(device.math, advantage_std - advantage_mean * advantage_mean);
+                    advantage_std = math::sqrt(device.math, math::max(device.math, (T)0, advantage_std - advantage_mean * advantage_mean));
                 }
 //                add_scalar(device, device.logger, "ppo/advantage/mean", advantage_mean);
 //                add_scalar(device, device.logger, "ppo/advantage/std", advantage_std);
 
                 forward(device, ppo.actor, batch_observations, ppo_buffers.current_batch_actions, rng);
 //                auto abs_diff = abs_diff(device, batch_actions, dataset.actions);
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 #include "../../../../../rl/loop/loop.h"
 #include "state.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     namespace rl::algorithms::ppo::loop::core{
         // Config State (Init/Step)
-        using namespace nn_models::sequential::interface;
 
         struct ParametersTag{};
         template<typename T, typename TI, typename ENVIRONMENT>
         struct Parameters{
             using TAG = ParametersTag;
             using PPO_PARAMETERS = rl::algorithms::ppo::DefaultParameters<T, TI>;
             static constexpr TI STEP_LIMIT = 100;
@@ -37,25 +36,24 @@
             static constexpr TI BATCH_SIZE = ON_POLICY_RUNNER_STEPS_PER_ENV * N_ENVIRONMENTS;
 
             using OPTIMIZER_PARAMETERS = nn::optimizers::adam::DEFAULT_PARAMETERS_TENSORFLOW<T>;
         };
 
         template<typename T, typename TI, typename ENVIRONMENT, typename PARAMETERS>
         struct ConfigApproximatorsMLP{
-            using ACTOR_STRUCTURE_SPEC = nn_models::mlp::StructureSpecification<T, TI, ENVIRONMENT::OBSERVATION_DIM, ENVIRONMENT::ACTION_DIM, PARAMETERS::ACTOR_NUM_LAYERS, PARAMETERS::ACTOR_HIDDEN_DIM, PARAMETERS::ACTOR_ACTIVATION_FUNCTION, nn::activation_functions::IDENTITY, PARAMETERS::BATCH_SIZE>;
+            using ACTOR_SPEC = nn_models::mlp::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM, ENVIRONMENT::ACTION_DIM, PARAMETERS::ACTOR_NUM_LAYERS, PARAMETERS::ACTOR_HIDDEN_DIM, PARAMETERS::ACTOR_ACTIVATION_FUNCTION, nn::activation_functions::IDENTITY, PARAMETERS::BATCH_SIZE>;
             using ACTOR_OPTIMIZER_SPEC = nn::optimizers::adam::Specification<T, TI, typename PARAMETERS::OPTIMIZER_PARAMETERS>;
             using CRITIC_OPTIMIZER_SPEC = nn::optimizers::adam::Specification<T, TI, typename PARAMETERS::OPTIMIZER_PARAMETERS>;
             using ACTOR_OPTIMIZER = nn::optimizers::Adam<ACTOR_OPTIMIZER_SPEC>;
             using CRITIC_OPTIMIZER = nn::optimizers::Adam<CRITIC_OPTIMIZER_SPEC>;
-            using ACTOR_SPEC = nn_models::mlp::AdamSpecification<ACTOR_STRUCTURE_SPEC>;
-            using ACTOR_TYPE = nn_models::mlp_unconditional_stddev::NeuralNetworkAdam<ACTOR_SPEC>;
-            using ACTOR_TYPE_INFERENCE = nn_models::mlp_unconditional_stddev::NeuralNetwork<ACTOR_SPEC>;
-            using CRITIC_STRUCTURE_SPEC = nn_models::mlp::StructureSpecification<T, TI, ENVIRONMENT::OBSERVATION_DIM, 1, PARAMETERS::CRITIC_NUM_LAYERS, PARAMETERS::CRITIC_HIDDEN_DIM, PARAMETERS::CRITIC_ACTIVATION_FUNCTION, nn::activation_functions::IDENTITY, PARAMETERS::BATCH_SIZE>;
-            using CRITIC_SPEC = nn_models::mlp::AdamSpecification<CRITIC_STRUCTURE_SPEC>;
-            using CRITIC_TYPE = nn_models::mlp::NeuralNetworkAdam<CRITIC_SPEC>;
+            using CAPABILITY_ADAM = nn::layer_capability::Gradient<nn::parameters::Adam>;
+            using ACTOR_TYPE = nn_models::mlp_unconditional_stddev::NeuralNetwork<CAPABILITY_ADAM, ACTOR_SPEC>;
+            using ACTOR_TYPE_INFERENCE = nn_models::mlp_unconditional_stddev::NeuralNetwork<nn::layer_capability::Forward, ACTOR_SPEC>;
+            using CRITIC_SPEC = nn_models::mlp::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM, 1, PARAMETERS::CRITIC_NUM_LAYERS, PARAMETERS::CRITIC_HIDDEN_DIM, PARAMETERS::CRITIC_ACTIVATION_FUNCTION, nn::activation_functions::IDENTITY, PARAMETERS::BATCH_SIZE>;
+            using CRITIC_TYPE = nn_models::mlp::NeuralNetwork<CAPABILITY_ADAM, CRITIC_SPEC>;
         };
 
         struct ConfigTag{};
         template<typename T_T, typename T_TI, typename T_RNG, typename T_ENVIRONMENT, typename T_PARAMETERS = Parameters<T_T, T_TI, T_ENVIRONMENT>, template<typename, typename, typename, typename> class APPROXIMATOR_CONFIG=ConfigApproximatorsMLP>
         struct Config: rl::loop::Config{
             using TAG = ConfigTag;
             using T = T_T;
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #include "../../../../../version.h"
 #if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_RL_ALGORITHMS_PPO_LOOP_CORE_OPERATIONS_GENERIC_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
 #define RL_TOOLS_RL_ALGORITHMS_PPO_LOOP_CORE_OPERATIONS_GENERIC_H
 
+#include "../../../../../nn/optimizers/adam/operations_generic.h"
 #include "../../../../../rl/algorithms/sac/operations_generic.h"
 #include "../../../../../rl/algorithms/ppo/operations_generic.h"
 #include "../../../../../rl/components/on_policy_runner/operations_generic.h"
 #include "../../../../../rl/components/running_normalizer/operations_generic.h"
 
 #include "config.h"
 
@@ -46,17 +47,14 @@
 
         init(device, ts.on_policy_runner, ts.envs, ts.rng);
         init(device, ts.observation_normalizer);
         set_all(device, ts.observations_mean, 0);
         set_all(device, ts.observations_std, 1);
         init(device, ts.ppo, ts.actor_optimizer, ts.critic_optimizer, ts.rng);
 
-        init(device);
-        init(device, device.logger);
-
         ts.step = 0;
     }
 
     template <typename DEVICE, typename T_CONFIG>
     void free(DEVICE& device, rl::algorithms::ppo::loop::core::State<T_CONFIG>& ts){
         free(device, ts.ppo);
         free(device, ts.ppo_buffers);
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         sample_actions_critic(device, training_buffers, action_noise);
         copy(device, device, batch.next_observations_privileged, training_buffers.next_observations);
         evaluate(device, actor_critic.critic_target_1, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_1, critic_buffers, rng);
         evaluate(device, actor_critic.critic_target_2, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_2, critic_buffers, rng);
 
         target_actions(device, batch, training_buffers, actor_critic.log_alpha);
         forward(device, critic, batch.observations_and_actions, rng);
-        nn::loss_functions::mse::gradient(device, output(critic), training_buffers.target_action_value, training_buffers.d_output, 0.5);
+        nn::loss_functions::mse::gradient(device, output(critic), training_buffers.target_action_value, training_buffers.d_output, 0.5); // SB3/SBX uses 1/2, CleanRL doesn't
         backward(device, critic, batch.observations_and_actions, training_buffers.d_output, critic_buffers);
         step(device, optimizer, critic);
     }
     template <typename DEVICE, typename SPEC, typename CRITIC_TYPE, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename RNG>
     typename SPEC::T critic_loss(DEVICE& device, const rl::algorithms::sac::ActorCritic<SPEC>& actor_critic, CRITIC_TYPE& critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, typename SPEC::ACTOR_NETWORK_TYPE::template Buffers<BATCH_SIZE>& actor_buffers, typename CRITIC_TYPE::template Buffers<BATCH_SIZE>& critic_buffers, rl::algorithms::sac::CriticTrainingBuffers<SPEC>& training_buffers, RNG& rng) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
@@ -230,15 +230,15 @@
     RL_TOOLS_FUNCTION_PLACEMENT void sample_actions_actor_per_sample(DEVICE& device, Matrix<OUTPUT_SPEC>& output, rl::algorithms::sac::ActorTrainingBuffers<SPEC>& training_buffers, Matrix<ACTION_NOISE_SPEC>& action_noise, TI_SAMPLE batch_i) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         constexpr TI ACTION_DIM = SPEC::ENVIRONMENT::ACTION_DIM;
         for(TI action_i = 0; action_i < ACTION_DIM; action_i++){
             T log_std_pre_clip = get(output, batch_i, action_i + ACTION_DIM);
             T log_std_clip = math::clamp(device.math, log_std_pre_clip, (T)SPEC::PARAMETERS::ACTION_LOG_STD_LOWER_BOUND, (T)SPEC::PARAMETERS::ACTION_LOG_STD_UPPER_BOUND);
-            T std = math::exp(typename DEVICE::SPEC::MATH{}, log_std_pre_clip);
+            T std = math::exp(typename DEVICE::SPEC::MATH{}, log_std_clip);
             // action_sample = noise * std + mean
 //            T noise = random::normal_distribution::sample(typename DEVICE::SPEC::RANDOM{}, (T)0, (T)1, rng);
             T noise = get(action_noise, batch_i, action_i);
             set(training_buffers.action_noise, batch_i, action_i, noise);
             T action_sample = get(output, batch_i, action_i) + std * noise;
             set(training_buffers.action_sample, batch_i, action_i, action_sample);
             T action = math::tanh(typename DEVICE::SPEC::MATH{}, action_sample);
@@ -284,15 +284,15 @@
         bool critic_1_value = get(critic_1_output, batch_i, 0) < get(critic_2_output, batch_i, 0);
         T entropy = 0;
         for(TI action_i = 0; action_i < ACTION_DIM; action_i++){
             T action = get(training_buffers.actions, batch_i, action_i); // tanh(action_sample)
             T d_mu = 0;
             T d_std = 0;
             {
-                T d_input = 0;
+                T d_input = 0; // note this d_input is already taking into account the mean of the batch (d_output is -1/BATCH_SIZE for the backward pass of the critics)
                 if(critic_1_value) {
                     d_input = get(training_buffers.d_critic_1_input, batch_i, SPEC::CRITIC_NETWORK_TYPE::INPUT_DIM - ACTION_DIM + action_i);
                 }
                 else{
                     d_input = get(training_buffers.d_critic_2_input, batch_i, SPEC::CRITIC_NETWORK_TYPE::INPUT_DIM - ACTION_DIM + action_i);
                 }
                 T d_tanh_pre_activation = d_input * (1-action*action);
@@ -390,29 +390,29 @@
         auto& critic = actor_critic.critic_1;
         evaluate(device, critic, training_buffers.state_action_value_input, training_buffers.state_action_value, critic_buffers, rng);
         return mean(device, training_buffers.state_action_value);
     }
 
     namespace rl::algorithms::sac{
         template<typename DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
-        void update_target_layer(DEVICE& device, const  nn::layers::dense::Layer<SOURCE_SPEC>& source, nn::layers::dense::Layer<TARGET_SPEC>& target, typename SOURCE_SPEC::T polyak) {
+        void update_target_layer(DEVICE& device, const  nn::layers::dense::LayerForward<SOURCE_SPEC>& source, nn::layers::dense::LayerForward<TARGET_SPEC>& target, typename SOURCE_SPEC::T polyak) {
             rl_tools::utils::polyak::update(device, source.weights.parameters, target.weights.parameters, polyak);
             rl_tools::utils::polyak::update(device, source.biases.parameters , target.biases.parameters , polyak);
         }
         template<typename T, typename DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
-        void update_target_network(DEVICE& device, const  nn_models::mlp::NeuralNetwork<SOURCE_SPEC>& source, nn_models::mlp::NeuralNetwork<TARGET_SPEC>& target, T polyak) {
-            using TargetNetworkType = nn_models::mlp::NeuralNetwork<TARGET_SPEC>;
+        void update_target_network(DEVICE& device, const  nn_models::mlp::NeuralNetworkForward<SOURCE_SPEC>& source, nn_models::mlp::NeuralNetworkForward<TARGET_SPEC>& target, T polyak) {
+            using TargetNetworkType = nn_models::mlp::NeuralNetworkForward<TARGET_SPEC>;
             update_target_layer(device, source.input_layer, target.input_layer, polyak);
             for(typename DEVICE::index_t layer_i=0; layer_i < TargetNetworkType::NUM_HIDDEN_LAYERS; layer_i++){
                 update_target_layer(device, source.hidden_layers[layer_i], target.hidden_layers[layer_i], polyak);
             }
             update_target_layer(device, source.output_layer, target.output_layer, polyak);
         }
         template<typename T, typename DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
-        void update_target_network(DEVICE& device, const  nn_models::sequential::Module<SOURCE_SPEC>& source, nn_models::sequential::Module<TARGET_SPEC>& target, T polyak) {
+        void update_target_network(DEVICE& device, const  nn_models::sequential::ModuleForward<SOURCE_SPEC>& source, nn_models::sequential::ModuleForward<TARGET_SPEC>& target, T polyak) {
             update_target_layer(device, source.content, target.content, polyak);
             if constexpr(!rl_tools::utils::typing::is_same_v<typename SOURCE_SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
                 update_target_network(device, source.next_module, target.next_module, polyak);
             }
         }
     }
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,144 +1,146 @@
 #include "../../../../../version.h"
-#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_RL_ALGORITHMS_SAC_LOOP_CORE_CONFIG_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
+#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_RL_ALGORITHMS_TD3_LOOP_CORE_CONFIG_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
-#define RL_TOOLS_RL_ALGORITHMS_SAC_LOOP_CORE_CONFIG_H
+#define RL_TOOLS_RL_ALGORITHMS_TD3_LOOP_CORE_CONFIG_H
 
 #include "../../../../../nn_models/sequential/model.h"
 #include "../../../../../nn_models/mlp/network.h"
-#include "../../../../../nn_models/uniform_random/model.h"
-#include "../../../../../rl/algorithms/sac/sac.h"
+#include "../../../../../nn_models/random_uniform/model.h"
+#include "../../../../../rl/algorithms/td3/td3.h"
 #include "../../../../../nn/optimizers/adam/adam.h"
 #include "state.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
-namespace rl_tools::rl::algorithms::sac::loop::core{
+namespace rl_tools::rl::algorithms::td3::loop::core{
     // Config State (Init/Step)
-    using namespace nn_models::sequential::interface;
 
     template<typename T, typename TI, typename ENVIRONMENT>
     struct DefaultParameters{
-        using SAC_PARAMETERS = rl::algorithms::sac::DefaultParameters<T, TI, ENVIRONMENT::ACTION_DIM>;
+        using TD3_PARAMETERS = rl::algorithms::td3::DefaultParameters<T, TI>;
         static constexpr TI N_ENVIRONMENTS = 1;
-        static constexpr TI N_WARMUP_STEPS = 100;
-        static_assert(N_WARMUP_STEPS >= SAC_PARAMETERS::ACTOR_BATCH_SIZE);
+        static constexpr TI N_WARMUP_STEPS = TD3_PARAMETERS::ACTOR_BATCH_SIZE;
         static constexpr TI STEP_LIMIT = 10000;
         static constexpr TI REPLAY_BUFFER_CAP = STEP_LIMIT; // Note: when inheriting from this class for overwriting the default STEP_LIMIT you need to set the REPLAY_BUFFER_CAP as well otherwise it will be the default step limit
         static constexpr TI EPISODE_STEP_LIMIT = 200;
 
         static constexpr TI ACTOR_HIDDEN_DIM = 64;
         static constexpr TI ACTOR_NUM_LAYERS = 3;
         static constexpr auto ACTOR_ACTIVATION_FUNCTION = nn::activation_functions::ActivationFunction::RELU;
         static constexpr TI CRITIC_HIDDEN_DIM = 64;
         static constexpr TI CRITIC_NUM_LAYERS = 3;
         static constexpr auto CRITIC_ACTIVATION_FUNCTION = nn::activation_functions::ActivationFunction::RELU;
 
         static constexpr bool COLLECT_EPISODE_STATS = true;
         static constexpr TI EPISODE_STATS_BUFFER_SIZE = 1000;
 
+        static constexpr T EXPLORATION_NOISE = 0.1;
+        static constexpr bool SHARED_BATCH = true;
+
         using OPTIMIZER_PARAMETERS = nn::optimizers::adam::DEFAULT_PARAMETERS_TENSORFLOW<T>;
     };
 
     // The approximator config sets up any types that support the usual rl_tools::forward and rl_tools::backward operations (can be custom as well)
     // We provide approximators based on the sequential and mlp models. The latter (mlp) allows for a variable number of layers, but is restricted to a uniform hidden layer size while the former allows for arbitrary layers to be combined in a sequential manner. Both support compile-time autodiff
-    template<typename T, typename TI, typename ENVIRONMENT, typename PARAMETERS, typename CONTAINER_TYPE_TAG>
+    template<typename T, typename TI, typename ENVIRONMENT, typename PARAMETERS>
     struct ConfigApproximatorsSequential{
-        template <typename PARAMETER_TYPE, template<typename> class LAYER_TYPE = nn::layers::dense::LayerBackwardGradient>
+        template <typename CAPABILITY>
         struct ACTOR{
             static constexpr TI HIDDEN_DIM = PARAMETERS::ACTOR_HIDDEN_DIM;
-            static constexpr TI BATCH_SIZE = PARAMETERS::SAC_PARAMETERS::ACTOR_BATCH_SIZE;
+            static constexpr TI BATCH_SIZE = PARAMETERS::TD3_PARAMETERS::ACTOR_BATCH_SIZE;
             static constexpr auto ACTIVATION_FUNCTION = PARAMETERS::ACTOR_ACTIVATION_FUNCTION;
-            using LAYER_1_SPEC = nn::layers::dense::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, PARAMETER_TYPE, BATCH_SIZE, nn::parameters::groups::Input, CONTAINER_TYPE_TAG>;
-            using LAYER_1 = LAYER_TYPE<LAYER_1_SPEC>;
-            using LAYER_2_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, PARAMETER_TYPE, BATCH_SIZE, nn::parameters::groups::Normal, CONTAINER_TYPE_TAG>;
-            using LAYER_2 = LAYER_TYPE<LAYER_2_SPEC>;
-            static constexpr TI ACTOR_OUTPUT_DIM = ENVIRONMENT::ACTION_DIM * 2; // to express mean and log_std for each action
-            using LAYER_3_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, ACTOR_OUTPUT_DIM, nn::activation_functions::ActivationFunction::IDENTITY, PARAMETER_TYPE, BATCH_SIZE, nn::parameters::groups::Output, CONTAINER_TYPE_TAG>; // note the output activation should be identity because we want to sample from a gaussian and then squash afterwards (taking into account the squashing in the distribution)
-            using LAYER_3 = LAYER_TYPE<LAYER_3_SPEC>;
+            using LAYER_1_SPEC = nn::layers::dense::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, BATCH_SIZE>;
+            using LAYER_1 = nn::layers::dense::BindSpecification<LAYER_1_SPEC>;
+            using LAYER_2_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, BATCH_SIZE>;
+            using LAYER_2 = nn::layers::dense::BindSpecification<LAYER_2_SPEC>;
+            static constexpr TI ACTOR_OUTPUT_DIM = ENVIRONMENT::ACTION_DIM;
+            using LAYER_3_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, ACTOR_OUTPUT_DIM, nn::activation_functions::ActivationFunction::TANH, BATCH_SIZE>;
+            using LAYER_3 = nn::layers::dense::BindSpecification<LAYER_3_SPEC>;
 
-            using MODEL = Module<LAYER_1, Module<LAYER_2, Module<LAYER_3>>>;
+            using IF = nn_models::sequential::Interface<CAPABILITY>;
+            using MODEL = typename IF::template Module<LAYER_1::template Layer, typename IF::template Module<LAYER_2::template Layer, typename IF::template Module<LAYER_3::template Layer>>>;
         };
 
-        template <typename PARAMETER_TYPE, template<typename> class LAYER_TYPE = nn::layers::dense::LayerBackwardGradient>
+        template <typename CAPABILITY>
         struct CRITIC{
             static constexpr TI HIDDEN_DIM = PARAMETERS::CRITIC_HIDDEN_DIM;
-            static constexpr TI BATCH_SIZE = PARAMETERS::SAC_PARAMETERS::CRITIC_BATCH_SIZE;
+            static constexpr TI BATCH_SIZE = PARAMETERS::TD3_PARAMETERS::CRITIC_BATCH_SIZE;
             static constexpr auto ACTIVATION_FUNCTION = PARAMETERS::CRITIC_ACTIVATION_FUNCTION;
 
-            using LAYER_1_SPEC = nn::layers::dense::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM + ENVIRONMENT::ACTION_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, PARAMETER_TYPE, BATCH_SIZE, nn::parameters::groups::Input, CONTAINER_TYPE_TAG>;
-            using LAYER_1 = LAYER_TYPE<LAYER_1_SPEC>;
-            using LAYER_2_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, PARAMETER_TYPE, BATCH_SIZE, nn::parameters::groups::Normal, CONTAINER_TYPE_TAG>;
-            using LAYER_2 = LAYER_TYPE<LAYER_2_SPEC>;
-            using LAYER_3_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, 1, nn::activation_functions::ActivationFunction::IDENTITY, PARAMETER_TYPE, BATCH_SIZE, nn::parameters::groups::Output, CONTAINER_TYPE_TAG>;
-            using LAYER_3 = LAYER_TYPE<LAYER_3_SPEC>;
+            using LAYER_1_SPEC = nn::layers::dense::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM + ENVIRONMENT::ACTION_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, BATCH_SIZE>;
+            using LAYER_1 = nn::layers::dense::BindSpecification<LAYER_1_SPEC>;
+            using LAYER_2_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, BATCH_SIZE>;
+            using LAYER_2 = nn::layers::dense::BindSpecification<LAYER_2_SPEC>;
+            using LAYER_3_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, 1, nn::activation_functions::ActivationFunction::IDENTITY, BATCH_SIZE>;
+            using LAYER_3 = nn::layers::dense::BindSpecification<LAYER_3_SPEC>;
 
-            using MODEL = Module<LAYER_1, Module<LAYER_2, Module<LAYER_3>>>;
+            using IF = nn_models::sequential::Interface<CAPABILITY>;
+            using MODEL = typename IF::template Module<LAYER_1::template Layer, typename IF::template Module<LAYER_2::template Layer, typename IF::template Module<LAYER_3::template Layer>>>;
         };
 
         using OPTIMIZER_SPEC = nn::optimizers::adam::Specification<T, TI, typename PARAMETERS::OPTIMIZER_PARAMETERS>;
 
         using OPTIMIZER = nn::optimizers::Adam<OPTIMIZER_SPEC>;
 
-        using ACTOR_TYPE = typename ACTOR<nn::parameters::Adam>::MODEL;
-        using CRITIC_TYPE = typename CRITIC<nn::parameters::Adam>::MODEL;
-        using CRITIC_TARGET_TYPE = typename CRITIC<nn::parameters::Plain, nn::layers::dense::Layer>::MODEL;
+        using ACTOR_TYPE = typename ACTOR<nn::layer_capability::Gradient<nn::parameters::Adam>>::MODEL;
+        using ACTOR_TARGET_TYPE = typename ACTOR<nn::layer_capability::Forward>::MODEL;
+        using CRITIC_TYPE = typename CRITIC<nn::layer_capability::Gradient<nn::parameters::Adam>>::MODEL;
+        using CRITIC_TARGET_TYPE = typename CRITIC<nn::layer_capability::Forward>::MODEL;
     };
 
-    template<typename T, typename TI, typename ENVIRONMENT, typename PARAMETERS, typename T_CONTAINER_TYPE_TAG>
+    template<typename T, typename TI, typename ENVIRONMENT, typename PARAMETERS>
     struct ConfigApproximatorsMLP{
-        using CONTAINER_TYPE_TAG = T_CONTAINER_TYPE_TAG;
-        using ACTOR_STRUCTURE_SPEC = nn_models::mlp::StructureSpecification<T, TI, ENVIRONMENT::OBSERVATION_DIM, 2*ENVIRONMENT::ACTION_DIM, PARAMETERS::ACTOR_NUM_LAYERS, PARAMETERS::ACTOR_HIDDEN_DIM, PARAMETERS::ACTOR_ACTIVATION_FUNCTION, nn::activation_functions::TANH, PARAMETERS::SAC_PARAMETERS::ACTOR_BATCH_SIZE, CONTAINER_TYPE_TAG>;
-        using CRITIC_STRUCTURE_SPEC = nn_models::mlp::StructureSpecification<T, TI, ENVIRONMENT::OBSERVATION_DIM + ENVIRONMENT::ACTION_DIM, 1, PARAMETERS::CRITIC_NUM_LAYERS, PARAMETERS::CRITIC_HIDDEN_DIM, PARAMETERS::CRITIC_ACTIVATION_FUNCTION, nn::activation_functions::IDENTITY, PARAMETERS::SAC_PARAMETERS::CRITIC_BATCH_SIZE, CONTAINER_TYPE_TAG>;
+        using ACTOR_SPEC = nn_models::mlp::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM, ENVIRONMENT::ACTION_DIM, PARAMETERS::ACTOR_NUM_LAYERS, PARAMETERS::ACTOR_HIDDEN_DIM, PARAMETERS::ACTOR_ACTIVATION_FUNCTION, nn::activation_functions::TANH, PARAMETERS::TD3_PARAMETERS::ACTOR_BATCH_SIZE>;
+        using CRITIC_SPEC = nn_models::mlp::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM + ENVIRONMENT::ACTION_DIM, 1, PARAMETERS::CRITIC_NUM_LAYERS, PARAMETERS::CRITIC_HIDDEN_DIM, PARAMETERS::CRITIC_ACTIVATION_FUNCTION, nn::activation_functions::IDENTITY, PARAMETERS::TD3_PARAMETERS::CRITIC_BATCH_SIZE>;
         using OPTIMIZER_SPEC = typename nn::optimizers::adam::Specification<T, TI, typename PARAMETERS::OPTIMIZER_PARAMETERS>;
         using OPTIMIZER = nn::optimizers::Adam<OPTIMIZER_SPEC>;
-        using ACTOR_SPEC = nn_models::mlp::AdamSpecification<ACTOR_STRUCTURE_SPEC>;
-        using ACTOR_TYPE = nn_models::mlp::NeuralNetworkAdam<ACTOR_SPEC>;
 
-        using CRITIC_SPEC = nn_models::mlp::AdamSpecification<CRITIC_STRUCTURE_SPEC>;
-        using CRITIC_TYPE = nn_models::mlp::NeuralNetworkAdam<CRITIC_SPEC>;
+        using CAPABILITY_LEARNING = nn::layer_capability::Gradient<nn::parameters::Adam>;
+        using ACTOR_TYPE = nn_models::mlp::NeuralNetwork<CAPABILITY_LEARNING, ACTOR_SPEC>;
+        using ACTOR_TARGET_TYPE = typename ACTOR_TYPE::template CHANGE_CAPABILITY<nn::layer_capability::Forward>; //nn_models::mlp::NeuralNetwork<nn::layer_capability::Forward, ACTOR_SPEC>; // todo: replace with something like: ACTOR_TYPE::CHANGE_CAPABILITY<nn::layer_capability::Forward>
 
-        using CRITIC_TARGET_SPEC = nn_models::mlp::InferenceSpecification<CRITIC_STRUCTURE_SPEC>;
-        using CRITIC_TARGET_TYPE = nn_models::mlp::NeuralNetwork<CRITIC_TARGET_SPEC>;
+        using CRITIC_TYPE = nn_models::mlp::NeuralNetwork<CAPABILITY_LEARNING, CRITIC_SPEC>;
+        using CRITIC_TARGET_TYPE = typename CRITIC_TYPE::template CHANGE_CAPABILITY<nn::layer_capability::Forward>; //nn_models::mlp::NeuralNetwork<nn::layer_capability::Forward, CRITIC_SPEC>;
     };
 
-    template<typename T_T, typename T_TI, typename T_RNG, typename T_ENVIRONMENT, typename T_PARAMETERS = DefaultParameters<T_T, T_TI, T_ENVIRONMENT>, template<typename, typename, typename, typename, typename> class APPROXIMATOR_CONFIG=ConfigApproximatorsSequential, typename T_CONTAINER_TYPE_TAG = MatrixDynamicTag>
+    template<typename T_T, typename T_TI, typename T_RNG, typename T_ENVIRONMENT, typename T_PARAMETERS = DefaultParameters<T_T, T_TI, T_ENVIRONMENT>, template<typename, typename, typename, typename> class APPROXIMATOR_CONFIG=ConfigApproximatorsMLP>
     struct Config{
         using T = T_T;
         using TI = T_TI;
         using RNG = T_RNG;
         using ENVIRONMENT = T_ENVIRONMENT;
         using ENVIRONMENT_EVALUATION = T_ENVIRONMENT;
-        using CORE_PARAMETERS = T_PARAMETERS;
-        using CONTAINER_TYPE_TAG = T_CONTAINER_TYPE_TAG;
 
-        using NN = APPROXIMATOR_CONFIG<T, TI, T_ENVIRONMENT, CORE_PARAMETERS, CONTAINER_TYPE_TAG>;
+        using NN = APPROXIMATOR_CONFIG<T, TI, T_ENVIRONMENT, T_PARAMETERS>;
 //        using NN = ConfigApproximatorsMLP<T, TI, T_ENVIRONMENT, T_PARAMETERS>;
 
-        using EXPLORATION_POLICY_SPEC = nn_models::uniform_random::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM, ENVIRONMENT::ACTION_DIM, nn_models::uniform_random::Range::MINUS_ONE_TO_ONE>;
-        using EXPLORATION_POLICY = nn_models::UniformRandom<EXPLORATION_POLICY_SPEC>;
+        using CORE_PARAMETERS = T_PARAMETERS;
 
-        using ALPHA_PARAMETER_TYPE = nn::parameters::Adam;
-        using ALPHA_OPTIMIZER = nn::optimizers::Adam<typename NN::OPTIMIZER_SPEC>;
+        using EXPLORATION_POLICY_SPEC = nn_models::random_uniform::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM, ENVIRONMENT::ACTION_DIM, nn_models::random_uniform::Range::MINUS_ONE_TO_ONE>;
+        using EXPLORATION_POLICY = nn_models::RandomUniform<EXPLORATION_POLICY_SPEC>;
 
-        using ACTOR_CRITIC_SPEC = rl::algorithms::sac::Specification<T, TI, ENVIRONMENT, typename NN::ACTOR_TYPE, typename NN::CRITIC_TYPE, typename NN::CRITIC_TARGET_TYPE, ALPHA_PARAMETER_TYPE, typename NN::OPTIMIZER, typename NN::OPTIMIZER, ALPHA_OPTIMIZER, typename CORE_PARAMETERS::SAC_PARAMETERS, CONTAINER_TYPE_TAG>;
-        using ACTOR_CRITIC_TYPE = rl::algorithms::sac::ActorCritic<ACTOR_CRITIC_SPEC>;
+        using ACTOR_CRITIC_SPEC = rl::algorithms::td3::Specification<T, TI, ENVIRONMENT, typename NN::ACTOR_TYPE, typename NN::ACTOR_TARGET_TYPE, typename NN::CRITIC_TYPE, typename NN::CRITIC_TARGET_TYPE, typename NN::OPTIMIZER, typename CORE_PARAMETERS::TD3_PARAMETERS>;
+        using ACTOR_CRITIC_TYPE = rl::algorithms::td3::ActorCritic<ACTOR_CRITIC_SPEC>;
+
+        struct OFF_POLICY_RUNNER_PARAMETERS{
+            static constexpr TI N_ENVIRONMENTS = CORE_PARAMETERS::N_ENVIRONMENTS;
+            static constexpr bool ASYMMETRIC_OBSERVATIONS = false;
+            static constexpr TI REPLAY_BUFFER_CAPACITY = CORE_PARAMETERS::REPLAY_BUFFER_CAP;
+            static constexpr TI EPISODE_STEP_LIMIT = CORE_PARAMETERS::EPISODE_STEP_LIMIT;
+            static constexpr bool STOCHASTIC_POLICY = false;
+            static constexpr bool COLLECT_EPISODE_STATS = CORE_PARAMETERS::COLLECT_EPISODE_STATS;
+            static constexpr TI EPISODE_STATS_BUFFER_SIZE = CORE_PARAMETERS::EPISODE_STATS_BUFFER_SIZE;
+            static constexpr T EXPLORATION_NOISE = CORE_PARAMETERS::EXPLORATION_NOISE;
+        };
 
-        static constexpr bool STOCHASTIC_POLICY = true;
         using OFF_POLICY_RUNNER_SPEC = rl::components::off_policy_runner::Specification<
                 T,
                 TI,
                 ENVIRONMENT,
-                CORE_PARAMETERS::N_ENVIRONMENTS,
-                false,
-                CORE_PARAMETERS::REPLAY_BUFFER_CAP,
-                CORE_PARAMETERS::EPISODE_STEP_LIMIT,
-                STOCHASTIC_POLICY,
-                CORE_PARAMETERS::COLLECT_EPISODE_STATS,
-                CORE_PARAMETERS::EPISODE_STATS_BUFFER_SIZE,
-                CONTAINER_TYPE_TAG
+                OFF_POLICY_RUNNER_PARAMETERS
         >;
         static_assert(ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::ACTOR_BATCH_SIZE == ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::CRITIC_BATCH_SIZE);
         template <typename CONFIG>
         using State = State<CONFIG>;
     };
 }
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 #include "../../../../../version.h"
 #if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_RL_ALGORITHMS_SAC_LOOP_CORE_OPERATIONS_GENERIC_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
 #define RL_TOOLS_RL_ALGORITHMS_SAC_LOOP_CORE_OPERATIONS_GENERIC_H
 
 #include "../../../../../nn_models/operations_generic.h"
-#include "../../../../../nn_models/uniform_random/operations_generic.h"
+#include "../../../../../nn_models/random_uniform/operations_generic.h"
 #include "../../../../../rl/algorithms/sac/operations_generic.h"
+#include "../../../../../nn/optimizers/adam/operations_generic.h"
 #include "../../../../../rl/components/off_policy_runner/operations_generic.h"
 #include "../../../../../rl/utils/evaluation.h"
 
 #include "config.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template <typename DEVICE, typename T_CONFIG>
     void malloc(DEVICE& device, rl::algorithms::sac::loop::core::State<T_CONFIG>& ts, typename T_CONFIG::TI seed = 0){
         malloc(device, ts.actor_critic);
         malloc(device, ts.off_policy_runner);
-        malloc(device, ts.critic_batch[0]);
-        malloc(device, ts.critic_batch[1]);
+        malloc(device, ts.critic_batch);
         malloc(device, ts.critic_training_buffers[0]);
         malloc(device, ts.critic_training_buffers[1]);
-        malloc(device, ts.action_noise_critic[0]);
-        malloc(device, ts.action_noise_critic[1]);
+        malloc(device, ts.action_noise_critic);
         malloc(device, ts.critic_buffers[0]);
         malloc(device, ts.critic_buffers[1]);
         malloc(device, ts.actor_batch);
         malloc(device, ts.actor_training_buffers);
         malloc(device, ts.action_noise_actor);
         malloc(device, ts.actor_buffers_eval);
         malloc(device, ts.actor_buffers[0]);
@@ -55,54 +54,46 @@
 
         init(device, ts.off_policy_runner, ts.envs);
 
 
         set_all(device, ts.observations_mean, 0);
         set_all(device, ts.observations_std, 1);
 
-        ts.off_policy_runner.parameters = rl::components::off_policy_runner::default_parameters<T>;
-
-        init(device);
-        init(device, device.logger);
-
         ts.step = 0;
     }
     template <typename DEVICE_SOURCE, typename DEVICE_TARGET, typename T_CONFIG_SOURCE, typename T_CONFIG_TARGET>
     void copy(DEVICE_SOURCE& device_source, DEVICE_TARGET& device_target, rl::algorithms::sac::loop::core::State<T_CONFIG_SOURCE>& source, rl::algorithms::sac::loop::core::State<T_CONFIG_TARGET>& target){
         copy(device_source, device_target, source.actor_critic, target.actor_critic);
         copy(device_source, device_target, source.off_policy_runner, target.off_policy_runner);
-        copy(device_source, device_target, source.critic_batch[0], target.critic_batch[0]);
-        copy(device_source, device_target, source.critic_batch[1], target.critic_batch[1]);
+        copy(device_source, device_target, source.critic_batch, target.critic_batch);
         copy(device_source, device_target, source.critic_training_buffers[0], target.critic_training_buffers[0]);
         copy(device_source, device_target, source.critic_training_buffers[1], target.critic_training_buffers[1]);
         copy(device_source, device_target, source.critic_buffers[0], target.critic_buffers[0]);
         copy(device_source, device_target, source.critic_buffers[1], target.critic_buffers[1]);
         copy(device_source, device_target, source.actor_batch, target.actor_batch);
         copy(device_source, device_target, source.actor_training_buffers, target.actor_training_buffers);
         copy(device_source, device_target, source.actor_buffers_eval, target.actor_buffers_eval);
         copy(device_source, device_target, source.actor_buffers[0], target.actor_buffers[0]);
         copy(device_source, device_target, source.actor_buffers[1], target.actor_buffers[1]);
         copy(device_source, device_target, source.observations_mean, target.observations_mean);
         copy(device_source, device_target, source.observations_std, target.observations_std);
         copy(device_source, device_target, source.actor_deterministic_evaluation_buffers, target.actor_deterministic_evaluation_buffers);
 //        target.rng = source.rng;
-        target.off_policy_runner.parameters = source.off_policy_runner.parameters;
+        target.off_policy_runner.parameters.exploration_noise = source.off_policy_runner.parameters.exploration_noise;
         target.step = source.step;
     }
 
     template <typename DEVICE, typename T_CONFIG>
     void free(DEVICE& device, rl::algorithms::sac::loop::core::State<T_CONFIG>& ts){
         free(device, ts.actor_critic);
         free(device, ts.off_policy_runner);
-        free(device, ts.critic_batch[0]);
-        free(device, ts.critic_batch[1]);
+        free(device, ts.critic_batch);
         free(device, ts.critic_training_buffers[0]);
         free(device, ts.critic_training_buffers[1]);
-        free(device, ts.action_noise_critic[0]);
-        free(device, ts.action_noise_critic[1]);
+        free(device, ts.action_noise_critic);
         free(device, ts.critic_buffers[0]);
         free(device, ts.critic_buffers[1]);
         free(device, ts.actor_batch);
         free(device, ts.actor_training_buffers);
         free(device, ts.action_noise_actor);
         free(device, ts.actor_buffers_eval);
         free(device, ts.actor_buffers[0]);
@@ -125,25 +116,36 @@
         }
         else{
             typename CONFIG::EXPLORATION_POLICY exploration_policy;
             typename CONFIG::EXPLORATION_POLICY::template Buffer<> exploration_policy_buffer;
             step(device, ts.off_policy_runner, exploration_policy, exploration_policy_buffer, ts.rng);
         }
         if(ts.step >= CONFIG::CORE_PARAMETERS::N_WARMUP_STEPS){
+            if constexpr(CONFIG::CORE_PARAMETERS::SHARED_BATCH){
+                gather_batch(device, ts.off_policy_runner, ts.critic_batch, ts.rng);
+                randn(device, ts.action_noise_critic, ts.rng);
+            }
             if(ts.step % CONFIG::CORE_PARAMETERS::SAC_PARAMETERS::CRITIC_TRAINING_INTERVAL == 0){
                 for(int critic_i = 0; critic_i < 2; critic_i++){
-                    gather_batch(device, ts.off_policy_runner, ts.critic_batch[critic_i], ts.rng);
-                    randn(device, ts.action_noise_critic[critic_i], ts.rng);
-                    train_critic(device, ts.actor_critic, critic_i == 0 ? ts.actor_critic.critic_1 : ts.actor_critic.critic_2, ts.critic_batch[critic_i], ts.critic_optimizers[critic_i], ts.actor_buffers[critic_i], ts.critic_buffers[critic_i], ts.critic_training_buffers[critic_i], ts.action_noise_critic[critic_i], ts.rng);
+                    if constexpr(!CONFIG::CORE_PARAMETERS::SHARED_BATCH) {
+                        gather_batch(device, ts.off_policy_runner, ts.critic_batch, ts.rng);
+                        randn(device, ts.action_noise_critic, ts.rng);
+                    }
+                    train_critic(device, ts.actor_critic, critic_i == 0 ? ts.actor_critic.critic_1 : ts.actor_critic.critic_2, ts.critic_batch, ts.critic_optimizers[critic_i], ts.actor_buffers[critic_i], ts.critic_buffers[critic_i], ts.critic_training_buffers[critic_i], ts.action_noise_critic, ts.rng);
                 }
             }
             if(ts.step % CONFIG::CORE_PARAMETERS::SAC_PARAMETERS::ACTOR_TRAINING_INTERVAL == 0){
-                gather_batch(device, ts.off_policy_runner, ts.actor_batch, ts.rng);
                 randn(device, ts.action_noise_actor, ts.rng);
-                train_actor(device, ts.actor_critic, ts.actor_batch, ts.actor_optimizer, ts.actor_buffers[0], ts.critic_buffers[0], ts.actor_training_buffers, ts.action_noise_actor, ts.rng);
+                if constexpr(CONFIG::CORE_PARAMETERS::SHARED_BATCH){
+                    train_actor(device, ts.actor_critic, ts.critic_batch, ts.actor_optimizer, ts.actor_buffers[0], ts.critic_buffers[0], ts.actor_training_buffers, ts.action_noise_actor, ts.rng);
+                }
+                else{
+                    gather_batch(device, ts.off_policy_runner, ts.actor_batch, ts.rng);
+                    train_actor(device, ts.actor_critic, ts.actor_batch, ts.actor_optimizer, ts.actor_buffers[0], ts.critic_buffers[0], ts.actor_training_buffers, ts.action_noise_actor, ts.rng);
+                }
                 update_critic_targets(device, ts.actor_critic);
             }
         }
         ts.step++;
         if(ts.step > CONFIG::CORE_PARAMETERS::STEP_LIMIT){
             return true;
         }
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h`

 * *Files 7% similar despite different names*

```diff
@@ -20,24 +20,24 @@
             using CONTAINER_TYPE = typename CONFIG::CONTAINER_TYPE_TAG::template type<SPEC>;
             typename CONFIG::NN::OPTIMIZER actor_optimizer, critic_optimizers[2];
             typename CONFIG::RNG rng;
             rl::components::OffPolicyRunner<typename CONFIG::OFF_POLICY_RUNNER_SPEC> off_policy_runner;
             typename CONFIG::ENVIRONMENT envs[decltype(off_policy_runner)::N_ENVIRONMENTS];
             typename CONFIG::ACTOR_CRITIC_TYPE actor_critic;
             typename CONFIG::NN::ACTOR_TYPE::template Buffer<1> actor_deterministic_evaluation_buffers;
-            rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<typename decltype(off_policy_runner)::SPEC, CONFIG::ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::CRITIC_BATCH_SIZE>> critic_batch[2];
+            rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<typename decltype(off_policy_runner)::SPEC, CONFIG::ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::CRITIC_BATCH_SIZE>> critic_batch;
             rl::algorithms::sac::CriticTrainingBuffers<typename CONFIG::ACTOR_CRITIC_SPEC> critic_training_buffers[2];
-            CONTAINER_TYPE<matrix::Specification<T, TI, CONFIG::CORE_PARAMETERS::SAC_PARAMETERS::CRITIC_BATCH_SIZE, CONFIG::ENVIRONMENT::ACTION_DIM>> action_noise_critic[2];
+            CONTAINER_TYPE<matrix::Specification<T, TI, CONFIG::CORE_PARAMETERS::SAC_PARAMETERS::CRITIC_BATCH_SIZE, CONFIG::ENVIRONMENT::ACTION_DIM>> action_noise_critic;
             CONTAINER_TYPE<matrix::Specification<typename CONFIG::T, TI, 1, CONFIG::ENVIRONMENT::OBSERVATION_DIM>> observations_mean, observations_std;
             typename CONFIG::NN::CRITIC_TYPE::template Buffer<CONFIG::ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::CRITIC_BATCH_SIZE> critic_buffers[2];
             rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<typename decltype(off_policy_runner)::SPEC, CONFIG::ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::ACTOR_BATCH_SIZE>> actor_batch;
             rl::algorithms::sac::ActorTrainingBuffers<typename CONFIG::ACTOR_CRITIC_TYPE::SPEC> actor_training_buffers;
             CONTAINER_TYPE<matrix::Specification<T, TI, CONFIG::CORE_PARAMETERS::SAC_PARAMETERS::CRITIC_BATCH_SIZE, CONFIG::ENVIRONMENT::ACTION_DIM>> action_noise_actor;
             typename CONFIG::NN::ACTOR_TYPE::template Buffer<CONFIG::ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::ACTOR_BATCH_SIZE> actor_buffers[2];
-            typename CONFIG::NN::ACTOR_TYPE::template Buffer<CONFIG::OFF_POLICY_RUNNER_SPEC::N_ENVIRONMENTS> actor_buffers_eval;
+            typename CONFIG::NN::ACTOR_TYPE::template Buffer<CONFIG::OFF_POLICY_RUNNER_SPEC::PARAMETERS::N_ENVIRONMENTS> actor_buffers_eval;
             TI step;
             bool allocated = false;
         };
     }
     template <typename T_CONFIG>
     constexpr auto& get_actor(rl::algorithms::sac::loop::core::State<T_CONFIG>& ts){
         return ts.actor_critic.actor;
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             bool terminated = get(batch.terminated, 0, batch_step_i);
             T future_value = SPEC::PARAMETERS::IGNORE_TERMINATION || !terminated ? gamma * min_next_state_action_value : 0;
             T current_target_action_value = reward + future_value;
             set(training_buffers.target_action_value, batch_step_i, 0, current_target_action_value); // todo: improve pitch of target action values etc. (by transformig it into row vectors instead of column vectors)
         }
     }
     template <typename DEV_SPEC, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename SPEC>
-    void target_actions(devices::CUDA<DEV_SPEC>& device, const rl::algorithms::td3::ActorCritic<SPEC>& actor_critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>> batch, rl::algorithms::td3::CriticTrainingBuffers<SPEC> training_buffers) {
+    void target_action_values(devices::CUDA<DEV_SPEC>& device, const rl::algorithms::td3::ActorCritic<SPEC>& actor_critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>> batch, rl::algorithms::td3::CriticTrainingBuffers<SPEC> training_buffers) {
         using DEVICE = devices::CUDA<DEV_SPEC>;
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         constexpr TI BLOCKSIZE_COLS = 32;
         constexpr TI N_BLOCKS_COLS = RL_TOOLS_DEVICES_CUDA_CEIL(BATCH_SIZE, BLOCKSIZE_COLS);
         dim3 bias_grid(N_BLOCKS_COLS);
         dim3 bias_block(BLOCKSIZE_COLS);
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 #define RL_TOOLS_RL_ALGORITHMS_TD3_OPERATIONS_GENERIC_H
 
 #include "td3.h"
 
 #include "../../../rl/components/replay_buffer/replay_buffer.h"
 #include "../../../rl/components/off_policy_runner/off_policy_runner.h"
 #include "../../../nn/nn.h"
-#include "../../../nn_models/operations_generic.h"
 #include "../../../utils/polyak/operations_generic.h"
 #include "../../../math/operations_generic.h"
 #include "../../../utils/generic/memcpy.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template <typename DEVICE, typename SPEC>
@@ -128,15 +127,15 @@
                 T noisy_next_action = get(training_buffers.next_actions, batch_step_i, action_i) + get(training_buffers.target_next_action_noise, batch_step_i, action_i);
                 noisy_next_action = math::clamp<T>(device.math, noisy_next_action, -1, 1);
                 set(training_buffers.next_actions, batch_step_i, action_i, noisy_next_action);
             }
         }
     }
     template <typename DEVICE, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename SPEC>
-    void target_actions(DEVICE& device, const rl::algorithms::td3::ActorCritic<SPEC>& actor_critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, rl::algorithms::td3::CriticTrainingBuffers<SPEC>& training_buffers) {
+    void target_action_values(DEVICE& device, const rl::algorithms::td3::ActorCritic<SPEC>& actor_critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, rl::algorithms::td3::CriticTrainingBuffers<SPEC>& training_buffers) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         using BUFFERS = rl::algorithms::td3::CriticTrainingBuffers<SPEC>;
         static_assert(BATCH_SIZE == BUFFERS::BATCH_SIZE);
         constexpr auto OBSERVATION_DIM = SPEC::ENVIRONMENT::OBSERVATION_DIM;
         constexpr auto ACTION_DIM = SPEC::ENVIRONMENT::ACTION_DIM;
         for(TI batch_step_i = 0; batch_step_i < BATCH_SIZE; batch_step_i++){
@@ -163,15 +162,15 @@
 
         evaluate(device, actor_critic.actor_target, batch.next_observations, training_buffers.next_actions, actor_buffers, rng);
         noisy_next_actions(device, training_buffers);
         copy(device, device, batch.next_observations_privileged, training_buffers.next_observations);
         evaluate(device, actor_critic.critic_target_1, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_1, critic_buffers, rng);
         evaluate(device, actor_critic.critic_target_2, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_2, critic_buffers, rng);
 
-        target_actions(device, actor_critic, batch, training_buffers);
+        target_action_values(device, actor_critic, batch, training_buffers);
         forward(device, critic, batch.observations_and_actions, rng);
         nn::loss_functions::mse::gradient(device, output(critic), training_buffers.target_action_value, training_buffers.d_output);
         backward(device, critic, batch.observations_and_actions, training_buffers.d_output, critic_buffers);
         step(device, optimizer, critic);
     }
     template <typename DEVICE, typename SPEC, typename CRITIC_TYPE, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename RNG>
     typename SPEC::T critic_loss(DEVICE& device, const rl::algorithms::td3::ActorCritic<SPEC>& actor_critic, CRITIC_TYPE& critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, typename SPEC::ACTOR_TYPE::template Buffer<BATCH_SIZE>& actor_buffers, typename CRITIC_TYPE::template Buffer<BATCH_SIZE>& critic_buffers, rl::algorithms::td3::CriticTrainingBuffers<SPEC>& training_buffers, RNG& rng) {
@@ -182,15 +181,15 @@
 
         evaluate(device, actor_critic.actor_target, batch.next_observations, training_buffers.next_actions, actor_buffers, rng);
         noisy_next_actions(device, training_buffers);
         copy(device, device, batch.next_observations_privileged, training_buffers.next_observations);
         evaluate(device, actor_critic.critic_target_1, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_1, critic_buffers, rng);
         evaluate(device, actor_critic.critic_target_2, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_2, critic_buffers, rng);
 
-        target_actions(device, actor_critic, batch, training_buffers);
+        target_action_values(device, actor_critic, batch, training_buffers);
         evaluate(device, critic, batch.observations_and_actions, training_buffers.action_value, critic_buffers, rng);
         return nn::loss_functions::mse::evaluate(device, training_buffers.action_value, training_buffers.target_action_value);
     }
     template <typename DEVICE, typename SPEC, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename OPTIMIZER, typename ACTOR_BUFFERS, typename CRITIC_BUFFERS, typename RNG>
     void train_actor(DEVICE& device, rl::algorithms::td3::ActorCritic<SPEC>& actor_critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, OPTIMIZER& optimizer, ACTOR_BUFFERS& actor_buffers, CRITIC_BUFFERS& critic_buffers, rl::algorithms::td3::ActorTrainingBuffers<SPEC>& training_buffers, RNG& rng) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
@@ -224,29 +223,29 @@
         auto& critic = actor_critic.critic_1;
         evaluate(device, critic, training_buffers.state_action_value_input, training_buffers.state_action_value, critic_buffers, rng);
         return mean(device, training_buffers.state_action_value);
     }
 
     namespace rl::algorithms::td3{
         template<typename DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
-        void update_target_layer(DEVICE& device, const  nn::layers::dense::Layer<SOURCE_SPEC>& source, nn::layers::dense::Layer<TARGET_SPEC>& target, typename SOURCE_SPEC::T polyak) {
+        void update_target_layer(DEVICE& device, const  nn::layers::dense::LayerForward<SOURCE_SPEC>& source, nn::layers::dense::LayerForward<TARGET_SPEC>& target, typename SOURCE_SPEC::T polyak) {
             rl_tools::utils::polyak::update(device, source.weights.parameters, target.weights.parameters, polyak);
             rl_tools::utils::polyak::update(device, source.biases.parameters , target.biases.parameters , polyak);
         }
         template<typename T, typename DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
-        void update_target_network(DEVICE& device, const  nn_models::mlp::NeuralNetwork<SOURCE_SPEC>& source, nn_models::mlp::NeuralNetwork<TARGET_SPEC>& target, T polyak) {
-            using TargetNetworkType = nn_models::mlp::NeuralNetwork<TARGET_SPEC>;
+        void update_target_network(DEVICE& device, const  nn_models::mlp::NeuralNetworkForward<SOURCE_SPEC>& source, nn_models::mlp::NeuralNetworkForward<TARGET_SPEC>& target, T polyak) {
+            using TargetNetworkType = nn_models::mlp::NeuralNetworkForward<TARGET_SPEC>;
             update_target_layer(device, source.input_layer, target.input_layer, polyak);
             for(typename DEVICE::index_t layer_i=0; layer_i < TargetNetworkType::NUM_HIDDEN_LAYERS; layer_i++){
                 update_target_layer(device, source.hidden_layers[layer_i], target.hidden_layers[layer_i], polyak);
             }
             update_target_layer(device, source.output_layer, target.output_layer, polyak);
         }
         template<typename T, typename DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
-        void update_target_network(DEVICE& device, const  nn_models::sequential::Module<SOURCE_SPEC>& source, nn_models::sequential::Module<TARGET_SPEC>& target, T polyak) {
+        void update_target_network(DEVICE& device, const  nn_models::sequential::ModuleForward<SOURCE_SPEC>& source, nn_models::sequential::ModuleForward<TARGET_SPEC>& target, T polyak) {
             update_target_layer(device, source.content, target.content, polyak);
             if constexpr(!rl_tools::utils::typing::is_same_v<typename SOURCE_SPEC::NEXT_MODULE, nn_models::sequential::OutputModule>){
                 update_target_network(device, source.next_module, target.next_module, polyak);
             }
         }
     }
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools::rl::algorithms::td3 {
     template<typename T, typename TI>
     struct DefaultParameters {
         static constexpr T GAMMA = 0.99;
         static constexpr TI ACTOR_BATCH_SIZE = 100;
         static constexpr TI CRITIC_BATCH_SIZE = 100;
-        static constexpr TI N_WARMUP_STEPS_CRITIC = 0;
-        static constexpr TI N_WARMUP_STEPS_ACTOR = 0;
         static constexpr TI CRITIC_TRAINING_INTERVAL = 1;
         static constexpr TI ACTOR_TRAINING_INTERVAL = 2;
         static constexpr TI CRITIC_TARGET_UPDATE_INTERVAL = 2;
         static constexpr TI ACTOR_TARGET_UPDATE_INTERVAL = 2;
         static constexpr T ACTOR_POLYAK = 1.0 - 0.005;
         static constexpr T CRITIC_POLYAK = 1.0 - 0.005;
         static constexpr T TARGET_NEXT_ACTION_NOISE_STD = 0.2;
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,144 +1,160 @@
-#include "../../../../../version.h"
-#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_RL_ALGORITHMS_TD3_LOOP_CORE_CONFIG_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
+#include "../../../version.h"
+#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_RL_COMPONENTS_OFF_POLICY_RUNNER_OFF_POLICY_RUNNER_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
-#define RL_TOOLS_RL_ALGORITHMS_TD3_LOOP_CORE_CONFIG_H
+#define RL_TOOLS_RL_COMPONENTS_OFF_POLICY_RUNNER_OFF_POLICY_RUNNER_H
 
-#include "../../../../../nn_models/sequential/model.h"
-#include "../../../../../nn_models/mlp/network.h"
-#include "../../../../../rl/algorithms/td3/td3.h"
-#include "../../../../../nn/optimizers/adam/adam.h"
-#include "state.h"
+// Please include the file containing the environments operations before including this file
+#include "../../../rl/components/replay_buffer/replay_buffer.h"
+
+
+/* requirements
+- Multiple environments
+- Batched action inference
+
+
+*/
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
-namespace rl_tools::rl::algorithms::td3::loop::core{
-    // Config State (Init/Step)
-    using namespace nn_models::sequential::interface;
-
-    template<typename T, typename TI, typename ENVIRONMENT>
-    struct DefaultParameters{
-        using TD3_PARAMETERS = rl::algorithms::td3::DefaultParameters<T, TI>;
+namespace rl_tools::rl::components::off_policy_runner {
+    template <typename TI, TI T_NUM_THREADS>
+    struct ExecutionHints{
+        static constexpr TI NUM_THREADS = T_NUM_THREADS;
+    };
+    template <typename T_T, typename T_TI>
+    struct ParametersDefault{
+        using T = T_T;
+        using TI = T_TI;
         static constexpr TI N_ENVIRONMENTS = 1;
-        static constexpr int N_WARMUP_STEPS = TD3_PARAMETERS::ACTOR_BATCH_SIZE;
-        static constexpr TI STEP_LIMIT = 10000;
-        static constexpr TI REPLAY_BUFFER_CAP = STEP_LIMIT; // Note: when inheriting from this class for overwriting the default STEP_LIMIT you need to set the REPLAY_BUFFER_CAP as well otherwise it will be the default step limit
-        static constexpr TI EPISODE_STEP_LIMIT = 200;
-
-        static constexpr TI ACTOR_HIDDEN_DIM = 64;
-        static constexpr TI ACTOR_NUM_LAYERS = 3;
-        static constexpr auto ACTOR_ACTIVATION_FUNCTION = nn::activation_functions::ActivationFunction::RELU;
-        static constexpr TI CRITIC_HIDDEN_DIM = 64;
-        static constexpr TI CRITIC_NUM_LAYERS = 3;
-        static constexpr auto CRITIC_ACTIVATION_FUNCTION = nn::activation_functions::ActivationFunction::RELU;
-
-        static constexpr bool COLLECT_EPISODE_STATS = true;
-        static constexpr TI EPISODE_STATS_BUFFER_SIZE = 1000;
-
-        using OPTIMIZER_PARAMETERS = nn::optimizers::adam::DEFAULT_PARAMETERS_TENSORFLOW<T>;
-    };
-
-    // The approximator config sets up any types that support the usual rl_tools::forward and rl_tools::backward operations (can be custom as well)
-    // We provide approximators based on the sequential and mlp models. The latter (mlp) allows for a variable number of layers, but is restricted to a uniform hidden layer size while the former allows for arbitrary layers to be combined in a sequential manner. Both support compile-time autodiff
-    template<typename T, typename TI, typename ENVIRONMENT, typename PARAMETERS>
-    struct ConfigApproximatorsSequential{
-        template <typename PARAMETER_TYPE, template<typename> class LAYER_TYPE = nn::layers::dense::LayerBackwardGradient>
-        struct ACTOR{
-            static constexpr TI HIDDEN_DIM = PARAMETERS::ACTOR_HIDDEN_DIM;
-            static constexpr TI BATCH_SIZE = PARAMETERS::TD3_PARAMETERS::ACTOR_BATCH_SIZE;
-            static constexpr auto ACTIVATION_FUNCTION = PARAMETERS::ACTOR_ACTIVATION_FUNCTION;
-            using LAYER_1_SPEC = nn::layers::dense::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, PARAMETER_TYPE, BATCH_SIZE>;
-            using LAYER_1 = LAYER_TYPE<LAYER_1_SPEC>;
-            using LAYER_2_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, PARAMETER_TYPE, BATCH_SIZE>;
-            using LAYER_2 = LAYER_TYPE<LAYER_2_SPEC>;
-            static constexpr TI ACTOR_OUTPUT_DIM = ENVIRONMENT::ACTION_DIM;
-            using LAYER_3_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, ACTOR_OUTPUT_DIM, nn::activation_functions::ActivationFunction::IDENTITY, PARAMETER_TYPE, BATCH_SIZE>; // note the output activation should be identity because we want to sample from a gaussian and then squash afterwards (taking into account the squashing in the distribution)
-            using LAYER_3 = LAYER_TYPE<LAYER_3_SPEC>;
-
-            using MODEL = Module<LAYER_1, Module<LAYER_2, Module<LAYER_3>>>;
-        };
-
-        template <typename PARAMETER_TYPE, template<typename> class LAYER_TYPE = nn::layers::dense::LayerBackwardGradient>
-        struct CRITIC{
-            static constexpr TI HIDDEN_DIM = PARAMETERS::CRITIC_HIDDEN_DIM;
-            static constexpr TI BATCH_SIZE = PARAMETERS::TD3_PARAMETERS::CRITIC_BATCH_SIZE;
-            static constexpr auto ACTIVATION_FUNCTION = PARAMETERS::CRITIC_ACTIVATION_FUNCTION;
-
-            using LAYER_1_SPEC = nn::layers::dense::Specification<T, TI, ENVIRONMENT::OBSERVATION_DIM + ENVIRONMENT::ACTION_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, PARAMETER_TYPE, BATCH_SIZE>;
-            using LAYER_1 = LAYER_TYPE<LAYER_1_SPEC>;
-            using LAYER_2_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, HIDDEN_DIM, ACTIVATION_FUNCTION, PARAMETER_TYPE, BATCH_SIZE>;
-            using LAYER_2 = LAYER_TYPE<LAYER_2_SPEC>;
-            using LAYER_3_SPEC = nn::layers::dense::Specification<T, TI, HIDDEN_DIM, 1, nn::activation_functions::ActivationFunction::IDENTITY, PARAMETER_TYPE, BATCH_SIZE>;
-            using LAYER_3 = LAYER_TYPE<LAYER_3_SPEC>;
-
-            using MODEL = Module<LAYER_1, Module<LAYER_2, Module<LAYER_3>>>;
-        };
-
-        using OPTIMIZER_SPEC = nn::optimizers::adam::Specification<T, TI, typename PARAMETERS::OPTIMIZER_PARAMETERS>;
-
-        using OPTIMIZER = nn::optimizers::Adam<OPTIMIZER_SPEC>;
-
-        using ACTOR_TYPE = typename ACTOR<nn::parameters::Adam>::MODEL;
-        using ACTOR_TARGET_TYPE = typename ACTOR<nn::parameters::Adam, nn::layers::dense::Layer>::MODEL;
-        using CRITIC_TYPE = typename CRITIC<nn::parameters::Adam>::MODEL;
-        using CRITIC_TARGET_TYPE = typename CRITIC<nn::parameters::Adam, nn::layers::dense::Layer>::MODEL;
-    };
-
-    template<typename T, typename TI, typename ENVIRONMENT, typename PARAMETERS>
-    struct ConfigApproximatorsMLP{
-        using ACTOR_STRUCTURE_SPEC = nn_models::mlp::StructureSpecification<T, TI, ENVIRONMENT::OBSERVATION_DIM, ENVIRONMENT::ACTION_DIM, PARAMETERS::ACTOR_NUM_LAYERS, PARAMETERS::ACTOR_HIDDEN_DIM, PARAMETERS::ACTOR_ACTIVATION_FUNCTION, nn::activation_functions::TANH, PARAMETERS::TD3_PARAMETERS::ACTOR_BATCH_SIZE>;
-        using CRITIC_STRUCTURE_SPEC = nn_models::mlp::StructureSpecification<T, TI, ENVIRONMENT::OBSERVATION_DIM + ENVIRONMENT::ACTION_DIM, 1, PARAMETERS::CRITIC_NUM_LAYERS, PARAMETERS::CRITIC_HIDDEN_DIM, PARAMETERS::CRITIC_ACTIVATION_FUNCTION, nn::activation_functions::IDENTITY, PARAMETERS::TD3_PARAMETERS::CRITIC_BATCH_SIZE>;
-        using OPTIMIZER_SPEC = typename nn::optimizers::adam::Specification<T, TI, typename PARAMETERS::OPTIMIZER_PARAMETERS>;
-        using OPTIMIZER = nn::optimizers::Adam<OPTIMIZER_SPEC>;
-        using ACTOR_SPEC = nn_models::mlp::AdamSpecification<ACTOR_STRUCTURE_SPEC >;
-        using ACTOR_TYPE = nn_models::mlp::NeuralNetworkAdam<ACTOR_SPEC>;
-
-        using ACTOR_TARGET_SPEC = nn_models::mlp::InferenceSpecification<ACTOR_STRUCTURE_SPEC>;
-        using ACTOR_TARGET_TYPE = nn_models::mlp::NeuralNetwork<ACTOR_TARGET_SPEC>;
-
-        using CRITIC_SPEC = nn_models::mlp::AdamSpecification<CRITIC_STRUCTURE_SPEC>;
-        using CRITIC_TYPE = nn_models::mlp::NeuralNetworkAdam<CRITIC_SPEC>;
+        static constexpr bool ASYMMETRIC_OBSERVATIONS = false;
+        static constexpr TI REPLAY_BUFFER_CAPACITY = 10000;
+        static constexpr TI EPISODE_STEP_LIMIT = 1000;
+        static constexpr bool STOCHASTIC_POLICY = false;
+        static constexpr bool COLLECT_EPISODE_STATS = false;
+        static constexpr TI EPISODE_STATS_BUFFER_SIZE = 0;
 
-        using CRITIC_TARGET_SPEC = nn_models::mlp::InferenceSpecification<CRITIC_STRUCTURE_SPEC >;
-        using CRITIC_TARGET_TYPE = nn_models::mlp::NeuralNetwork<CRITIC_TARGET_SPEC>;
+        static constexpr T EXPLORATION_NOISE = 0.1;
     };
-
-    template<typename T_T, typename T_TI, typename T_RNG, typename T_ENVIRONMENT, typename T_PARAMETERS = DefaultParameters<T_T, T_TI, T_ENVIRONMENT>, template<typename, typename, typename, typename> class APPROXIMATOR_CONFIG=ConfigApproximatorsSequential>
-    struct Config{
+    template <typename SPEC>
+    struct ParametersRuntime{
+        using T = typename SPEC::T;
+        T exploration_noise = SPEC::PARAMETERS::EXPLORATION_NOISE;
+    };
+    template<typename T_T, typename T_TI, typename T_ENVIRONMENT, typename T_PARAMETERS, typename T_CONTAINER_TYPE_TAG = MatrixDynamicTag>
+    struct Specification{
         using T = T_T;
         using TI = T_TI;
-        using RNG = T_RNG;
-        using ENVIRONMENT = T_ENVIRONMENT;
-        using ENVIRONMENT_EVALUATION = T_ENVIRONMENT;
+        using ENVIRONMENT =  T_ENVIRONMENT;
+        using PARAMETERS = T_PARAMETERS;
+        static_assert((PARAMETERS::ASYMMETRIC_OBSERVATIONS && ENVIRONMENT::OBSERVATION_DIM_PRIVILEGED > 0) == PARAMETERS::ASYMMETRIC_OBSERVATIONS, "ASYMMETRIC_OBSERVATIONS requested but not available in the environment");
+        static constexpr TI OBSERVATION_DIM_PRIVILEGED = PARAMETERS::ASYMMETRIC_OBSERVATIONS ? ENVIRONMENT::OBSERVATION_DIM_PRIVILEGED : ENVIRONMENT::OBSERVATION_DIM;
+        static constexpr TI OBSERVATION_DIM_PRIVILEGED_ACTUAL = PARAMETERS::ASYMMETRIC_OBSERVATIONS ? ENVIRONMENT::OBSERVATION_DIM_PRIVILEGED : 0;
+        static constexpr bool ACTION_CLAMPING_TANH = PARAMETERS::STOCHASTIC_POLICY;
 
-        using NN = APPROXIMATOR_CONFIG<T, TI, T_ENVIRONMENT, T_PARAMETERS>;
-//        using NN = ConfigApproximatorsMLP<T, TI, T_ENVIRONMENT, T_PARAMETERS>;
+        using CONTAINER_TYPE_TAG = T_CONTAINER_TYPE_TAG;
+    };
 
-        using CORE_PARAMETERS = T_PARAMETERS;
+    template<typename SPEC>
+    struct Buffers{
+        // todo: make the buffer exploit the observation = observation_priviliged to save memory in the case of symmetric observations
+        using T = typename SPEC::T;
+        using TI = typename SPEC::TI;
+
+        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, SPEC::PARAMETERS::N_ENVIRONMENTS, SPEC::ENVIRONMENT::OBSERVATION_DIM>> observations;
+        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, SPEC::PARAMETERS::N_ENVIRONMENTS, SPEC::OBSERVATION_DIM_PRIVILEGED>> observations_privileged;
+        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, SPEC::PARAMETERS::N_ENVIRONMENTS, SPEC::ENVIRONMENT::ACTION_DIM * (SPEC::PARAMETERS::STOCHASTIC_POLICY ? 2 : 1)>> actions;
+        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, SPEC::PARAMETERS::N_ENVIRONMENTS, SPEC::ENVIRONMENT::OBSERVATION_DIM>> next_observations;
+        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, SPEC::PARAMETERS::N_ENVIRONMENTS, SPEC::OBSERVATION_DIM_PRIVILEGED>> next_observations_privileged;
+    };
 
 
-        using ALPHA_PARAMETER_TYPE = nn::parameters::Adam;
-        using ALPHA_OPTIMIZER = nn::optimizers::Adam<typename NN::OPTIMIZER_SPEC>;
 
-        using ACTOR_CRITIC_SPEC = rl::algorithms::td3::Specification<T, TI, ENVIRONMENT, typename NN::ACTOR_TYPE, typename NN::ACTOR_TARGET_TYPE, typename NN::CRITIC_TYPE, typename NN::CRITIC_TARGET_TYPE, typename NN::OPTIMIZER, typename CORE_PARAMETERS::TD3_PARAMETERS>;
-        using ACTOR_CRITIC_TYPE = rl::algorithms::td3::ActorCritic<ACTOR_CRITIC_SPEC>;
+    template<typename T_SPEC, typename T_SPEC::TI T_BATCH_SIZE, typename T_CONTAINER_TYPE_TAG = typename T_SPEC::CONTAINER_TYPE_TAG>
+    struct BatchSpecification {
+        using SPEC = T_SPEC;
+        using CONTAINER_TYPE_TAG = T_CONTAINER_TYPE_TAG;
+        static constexpr typename SPEC::TI BATCH_SIZE = T_BATCH_SIZE;
+    };
 
-        static constexpr bool STOCHASTIC_POLICY = false;
-        using OFF_POLICY_RUNNER_SPEC = rl::components::off_policy_runner::Specification<
-                T,
-                TI,
-                ENVIRONMENT,
-                CORE_PARAMETERS::N_ENVIRONMENTS,
-                false,
-                CORE_PARAMETERS::REPLAY_BUFFER_CAP,
-                CORE_PARAMETERS::EPISODE_STEP_LIMIT,
-                STOCHASTIC_POLICY,
-                CORE_PARAMETERS::COLLECT_EPISODE_STATS,
-                CORE_PARAMETERS::EPISODE_STATS_BUFFER_SIZE
-        >;
-        static_assert(ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::ACTOR_BATCH_SIZE == ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::CRITIC_BATCH_SIZE);
-        template <typename CONFIG>
-        using State = State<CONFIG>;
+    template <typename T_SPEC>
+    struct Batch{
+        using SPEC = typename T_SPEC::SPEC;
+        using T = typename SPEC::T;
+        using TI = typename SPEC::TI;
+
+        static constexpr TI BATCH_SIZE = T_SPEC::BATCH_SIZE;
+        static constexpr TI OBSERVATION_DIM = SPEC::ENVIRONMENT::OBSERVATION_DIM;
+        static constexpr bool ASYMMETRIC_OBSERVATIONS = SPEC::PARAMETERS::ASYMMETRIC_OBSERVATIONS;
+        static constexpr TI OBSERVATION_DIM_PRIVILEGED = SPEC::OBSERVATION_DIM_PRIVILEGED;
+        static constexpr TI ACTION_DIM = SPEC::ENVIRONMENT::ACTION_DIM;
+
+        static constexpr TI DATA_DIM = OBSERVATION_DIM + SPEC::OBSERVATION_DIM_PRIVILEGED_ACTUAL + ACTION_DIM + OBSERVATION_DIM + SPEC::OBSERVATION_DIM_PRIVILEGED_ACTUAL;
+        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, BATCH_SIZE, DATA_DIM>> observations_actions_next_observations;
+
+        template<typename SPEC::TI DIM>
+        using OANO_VIEW = typename decltype(observations_actions_next_observations)::template VIEW<BATCH_SIZE, DIM>;
+
+        OANO_VIEW<OBSERVATION_DIM> observations;
+        OANO_VIEW<SPEC::OBSERVATION_DIM_PRIVILEGED> observations_privileged;
+        OANO_VIEW<ACTION_DIM> actions;
+        OANO_VIEW<SPEC::OBSERVATION_DIM_PRIVILEGED + ACTION_DIM> observations_and_actions;
+        OANO_VIEW<OBSERVATION_DIM> next_observations;
+        OANO_VIEW<SPEC::OBSERVATION_DIM_PRIVILEGED> next_observations_privileged;
+
+        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, 1, BATCH_SIZE>> rewards;
+        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<bool, TI, 1, BATCH_SIZE>> terminated;
+        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<bool, TI, 1, BATCH_SIZE>> truncated;
+    };
+
+    template<typename SPEC>
+    struct EpisodeStats{
+        using T = typename SPEC::T;
+        using TI = typename SPEC::TI;
+        static constexpr TI BUFFER_SIZE = SPEC::PARAMETERS::EPISODE_STATS_BUFFER_SIZE;
+        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, BUFFER_SIZE, 2>> data;
+
+        TI next_episode_i = 0;
+        template<typename SPEC::TI DIM>
+        using STATS_VIEW = typename decltype(data)::template VIEW<BUFFER_SIZE, DIM>;
+        STATS_VIEW<1> returns;
+        STATS_VIEW<1> steps;
     };
 }
+RL_TOOLS_NAMESPACE_WRAPPER_END
 
+RL_TOOLS_NAMESPACE_WRAPPER_START
+namespace rl_tools::rl::components{
+    template<typename T_SPEC>
+    struct OffPolicyRunner {
+        using SPEC = T_SPEC;
+        using T = typename SPEC::T;
+        using TI = typename SPEC::TI;
+        using ENVIRONMENT = typename SPEC::ENVIRONMENT;
+        using REPLAY_BUFFER_SPEC = replay_buffer::Specification<typename SPEC::T, typename SPEC::TI, SPEC::ENVIRONMENT::OBSERVATION_DIM, ENVIRONMENT::OBSERVATION_DIM_PRIVILEGED, SPEC::PARAMETERS::ASYMMETRIC_OBSERVATIONS, SPEC::ENVIRONMENT::ACTION_DIM, SPEC::PARAMETERS::REPLAY_BUFFER_CAPACITY, typename SPEC::CONTAINER_TYPE_TAG>;
+        using REPLAY_BUFFER_WITH_STATES_SPEC = replay_buffer::SpecificationWithStates<ENVIRONMENT, REPLAY_BUFFER_SPEC>;
+        using REPLAY_BUFFER_TYPE = ReplayBufferWithStates<REPLAY_BUFFER_WITH_STATES_SPEC>;
+        static constexpr TI N_ENVIRONMENTS = SPEC::PARAMETERS::N_ENVIRONMENTS;
+//        using POLICY_EVAL_BUFFERS = typename POLICY::template Buffers<N_ENVIRONMENTS>;
+
+        off_policy_runner::ParametersRuntime<SPEC> parameters;
+        template<typename T_SPEC::TI T_BATCH_SIZE, typename T_CONTAINER_TYPE_TAG = typename T_SPEC::CONTAINER_TYPE_TAG>
+        using Batch = off_policy_runner::Batch<typename off_policy_runner::BatchSpecification<SPEC, T_BATCH_SIZE, T_CONTAINER_TYPE_TAG>>;
+
+        off_policy_runner::Buffers<SPEC> buffers;
+
+        // todo: change to "environments"
+        ENVIRONMENT envs[N_ENVIRONMENTS];
+        off_policy_runner::EpisodeStats<SPEC> episode_stats[N_ENVIRONMENTS];
+        REPLAY_BUFFER_TYPE replay_buffers[N_ENVIRONMENTS];
+
+        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<typename SPEC::ENVIRONMENT::State, TI, 1, N_ENVIRONMENTS>> states;
+        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, 1, N_ENVIRONMENTS>> episode_return;
+        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<TI, TI, 1, N_ENVIRONMENTS>> episode_step;
+        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<bool, TI, 1, N_ENVIRONMENTS>> truncated; // init to true !!
+#ifdef RL_TOOLS_DEBUG_RL_COMPONENTS_OFF_POLICY_RUNNER_CHECK_INIT
+        bool initialized = false;
 #endif
+    };
+}
+RL_TOOLS_NAMESPACE_WRAPPER_END
 
+#endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #include "../../../../../version.h"
 #if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_RL_ALGORITHMS_TD3_LOOP_CORE_OPERATIONS_GENERIC_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
 #define RL_TOOLS_RL_ALGORITHMS_TD3_LOOP_CORE_OPERATIONS_GENERIC_H
 
 #include "../../../../../rl/algorithms/td3/operations_generic.h"
+#include "../../../../../nn_models/random_uniform/operations_generic.h"
 #include "../../../../../rl/components/off_policy_runner/operations_generic.h"
 #include "../../../../../rl/utils/evaluation.h"
 
 #include "config.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
@@ -42,17 +43,15 @@
 
         for(auto& env: ts.envs){
             rl_tools::init(device, env);
         }
         init(device, ts.off_policy_runner, ts.envs);
         set_all(device, ts.observations_mean, 0);
         set_all(device, ts.observations_std, 1);
-        ts.off_policy_runner.parameters = rl::components::off_policy_runner::default_parameters<T>;
-        init(device);
-        init(device, device.logger);
+
         ts.step = 0;
     }
 
     template <typename DEVICE, typename T_CONFIG>
     void free(DEVICE& device, rl::algorithms::td3::loop::core::State<T_CONFIG>& ts){
         free(device, ts.critic_batch);
         free(device, ts.critic_training_buffers);
@@ -68,26 +67,44 @@
     }
 
     template <typename DEVICE, typename T_CONFIG>
     bool step(DEVICE& device, rl::algorithms::td3::loop::core::State<T_CONFIG>& ts){
         using CONFIG = T_CONFIG;
         set_step(device, device.logger, ts.step);
         bool finished = false;
-        step(device, ts.off_policy_runner, ts.actor_critic.actor, ts.actor_buffers_eval, ts.rng);
-        if(ts.step > CONFIG::CORE_PARAMETERS::N_WARMUP_STEPS){
+        if(ts.step >= CONFIG::CORE_PARAMETERS::N_WARMUP_STEPS){
+            step(device, ts.off_policy_runner, get_actor(ts), ts.actor_buffers_eval, ts.rng);
+        }
+        else{
+            typename CONFIG::EXPLORATION_POLICY exploration_policy;
+            typename CONFIG::EXPLORATION_POLICY::template Buffer<> exploration_policy_buffer;
+            step(device, ts.off_policy_runner, exploration_policy, exploration_policy_buffer, ts.rng);
+        }
+        if(ts.step >= CONFIG::CORE_PARAMETERS::N_WARMUP_STEPS){
+            if constexpr(CONFIG::CORE_PARAMETERS::SHARED_BATCH){
+                gather_batch(device, ts.off_policy_runner, ts.critic_batch, ts.rng);
+                target_action_noise(device, ts.actor_critic, ts.critic_training_buffers.target_next_action_noise, ts.rng);
+            }
             if(ts.step % CONFIG::CORE_PARAMETERS::TD3_PARAMETERS::CRITIC_TRAINING_INTERVAL == 0){
                 for(int critic_i = 0; critic_i < 2; critic_i++){
-                    gather_batch(device, ts.off_policy_runner, ts.critic_batch, ts.rng);
-                    target_action_noise(device, ts.actor_critic, ts.critic_training_buffers.target_next_action_noise, ts.rng);
+                    if constexpr(!CONFIG::CORE_PARAMETERS::SHARED_BATCH) {
+                        gather_batch(device, ts.off_policy_runner, ts.critic_batch, ts.rng);
+                        target_action_noise(device, ts.actor_critic, ts.critic_training_buffers.target_next_action_noise, ts.rng);
+                    }
                     train_critic(device, ts.actor_critic, critic_i == 0 ? ts.actor_critic.critic_1 : ts.actor_critic.critic_2, ts.critic_batch, ts.actor_critic.critic_optimizers[critic_i], ts.actor_buffers[critic_i], ts.critic_buffers[critic_i], ts.critic_training_buffers, ts.rng);
                 }
             }
             if(ts.step % CONFIG::CORE_PARAMETERS::TD3_PARAMETERS::ACTOR_TRAINING_INTERVAL == 0){
-                gather_batch(device, ts.off_policy_runner, ts.actor_batch, ts.rng);
-                train_actor(device, ts.actor_critic, ts.actor_batch, ts.actor_critic.actor_optimizer, ts.actor_buffers[0], ts.critic_buffers[0], ts.actor_training_buffers);
+                if constexpr(CONFIG::CORE_PARAMETERS::SHARED_BATCH) {
+                    train_actor(device, ts.actor_critic, ts.critic_batch, ts.actor_critic.actor_optimizer, ts.actor_buffers[0], ts.critic_buffers[0], ts.actor_training_buffers, ts.rng);
+                }
+                else{
+                    gather_batch(device, ts.off_policy_runner, ts.actor_batch, ts.rng);
+                    train_actor(device, ts.actor_critic, ts.actor_batch, ts.actor_critic.actor_optimizer, ts.actor_buffers[0], ts.critic_buffers[0], ts.actor_training_buffers, ts.rng);
+                }
             }
             if(ts.step % CONFIG::CORE_PARAMETERS::TD3_PARAMETERS::CRITIC_TARGET_UPDATE_INTERVAL == 0){
                 update_critic_targets(device, ts.actor_critic);
             }
             if(ts.step % CONFIG::CORE_PARAMETERS::TD3_PARAMETERS::ACTOR_TARGET_UPDATE_INTERVAL == 0){
                 update_actor_target(device, ts.actor_critic);
             }
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<typename decltype(off_policy_runner)::SPEC, CONFIG::ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::CRITIC_BATCH_SIZE>> critic_batch;
             rl::algorithms::td3::CriticTrainingBuffers<typename CONFIG::ACTOR_CRITIC_SPEC> critic_training_buffers;
             MatrixDynamic<matrix::Specification<typename CONFIG::T, TI, 1, CONFIG::ENVIRONMENT::OBSERVATION_DIM>> observations_mean, observations_std;
             typename CONFIG::NN::CRITIC_TYPE::template Buffer<CONFIG::ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::CRITIC_BATCH_SIZE> critic_buffers[2];
             rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<typename decltype(off_policy_runner)::SPEC, CONFIG::ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::ACTOR_BATCH_SIZE>> actor_batch;
             rl::algorithms::td3::ActorTrainingBuffers<typename CONFIG::ACTOR_CRITIC_TYPE::SPEC> actor_training_buffers;
             typename CONFIG::NN::ACTOR_TYPE::template Buffer<CONFIG::ACTOR_CRITIC_TYPE::SPEC::PARAMETERS::ACTOR_BATCH_SIZE> actor_buffers[2];
-            typename CONFIG::NN::ACTOR_TYPE::template Buffer<CONFIG::OFF_POLICY_RUNNER_SPEC::N_ENVIRONMENTS> actor_buffers_eval;
+            typename CONFIG::NN::ACTOR_TYPE::template Buffer<CONFIG::OFF_POLICY_RUNNER_SPEC::PARAMETERS::N_ENVIRONMENTS> actor_buffers_eval;
             TI step;
         };
     }
     template <typename T_CONFIG>
     constexpr auto& get_actor(rl::algorithms::td3::loop::core::State<T_CONFIG>& ts){
         return ts.actor_critic.actor;
     }
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,154 +1,153 @@
-#include "../../../version.h"
-#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_RL_COMPONENTS_OFF_POLICY_RUNNER_OFF_POLICY_RUNNER_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
+#include "../../version.h"
+#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_RL_UTILS_EVALUATION_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
-#define RL_TOOLS_RL_COMPONENTS_OFF_POLICY_RUNNER_OFF_POLICY_RUNNER_H
+#define RL_TOOLS_RL_UTILS_EVALUATION_H
+/*
+ * This file relies on the environments methods hence it should be included after the operations of the environments that it will be used with
+ */
 
-// Please include the file containing the environments operations before including this file
-#include "../../../rl/components/replay_buffer/replay_buffer.h"
-
-
-/* requirements
-- Multiple environments
-- Batched action inference
-
-
-*/
+#include "../../math/operations_generic.h"
+#include "../environments/operations_generic.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
-namespace rl_tools::rl::components::off_policy_runner {
-    template <typename TI, TI T_NUM_THREADS>
-    struct ExecutionHints{
-        static constexpr TI NUM_THREADS = T_NUM_THREADS;
-    };
-    template<typename T>
-    struct Parameters{
-        T exploration_noise;
-    };
-    template<typename T>
-    Parameters<T> default_parameters{
-        0.1 // exploration_noise
-    };
-    template<typename T_T, typename T_TI, typename T_ENVIRONMENT, T_TI T_N_ENVIRONMENTS, bool T_ASYMMETRIC_OBSERVATIONS, T_TI T_REPLAY_BUFFER_CAPACITY, T_TI T_STEP_LIMIT, bool T_STOCHASTIC_POLICY = false, bool T_COLLECT_EPISODE_STATS = false, T_TI T_EPISODE_STATS_BUFFER_SIZE = 0, typename T_CONTAINER_TYPE_TAG = MatrixDynamicTag>
-    struct Specification{
-        using T = T_T;
-        using TI = T_TI;
-        using ENVIRONMENT =  T_ENVIRONMENT;
-        static constexpr TI N_ENVIRONMENTS = T_N_ENVIRONMENTS;
-        static constexpr TI REPLAY_BUFFER_CAPACITY = T_REPLAY_BUFFER_CAPACITY;
-        static constexpr TI STEP_LIMIT = T_STEP_LIMIT;
-        static constexpr bool STOCHASTIC_POLICY = T_STOCHASTIC_POLICY;
-        static constexpr bool COLLECT_EPISODE_STATS = T_COLLECT_EPISODE_STATS;
-        static constexpr TI EPISODE_STATS_BUFFER_SIZE = T_EPISODE_STATS_BUFFER_SIZE;
-        using CONTAINER_TYPE_TAG = T_CONTAINER_TYPE_TAG;
-        static constexpr bool ASYMMETRIC_OBSERVATIONS = T_ASYMMETRIC_OBSERVATIONS && ENVIRONMENT::OBSERVATION_DIM_PRIVILEGED > 0;
-        static_assert(ASYMMETRIC_OBSERVATIONS == T_ASYMMETRIC_OBSERVATIONS, "ASYMMETRIC_OBSERVATIONS requested but not available in the environment");
-        static constexpr TI OBSERVATION_DIM_PRIVILEGED = ASYMMETRIC_OBSERVATIONS ? ENVIRONMENT::OBSERVATION_DIM_PRIVILEGED : ENVIRONMENT::OBSERVATION_DIM;
-        static constexpr TI OBSERVATION_DIM_PRIVILEGED_ACTUAL = ASYMMETRIC_OBSERVATIONS ? ENVIRONMENT::OBSERVATION_DIM_PRIVILEGED : 0;
-        static constexpr bool ACTION_CLAMPING_TANH = T_STOCHASTIC_POLICY;
-    };
+namespace rl_tools::rl::utils::evaluation{
+    template <typename T, typename TI, typename ENV_STATE>
+    struct State{
+        T episode_return = 0;
+        TI episode_step = 0;
 
-    template<typename SPEC>
-    struct Buffers{
-        // todo: make the buffer exploit the observation = observation_priviliged to save memory in the case of symmetric observations
-        using T = typename SPEC::T;
-        using TI = typename SPEC::TI;
-
-        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, SPEC::N_ENVIRONMENTS, SPEC::ENVIRONMENT::OBSERVATION_DIM>> observations;
-        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, SPEC::N_ENVIRONMENTS, SPEC::OBSERVATION_DIM_PRIVILEGED>> observations_privileged;
-        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, SPEC::N_ENVIRONMENTS, SPEC::ENVIRONMENT::ACTION_DIM * (SPEC::STOCHASTIC_POLICY ? 2 : 1)>> actions;
-        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, SPEC::N_ENVIRONMENTS, SPEC::ENVIRONMENT::OBSERVATION_DIM>> next_observations;
-        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, SPEC::N_ENVIRONMENTS, SPEC::OBSERVATION_DIM_PRIVILEGED>> next_observations_privileged;
+        ENV_STATE state;
     };
-
-
-
-    template<typename T_SPEC, typename T_SPEC::TI T_BATCH_SIZE, typename T_CONTAINER_TYPE_TAG = typename T_SPEC::CONTAINER_TYPE_TAG>
-    struct BatchSpecification {
-        using SPEC = T_SPEC;
-        using CONTAINER_TYPE_TAG = T_CONTAINER_TYPE_TAG;
-        static constexpr typename SPEC::TI BATCH_SIZE = T_BATCH_SIZE;
-    };
-
-    template <typename T_SPEC>
-    struct Batch{
-        using SPEC = typename T_SPEC::SPEC;
-        using T = typename SPEC::T;
-        using TI = typename SPEC::TI;
-
-        static constexpr TI BATCH_SIZE = T_SPEC::BATCH_SIZE;
-        static constexpr TI OBSERVATION_DIM = SPEC::ENVIRONMENT::OBSERVATION_DIM;
-        static constexpr bool ASYMMETRIC_OBSERVATIONS = SPEC::ASYMMETRIC_OBSERVATIONS;
-        static constexpr TI OBSERVATION_DIM_PRIVILEGED = SPEC::OBSERVATION_DIM_PRIVILEGED;
-        static constexpr TI ACTION_DIM = SPEC::ENVIRONMENT::ACTION_DIM;
-
-        static constexpr TI DATA_DIM = OBSERVATION_DIM + SPEC::OBSERVATION_DIM_PRIVILEGED_ACTUAL + ACTION_DIM + OBSERVATION_DIM + SPEC::OBSERVATION_DIM_PRIVILEGED_ACTUAL;
-        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, BATCH_SIZE, DATA_DIM>> observations_actions_next_observations;
-
-        template<typename SPEC::TI DIM>
-        using OANO_VIEW = typename decltype(observations_actions_next_observations)::template VIEW<BATCH_SIZE, DIM>;
-
-        OANO_VIEW<OBSERVATION_DIM> observations;
-        OANO_VIEW<SPEC::OBSERVATION_DIM_PRIVILEGED> observations_privileged;
-        OANO_VIEW<ACTION_DIM> actions;
-        OANO_VIEW<SPEC::OBSERVATION_DIM_PRIVILEGED + ACTION_DIM> observations_and_actions;
-        OANO_VIEW<OBSERVATION_DIM> next_observations;
-        OANO_VIEW<SPEC::OBSERVATION_DIM_PRIVILEGED> next_observations_privileged;
-
-        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, 1, BATCH_SIZE>> rewards;
-        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<bool, TI, 1, BATCH_SIZE>> terminated;
-        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<bool, TI, 1, BATCH_SIZE>> truncated;
+    template <auto T_N_EPISODES, auto T_STEP_LIMIT>
+    struct Specification{
+        constexpr static auto N_EPISODES = T_N_EPISODES;
+        constexpr static auto STEP_LIMIT = T_STEP_LIMIT;
     };
-
-    template<typename SPEC>
-    struct EpisodeStats{
-        using T = typename SPEC::T;
-        using TI = typename SPEC::TI;
-        static constexpr TI BUFFER_SIZE = SPEC::EPISODE_STATS_BUFFER_SIZE;
-        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, BUFFER_SIZE, 2>> data;
-
-        TI next_episode_i = 0;
-        template<typename SPEC::TI DIM>
-        using STATS_VIEW = typename decltype(data)::template VIEW<BUFFER_SIZE, DIM>;
-        STATS_VIEW<1> returns;
-        STATS_VIEW<1> steps;
+    template <typename T, typename TI, auto T_N_EPISODES>
+    struct Result{
+        constexpr static auto N_EPISODES = T_N_EPISODES;
+        T returns[N_EPISODES];
+        T returns_mean;
+        T returns_std;
+        TI episode_length[N_EPISODES];
+        T episode_length_mean;
+        T episode_length_std;
     };
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
-namespace rl_tools::rl::components{
-    template<typename T_SPEC>
-    struct OffPolicyRunner {
-        using SPEC = T_SPEC;
-        using T = typename SPEC::T;
-        using TI = typename SPEC::TI;
-        using ENVIRONMENT = typename SPEC::ENVIRONMENT;
-        using REPLAY_BUFFER_SPEC = replay_buffer::Specification<typename SPEC::T, typename SPEC::TI, SPEC::ENVIRONMENT::OBSERVATION_DIM, ENVIRONMENT::OBSERVATION_DIM_PRIVILEGED, SPEC::ASYMMETRIC_OBSERVATIONS, SPEC::ENVIRONMENT::ACTION_DIM, SPEC::REPLAY_BUFFER_CAPACITY, typename SPEC::CONTAINER_TYPE_TAG>;
-        using REPLAY_BUFFER_WITH_STATES_SPEC = replay_buffer::SpecificationWithStates<ENVIRONMENT, REPLAY_BUFFER_SPEC>;
-        using REPLAY_BUFFER_TYPE = ReplayBufferWithStates<REPLAY_BUFFER_WITH_STATES_SPEC>;
-        static constexpr TI N_ENVIRONMENTS = SPEC::N_ENVIRONMENTS;
-//        using POLICY_EVAL_BUFFERS = typename POLICY::template Buffers<N_ENVIRONMENTS>;
-
-        off_policy_runner::Parameters<T> parameters;
-        template<typename T_SPEC::TI T_BATCH_SIZE, typename T_CONTAINER_TYPE_TAG = typename T_SPEC::CONTAINER_TYPE_TAG>
-        using Batch = off_policy_runner::Batch<typename off_policy_runner::BatchSpecification<SPEC, T_BATCH_SIZE, T_CONTAINER_TYPE_TAG>>;
-
-        off_policy_runner::Buffers<SPEC> buffers;
-
-        // todo: change to "environments"
-        ENVIRONMENT envs[N_ENVIRONMENTS];
-        off_policy_runner::EpisodeStats<SPEC> episode_stats[N_ENVIRONMENTS];
-        REPLAY_BUFFER_TYPE replay_buffers[N_ENVIRONMENTS];
-
-        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<typename SPEC::ENVIRONMENT::State, TI, 1, N_ENVIRONMENTS>> states;
-        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, 1, N_ENVIRONMENTS>> episode_return;
-        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<TI, TI, 1, N_ENVIRONMENTS>> episode_step;
-        typename SPEC::CONTAINER_TYPE_TAG::template type<matrix::Specification<bool, TI, 1, N_ENVIRONMENTS>> truncated; // init to true !!
-#ifdef RL_TOOLS_DEBUG_RL_COMPONENTS_OFF_POLICY_RUNNER_CHECK_INIT
-        bool initialized = false;
+namespace rl_tools{
+
+    template<typename DEVICE, typename ENVIRONMENT, typename UI, typename POLICY, typename EVAL_STATE, typename OBSERVATION_MEAN_SPEC, typename OBSERVATION_STD_SPEC, typename POLICY_EVAL_BUFFERS, typename RNG>
+    bool evaluate_step(DEVICE& device, ENVIRONMENT& env, UI& ui, const POLICY& policy, EVAL_STATE& eval_state, Matrix<OBSERVATION_MEAN_SPEC>& observation_mean, Matrix<OBSERVATION_STD_SPEC>& observation_std, POLICY_EVAL_BUFFERS& policy_eval_buffers, RNG& rng) {
+        using T = typename POLICY::T;
+        using TI = typename DEVICE::index_t;
+        static_assert(ENVIRONMENT::ACTION_DIM == POLICY::OUTPUT_DIM || (2*ENVIRONMENT::ACTION_DIM == POLICY::OUTPUT_DIM));
+        constexpr bool STOCHASTIC_POLICY = ENVIRONMENT::ACTION_DIM*2 == POLICY::OUTPUT_DIM;
+        typename ENVIRONMENT::State state = eval_state.state;
+
+#ifndef RL_TOOLS_DISABLE_DYNAMIC_MEMORY_ALLOCATIONS
+        MatrixDynamic<matrix::Specification<T, TI, 1, ENVIRONMENT::ACTION_DIM * (STOCHASTIC_POLICY ? 2 : 1)>> action_full;
+        MatrixDynamic<matrix::Specification<T, TI, 1, ENVIRONMENT::OBSERVATION_DIM>> observation, observation_normalized;
+#else
+        MatrixStatic<matrix::Specification<T, TI, 1, ENVIRONMENT::ACTION_DIM * (STOCHASTIC_POLICY ? 2 : 1)>> action_full;
+        MatrixStatic<matrix::Specification<T, TI, 1, ENVIRONMENT::OBSERVATION_DIM>> observation, observation_normalized;
 #endif
-    };
+        malloc(device, observation);
+        malloc(device, observation_normalized);
+        malloc(device, action_full);
+        observe(device, env, state, observation, rng);
+        normalize(device, observation_mean, observation_std, observation, observation_normalized);
+
+        auto action = view(device, action_full, matrix::ViewSpec<1, ENVIRONMENT::ACTION_DIM>{});
+        evaluate(device, policy, observation_normalized, action_full, policy_eval_buffers, rng);
+
+        if constexpr(STOCHASTIC_POLICY){ // todo: This is a special case for SAC, will be uneccessary once (https://github.com/rl-tools/rl-tools/blob/72a59eabf4038502c3be86a4f772bd72526bdcc8/TODO.md?plain=1#L22) is implemented
+            for(TI action_i=0; action_i<ENVIRONMENT::ACTION_DIM; action_i++){
+                    set(action, 0, action_i, math::tanh<T>(device.math, get(action, 0, action_i)));
+            }
+        }
+        typename ENVIRONMENT::State next_state;
+        T dt = step(device, env, state, action, next_state, rng);
+        set_state(device, env, ui, state);
+        set_action(device, env, ui, action);
+        render(device, env, ui);
+        T r = reward(device, env, state, action, next_state, rng);
+        state = next_state;
+        eval_state.episode_return += r;
+        eval_state.episode_step += 1;
+        eval_state.state = state;
+        free(device, observation);
+        free(device, observation_normalized);
+        free(device, action_full);
+        return terminated(device, env, state, rng);
+    }
+    template<typename DEVICE, typename ENVIRONMENT, typename UI, typename POLICY, typename SPEC, typename OBSERVATION_MEAN_SPEC, typename OBSERVATION_STD_SPEC, typename POLICY_EVALUATION_BUFFERS, typename RNG>
+    auto evaluate(DEVICE& device, ENVIRONMENT& env, UI& ui, const POLICY& policy, const typename ENVIRONMENT::State initial_state, const SPEC& eval_spec_tag, Matrix<OBSERVATION_MEAN_SPEC>& observation_mean, Matrix<OBSERVATION_STD_SPEC>& observation_std, POLICY_EVALUATION_BUFFERS& policy_evaluation_buffers, RNG& rng) {
+        using T = typename POLICY::T;
+        using TI = typename DEVICE::index_t;
+        rl::utils::evaluation::State<T, TI, typename ENVIRONMENT::State> state;
+        state.state = initial_state;
+        state.episode_return = 0;
+        state.episode_step = 0;
+        for (TI i = 0; i < SPEC::STEP_LIMIT; i++) {
+            if(evaluate_step(device, env, ui, policy, state, observation_mean, observation_std, policy_evaluation_buffers, rng)){
+                break;
+            }
+        }
+        return state;
+    }
+    template<typename DEVICE, typename ENVIRONMENT, typename UI, typename POLICY, typename RNG, typename SPEC, typename OBSERVATION_MEAN_SPEC, typename OBSERVATION_STD_SPEC, typename POLICY_EVALUATION_BUFFERS>
+    auto evaluate(DEVICE& device, ENVIRONMENT& env, UI& ui, const POLICY& policy, const SPEC& eval_spec_tag, Matrix<OBSERVATION_MEAN_SPEC>& observation_mean, Matrix<OBSERVATION_STD_SPEC>& observation_std, POLICY_EVALUATION_BUFFERS& policy_evaluation_buffers, RNG &rng, bool deterministic = false){
+        using T = typename POLICY::T;
+        using TI = typename DEVICE::index_t;
+        static_assert(ENVIRONMENT::OBSERVATION_DIM == POLICY::INPUT_DIM, "Observation and policy input dimensions must match");
+        static_assert(ENVIRONMENT::ACTION_DIM == POLICY::OUTPUT_DIM || (2*ENVIRONMENT::ACTION_DIM == POLICY::OUTPUT_DIM), "Action and policy output dimensions must match");
+        static bool STOCHASTIC_POLICY = ENVIRONMENT::ACTION_DIM == 2*POLICY::OUTPUT_DIM;
+        rl::utils::evaluation::Result<T, TI, SPEC::N_EPISODES> results;
+        results.returns_mean = 0;
+        results.returns_std = 0;
+        results.episode_length_mean = 0;
+        results.episode_length_std = 0;
+        for(TI i = 0; i < SPEC::N_EPISODES; i++) {
+            typename ENVIRONMENT::State initial_state;
+            if(deterministic) {
+                rl_tools::initial_state(device, env, initial_state);
+            }
+            else{
+                sample_initial_state(device, env, initial_state, rng);
+            }
+            auto final_state = evaluate(device, env, ui, policy, initial_state, eval_spec_tag, observation_mean, observation_std, policy_evaluation_buffers, rng);
+            results.returns[i] = final_state.episode_return;
+            results.returns_mean += final_state.episode_return;
+            results.returns_std += final_state.episode_return*final_state.episode_return;
+            results.episode_length[i] = final_state.episode_step;
+            results.episode_length_mean += final_state.episode_step;
+            results.episode_length_std += final_state.episode_step*final_state.episode_step;
+        }
+        results.returns_mean /= SPEC::N_EPISODES;
+        results.returns_std = math::sqrt(device.math, results.returns_std/SPEC::N_EPISODES - results.returns_mean*results.returns_mean);
+        results.episode_length_mean /= SPEC::N_EPISODES;
+        results.episode_length_std = math::sqrt(device.math, results.episode_length_std/SPEC::N_EPISODES - results.episode_length_mean*results.episode_length_mean);
+        return results;
+    }
+    template<typename DEVICE, typename ENVIRONMENT, typename UI, typename POLICY, typename RNG, typename SPEC, typename POLICY_EVALUATION_BUFFERS>
+    auto evaluate(DEVICE& device, ENVIRONMENT& env, UI& ui, const POLICY& policy, const SPEC& eval_spec_tag, POLICY_EVALUATION_BUFFERS& policy_evaluation_buffers, RNG &rng, bool deterministic = false){
+        using T = typename POLICY::T;
+        using TI = typename DEVICE::index_t;
+        MatrixDynamic<matrix::Specification<T, TI, 1, ENVIRONMENT::OBSERVATION_DIM>> observation_mean;
+        MatrixDynamic<matrix::Specification<T, TI, 1, ENVIRONMENT::OBSERVATION_DIM>> observation_std;
+        malloc(device, observation_mean);
+        malloc(device, observation_std);
+        set_all(device, observation_mean, 0);
+        set_all(device, observation_std, 1);
+        auto results = evaluate(device, env, ui, policy, eval_spec_tag, observation_mean, observation_std, policy_evaluation_buffers, rng, deterministic);
+        free(device, observation_mean);
+        free(device, observation_std);
+        return results;
+    }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h`

 * *Files 3% similar despite different names*

```diff
@@ -21,34 +21,34 @@
         using DEVICE = devices::CPU<DEV_SPEC>;
         using TI = typename DEVICE::index_t;
         std::vector<std::thread> threads;
 
         constexpr TI NUM_THREADS = get_num_threads(typename DEVICE::EXECUTION_HINTS());
 
         if(NUM_THREADS > 1){
-            RNG rngs[SPEC::N_ENVIRONMENTS];
+            RNG rngs[SPEC::PARAMETERS::N_ENVIRONMENTS];
             auto base = random::uniform_int_distribution(typename DEV_SPEC::RANDOM(), 0, 1000000, rng);
-            for (TI env_i = 0; env_i < SPEC::N_ENVIRONMENTS; env_i++) {
+            for (TI env_i = 0; env_i < SPEC::PARAMETERS::N_ENVIRONMENTS; env_i++) {
                 rngs[env_i] = rl_tools::random::default_engine(typename DEV_SPEC::RANDOM(), base + env_i);
             }
 
             for (TI thread_i = 0; thread_i < NUM_THREADS; thread_i++) {
                 threads.emplace_back([NUM_THREADS, &device, thread_i, &runner, &rngs](){
-                    for (TI env_i = thread_i; env_i < SPEC::N_ENVIRONMENTS; env_i += NUM_THREADS) {
+                    for (TI env_i = thread_i; env_i < SPEC::PARAMETERS::N_ENVIRONMENTS; env_i += NUM_THREADS) {
                         prologue_per_env(device, runner, rngs[env_i], env_i);
                     }
                 });
             }
 
             for (auto& thread : threads) {
                 thread.join();
             }
         }
         else{
-            for (TI env_i = 0; env_i < SPEC::N_ENVIRONMENTS; env_i++) {
+            for (TI env_i = 0; env_i < SPEC::PARAMETERS::N_ENVIRONMENTS; env_i++) {
                 prologue_per_env(device, runner, rng, env_i);
             }
         }
 
     }
 
     template<typename DEV_SPEC, typename SPEC, typename RNG>
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h`

 * *Files 4% similar despite different names*

```diff
@@ -15,31 +15,31 @@
             using T = typename RUNNER_SPEC::T;
             using TI = typename RUNNER_SPEC::TI;
             static_assert(decltype(batch.observations)::COL_PITCH == 1);
             static_assert(decltype(batch.actions)::COL_PITCH == 1);
             static_assert(decltype(batch.next_observations)::COL_PITCH == 1);
             // rng
             constexpr auto rand_max = 4294967296ULL;
-            static_assert(rand_max / RUNNER_SPEC::N_ENVIRONMENTS > 100);
-            static_assert(rand_max / RUNNER_SPEC::REPLAY_BUFFER_CAPACITY > 100); // so that the distribution is not skewed too much towards the remainder values
+            static_assert(rand_max / RUNNER_SPEC::PARAMETERS::N_ENVIRONMENTS > 100);
+            static_assert(rand_max / RUNNER_SPEC::PARAMETERS::REPLAY_BUFFER_CAPACITY > 100); // so that the distribution is not skewed too much towards the remainder values
 
             curandState rng_state;
 
             TI batch_step_i = threadIdx.x + blockIdx.x * blockDim.x;
             curand_init(rng, batch_step_i, 0, &rng_state);
 
-            typename DEVICE::index_t env_i = DETERMINISTIC ? 0 : curand(&rng_state) % RUNNER_SPEC::N_ENVIRONMENTS;
+            typename DEVICE::index_t env_i = DETERMINISTIC ? 0 : curand(&rng_state) % RUNNER_SPEC::PARAMETERS::N_ENVIRONMENTS;
             auto& replay_buffer = runner->replay_buffers[env_i];
             static_assert(decltype(replay_buffer.observations)::COL_PITCH == 1);
             static_assert(decltype(replay_buffer.actions)::COL_PITCH == 1);
             static_assert(decltype(replay_buffer.next_observations)::COL_PITCH == 1);
 
             if(batch_step_i < BATCH_SPEC::BATCH_SIZE){
                 set(batch.observations, batch_step_i, 0, get(replay_buffer.observations, batch_step_i, 0));
-                typename DEVICE::index_t sample_index_max = (replay_buffer.full ? RUNNER_SPEC::REPLAY_BUFFER_CAPACITY : replay_buffer.position);
+                typename DEVICE::index_t sample_index_max = (replay_buffer.full ? RUNNER_SPEC::PARAMETERS::REPLAY_BUFFER_CAPACITY : replay_buffer.position);
 #ifdef RL_TOOLS_DEBUG_DEVICE_CUDA_CHECK_BOUNDS
                 if(sample_index_max < 1){
                     printf("sample_index_max: %d\n", sample_index_max);
                     assert(sample_index_max > 0);
                 }
 #endif
                 typename DEVICE::index_t sample_index = DETERMINISTIC ? batch_step_i : curand(&rng_state) % sample_index_max;
@@ -64,61 +64,63 @@
         void prologue_kernel(DEVICE device, rl::components::OffPolicyRunner<SPEC>* runner, RNG rng) {
             using T = typename SPEC::T;
             using TI = typename SPEC::TI;
             // if the episode is done (step limit activated for STEP_LIMIT > 0) or if the step is the first step for this runner, reset the environment
             TI env_i = threadIdx.x + blockIdx.x * blockDim.x;
             curandState rng_state;
             curand_init(rng, env_i, 0, &rng_state);
-            if(env_i < SPEC::N_ENVIRONMENTS){
+            if(env_i < SPEC::PARAMETERS::N_ENVIRONMENTS){
                 prologue_per_env(device, *runner, rng_state, env_i);
             }
         }
         template<typename DEV_SPEC, typename SPEC, typename RNG>
         void prologue(devices::CUDA<DEV_SPEC>& device, rl::components::OffPolicyRunner<SPEC>* runner, RNG &rng) {
             using DEVICE = devices::CUDA<DEV_SPEC>;
             using T = typename SPEC::T;
             using TI = typename SPEC::TI;
             constexpr TI BLOCKSIZE_COLS = 32;
-            constexpr TI N_BLOCKS_COLS = RL_TOOLS_DEVICES_CUDA_CEIL(SPEC::N_ENVIRONMENTS, BLOCKSIZE_COLS);
+            constexpr TI N_BLOCKS_COLS = RL_TOOLS_DEVICES_CUDA_CEIL(SPEC::PARAMETERS::N_ENVIRONMENTS, BLOCKSIZE_COLS);
             dim3 grid(N_BLOCKS_COLS);
             dim3 block(BLOCKSIZE_COLS);
             devices::cuda::TAG<DEVICE, true> tag_device{};
             prologue_kernel<<<grid, block, 0, device.stream>>>(tag_device, runner, rng);
             check_status(device);
         }
         template<typename DEV_SPEC, typename SPEC, typename POLICY, typename RNG>
-        void interlude(devices::CUDA<DEV_SPEC>& device, rl::components::OffPolicyRunner<SPEC>& runner, POLICY& policy, typename POLICY::template Buffer<SPEC::N_ENVIRONMENTS>& policy_eval_buffers, RNG& rng) {
+        void interlude(devices::CUDA<DEV_SPEC>& device, rl::components::OffPolicyRunner<SPEC>& runner, POLICY& policy, typename POLICY::template Buffer<SPEC::PARAMETERS::N_ENVIRONMENTS>& policy_eval_buffers, RNG& rng) {
             // runner struct should be on the CPU while its buffers should be on the GPU
             evaluate(device, policy, runner.buffers.observations, runner.buffers.actions, policy_eval_buffers, rng);
         }
 
-        template<typename DEVICE, typename SPEC, typename RNG>
+        template<typename DEVICE, typename SPEC, typename POLICY, typename RNG>
         __global__
-        void epilogue_kernel(DEVICE device, rl::components::OffPolicyRunner<SPEC>* runner, RNG rng) {
+        void epilogue_kernel(DEVICE device, rl::components::OffPolicyRunner<SPEC>* runner, POLICY* policy, RNG rng) {
             using T = typename SPEC::T;
             using TI = typename SPEC::TI;
 
             TI env_i = threadIdx.x + blockIdx.x * blockDim.x;
             curandState rng_state;
             curand_init(rng, env_i, 0, &rng_state);
-            if(env_i < SPEC::N_ENVIRONMENTS){
-                epilogue_per_env(device, *runner, rng_state, env_i);
+            if(env_i < SPEC::PARAMETERS::N_ENVIRONMENTS){
+                POLICY dummy_policy;
+                epilogue_per_env(device, *runner, dummy_policy, rng_state, env_i);
             }
         }
-        template<typename DEV_SPEC, typename SPEC, typename RNG>
-        void epilogue(devices::CUDA<DEV_SPEC>& device, rl::components::OffPolicyRunner<SPEC>* runner, RNG& rng) {
+        template<typename DEV_SPEC, typename SPEC, typename POLICY, typename RNG>
+        void epilogue(devices::CUDA<DEV_SPEC>& device, rl::components::OffPolicyRunner<SPEC>* runner, const POLICY& policy, RNG& rng) {
             using DEVICE = devices::CUDA<DEV_SPEC>;
             using T = typename SPEC::T;
             using TI = typename SPEC::TI;
             constexpr TI BLOCKSIZE_COLS = 32;
-            constexpr TI N_BLOCKS_COLS = RL_TOOLS_DEVICES_CUDA_CEIL(SPEC::N_ENVIRONMENTS, BLOCKSIZE_COLS);
+            constexpr TI N_BLOCKS_COLS = RL_TOOLS_DEVICES_CUDA_CEIL(SPEC::PARAMETERS::N_ENVIRONMENTS, BLOCKSIZE_COLS);
             dim3 grid(N_BLOCKS_COLS);
             dim3 block(BLOCKSIZE_COLS);
             devices::cuda::TAG<DEVICE, true> tag_device{};
-            epilogue_kernel<<<grid, block, 0, device.stream>>>(tag_device, runner, rng);
+            POLICY dummy_policy; // just for type inference
+            epilogue_kernel<<<grid, block, 0, device.stream>>>(tag_device, runner, &dummy_policy, rng);
             check_status(device);
         }
     }
     template <typename DEV_SPEC, typename SPEC, typename BATCH_SPEC, typename RNG, bool DETERMINISTIC = false>
     void gather_batch(devices::CUDA<DEV_SPEC>& device, const rl::components::OffPolicyRunner<SPEC>* runner, rl::components::off_policy_runner::Batch<BATCH_SPEC>& batch, RNG rng){
         static_assert(utils::typing::is_same_v<RNG, random::cuda::RNG>);
         using DEVICE = devices::CUDA<DEV_SPEC>;
@@ -130,38 +132,38 @@
         constexpr TI N_BLOCKS_COLS = RL_TOOLS_DEVICES_CUDA_CEIL(BATCH_SIZE, BLOCKSIZE_COLS);
         dim3 bias_grid(N_BLOCKS_COLS);
         dim3 bias_block(BLOCKSIZE_COLS);
         rl::components::off_policy_runner::gather_batch_kernel<DEVICE, SPEC, BATCH_SPEC, RNG, DETERMINISTIC><<<bias_grid, bias_block, 0, device.stream>>>(runner, batch, rng);
         check_status(device);
     }
     template<typename DEV_SPEC, typename SPEC, typename POLICY, typename RNG>
-    void step(devices::CUDA<DEV_SPEC>& device, rl::components::OffPolicyRunner<SPEC>& runner, POLICY& policy_host, typename POLICY::template Buffer<SPEC::N_ENVIRONMENTS>& policy_eval_buffers_host, RNG &rng){
+    void step(devices::CUDA<DEV_SPEC>& device, rl::components::OffPolicyRunner<SPEC>& runner, POLICY& policy_host, typename POLICY::template Buffer<SPEC::PARAMETERS::N_ENVIRONMENTS>& policy_eval_buffers_host, RNG &rng){
         utils::assert_exit(device, false, "please use the step function signature passing a host and device (GPU) version of the runner");
     }
     template<typename DEV_SPEC, typename HOST_SPEC, typename DEVICE_SPEC, typename POLICY, typename RNG>
-    void step(devices::CUDA<DEV_SPEC>& device, rl::components::OffPolicyRunner<HOST_SPEC>& runner_host, rl::components::OffPolicyRunner<DEVICE_SPEC>* runner_device, POLICY& policy_host, typename POLICY::template Buffer<HOST_SPEC::N_ENVIRONMENTS>& policy_eval_buffers_host, RNG &rng){
+    void step(devices::CUDA<DEV_SPEC>& device, rl::components::OffPolicyRunner<HOST_SPEC>& runner_host, rl::components::OffPolicyRunner<DEVICE_SPEC>* runner_device, POLICY& policy_host, typename POLICY::template Buffer<HOST_SPEC::PARAMETERS::N_ENVIRONMENTS>& policy_eval_buffers_host, RNG &rng){
         using DEVICE = devices::CUDA<DEV_SPEC>;
 #ifdef RL_TOOLS_DEBUG_RL_COMPONENTS_OFF_POLICY_RUNNER_CHECK_INIT
         utils::assert_exit(device, runner_host.initialized, "OffPolicyRunner not initialized");
 #endif
         static_assert(POLICY::INPUT_DIM == HOST_SPEC::ENVIRONMENT::OBSERVATION_DIM, "The policy's input dimension must match the environment's observation dimension.");
         static_assert(POLICY::INPUT_DIM == DEVICE_SPEC::ENVIRONMENT::OBSERVATION_DIM, "The policy's input dimension must match the environment's observation dimension.");
-        static_assert(POLICY::OUTPUT_DIM == (HOST_SPEC::ENVIRONMENT::ACTION_DIM * (HOST_SPEC::STOCHASTIC_POLICY ? 2 : 1)), "The policy's output dimension must match the environment's action dimension.");
-        static_assert(POLICY::OUTPUT_DIM == (DEVICE_SPEC::ENVIRONMENT::ACTION_DIM * (DEVICE_SPEC::STOCHASTIC_POLICY ? 2 : 1)), "The policy's output dimension must match the environment's action dimension.");
+        static_assert(POLICY::OUTPUT_DIM == (HOST_SPEC::ENVIRONMENT::ACTION_DIM * (HOST_SPEC::PARAMETERS::STOCHASTIC_POLICY ? 2 : 1)), "The policy's output dimension must match the environment's action dimension.");
+        static_assert(POLICY::OUTPUT_DIM == (DEVICE_SPEC::ENVIRONMENT::ACTION_DIM * (DEVICE_SPEC::PARAMETERS::STOCHASTIC_POLICY ? 2 : 1)), "The policy's output dimension must match the environment's action dimension.");
         // todo: increase efficiency by removing the double observation of each state
         using T = typename DEVICE_SPEC::T;
         using TI = typename DEVICE_SPEC::TI;
         using ENVIRONMENT = typename DEVICE_SPEC::ENVIRONMENT;
 
         rng = random::next(typename DEVICE::SPEC::RANDOM{}, rng);
         rl::components::off_policy_runner::prologue(device, runner_device, rng);
-        rl::components::off_policy_runner::interlude(device, runner_host, policy_host, policy_eval_buffers_host);
+        rl::components::off_policy_runner::interlude(device, runner_host, policy_host, policy_eval_buffers_host, rng);
 //        evaluate(device, policy_host, runner_host.buffers.observations, runner_host.buffers.actions, policy_eval_buffers_host, rng);
         rng = random::next(typename DEVICE::SPEC::RANDOM{}, rng);
-        rl::components::off_policy_runner::epilogue(device, runner_device, rng);
+        rl::components::off_policy_runner::epilogue(device, runner_device, policy_host, rng);
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 #include "operations_generic.h"
 
 
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h`

 * *Files 8% similar despite different names*

```diff
@@ -14,37 +14,37 @@
 namespace rl_tools{
     template <typename DEVICE, typename SPEC>
     void malloc(DEVICE& device, rl::components::off_policy_runner::Buffers<SPEC>& buffers) {
         malloc(device, buffers.observations);
         malloc(device, buffers.actions);
         malloc(device, buffers.next_observations);
 
-        if constexpr(SPEC::ASYMMETRIC_OBSERVATIONS){
+        if constexpr(SPEC::PARAMETERS::ASYMMETRIC_OBSERVATIONS){
             malloc(device, buffers.observations_privileged);
             malloc(device, buffers.next_observations_privileged);
         }
         else{
             buffers.observations_privileged = buffers.observations;
             buffers.next_observations_privileged = buffers.next_observations;
         }
     }
     template <typename DEVICE, typename SPEC>
     void malloc(DEVICE& device, rl::components::off_policy_runner::EpisodeStats<SPEC>& episode_stats) {
         malloc(device, episode_stats.data);
-        episode_stats.returns = view<DEVICE, typename decltype(episode_stats.data)::SPEC, SPEC::EPISODE_STATS_BUFFER_SIZE, 1>(device, episode_stats.data, 0, 0);
-        episode_stats.steps   = view<DEVICE, typename decltype(episode_stats.data)::SPEC, SPEC::EPISODE_STATS_BUFFER_SIZE, 1>(device, episode_stats.data, 0, 1);
+        episode_stats.returns = view<DEVICE, typename decltype(episode_stats.data)::SPEC, SPEC::PARAMETERS::EPISODE_STATS_BUFFER_SIZE, 1>(device, episode_stats.data, 0, 0);
+        episode_stats.steps   = view<DEVICE, typename decltype(episode_stats.data)::SPEC, SPEC::PARAMETERS::EPISODE_STATS_BUFFER_SIZE, 1>(device, episode_stats.data, 0, 1);
     }
     template<typename DEVICE, typename SPEC>
     void malloc(DEVICE& device, rl::components::OffPolicyRunner<SPEC> &runner) {
         malloc(device, runner.buffers);
         malloc(device, runner.states);
         malloc(device, runner.episode_return);
         malloc(device, runner.episode_step);
         malloc(device, runner.truncated);
-        for (typename DEVICE::index_t env_i = 0; env_i < SPEC::N_ENVIRONMENTS; env_i++){
+        for (typename DEVICE::index_t env_i = 0; env_i < SPEC::PARAMETERS::N_ENVIRONMENTS; env_i++){
             malloc(device, runner.replay_buffers[env_i]);
             malloc(device, runner.episode_stats[env_i]);
         }
     }
     template <typename DEVICE, typename BATCH_SPEC>
     void malloc(DEVICE& device, rl::components::off_policy_runner::Batch<BATCH_SPEC>& batch) {
         using BATCH = rl::components::off_policy_runner::Batch<BATCH_SPEC>;
@@ -79,15 +79,15 @@
     template<typename DEVICE, typename SPEC>
     void free(DEVICE& device, rl::components::OffPolicyRunner<SPEC> &runner) {
         free(device, runner.buffers);
         free(device, runner.states);
         free(device, runner.episode_return);
         free(device, runner.episode_step);
         free(device, runner.truncated);
-        for (typename DEVICE::index_t env_i = 0; env_i < SPEC::N_ENVIRONMENTS; env_i++){
+        for (typename DEVICE::index_t env_i = 0; env_i < SPEC::PARAMETERS::N_ENVIRONMENTS; env_i++){
             free(device, runner.replay_buffers[env_i]);
             free(device, runner.episode_stats[env_i]);
         }
     }
     template <typename DEVICE, typename SPEC>
     void free(DEVICE& device, rl::components::off_policy_runner::Batch<SPEC>& batch) {
         free(device, batch.observations_actions_next_observations);
@@ -98,44 +98,44 @@
         batch.next_observations.           _data = nullptr;
         batch.next_observations_privileged._data = nullptr;
         free(device, batch.rewards);
         free(device, batch.terminated);
         free(device, batch.truncated);
     }
     template<typename DEVICE, typename SPEC>
-    void init(DEVICE& device, rl::components::OffPolicyRunner<SPEC> &runner, typename SPEC::ENVIRONMENT envs[SPEC::N_ENVIRONMENTS]) {
+    void init(DEVICE& device, rl::components::OffPolicyRunner<SPEC> &runner, typename SPEC::ENVIRONMENT envs[SPEC::PARAMETERS::N_ENVIRONMENTS]) {
         set_all(device, runner.truncated, true);
-        for (typename DEVICE::index_t env_i = 0; env_i < SPEC::N_ENVIRONMENTS; env_i++){
+        for (typename DEVICE::index_t env_i = 0; env_i < SPEC::PARAMETERS::N_ENVIRONMENTS; env_i++){
             init(device, runner.replay_buffers[env_i]);
             runner.envs[env_i] = envs[env_i];
         }
 #ifdef RL_TOOLS_DEBUG_RL_COMPONENTS_OFF_POLICY_RUNNER_CHECK_INIT
         runner.initialized = true;
 #endif
     }
     namespace rl::components::off_policy_runner{
         template<typename DEVICE, typename SPEC, typename RNG>
         void prologue(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, RNG &rng) {
             using TI = typename DEVICE::index_t;
-            for (TI env_i = 0; env_i < SPEC::N_ENVIRONMENTS; env_i++) {
+            for (TI env_i = 0; env_i < SPEC::PARAMETERS::N_ENVIRONMENTS; env_i++) {
                 prologue_per_env(device, runner, rng, env_i);
             }
         }
         template<typename DEVICE, typename SPEC, typename POLICY, typename POLICY_BUFFERS, typename RNG>
         void interlude(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, POLICY &policy, POLICY_BUFFERS& policy_eval_buffers, RNG& rng){
             using TI = typename DEVICE::index_t;
             constexpr TI BATCH_SIZE = decltype(runner.buffers.actions)::ROWS;
             auto action_view = view(device, runner.buffers.actions, matrix::ViewSpec<BATCH_SIZE, POLICY::OUTPUT_DIM>{});
             evaluate(device, policy, runner.buffers.observations, action_view, policy_eval_buffers, rng);
         }
 
         template<typename DEVICE, typename SPEC, typename POLICY, typename RNG>
         void epilogue(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, const POLICY& policy, RNG& rng){
             using TI = typename DEVICE::index_t;
-            for (TI env_i = 0; env_i < SPEC::N_ENVIRONMENTS; env_i++){
+            for (TI env_i = 0; env_i < SPEC::PARAMETERS::N_ENVIRONMENTS; env_i++){
                 epilogue_per_env(device, runner, policy, rng, env_i);
             }
         }
     }
     template<typename DEVICE, typename SPEC, typename POLICY, typename POLICY_BUFFERS, typename RNG>
     void step(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, POLICY& policy, POLICY_BUFFERS& policy_eval_buffers, RNG &rng){
 #ifdef RL_TOOLS_DEBUG_RL_COMPONENTS_OFF_POLICY_RUNNER_CHECK_INIT
@@ -193,15 +193,15 @@
     void gather_batch(DEVICE& device, const rl::components::OffPolicyRunner<SPEC>& runner, rl::components::off_policy_runner::Batch<BATCH_SPEC>& batch, RNG& rng) {
         static_assert(utils::typing::is_same_v<SPEC, typename BATCH_SPEC::SPEC>);
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         using RUNNER = rl::components::OffPolicyRunner<SPEC>;
         constexpr typename DEVICE::index_t BATCH_SIZE = BATCH_SPEC::BATCH_SIZE;
         for(typename DEVICE::index_t batch_step_i=0; batch_step_i < BATCH_SIZE; batch_step_i++) {
-            typename DEVICE::index_t env_i = DETERMINISTIC ? 0 : random::uniform_int_distribution(typename DEVICE::SPEC::RANDOM(), (typename DEVICE::index_t) 0, SPEC::N_ENVIRONMENTS - 1, rng);
+            typename DEVICE::index_t env_i = DETERMINISTIC ? 0 : random::uniform_int_distribution(typename DEVICE::SPEC::RANDOM(), (typename DEVICE::index_t) 0, SPEC::PARAMETERS::N_ENVIRONMENTS - 1, rng);
             auto& replay_buffer = runner.replay_buffers[env_i];
             gather_batch<DEVICE, typename RUNNER::REPLAY_BUFFER_SPEC, BATCH_SPEC, RNG, DETERMINISTIC>(device, replay_buffer, batch, batch_step_i, rng);
         }
     }
 //    template<typename SOURCE_DEVICE, typename TARGET_DEVICE,  typename SOURCE_SPEC, typename TARGET_SPEC>
 //    void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, const  rl::components::off_policy_runner::Batch<SOURCE_SPEC>& source, nn_models::mlp::NeuralNetworkBuffersForwardBackward<TARGET_SPEC>& target){
 //        copy(source_device, target_device, (nn_models::mlp::NeuralNetworkBuffers<SOURCE_SPEC>&)source, (nn_models::mlp::NeuralNetworkBuffers<TARGET_SPEC>&)target);
@@ -228,15 +228,15 @@
     template <typename SOURCE_DEVICE, typename TARGET_DEVICE, typename SOURCE_SPEC, typename TARGET_SPEC>
     void copy(SOURCE_DEVICE& source_device, TARGET_DEVICE& target_device, rl::components::OffPolicyRunner<SOURCE_SPEC>& source, rl::components::OffPolicyRunner<TARGET_SPEC>& target){
         copy(source_device, target_device, source.buffers, target.buffers);
         copy(source_device, target_device, source.states, target.states);
         copy(source_device, target_device, source.episode_return, target.episode_return);
         copy(source_device, target_device, source.episode_step, target.episode_step);
         copy(source_device, target_device, source.truncated, target.truncated);
-        for (typename SOURCE_DEVICE::index_t env_i = 0; env_i < SOURCE_SPEC::N_ENVIRONMENTS; env_i++){
+        for (typename SOURCE_DEVICE::index_t env_i = 0; env_i < SOURCE_SPEC::PARAMETERS::N_ENVIRONMENTS; env_i++){
             copy(source_device, target_device, source.replay_buffers[env_i], target.replay_buffers[env_i]);
             copy(source_device, target_device, source.episode_stats[env_i], target.episode_stats[env_i]);
             target.envs[env_i] = source.envs[env_i];
         }
 #ifdef RL_TOOLS_DEBUG_RL_COMPONENTS_OFF_POLICY_RUNNER_CHECK_INIT
         target.initialized = source.initialized;
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h`

 * *Files 3% similar despite different names*

```diff
@@ -10,70 +10,69 @@
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         // if the episode is done (step limit activated for STEP_LIMIT > 0) or if the step is the first step for this runner, reset the environment
         using RUNNER = rl::components::OffPolicyRunner<SPEC>;
         using ENVIRONMENT = typename SPEC::ENVIRONMENT;
         auto& env = runner.envs[env_i];
         auto& state = get(runner.states, 0, env_i);
-        static_assert(!SPEC::COLLECT_EPISODE_STATS || SPEC::EPISODE_STATS_BUFFER_SIZE > 1);
+        static_assert(!SPEC::PARAMETERS::COLLECT_EPISODE_STATS || SPEC::PARAMETERS::EPISODE_STATS_BUFFER_SIZE > 1);
         if (get(runner.truncated, 0, env_i)){
-            if constexpr(SPEC::COLLECT_EPISODE_STATS){
+            if constexpr(SPEC::PARAMETERS::COLLECT_EPISODE_STATS){
                 // todo: the first episode is always zero steps and zero return because the initialization is done by setting truncated to true
                 auto& episode_stats = runner.episode_stats[env_i];
                 TI next_episode_i = episode_stats.next_episode_i;
                 if(next_episode_i > 0){
                     TI episode_i = next_episode_i - 1;
                     set(episode_stats.returns, episode_i, 0, get(runner.episode_return, 0, env_i));
                     set(episode_stats.steps  , episode_i, 0, get(runner.episode_step  , 0, env_i));
-                    episode_i = (episode_i + 1) % SPEC::EPISODE_STATS_BUFFER_SIZE;
+                    episode_i = (episode_i + 1) % SPEC::PARAMETERS::EPISODE_STATS_BUFFER_SIZE;
                     next_episode_i = episode_i + 1;
                 }
                 else{
                     next_episode_i = 1;
                 }
                 episode_stats.next_episode_i = next_episode_i;
             }
             sample_initial_state(device, env, state, rng);
             set(runner.episode_step, 0, env_i, 0);
             set(runner.episode_return, 0, env_i, 0);
         }
         auto observation            = view<DEVICE, typename decltype(runner.buffers.observations           )::SPEC, 1, ENVIRONMENT::OBSERVATION_DIM           >(device, runner.buffers.observations           , env_i, 0);
         auto observation_privileged = view<DEVICE, typename decltype(runner.buffers.observations_privileged)::SPEC, 1, SPEC::OBSERVATION_DIM_PRIVILEGED>(device, runner.buffers.observations_privileged, env_i, 0);
         observe(device, env, state, observation, rng);
-        if constexpr(SPEC::ASYMMETRIC_OBSERVATIONS){
+        if constexpr(SPEC::PARAMETERS::ASYMMETRIC_OBSERVATIONS){
             observe_privileged(device, env, state, observation_privileged, rng);
         }
     }
     template<typename DEVICE, typename SPEC, typename POLICY, typename RNG>
     RL_TOOLS_FUNCTION_PLACEMENT auto process_and_get_action(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, const POLICY& policy, RNG &rng, typename DEVICE::index_t env_i) {
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         using ENVIRONMENT = typename SPEC::ENVIRONMENT;
         static constexpr bool STOCHASTIC_POLICY = POLICY::OUTPUT_DIM == ENVIRONMENT::ACTION_DIM * 2;
         if constexpr(STOCHASTIC_POLICY){
             for (TI i = 0; i < ENVIRONMENT::ACTION_DIM; i++){
                 T log_std = get(runner.buffers.actions, env_i, ENVIRONMENT::ACTION_DIM+i);
-                T log_std_clip = math::clamp<T>(device.math, log_std, -20, 2); // todo: absorb this into the policy
+                T log_std_clip = math::clamp<T>(device.math, log_std, (T)-20, (T)2); // todo: absorb this into the policy
                 T std = math::exp(typename DEVICE::SPEC::MATH{}, log_std_clip);
                 T mu = get(runner.buffers.actions, env_i, i);
                 T action_noisy = random::normal_distribution::sample(typename DEVICE::SPEC::RANDOM(), mu, std, rng);
-                static_assert(SPEC::ACTION_CLAMPING_TANH);
                 if constexpr(SPEC::ACTION_CLAMPING_TANH){
                     set(runner.buffers.actions, env_i, i, math::tanh<T>(device.math, action_noisy));
                 }
                 else{
-                    set(runner.buffers.actions, env_i, i, math::clamp<T>(device.math, action_noisy, -1, 1));
+                    set(runner.buffers.actions, env_i, i, math::clamp<T>(device.math, action_noisy, (T)-1, (T)1));
                 }
             }
             return view(device, runner.buffers.actions, matrix::ViewSpec<1, SPEC::ENVIRONMENT::ACTION_DIM>{}, env_i, 0);
         }
         else{
             for (TI i = 0; i < ENVIRONMENT::ACTION_DIM; i++){
                 T action_noisy = get(runner.buffers.actions, env_i, i) + random::normal_distribution::sample(typename DEVICE::SPEC::RANDOM(), (T) 0, runner.parameters.exploration_noise, rng);
-                set(runner.buffers.actions, env_i, i, math::clamp<T>(device.math, action_noisy, -1, 1));
+                set(runner.buffers.actions, env_i, i, math::clamp<T>(device.math, action_noisy, (T)-1, (T)1));
             }
             return view(device, runner.buffers.actions, matrix::ViewSpec<1, SPEC::ENVIRONMENT::ACTION_DIM>{}, env_i, 0);
 //            return row(device, runner.buffers.actions, env_i);
         }
 
     }
     template<typename DEVICE, typename SPEC, typename POLICY, typename RNG>
@@ -93,23 +92,23 @@
         auto action = process_and_get_action(device, runner, policy, rng, env_i);
 
         step(device, env, state, action, next_state, rng);
 
         T reward_value = reward(device, env, state, action, next_state, rng);
 
         observe(device, env, next_state, next_observation, rng);
-        if constexpr(SPEC::ASYMMETRIC_OBSERVATIONS) {
+        if constexpr(SPEC::PARAMETERS::ASYMMETRIC_OBSERVATIONS) {
             observe_privileged(device, env, next_state, next_observation_privileged, rng);
         }
 
         bool terminated_flag = terminated(device, env, next_state, rng);
         increment(runner.episode_step, 0, env_i, 1);
         increment(runner.episode_return, 0, env_i, reward_value);
         auto episode_step_i = get(runner.episode_step, 0, env_i);
-        bool truncated = terminated_flag || episode_step_i == SPEC::STEP_LIMIT;
+        bool truncated = terminated_flag || episode_step_i == SPEC::PARAMETERS::EPISODE_STEP_LIMIT;
         set(runner.truncated, 0, env_i, truncated);
         add(device, runner.replay_buffers[env_i], state, observation, observation_privileged, action, reward_value, next_state, next_observation, next_observation_privileged, terminated_flag, truncated);
 
         // state progression needs to come after the addition to the replay buffer because "observation" can point to the memory of runner_state.state (in the case of REQUIRES_OBSERVATION=false)
         state = next_state;
     }
 }
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h`

 * *Files 6% similar despite different names*

```diff
@@ -11,12 +11,13 @@
     template<typename T_CONFIG, typename T_NEXT = typename T_CONFIG::NEXT::template State<typename T_CONFIG::NEXT>>
     struct State: T_NEXT {
         using CONFIG = T_CONFIG;
         using NEXT = T_NEXT;
         std::chrono::high_resolution_clock::time_point start_time;
     };
 }
+RL_TOOLS_NAMESPACE_WRAPPER_END
 #endif
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         beast::flat_buffer buffer_;
     };
 
 
     class http_connection: public std::enable_shared_from_this<http_connection>
     {
     public:
-        http_connection(tcp::socket socket, State& state, std::string static_path): socket_(std::move(socket)), state(state), static_path(static_path){ }
+        http_connection(tcp::socket socket, State& state, std::string static_path): static_path(static_path), state(state), socket_(std::move(socket)){ }
         void start(){
             read_request();
             check_deadline();
         }
 
     private:
         std::string static_path;
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h`

 * *Files 6% similar despite different names*

```diff
@@ -34,37 +34,39 @@
         ui.buffer.push(message.dump());
     }
     template <typename DEVICE, typename ENVIRONMENT, typename ACTION_SPEC>
     void set_state(DEVICE& dev, ENVIRONMENT& env, ui_server::client::UIBuffered<ENVIRONMENT>& ui, const typename ENVIRONMENT::State& state, const Matrix<ACTION_SPEC>& action){
         static_assert(ACTION_SPEC::COLS == ENVIRONMENT::ACTION_DIM);
         static_assert(ACTION_SPEC::ROWS == 1);
         using T = typename ACTION_SPEC::T;
+        using TI = typename DEVICE::index_t;
         nlohmann::json message;
         message["namespace"] = ui.ns;
         message["channel"] = "setState";
         message["data"] = nlohmann::json();
         message["data"]["state"] = json(dev, state);
         std::vector<T> action_vector;
-        for(int i = 0; i < ENVIRONMENT::ACTION_DIM; i++){
+        for(TI i = 0; i < ENVIRONMENT::ACTION_DIM; i++){
             action_vector.push_back(get(action, 0, i));
         }
         message["data"]["action"] = action_vector;
         ui.buffer.push(message.dump());
     }
     template <typename DEVICE, typename ENVIRONMENT, typename ACTION_SPEC>
     void set_action(DEVICE& dev, ENVIRONMENT& env, ui_server::client::UIBuffered<ENVIRONMENT>& ui, const Matrix<ACTION_SPEC>& action){
         static_assert(ACTION_SPEC::COLS == ENVIRONMENT::ACTION_DIM);
         static_assert(ACTION_SPEC::ROWS == 1);
         using T = typename ACTION_SPEC::T;
+        using TI = typename DEVICE::index_t;
         nlohmann::json message;
         message["namespace"] = ui.ns;
         message["channel"] = "setAction";
         message["data"] = nlohmann::json();
         std::vector<T> action_vector;
-        for(int i = 0; i < ENVIRONMENT::ACTION_DIM; i++){
+        for(TI i = 0; i < ENVIRONMENT::ACTION_DIM; i++){
             action_vector.push_back(get(action, 0, i));
         }
         message["data"]["action"] = action_vector;
         ui.buffer.push(message.dump());
     }
     template <typename DEVICE, typename ENVIRONMENT>
     void render(DEVICE& dev, ENVIRONMENT& env, ui_server::client::UIBuffered<ENVIRONMENT>& ui){
```

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h` & `tinyrl-0.4.3/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/interface/algorithms/ppo/template.h` & `tinyrl-0.4.3/tinyrl/interface/algorithms/ppo/template.h`

 * *Files 1% similar despite different names*

```diff
@@ -44,13 +44,14 @@
     static constexpr TI BATCH_SIZE = $BATCH_SIZE;
 
     struct OPTIMIZER_PARAMETERS: rlt::nn::optimizers::adam::DEFAULT_PARAMETERS_TENSORFLOW<T>{
         static constexpr T ALPHA = $OPTIMIZER_ALPHA;
         static constexpr T BETA_1 = $OPTIMIZER_BETA_1;
         static constexpr T BETA_2 = $OPTIMIZER_BETA_2;
         static constexpr T EPSILON = $OPTIMIZER_EPSILON;
+        static constexpr T EPSILON_SQRT = $OPTIMIZER_EPSILON_SQRT;
     };
 };
 
 
 template <typename T, typename TI, typename RNG, typename ENVIRONMENT, TI T_EPISODE_STEP_LIMIT>
 using LOOP_CORE_CONFIG_FACTORY = rlt::rl::algorithms::ppo::loop::core::Config<T, TI, RNG, ENVIRONMENT, PPO_LOOP_CORE_PARAMETERS<T, TI, ENVIRONMENT, T_EPISODE_STEP_LIMIT>>;
```

### Comparing `tinyrl-0.4.2/tinyrl/interface/algorithms/sac/template.h` & `tinyrl-0.4.3/tinyrl/interface/algorithms/sac/template.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #include <rl_tools/rl/algorithms/sac/loop/core/config.h>
 #include <rl_tools/rl/loop/steps/evaluation/config.h>
 #include <rl_tools/rl/loop/steps/timing/config.h>
-#include <rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h>
+#include <rl_tools/rl/algorithms/sac/loop/core/operations_generic.h>
 #include <rl_tools/rl/loop/steps/evaluation/operations_generic.h>
 #include <rl_tools/rl/loop/steps/timing/operations_cpu.h>
 
 namespace TINYRL_MODULE_NAME{
 
     namespace rlt = rl_tools;
 
@@ -39,18 +39,20 @@
         static constexpr TI ACTOR_NUM_LAYERS = $ACTOR_NUM_LAYERS;
         static constexpr auto ACTOR_ACTIVATION_FUNCTION = rlt::nn::activation_functions::ActivationFunction::$ACTOR_ACTIVATION_FUNCTION;
         static constexpr TI CRITIC_HIDDEN_DIM = $CRITIC_HIDDEN_DIM;
         static constexpr TI CRITIC_NUM_LAYERS = $CRITIC_NUM_LAYERS;
         static constexpr auto CRITIC_ACTIVATION_FUNCTION = rlt::nn::activation_functions::ActivationFunction::$CRITIC_ACTIVATION_FUNCTION;
         static constexpr bool COLLECT_EPISODE_STATS = $COLLECT_EPISODE_STATS;
         static constexpr TI EPISODE_STATS_BUFFER_SIZE = $EPISODE_STATS_BUFFER_SIZE;
+        static constexpr bool SHARED_BATCH = $SHARED_BATCH;
         struct OPTIMIZER_PARAMETERS: rlt::nn::optimizers::adam::DEFAULT_PARAMETERS_TENSORFLOW<T>{
             static constexpr T ALPHA = $OPTIMIZER_ALPHA;
             static constexpr T BETA_1 = $OPTIMIZER_BETA_1;
             static constexpr T BETA_2 = $OPTIMIZER_BETA_2;
             static constexpr T EPSILON = $OPTIMIZER_EPSILON;
+            static constexpr T EPSILON_SQRT = $OPTIMIZER_EPSILON_SQRT;
         };
     };
 
     template <typename T, typename TI, typename RNG, typename ENVIRONMENT, TI T_EPISODE_STEP_LIMIT>
     using LOOP_CORE_CONFIG_FACTORY = rlt::rl::algorithms::sac::loop::core::Config<T, TI, RNG, ENVIRONMENT, SAC_LOOP_CORE_PARAMETERS<T, TI, ENVIRONMENT, T_EPISODE_STEP_LIMIT>>;
 }
```

### Comparing `tinyrl-0.4.2/tinyrl/interface/algorithms/td3/template.h` & `tinyrl-0.4.3/tinyrl/interface/algorithms/td3/template.h`

 * *Files 20% similar despite different names*

```diff
@@ -12,16 +12,14 @@
     // This should stay in sync with the parameters in https://github.com/rl-tools/rl-tools/blob/a98bc461f7ebfed0ba71c653216edec6d9334b78/include/rl_tools/rl/algorithms/td3/loop/core/config.h#L18
     template <typename T, typename TI, typename ENVIRONMENT, TI T_EPISODE_STEP_LIMIT>
     struct TD3_LOOP_CORE_PARAMETERS: rlt::rl::algorithms::td3::loop::core::DefaultParameters<T, TI, ENVIRONMENT>{
         struct TD3_PARAMETERS{
             static constexpr T GAMMA = $GAMMA;
             static constexpr TI ACTOR_BATCH_SIZE = $ACTOR_BATCH_SIZE;
             static constexpr TI CRITIC_BATCH_SIZE = $CRITIC_BATCH_SIZE;
-            static constexpr TI N_WARMUP_STEPS_CRITIC = $N_WARMUP_STEPS_CRITIC;
-            static constexpr TI N_WARMUP_STEPS_ACTOR = $N_WARMUP_STEPS_ACTOR;
             static constexpr TI CRITIC_TRAINING_INTERVAL = $CRITIC_TRAINING_INTERVAL;
             static constexpr TI ACTOR_TRAINING_INTERVAL = $ACTOR_TRAINING_INTERVAL;
             static constexpr TI CRITIC_TARGET_UPDATE_INTERVAL = $CRITIC_TARGET_UPDATE_INTERVAL;
             static constexpr TI ACTOR_TARGET_UPDATE_INTERVAL = $ACTOR_TARGET_UPDATE_INTERVAL;
             static constexpr T ACTOR_POLYAK = $ACTOR_POLYAK;
             static constexpr T CRITIC_POLYAK = $CRITIC_POLYAK;
             static constexpr T TARGET_NEXT_ACTION_NOISE_STD = $TARGET_NEXT_ACTION_NOISE_STD;
@@ -39,19 +37,22 @@
         static constexpr auto ACTOR_ACTIVATION_FUNCTION = rlt::nn::activation_functions::ActivationFunction::$ACTOR_ACTIVATION_FUNCTION;
         static constexpr TI CRITIC_HIDDEN_DIM = $CRITIC_HIDDEN_DIM;
         static constexpr TI CRITIC_NUM_LAYERS = $CRITIC_NUM_LAYERS;
         static constexpr auto CRITIC_ACTIVATION_FUNCTION = rlt::nn::activation_functions::ActivationFunction::$CRITIC_ACTIVATION_FUNCTION;
 
         static constexpr bool COLLECT_EPISODE_STATS = $COLLECT_EPISODE_STATS;
         static constexpr TI EPISODE_STATS_BUFFER_SIZE = $EPISODE_STATS_BUFFER_SIZE;
+        static constexpr T EXPLORATION_NOISE = $EXPLORATION_NOISE;
+        static constexpr bool SHARED_BATCH = $SHARED_BATCH;
 
         struct OPTIMIZER_PARAMETERS: rlt::nn::optimizers::adam::DEFAULT_PARAMETERS_TENSORFLOW<T>{
             static constexpr T ALPHA = $OPTIMIZER_ALPHA;
             static constexpr T BETA_1 = $OPTIMIZER_BETA_1;
             static constexpr T BETA_2 = $OPTIMIZER_BETA_2;
             static constexpr T EPSILON = $OPTIMIZER_EPSILON;
+            static constexpr T EPSILON_SQRT = $OPTIMIZER_EPSILON_SQRT;
         };
     };
 
     template <typename T, typename TI, typename RNG, typename ENVIRONMENT, TI T_EPISODE_STEP_LIMIT>
     using LOOP_CORE_CONFIG_FACTORY = rlt::rl::algorithms::td3::loop::core::Config<T, TI, RNG, ENVIRONMENT, TD3_LOOP_CORE_PARAMETERS<T, TI, ENVIRONMENT, T_EPISODE_STEP_LIMIT>>;
 }
```

### Comparing `tinyrl-0.4.2/tinyrl/interface/inference/inference.cpp` & `tinyrl-0.4.3/tinyrl/interface/inference/inference.cpp`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/interface/python_environment/operations_cpu.h` & `tinyrl-0.4.3/tinyrl/interface/python_environment/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/interface/python_environment/python_environment.h` & `tinyrl-0.4.3/tinyrl/interface/python_environment/python_environment.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/interface/training/training.cpp` & `tinyrl-0.4.3/tinyrl/interface/training/training.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 #include <rl_tools/nn/optimizers/adam/persist_code.h>
 #include <rl_tools/nn/layers/dense/persist_code.h>
 #include <rl_tools/nn/parameters/persist_code.h>
 #include <rl_tools/nn_models/sequential/persist_code.h>
 #include <rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h>
 #include <rl_tools/nn_models/mlp/persist_code.h>
 // #include <rl_tools/nn_models/mlp/persist_code.h>
+#include <rl_tools/nn/optimizers/adam/operations_generic.h>
 
 #include "loop_core_config.h"
 
 namespace rlt = rl_tools;
 
 #include <pybind11/pybind11.h>
 #include <pybind11/functional.h>
```

### Comparing `tinyrl-0.4.2/tinyrl/src/accelerate.py` & `tinyrl-0.4.3/tinyrl/src/accelerate.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/src/compile.py` & `tinyrl-0.4.3/tinyrl/src/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
     compilers = unix_compilers if (sys.platform in ["linux", "darwin"]) else windows_compilers
     compilers = [compiler for compiler in compilers if shutil.which(compiler) is not None]
     raw_platform_compiler = platform.python_compiler()
     if raw_platform_compiler.startswith("MSC"):
         platform_compiler = "cl"
     elif raw_platform_compiler.startswith("GCC"):
         platform_compiler = "g++"
+    elif raw_platform_compiler.startswith("Clang"):
+        platform_compiler = "clang++"
     else:
         platform_compiler = None
     if platform_compiler is None:
         warnings.warn(f"The platform compiler {raw_platform_compiler} is not recognized.")
     else:
         if platform_compiler not in compilers:
             warnings.warn(f"The platform compiler {platform_compiler} (used for compiling Python) is not found (found: {compilers}).")
```

### Comparing `tinyrl-0.4.2/tinyrl/src/link_blas.py` & `tinyrl-0.4.3/tinyrl/src/link_blas.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/src/link_mkl.py` & `tinyrl-0.4.3/tinyrl/src/link_mkl.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/src/load_checkpoint.py` & `tinyrl-0.4.3/tinyrl/src/load_checkpoint.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/src/ppo.py` & `tinyrl-0.4.3/tinyrl/src/ppo.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     ON_POLICY_RUNNER_STEPS_PER_ENV = 64,
     BATCH_SIZE = 64,
     # optimizer
     OPTIMIZER_ALPHA=1e-3,
     OPTIMIZER_BETA_1=0.9,
     OPTIMIZER_BETA_2=0.999,
     OPTIMIZER_EPSILON=1e-7,
+    OPTIMIZER_EPSILON_SQRT=1e-7,
     **kwargs
     ):
     assert STEP_LIMIT is not None or TOTAL_STEP_LIMIT is not None, "Either STEP_LIMIT or TOTAL_STEP_LIMIT must be set"
     evaluation_interval = evaluation_interval if evaluation_interval is not None else 10
     verbose = verbose or "TINYRL_VERBOSE" in os.environ
     if STEP_LIMIT is None:
         STEP_LIMIT = math.floor(TOTAL_STEP_LIMIT/(ON_POLICY_RUNNER_STEPS_PER_ENV * N_ENVIRONMENTS))
```

### Comparing `tinyrl-0.4.2/tinyrl/src/render.py` & `tinyrl-0.4.3/tinyrl/src/render.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/tinyrl/src/sac.py` & `tinyrl-0.4.3/tinyrl/src/sac.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,21 @@
     ACTOR_NUM_LAYERS = 3,
     ACTOR_ACTIVATION_FUNCTION = "RELU",
     CRITIC_HIDDEN_DIM = 64,
     CRITIC_NUM_LAYERS = 3,
     CRITIC_ACTIVATION_FUNCTION = "RELU",
     COLLECT_EPISODE_STATS = True,
     EPISODE_STATS_BUFFER_SIZE = 1000,
+    SHARED_BATCH = True,
     # optimizer
     OPTIMIZER_ALPHA=1e-3,
     OPTIMIZER_BETA_1=0.9,
     OPTIMIZER_BETA_2=0.999,
     OPTIMIZER_EPSILON=1e-7,
+    OPTIMIZER_EPSILON_SQRT=1e-7,
     **kwargs
     ):
     verbose = verbose or "TINYRL_VERBOSE" in os.environ
 
 
     # The action dim is needed to set the default target entropy
     use_python_environment = type(env_factory) != dict
```

### Comparing `tinyrl-0.4.2/tinyrl/src/td3.py` & `tinyrl-0.4.3/tinyrl/src/td3.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,14 @@
     num_evaluation_episodes=10,
     interface_name="default", # this is the namespace used for the compilation of the TinyRL interface (in a temporary directory) and should be unique if run in parallel. We don't choose a random uuid because it would invalidate the cache and require a re-compilation every time
     # Compile-time parameters:
     # Same set of parameters as: rl::algorithms::td3::DefaultParameters
     GAMMA = 0.99,
     ACTOR_BATCH_SIZE = 100,
     CRITIC_BATCH_SIZE = 100,
-    N_WARMUP_STEPS_CRITIC = 0,
-    N_WARMUP_STEPS_ACTOR = 0,
     CRITIC_TRAINING_INTERVAL = 1,
     ACTOR_TRAINING_INTERVAL = 2,
     CRITIC_TARGET_UPDATE_INTERVAL = 2,
     ACTOR_TARGET_UPDATE_INTERVAL = 2,
     ACTOR_POLYAK = 1.0 - 0.005,
     CRITIC_POLYAK = 1.0 - 0.005,
     TARGET_NEXT_ACTION_NOISE_STD = 0.2,
@@ -41,19 +39,22 @@
     ACTOR_NUM_LAYERS = 3,
     ACTOR_ACTIVATION_FUNCTION = "RELU",
     CRITIC_HIDDEN_DIM = 64,
     CRITIC_NUM_LAYERS = 3,
     CRITIC_ACTIVATION_FUNCTION = "RELU",
     COLLECT_EPISODE_STATS = True,
     EPISODE_STATS_BUFFER_SIZE = 1000,
+    EXPLORATION_NOISE = 0.1,
+    SHARED_BATCH = True,
     # optimizer
     OPTIMIZER_ALPHA=1e-3,
     OPTIMIZER_BETA_1=0.9,
     OPTIMIZER_BETA_2=0.999,
     OPTIMIZER_EPSILON=1e-7,
+    OPTIMIZER_EPSILON_SQRT=1e-7,
     **kwargs
     ):
     verbose = verbose or "TINYRL_VERBOSE" in os.environ
 
     REPLAY_BUFFER_CAP = REPLAY_BUFFER_CAP if REPLAY_BUFFER_CAP is not None else STEP_LIMIT
     N_WARMUP_STEPS = N_WARMUP_STEPS if N_WARMUP_STEPS is not None else max(ACTOR_BATCH_SIZE, CRITIC_BATCH_SIZE)
```

### Comparing `tinyrl-0.4.2/tinyrl/src/training.py` & `tinyrl-0.4.3/tinyrl/src/training.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/LICENSE` & `tinyrl-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/README.md` & `tinyrl-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `tinyrl-0.4.2/pyproject.toml` & `tinyrl-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tinyrl"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="Jonas Eschmann", email="jonas.eschmann@gmail.com" },
 ]
 description = "A Python wrapper for RLtools"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tinyrl-0.4.2/PKG-INFO` & `tinyrl-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tinyrl
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python wrapper for RLtools
 Project-URL: Homepage, https://github.com/rl-tools/tinyrl
 Project-URL: Issues, https://github.com/rl-tools/tinyrl/issues
 Author-email: Jonas Eschmann <jonas.eschmann@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

