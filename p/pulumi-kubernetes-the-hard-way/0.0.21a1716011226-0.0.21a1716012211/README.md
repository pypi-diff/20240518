# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.21a1716011226.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.21a1716012211.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.21a1716011226.tar", last modified: Sat May 18 05:49:43 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.21a1716012211.tar", last modified: Sat May 18 06:06:08 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226.tar` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:43.983926 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-18 05:49:43.983926 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:43.971926 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4366 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:43.971926 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      418 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21101 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8728 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)    23922 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    29159 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:43.979926 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)     1076 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    18005 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    13340 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     8612 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     7575 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8328 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    16864 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5113 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)    10944 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:43.979926 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3019 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     2983 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:43.983926 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      590 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     3166 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)   108491 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    14976 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/curl.py
--rw-------   0 runner    (1001) docker     (127)    15049 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    15189 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14992 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    91820 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    15119 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    14907 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    14922 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:43.983926 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-18 05:49:43.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-18 05:49:43.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 05:49:43.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-18 05:49:43.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-18 05:49:43.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      899 2024-05-18 05:49:37.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 05:49:43.983926 pulumi_kubernetes_the_hard_way-0.0.21a1716011226/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:06:08.857190 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-18 06:06:08.857190 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:06:08.841189 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     4454 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:06:08.845189 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      418 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21101 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     8728 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)    23922 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    29159 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:06:08.849189 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)     1116 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    24968 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    13340 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     8612 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     7575 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)     6879 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8328 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    25169 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5113 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)    10944 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:06:08.853190 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3019 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     2983 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:06:08.857190 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      590 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     3166 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)   108491 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    14976 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/curl.py
+-rw-------   0 runner    (1001) docker     (127)    15049 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    15189 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    14992 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    91820 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    15119 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14907 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    14922 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:06:08.857190 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-18 06:06:08.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-18 06:06:08.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 06:06:08.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-18 06:06:08.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-18 06:06:08.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      899 2024-05-18 06:06:00.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 06:06:08.857190 pulumi_kubernetes_the_hard_way-0.0.21a1716012211/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.21a1716011226
+Version: 0.0.21a1716012211
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/README.md` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
   "mod": "remote",
   "fqn": "pulumi_kubernetes_the_hard_way.remote",
   "classes": {
    "kubernetes-the-hard-way:remote:CniBridgePluginConfiguration": "CniBridgePluginConfiguration",
    "kubernetes-the-hard-way:remote:CniLoopbackPluginConfiguration": "CniLoopbackPluginConfiguration",
    "kubernetes-the-hard-way:remote:CniPluginConfiguration": "CniPluginConfiguration",
    "kubernetes-the-hard-way:remote:CniPluginsInstall": "CniPluginsInstall",
+   "kubernetes-the-hard-way:remote:ContainerdConfiguration": "ContainerdConfiguration",
    "kubernetes-the-hard-way:remote:ContainerdInstall": "ContainerdInstall",
    "kubernetes-the-hard-way:remote:CrictlInstall": "CrictlInstall",
    "kubernetes-the-hard-way:remote:Download": "Download",
    "kubernetes-the-hard-way:remote:EtcdCluster": "EtcdCluster",
    "kubernetes-the-hard-way:remote:EtcdConfiguration": "EtcdConfiguration",
    "kubernetes-the-hard-way:remote:EtcdInstall": "EtcdInstall",
    "kubernetes-the-hard-way:remote:EtcdService": "EtcdService",
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import typing
 # Export this package's modules as members:
 from ._enums import *
 from .cni_bridge_plugin_configuration import *
 from .cni_loopback_plugin_configuration import *
 from .cni_plugin_configuration import *
 from .cni_plugins_install import *
+from .containerd_configuration import *
 from .containerd_install import *
 from .crictl_install import *
 from .download import *
 from .etcd_cluster import *
 from .etcd_configuration import *
 from .etcd_install import *
 from .etcd_service import *
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from ._enums import *
 import pulumi_command
 
 __all__ = [
     'CniBridgeIpamArgs',
+    'ContainerdCriPluginConfigurationCniArgs',
+    'ContainerdCriPluginConfigurationContainerdRuncOptionsArgs',
+    'ContainerdCriPluginConfigurationContainerdRuncArgs',
+    'ContainerdCriPluginConfigurationContainerdArgs',
+    'ContainerdCriPluginConfigurationArgs',
     'EtcdConfigurationPropsArgs',
     'EtcdNodeArgs',
     'SystemdInstallSectionArgs',
     'SystemdServiceSectionArgs',
     'SystemdUnitSectionArgs',
 ]
 
@@ -73,14 +78,211 @@
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
 
 @pulumi.input_type
+class ContainerdCriPluginConfigurationCniArgs:
+    def __init__(__self__, *,
+                 bin_dir: Optional[pulumi.Input[str]] = None,
+                 conf_dir: Optional[pulumi.Input[str]] = None):
+        """
+        containerd cri plugin configuration.
+        :param pulumi.Input[str] bin_dir: bin_dir
+        :param pulumi.Input[str] conf_dir: conf_dir
+        """
+        if bin_dir is not None:
+            pulumi.set(__self__, "bin_dir", bin_dir)
+        if conf_dir is not None:
+            pulumi.set(__self__, "conf_dir", conf_dir)
+
+    @property
+    @pulumi.getter(name="binDir")
+    def bin_dir(self) -> Optional[pulumi.Input[str]]:
+        """
+        bin_dir
+        """
+        return pulumi.get(self, "bin_dir")
+
+    @bin_dir.setter
+    def bin_dir(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "bin_dir", value)
+
+    @property
+    @pulumi.getter(name="confDir")
+    def conf_dir(self) -> Optional[pulumi.Input[str]]:
+        """
+        conf_dir
+        """
+        return pulumi.get(self, "conf_dir")
+
+    @conf_dir.setter
+    def conf_dir(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "conf_dir", value)
+
+
+@pulumi.input_type
+class ContainerdCriPluginConfigurationContainerdRuncOptionsArgs:
+    def __init__(__self__, *,
+                 systemd_cgroup: Optional[pulumi.Input[bool]] = None):
+        """
+        containerd cri runc plugin configuration.
+        :param pulumi.Input[bool] systemd_cgroup: SystemdCgroup
+        """
+        if systemd_cgroup is not None:
+            pulumi.set(__self__, "systemd_cgroup", systemd_cgroup)
+
+    @property
+    @pulumi.getter(name="systemdCgroup")
+    def systemd_cgroup(self) -> Optional[pulumi.Input[bool]]:
+        """
+        SystemdCgroup
+        """
+        return pulumi.get(self, "systemd_cgroup")
+
+    @systemd_cgroup.setter
+    def systemd_cgroup(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "systemd_cgroup", value)
+
+
+@pulumi.input_type
+class ContainerdCriPluginConfigurationContainerdRuncArgs:
+    def __init__(__self__, *,
+                 options: 'ContainerdCriPluginConfigurationContainerdRuncOptionsArgs',
+                 runtime_type: Optional[pulumi.Input[str]] = None):
+        """
+        containerd cri runc plugin configuration.
+        :param 'ContainerdCriPluginConfigurationContainerdRuncOptionsArgs' options: runc options.
+        :param pulumi.Input[str] runtime_type: runtime_type
+        """
+        pulumi.set(__self__, "options", options)
+        if runtime_type is not None:
+            pulumi.set(__self__, "runtime_type", runtime_type)
+
+    @property
+    @pulumi.getter
+    def options(self) -> 'ContainerdCriPluginConfigurationContainerdRuncOptionsArgs':
+        """
+        runc options.
+        """
+        return pulumi.get(self, "options")
+
+    @options.setter
+    def options(self, value: 'ContainerdCriPluginConfigurationContainerdRuncOptionsArgs'):
+        pulumi.set(self, "options", value)
+
+    @property
+    @pulumi.getter(name="runtimeType")
+    def runtime_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        runtime_type
+        """
+        return pulumi.get(self, "runtime_type")
+
+    @runtime_type.setter
+    def runtime_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "runtime_type", value)
+
+
+@pulumi.input_type
+class ContainerdCriPluginConfigurationContainerdArgs:
+    def __init__(__self__, *,
+                 default_runtime_name: Optional[pulumi.Input[str]] = None,
+                 runtimes: Optional['ContainerdCriPluginConfigurationContainerdRuncArgs'] = None,
+                 snapshotter: Optional[pulumi.Input[str]] = None):
+        """
+        containerd cri plugin configuration.
+        :param pulumi.Input[str] default_runtime_name: default_runtime_name
+        :param 'ContainerdCriPluginConfigurationContainerdRuncArgs' runtimes: The containerd runtime configuration.
+        :param pulumi.Input[str] snapshotter: snapshotter
+        """
+        if default_runtime_name is not None:
+            pulumi.set(__self__, "default_runtime_name", default_runtime_name)
+        if runtimes is not None:
+            pulumi.set(__self__, "runtimes", runtimes)
+        if snapshotter is not None:
+            pulumi.set(__self__, "snapshotter", snapshotter)
+
+    @property
+    @pulumi.getter(name="defaultRuntimeName")
+    def default_runtime_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        default_runtime_name
+        """
+        return pulumi.get(self, "default_runtime_name")
+
+    @default_runtime_name.setter
+    def default_runtime_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_runtime_name", value)
+
+    @property
+    @pulumi.getter
+    def runtimes(self) -> Optional['ContainerdCriPluginConfigurationContainerdRuncArgs']:
+        """
+        The containerd runtime configuration.
+        """
+        return pulumi.get(self, "runtimes")
+
+    @runtimes.setter
+    def runtimes(self, value: Optional['ContainerdCriPluginConfigurationContainerdRuncArgs']):
+        pulumi.set(self, "runtimes", value)
+
+    @property
+    @pulumi.getter
+    def snapshotter(self) -> Optional[pulumi.Input[str]]:
+        """
+        snapshotter
+        """
+        return pulumi.get(self, "snapshotter")
+
+    @snapshotter.setter
+    def snapshotter(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "snapshotter", value)
+
+
+@pulumi.input_type
+class ContainerdCriPluginConfigurationArgs:
+    def __init__(__self__, *,
+                 cni: 'ContainerdCriPluginConfigurationCniArgs',
+                 containerd: 'ContainerdCriPluginConfigurationContainerdArgs'):
+        """
+        containerd cri plugin configuration.
+        :param 'ContainerdCriPluginConfigurationCniArgs' cni: cni configuration.
+        :param 'ContainerdCriPluginConfigurationContainerdArgs' containerd: containerd configuration.
+        """
+        pulumi.set(__self__, "cni", cni)
+        pulumi.set(__self__, "containerd", containerd)
+
+    @property
+    @pulumi.getter
+    def cni(self) -> 'ContainerdCriPluginConfigurationCniArgs':
+        """
+        cni configuration.
+        """
+        return pulumi.get(self, "cni")
+
+    @cni.setter
+    def cni(self, value: 'ContainerdCriPluginConfigurationCniArgs'):
+        pulumi.set(self, "cni", value)
+
+    @property
+    @pulumi.getter
+    def containerd(self) -> 'ContainerdCriPluginConfigurationContainerdArgs':
+        """
+        containerd configuration.
+        """
+        return pulumi.get(self, "containerd")
+
+    @containerd.setter
+    def containerd(self, value: 'ContainerdCriPluginConfigurationContainerdArgs'):
+        pulumi.set(self, "containerd", value)
+
+
+@pulumi.input_type
 class EtcdConfigurationPropsArgs:
     def __init__(__self__, *,
                  ca_file_path: pulumi.Input[str],
                  cert_file_path: pulumi.Input[str],
                  data_directory: pulumi.Input[str],
                  etcd_path: pulumi.Input[str],
                  internal_ip: pulumi.Input[str],
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,19 +4,25 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
 from ._enums import *
 import pulumi_command
 
 __all__ = [
     'CniBridgeIpam',
+    'ContainerdCriPluginConfiguration',
+    'ContainerdCriPluginConfigurationCni',
+    'ContainerdCriPluginConfigurationContainerd',
+    'ContainerdCriPluginConfigurationContainerdRunc',
+    'ContainerdCriPluginConfigurationContainerdRuncOptions',
     'EtcdConfigurationProps',
     'EtcdNode',
     'SystemdInstallSection',
     'SystemdServiceSection',
     'SystemdUnitSection',
 ]
 
@@ -64,14 +70,256 @@
         """
         CNI bridge IPAM type
         """
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
+class ContainerdCriPluginConfiguration(dict):
+    """
+    containerd cri plugin configuration.
+    """
+    def __init__(__self__, *,
+                 cni: 'outputs.ContainerdCriPluginConfigurationCni',
+                 containerd: 'outputs.ContainerdCriPluginConfigurationContainerd'):
+        """
+        containerd cri plugin configuration.
+        :param 'ContainerdCriPluginConfigurationCni' cni: cni configuration.
+        :param 'ContainerdCriPluginConfigurationContainerd' containerd: containerd configuration.
+        """
+        pulumi.set(__self__, "cni", cni)
+        pulumi.set(__self__, "containerd", containerd)
+
+    @property
+    @pulumi.getter
+    def cni(self) -> 'outputs.ContainerdCriPluginConfigurationCni':
+        """
+        cni configuration.
+        """
+        return pulumi.get(self, "cni")
+
+    @property
+    @pulumi.getter
+    def containerd(self) -> 'outputs.ContainerdCriPluginConfigurationContainerd':
+        """
+        containerd configuration.
+        """
+        return pulumi.get(self, "containerd")
+
+
+@pulumi.output_type
+class ContainerdCriPluginConfigurationCni(dict):
+    """
+    containerd cri plugin configuration.
+    """
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "binDir":
+            suggest = "bin_dir"
+        elif key == "confDir":
+            suggest = "conf_dir"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ContainerdCriPluginConfigurationCni. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ContainerdCriPluginConfigurationCni.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ContainerdCriPluginConfigurationCni.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 bin_dir: Optional[str] = None,
+                 conf_dir: Optional[str] = None):
+        """
+        containerd cri plugin configuration.
+        :param str bin_dir: bin_dir
+        :param str conf_dir: conf_dir
+        """
+        if bin_dir is not None:
+            pulumi.set(__self__, "bin_dir", bin_dir)
+        if conf_dir is not None:
+            pulumi.set(__self__, "conf_dir", conf_dir)
+
+    @property
+    @pulumi.getter(name="binDir")
+    def bin_dir(self) -> Optional[str]:
+        """
+        bin_dir
+        """
+        return pulumi.get(self, "bin_dir")
+
+    @property
+    @pulumi.getter(name="confDir")
+    def conf_dir(self) -> Optional[str]:
+        """
+        conf_dir
+        """
+        return pulumi.get(self, "conf_dir")
+
+
+@pulumi.output_type
+class ContainerdCriPluginConfigurationContainerd(dict):
+    """
+    containerd cri plugin configuration.
+    """
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "defaultRuntimeName":
+            suggest = "default_runtime_name"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ContainerdCriPluginConfigurationContainerd. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ContainerdCriPluginConfigurationContainerd.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ContainerdCriPluginConfigurationContainerd.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 default_runtime_name: Optional[str] = None,
+                 runtimes: Optional['outputs.ContainerdCriPluginConfigurationContainerdRunc'] = None,
+                 snapshotter: Optional[str] = None):
+        """
+        containerd cri plugin configuration.
+        :param str default_runtime_name: default_runtime_name
+        :param 'ContainerdCriPluginConfigurationContainerdRunc' runtimes: The containerd runtime configuration.
+        :param str snapshotter: snapshotter
+        """
+        if default_runtime_name is not None:
+            pulumi.set(__self__, "default_runtime_name", default_runtime_name)
+        if runtimes is not None:
+            pulumi.set(__self__, "runtimes", runtimes)
+        if snapshotter is not None:
+            pulumi.set(__self__, "snapshotter", snapshotter)
+
+    @property
+    @pulumi.getter(name="defaultRuntimeName")
+    def default_runtime_name(self) -> Optional[str]:
+        """
+        default_runtime_name
+        """
+        return pulumi.get(self, "default_runtime_name")
+
+    @property
+    @pulumi.getter
+    def runtimes(self) -> Optional['outputs.ContainerdCriPluginConfigurationContainerdRunc']:
+        """
+        The containerd runtime configuration.
+        """
+        return pulumi.get(self, "runtimes")
+
+    @property
+    @pulumi.getter
+    def snapshotter(self) -> Optional[str]:
+        """
+        snapshotter
+        """
+        return pulumi.get(self, "snapshotter")
+
+
+@pulumi.output_type
+class ContainerdCriPluginConfigurationContainerdRunc(dict):
+    """
+    containerd cri runc plugin configuration.
+    """
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "runtimeType":
+            suggest = "runtime_type"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ContainerdCriPluginConfigurationContainerdRunc. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ContainerdCriPluginConfigurationContainerdRunc.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ContainerdCriPluginConfigurationContainerdRunc.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 options: 'outputs.ContainerdCriPluginConfigurationContainerdRuncOptions',
+                 runtime_type: Optional[str] = None):
+        """
+        containerd cri runc plugin configuration.
+        :param 'ContainerdCriPluginConfigurationContainerdRuncOptions' options: runc options.
+        :param str runtime_type: runtime_type
+        """
+        pulumi.set(__self__, "options", options)
+        if runtime_type is not None:
+            pulumi.set(__self__, "runtime_type", runtime_type)
+
+    @property
+    @pulumi.getter
+    def options(self) -> 'outputs.ContainerdCriPluginConfigurationContainerdRuncOptions':
+        """
+        runc options.
+        """
+        return pulumi.get(self, "options")
+
+    @property
+    @pulumi.getter(name="runtimeType")
+    def runtime_type(self) -> Optional[str]:
+        """
+        runtime_type
+        """
+        return pulumi.get(self, "runtime_type")
+
+
+@pulumi.output_type
+class ContainerdCriPluginConfigurationContainerdRuncOptions(dict):
+    """
+    containerd cri runc plugin configuration.
+    """
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "systemdCgroup":
+            suggest = "systemd_cgroup"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ContainerdCriPluginConfigurationContainerdRuncOptions. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ContainerdCriPluginConfigurationContainerdRuncOptions.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ContainerdCriPluginConfigurationContainerdRuncOptions.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 systemd_cgroup: Optional[bool] = None):
+        """
+        containerd cri runc plugin configuration.
+        :param bool systemd_cgroup: SystemdCgroup
+        """
+        if systemd_cgroup is not None:
+            pulumi.set(__self__, "systemd_cgroup", systemd_cgroup)
+
+    @property
+    @pulumi.getter(name="systemdCgroup")
+    def systemd_cgroup(self) -> Optional[bool]:
+        """
+        SystemdCgroup
+        """
+        return pulumi.get(self, "systemd_cgroup")
+
+
+@pulumi.output_type
 class EtcdConfigurationProps(dict):
     """
     Props for resources that consume etcd configuration.
     """
     @staticmethod
     def __key_warning(key: str):
         suggest = None
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/curl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/curl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.21a1716011226
+Version: 0.0.21a1716012211
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 pulumi_kubernetes_the_hard_way/remote/__init__.py
 pulumi_kubernetes_the_hard_way/remote/_enums.py
 pulumi_kubernetes_the_hard_way/remote/_inputs.py
 pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
 pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
 pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
 pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
 pulumi_kubernetes_the_hard_way/remote/containerd_install.py
 pulumi_kubernetes_the_hard_way/remote/crictl_install.py
 pulumi_kubernetes_the_hard_way/remote/download.py
 pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
 pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
 pulumi_kubernetes_the_hard_way/remote/etcd_install.py
 pulumi_kubernetes_the_hard_way/remote/etcd_service.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716011226/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.21a1716012211/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.11.1,<1.0.0", "pulumi-kubernetes>=4.11.0,<5.0.0", "pulumi-random>=4.16.1,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.21a1716011226"
+  version = "0.0.21a1716012211"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

