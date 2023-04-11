# Comparing `tmp/dtschema-2023.1.tar.gz` & `tmp/dtschema-2023.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtschema-2023.1.tar", last modified: Tue Jan 31 23:40:36 2023, max compression
+gzip compressed data, was "dtschema-2023.4.tar", last modified: Tue Apr 11 22:26:58 2023, max compression
```

## Comparing `dtschema-2023.1.tar` & `dtschema-2023.4.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.821775 dtschema-2023.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.797774 dtschema-2023.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.801774 dtschema-2023.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-31 23:40:22.000000 dtschema-2023.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-01-31 23:40:22.000000 dtschema-2023.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-31 23:40:22.000000 dtschema-2023.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-01-31 23:40:22.000000 dtschema-2023.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-01-31 23:40:36.821775 dtschema-2023.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-01-31 23:40:22.000000 dtschema-2023.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.801774 dtschema-2023.1/dtschema/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/dtb.py
--rw-r--r--   0 runner    (1001) docker     (123)    43041 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.805774 dtschema-2023.1/dtschema/meta-schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/boolean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/cell.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/clocks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/core.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/dma.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/gpios.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/hwlock.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/iio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/interrupts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/iommu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/items.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/keywords.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/mailbox.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/nodes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/nvmem.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/phy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/power-domain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/pwm.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/reset.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/string-array.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/meta-schemas/vendor-props.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.809774 dtschema-2023.1/dtschema/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/aliases.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/bootph.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.809774 dtschema-2023.1/dtschema/schemas/bus/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/bus/qemu,platform.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/cache-controller.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/cache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/chosen.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.809774 dtschema-2023.1/dtschema/schemas/clock/
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/clock/clock.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/cpu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/cpus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.809774 dtschema-2023.1/dtschema/schemas/dma/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/dma/dma.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/dt-core.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.809774 dtschema-2023.1/dtschema/schemas/gpio/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/gpio/gpio-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/gpio/gpio-hog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/gpio/gpio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/graph.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.809774 dtschema-2023.1/dtschema/schemas/hwlock/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/hwlock/hwlock-consumer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.809774 dtschema-2023.1/dtschema/schemas/i2c/
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/i2c/i2c-controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.813775 dtschema-2023.1/dtschema/schemas/iio/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/iio/iio-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/iio/iio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/interconnects.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/interrupt-controller.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/interrupts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.813775 dtschema-2023.1/dtschema/schemas/iommu/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/iommu/iommu.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.813775 dtschema-2023.1/dtschema/schemas/isa/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/isa/isa-bridge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/isa/isa-bus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.813775 dtschema-2023.1/dtschema/schemas/mbox/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/mbox/mbox-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/memory.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/msi-consumer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.813775 dtschema-2023.1/dtschema/schemas/opp/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/opp/opp.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.813775 dtschema-2023.1/dtschema/schemas/options/
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/options/u-boot.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/options.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.813775 dtschema-2023.1/dtschema/schemas/pci/
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/pci/pci-bus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/pci/pci-iommu.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.813775 dtschema-2023.1/dtschema/schemas/phy/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/phy/phy-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/phy/phy-provider.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.813775 dtschema-2023.1/dtschema/schemas/pinctrl/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/pinctrl/pinctrl-consumer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.813775 dtschema-2023.1/dtschema/schemas/power-domain/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/power-domain/power-domain-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/property-units.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.813775 dtschema-2023.1/dtschema/schemas/pwm/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/pwm/pwm-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/reg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.813775 dtschema-2023.1/dtschema/schemas/reset/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/reset/reset.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/root-node.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/serial.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/simple-bus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-01-31 23:40:22.000000 dtschema-2023.1/dtschema/schemas/types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-31 23:40:36.000000 dtschema-2023.1/dtschema/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.801774 dtschema-2023.1/dtschema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-01-31 23:40:36.000000 dtschema-2023.1/dtschema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-01-31 23:40:36.000000 dtschema-2023.1/dtschema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 23:40:36.000000 dtschema-2023.1/dtschema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-31 23:40:36.000000 dtschema-2023.1/dtschema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-31 23:40:36.000000 dtschema-2023.1/dtschema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-01-31 23:40:22.000000 dtschema-2023.1/example-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 23:40:36.821775 dtschema-2023.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1630 2023-01-31 23:40:22.000000 dtschema-2023.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.817775 dtschema-2023.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-01-31 23:40:22.000000 dtschema-2023.1/test/bootphases.dts
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-01-31 23:40:22.000000 dtschema-2023.1/test/child-node-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-01-31 23:40:22.000000 dtschema-2023.1/test/child-node.dts
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-01-31 23:40:22.000000 dtschema-2023.1/test/conditionals-allof-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-31 23:40:22.000000 dtschema-2023.1/test/conditionals-allof-pass.dts
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-01-31 23:40:22.000000 dtschema-2023.1/test/conditionals-single-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-01-31 23:40:22.000000 dtschema-2023.1/test/conditionals-single-pass.dts
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-01-31 23:40:22.000000 dtschema-2023.1/test/device-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-01-31 23:40:22.000000 dtschema-2023.1/test/device.dts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.817775 dtschema-2023.1/test/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-01-31 23:40:22.000000 dtschema-2023.1/test/schemas/bad-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-01-31 23:40:22.000000 dtschema-2023.1/test/schemas/child-node-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-01-31 23:40:22.000000 dtschema-2023.1/test/schemas/conditionals-allof-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-01-31 23:40:22.000000 dtschema-2023.1/test/schemas/conditionals-single-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-01-31 23:40:22.000000 dtschema-2023.1/test/schemas/good-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-31 23:40:22.000000 dtschema-2023.1/test/simple-bus-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-01-31 23:40:22.000000 dtschema-2023.1/test/simple-bus-pass.dts
--rwxr-xr-x   0 runner    (1001) docker     (123)     6384 2023-01-31 23:40:22.000000 dtschema-2023.1/test/test-dt-validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 23:40:36.821775 dtschema-2023.1/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-01-31 23:40:22.000000 dtschema-2023.1/tools/dt-check-compatible
--rwxr-xr-x   0 runner    (1001) docker     (123)     2128 2023-01-31 23:40:22.000000 dtschema-2023.1/tools/dt-doc-validate
--rwxr-xr-x   0 runner    (1001) docker     (123)     2494 2023-01-31 23:40:22.000000 dtschema-2023.1/tools/dt-extract-example
--rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-01-31 23:40:22.000000 dtschema-2023.1/tools/dt-extract-props
--rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-01-31 23:40:22.000000 dtschema-2023.1/tools/dt-mk-schema
--rwxr-xr-x   0 runner    (1001) docker     (123)     6206 2023-01-31 23:40:22.000000 dtschema-2023.1/tools/dt-prop-populate
--rwxr-xr-x   0 runner    (1001) docker     (123)     6934 2023-01-31 23:40:22.000000 dtschema-2023.1/tools/dt-validate
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-01-31 23:40:22.000000 dtschema-2023.1/tools/dtb2py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-01-31 23:40:22.000000 dtschema-2023.1/tools/extract-compatibles
--rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-01-31 23:40:22.000000 dtschema-2023.1/tools/yaml-format
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-01-31 23:40:22.000000 dtschema-2023.1/tools/yaml2json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.529180 dtschema-2023.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.485180 dtschema-2023.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.497180 dtschema-2023.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-11 22:26:40.000000 dtschema-2023.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-11 22:26:40.000000 dtschema-2023.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 22:26:40.000000 dtschema-2023.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-11 22:26:40.000000 dtschema-2023.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-11 22:26:58.529180 dtschema-2023.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-04-11 22:26:40.000000 dtschema-2023.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.497180 dtschema-2023.4/dtschema/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/dtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43162 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.505180 dtschema-2023.4/dtschema/meta-schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/boolean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/cell.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/clocks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/core.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/dma.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/gpios.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/hwlock.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/iio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/interrupts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/iommu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/items.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/keywords.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/mailbox.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/nodes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/nvmem.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/phy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/power-domain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/pwm.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/reset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/string-array.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/vendor-props.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/aliases.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/bootph.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/bus/qemu,platform.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/cache-controller.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/cache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9188 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/chosen.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/clock/
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/clock/clock.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/cpus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/dma/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/dma/dma.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/dt-core.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/gpio/gpio-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/gpio/gpio-hog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/gpio/gpio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/graph.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/hwlock/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/hwlock/hwlock-consumer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/i2c/
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/i2c/i2c-controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/iio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/iio/iio-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/iio/iio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/interconnects.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/interrupt-controller.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/interrupts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/iommu/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/iommu/iommu.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/isa/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/isa/isa-bridge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/isa/isa-bus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/mbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/mbox/mbox-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/memory.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/msi-consumer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/opp/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/opp/opp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/options/u-boot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/options.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/pci/
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/pci/pci-bus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/pci/pci-iommu.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/phy/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/phy/phy-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/phy/phy-provider.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/pinctrl/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/pinctrl/pinctrl-consumer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/power-domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/power-domain/power-domain-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/property-units.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.521180 dtschema-2023.4/dtschema/schemas/pwm/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/pwm/pwm-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/reg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.521180 dtschema-2023.4/dtschema/schemas/reset/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/reset/reset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/root-node.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/serial.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/simple-bus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 22:26:58.000000 dtschema-2023.4/dtschema/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.497180 dtschema-2023.4/dtschema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-11 22:26:58.000000 dtschema-2023.4/dtschema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-11 22:26:58.000000 dtschema-2023.4/dtschema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 22:26:58.000000 dtschema-2023.4/dtschema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-11 22:26:58.000000 dtschema-2023.4/dtschema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 22:26:58.000000 dtschema-2023.4/dtschema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-04-11 22:26:40.000000 dtschema-2023.4/example-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 22:26:58.529180 dtschema-2023.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1638 2023-04-11 22:26:40.000000 dtschema-2023.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.525180 dtschema-2023.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-11 22:26:40.000000 dtschema-2023.4/test/bootphases.dts
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-11 22:26:40.000000 dtschema-2023.4/test/child-node-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-11 22:26:40.000000 dtschema-2023.4/test/child-node.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-11 22:26:40.000000 dtschema-2023.4/test/conditionals-allof-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-11 22:26:40.000000 dtschema-2023.4/test/conditionals-allof-pass.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-11 22:26:40.000000 dtschema-2023.4/test/conditionals-single-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-11 22:26:40.000000 dtschema-2023.4/test/conditionals-single-pass.dts
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-11 22:26:40.000000 dtschema-2023.4/test/device-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-11 22:26:40.000000 dtschema-2023.4/test/device.dts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.525180 dtschema-2023.4/test/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-11 22:26:40.000000 dtschema-2023.4/test/schemas/bad-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-11 22:26:40.000000 dtschema-2023.4/test/schemas/child-node-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-11 22:26:40.000000 dtschema-2023.4/test/schemas/conditionals-allof-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-11 22:26:40.000000 dtschema-2023.4/test/schemas/conditionals-single-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-11 22:26:40.000000 dtschema-2023.4/test/schemas/good-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-11 22:26:40.000000 dtschema-2023.4/test/simple-bus-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-11 22:26:40.000000 dtschema-2023.4/test/simple-bus-pass.dts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6384 2023-04-11 22:26:40.000000 dtschema-2023.4/test/test-dt-validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.529180 dtschema-2023.4/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dt-check-compatible
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2128 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dt-doc-validate
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2628 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dt-extract-example
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dt-extract-props
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dt-mk-schema
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6206 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dt-prop-populate
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6934 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dt-validate
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dtb2py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/extract-compatibles
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/yaml-format
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/yaml2json
```

### Comparing `dtschema-2023.1/.github/workflows/ci.yml` & `dtschema-2023.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/.github/workflows/publish.yml` & `dtschema-2023.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/LICENSE.txt` & `dtschema-2023.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/PKG-INFO` & `dtschema-2023.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtschema
-Version: 2023.1
+Version: 2023.4
 Summary: DeviceTree validation schema and tools
 Home-page: https://github.com/devicetree-org/dt-schema
 Author: Rob Herring
 Author-email: robh@kernel.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dtschema-2023.1/README.md` & `dtschema-2023.4/README.md`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/dtb.py` & `dtschema-2023.4/dtschema/dtb.py`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/lib.py` & `dtschema-2023.4/dtschema/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,18 +495,19 @@
     schema['properties'].setdefault('$nodename', True)
     schema['properties'].setdefault('bootph-pre-sram', True)
     schema['properties'].setdefault('bootph-verify', True)
     schema['properties'].setdefault('bootph-pre-ram', True)
     schema['properties'].setdefault('bootph-some-ram', True)
     schema['properties'].setdefault('bootph-all', True)
 
-    keys = list()
-    if 'properties' in schema:
-        keys.extend(schema['properties'])
+    # 'dma-ranges' allowed when 'ranges' is present
+    if 'ranges' in schema['properties']:
+        schema['properties'].setdefault('dma-ranges', True)
 
+    keys = list(schema['properties'].keys())
     if 'patternProperties' in schema:
         keys.extend(schema['patternProperties'])
 
     for key in keys:
         if re.match(r'^pinctrl-[0-9]', key):
             break
     else:
@@ -1105,15 +1106,15 @@
 
             try:
                 schema = load_schema(uri.replace(schema_base_url, ''))
             except Exception as exc:
                 raise RefResolutionError('Unable to find schema file matching $id: ' + uri)
 
             try:
-                DTValidator.check_schema(schema)
+                DTValidator.check_schema(schema, strict=False)
             except Exception as exc:
                 raise RefResolutionError('Error in referenced schema matching $id: ' + uri)
 
             return schema
 
         from urllib.request import urlopen
```

### Comparing `dtschema-2023.1/dtschema/meta-schemas/base.yaml` & `dtschema-2023.4/dtschema/meta-schemas/base.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
               properties: true
               required: true
           - type: boolean
 
 propertyNames:
   enum: [ $id, $schema, title, description, examples, required, allOf, anyOf, oneOf,
           definitions, $defs, additionalProperties, dependencies, dependentRequired,
-          dependentSchemas, patternProperties, properties, if, then, else,
+          dependentSchemas, patternProperties, properties, not, if, then, else,
           unevaluatedProperties, deprecated, maintainers, select, $ref ]
 
 required:
   - $id
   - $schema
   - title
   - maintainers
```

### Comparing `dtschema-2023.1/dtschema/meta-schemas/cell.yaml` & `dtschema-2023.4/dtschema/meta-schemas/cell.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/meta-schemas/clocks.yaml` & `dtschema-2023.4/dtschema/meta-schemas/clocks.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/meta-schemas/core.yaml` & `dtschema-2023.4/dtschema/meta-schemas/core.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/meta-schemas/gpios.yaml` & `dtschema-2023.4/dtschema/meta-schemas/gpios.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/meta-schemas/interrupts.yaml` & `dtschema-2023.4/dtschema/meta-schemas/interrupts.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/meta-schemas/items.yaml` & `dtschema-2023.4/dtschema/meta-schemas/items.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/meta-schemas/keywords.yaml` & `dtschema-2023.4/dtschema/meta-schemas/keywords.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,15 @@
               const: const
             required:
               - const
   patternProperties:
     propertyNames:
       allOf:
         - description: Fixed strings belong in 'properties', not 'patternProperties'
+          pattern: '[\^$()*@]'
           not:
             pattern:  '^\^[a-zA-Z0-9,\-._#]+\$$'
         - description: A json-schema keyword was found instead of a DT property name.
           not:
             $ref: "#/definitions/json-schema-prop-names"
     additionalProperties:
       $ref: "#/definitions/sub-schemas"
```

### Comparing `dtschema-2023.1/dtschema/meta-schemas/nodes.yaml` & `dtschema-2023.4/dtschema/meta-schemas/nodes.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     - dependentSchemas
     - properties
     - patternProperties
     - additionalProperties
     - unevaluatedProperties
     - deprecated
     - required
+    - not
     - allOf
     - anyOf
     - oneOf
     - $ref
 
 required:
   - type
```

### Comparing `dtschema-2023.1/dtschema/meta-schemas/string-array.yaml` & `dtschema-2023.4/dtschema/meta-schemas/string-array.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/meta-schemas/vendor-props.yaml` & `dtschema-2023.4/dtschema/meta-schemas/vendor-props.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/aliases.yaml` & `dtschema-2023.4/dtschema/schemas/aliases.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/bootph.yaml` & `dtschema-2023.4/dtschema/schemas/bootph.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/bus/qemu,platform.yaml` & `dtschema-2023.4/dtschema/schemas/bus/qemu,platform.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/cache-controller.yaml` & `dtschema-2023.4/dtschema/schemas/cache-controller.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/cache.yaml` & `dtschema-2023.4/dtschema/schemas/cache.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,21 @@
   properties. A cache with a register interface or other resources should have
   its own compatible and schema. As L1 caches are described within CPU nodes,
   this binding only applies to L2 and higher level caches.
 
 maintainers:
   - Rob Herring <robh@kernel.org>
 
-# Disable until warnings fixed
-select: false
+select:
+  properties:
+    compatible:
+      const: cache
+
+  required:
+    - compatible
 
 allOf:
   - $ref: cache-controller.yaml#
 
 properties:
   $nodename:
     pattern: 'cache'
```

### Comparing `dtschema-2023.1/dtschema/schemas/chosen.yaml` & `dtschema-2023.4/dtschema/schemas/chosen.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -218,14 +218,40 @@
           };
       };
 
       This property does not represent real hardware, but the memory allocated for
       carrying the TPM measurement log. The address and the size are expressed in
       #address-cells and #size-cells, respectively of the root node.
 
+  linux,uefi-system-table:
+    $ref: types.yaml#/definitions/uint64
+    description:
+      Physical address of the UEFI System Table.
+
+  linux,uefi-mmap-start:
+    $ref: types.yaml#/definitions/uint64
+    description:
+      Physical address of the UEFI memory map, populated by the UEFI
+      GetMemoryMap() call.
+
+  linux,uefi-mmap-size:
+    $ref: types.yaml#/definitions/uint32
+    description:
+      Size in bytes of the UEFI memory map pointed to by linux,uefi-mmap-start.
+
+  linux,uefi-mmap-desc-size:
+    $ref: types.yaml#/definitions/uint32
+    description:
+      Size in bytes of each entry in the UEFI memory map.
+
+  linux,uefi-mmap-desc-ver:
+    $ref: types.yaml#/definitions/uint32
+    description:
+      Version of the mmap descriptor format.
+
   u-boot,bootconf:
     $ref: types.yaml#/definitions/string
     description:
       This property can be used by U-Boot to pass the selected configuration unit
       name of the booted image down to the operating system.
 
   u-boot,version:
```

### Comparing `dtschema-2023.1/dtschema/schemas/clock/clock.yaml` & `dtschema-2023.4/dtschema/schemas/clock/clock.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/cpu.yaml` & `dtschema-2023.4/dtschema/schemas/cpu.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/cpus.yaml` & `dtschema-2023.4/dtschema/schemas/cpus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/gpio/gpio-consumer.yaml` & `dtschema-2023.4/dtschema/schemas/gpio/gpio-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/gpio/gpio-hog.yaml` & `dtschema-2023.4/dtschema/schemas/gpio/gpio-hog.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/gpio/gpio.yaml` & `dtschema-2023.4/dtschema/schemas/gpio/gpio.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/graph.yaml` & `dtschema-2023.4/dtschema/schemas/graph.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/hwlock/hwlock-consumer.yaml` & `dtschema-2023.4/dtschema/schemas/hwlock/hwlock-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/i2c/i2c-controller.yaml` & `dtschema-2023.4/dtschema/schemas/i2c/i2c-controller.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -40,14 +40,26 @@
       Number of nanoseconds the IP core additionally needs to setup SCL.
 
   i2c-scl-rising-time-ns:
     description:
       Number of nanoseconds the SCL signal takes to rise; t(r) in the I2C
       specification.
 
+  i2c-scl-clk-low-timeout-us:
+    description:
+      Number of microseconds the clock line needs to be pulled down in order
+      to force a waiting state.
+
+  i2c-scl-has-clk-low-timeout:
+    type: boolean
+    description:
+      Indicates whether the controller implements the feature of wait
+      induction through SCL low, with the timeout being implemented
+      internally by the controller.
+
   i2c-sda-falling-time-ns:
     description:
       Number of nanoseconds the SDA signal takes to fall; t(f) in the I2C
       specification.
 
   i2c-analog-filter:
     type: boolean
@@ -117,14 +129,20 @@
 
   no-detect:
     type: boolean
     description:
       States that no other devices are present on this bus other than the ones
       listed in the devicetree.
 
+allOf:
+  - not:
+      required:
+        - i2c-scl-clk-low-timeout-us
+        - i2c-scl-has-clk-low-timeout
+
 patternProperties:
   '@[0-9a-f]+$':
     type: object
 
     properties:
       reg:
         items:
```

### Comparing `dtschema-2023.1/dtschema/schemas/iio/iio-consumer.yaml` & `dtschema-2023.4/dtschema/schemas/iio/iio-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/iio/iio.yaml` & `dtschema-2023.4/dtschema/schemas/iio/iio.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/interrupt-controller.yaml` & `dtschema-2023.4/dtschema/schemas/interrupt-controller.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/interrupts.yaml` & `dtschema-2023.4/dtschema/schemas/interrupts.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/isa/isa-bridge.yaml` & `dtschema-2023.4/dtschema/schemas/isa/isa-bridge.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/isa/isa-bus.yaml` & `dtschema-2023.4/dtschema/schemas/isa/isa-bus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/mbox/mbox-consumer.yaml` & `dtschema-2023.4/dtschema/schemas/mbox/mbox-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/memory.yaml` & `dtschema-2023.4/dtschema/schemas/memory.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/msi-consumer.yaml` & `dtschema-2023.4/dtschema/schemas/msi-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/opp/opp.yaml` & `dtschema-2023.4/dtschema/schemas/opp/opp.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/options/u-boot.yaml` & `dtschema-2023.4/dtschema/schemas/options/u-boot.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/options.yaml` & `dtschema-2023.4/dtschema/schemas/options.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/pci/pci-bus.yaml` & `dtschema-2023.4/test/schemas/good-example.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,188 +1,218 @@
-# SPDX-License-Identifier: (GPL2.0-only OR BSD-2-Clause)
+# SPDX-License-Identifier: BSD-2-Clause
 # Copyright 2018 Linaro Ltd.
+# Copyright 2018 Arm Ltd.
 %YAML 1.2
 ---
-$id: http://devicetree.org/schemas/pci/pci-bus.yaml#
-$schema: http://devicetree.org/meta-schemas/base.yaml#
+$id: http://devicetree.org/schemas/good-example.yaml#
+$schema: http://devicetree.org/meta-schemas/core.yaml#
 
-title: PCI Bus Nodes
+title: Test device with vendor properties of different types
 
-description: |
-  Common properties for PCI host bridge nodes and PCI bus structure.
-
-  PCI bus bridges have standardized Device Tree bindings:
-
-  PCI Bus Binding to: IEEE Std 1275-1994
-  http://www.devicetree.org/open-firmware/bindings/pci/pci2_1.pdf
-
-  And for the interrupt mapping part:
-
-  Open Firmware Recommended Practice: Interrupt Mapping
-  http://www.devicetree.org/open-firmware/practice/imap/imap0_9d.pdf
+description: A more detailed description for a good binding example.
 
 maintainers:
   - Rob Herring <robh@kernel.org>
 
 properties:
-  $nodename:
-    pattern: "^pcie?@"
-
-  ranges:
+  compatible:
     oneOf:
-      - $ref: /schemas/types.yaml#/definitions/flag
-      - minItems: 1
-        maxItems: 32    # Should be enough
-        items:
-          minItems: 5
-          maxItems: 7
-          additionalItems: true
-          items:
-            - enum:
-                - 0x01000000
-                - 0x02000000
-                - 0x03000000
-                - 0x42000000
-                - 0x43000000
-                - 0x81000000
-                - 0x82000000
-                - 0x83000000
-                - 0xc2000000
-                - 0xc3000000
+      - items:
+          - enum:
+              - vendor,soc4-ip
+              - vendor,soc3-ip
+              - vendor,soc2-ip
+          - enum:
+              - vendor,soc1-ip
+      - items:
+          - enum:
+              - vendor,soc1-ip
 
-  reg: true
+  reg:
+    maxItems: 2
 
-  dma-ranges:
-    oneOf:
-      - type: boolean
-      - minItems: 1
-        maxItems: 32    # Should be enough
-        items:
-          minItems: 5
-          maxItems: 7
-          additionalItems: true
-          items:
-            - enum:
-                - 0x02000000
-                - 0x03000000
-                - 0x42000000
-                - 0x43000000
+  reg-names:
+    items:
+      - const: "coreAAA"
+      - const: "aux"
 
-  "#address-cells":
-    const: 3
+  interrupts:
+    minItems: 1
+    items:
+      - description: 1st irq
+      - description: 2nd irq
+
+  interrupt-names:
+    minItems: 1
+    items:
+      - const: "tx irq"
+      - const: "rx irq"
 
-  "#size-cells":
+  '#interrupt-cells':
     const: 2
 
-  device_type:
-    const: pci
+  interrupt-controller: {}
 
-  bus-range:
-    $ref: /schemas/types.yaml#/definitions/uint32-array
-    minItems: 2
-    maxItems: 2
+  clock-frequency:
+    minimum: 100
+    maximum: 400000
+
+  clocks:
+    minItems: 1
+    items:
+      - description: 1st clock
+      - description: 2nd clock
+
+  clock-names:
     items:
-      maximum: 255
+      - const: "clk1"
+      - const: "clk2"
 
-  "#interrupt-cells":
+  '#clock-cells':
     const: 1
 
-  interrupt-map: true
-#    minItems: 1
-#    maxItems: 88    # 22 IDSEL x 4 IRQs
-#    items:
-#      minItems: 6   # 3 addr cells, 1 PCI IRQ cell, 1 phandle, 1+ parent addr and IRQ cells
-#      maxItems: 16
-
-  interrupt-map-mask:
-    items:
-      - description: PCI high address cell
-        minimum: 0
-        maximum: 0xf800
-      - description: PCI mid address cell
-        const: 0
-      - description: PCI low address cell
-        const: 0
-      - description: PCI IRQ cell
-        minimum: 0
-        maximum: 7
+  clock-output-names:
+    minItems: 1
+    maxItems: 2
 
-  linux,pci-domain:
-    $ref: /schemas/types.yaml#/definitions/uint32
+  some-gpios:
+    maxItems: 2
+
+  a-single-gpios:
+    description: A GPIO that does something
+    maxItems: 1
 
-  max-link-speed:
+  vendor,bool-prop:
+    $ref: /schemas/types.yaml#/definitions/flag
+    description: A vendor specific boolean property
+
+  vendor,int-prop:
     $ref: /schemas/types.yaml#/definitions/uint32
-    enum: [ 1, 2, 3, 4 ]
+    enum: [ 1, 2, 3 ]
+    description: Vendor specific single cell integer property
 
-  msi-map:
-    $ref: /schemas/types.yaml#/definitions/uint32-matrix
+  vendor,int-array-prop:
+    $ref: /schemas/types.yaml#/definitions/uint32-array
     items:
-      minItems: 3
-      items:
-        - description: The RID base matched by the entry
-        - description: phandle to msi-controller node
-        - description: (optional) The msi-specifier produced for the first RID matched
-            by the entry. Currently, msi-specifier is 0 or 1 cells.
-        - description: The length of consecutive RIDs following the RID base
-
-  msi-map-mask:
-    description: A mask to be applied to each Requester ID prior to being
-      mapped to an msi-specifier per the msi-map property.
-    $ref: /schemas/types.yaml#/definitions/uint32
+      minimum: 5
+      maximum: 10
+    description: Vendor specific integer array property
 
-  num-lanes:
-    description: The number of PCIe lanes
-    $ref: /schemas/types.yaml#/definitions/uint32
-    enum: [ 1, 2, 4, 8, 16, 32 ]
+  vendor,int-array-prop-2:
+    $ref: /schemas/types.yaml#/definitions/uint32-array
+    items:
+      - const: 5
+      - const: 10
+    description: Vendor specific integer array property
 
-  reset-gpios:
-    description: GPIO controlled connection to PERST# signal
-    maxItems: 1
+  vendor,int-array-size-only-prop:
+    $ref: /schemas/types.yaml#/definitions/uint32-array
+    minItems: 2
+    maxItems: 5
+    description: Vendor specific integer array property with only a size
+      range. This can use either form of brackets.
+
+  vendor,string-prop:
+    $ref: /schemas/types.yaml#/definitions/string
+    enum:
+      - foo
+      - bar
+    description: Vendor specific single string property
 
-  slot-power-limit-milliwatt:
-    description:
-      If present, specifies slot power limit in milliwatts.
-      This property is invalid in host bridge nodes.
-    maxItems: 1
+  vendor,string-list-prop:
+    $ref: /schemas/types.yaml#/definitions/string-array
+    items:
+      - const: foobar
+      - const: foobaz
+    description: Vendor specific string list property
+
+  vendor,int8-prop:
+    $ref: /schemas/types.yaml#/definitions/uint8
+    description: Vendor specific 8-bit integer property
 
-  supports-clkreq:
-    type: boolean
+  vendor,int8-array-prop:
+    $ref: /schemas/types.yaml#/definitions/uint8-array
+    minItems: 2
+    maxItems: 3
+    description: A vendor specific uint8 array property with 2 or 3 entries
 
-  aspm-no-l0s:
-    description: Disables ASPM L0s capability
-    type: boolean
+  vendor,int16-prop:
+    $ref: /schemas/types.yaml#/definitions/uint16
+    enum: [ 1, 2, 3 ]
+    description: Vendor specific 16-bit integer property
 
-  vendor-id:
-    description: The PCI vendor ID
-    $ref: /schemas/types.yaml#/definitions/uint32
+  vendor,int16-array-prop:
+    $ref: /schemas/types.yaml#/definitions/uint16-array
+    items:
+      - const: 1
+      - const: 2
+    description: Vendor specific 16-bit integer array property
+
+  vendor,int64-prop:
+    $ref: /schemas/types.yaml#/definitions/uint64
+    minimum: 0x1234
+
+    description: Vendor specific 16-bit integer property
+
+  vendor,int64-array-prop:
+    $ref: /schemas/types.yaml#/definitions/uint64-array
+    description: Vendor specific 64-bit integer array property
+
+  vendor,phandle-prop:
+    $ref: /schemas/types.yaml#/definitions/phandle
+    description: Vendor specific single cell phandle property
 
-  device-id:
-    description: The PCI device ID
-    $ref: /schemas/types.yaml#/definitions/uint32
+  vendor,phandle-array-prop:
+    $ref: /schemas/types.yaml#/definitions/phandle-array
+    minItems: 2
+    items:
+      maxItems: 1
+    description: Vendor specific array of phandles property
+
+  vendor,phandle-with-fixed-cells:
+    $ref: /schemas/types.yaml#/definitions/phandle-array
+    items:
+      - items:
+          - description: the phandle to something
+          - description: the 1st cell data
+          - description: the 2nd cell data
+    description: Vendor specific array of phandles property
 
-patternProperties:
-  "^[a-zA-Z][a-zA-Z0-9,+\\-._]{0,63}@1?[0-9a-f](,[0-7])?$":
-    type: object
-    properties:
-      compatible:
-        contains:
-          pattern: "^(pci[0-9a-f]{3,4},[0-9a-f]{1,4}|pciclass,[0-9a-f]{4,6})$"
-      reg:
-        items:
-          minItems: 5
-          maxItems: 5
-        minItems: 1
-        maxItems: 6   # Up to 6 BARs
-    required:
-      - reg
 
 required:
-  - device_type
-  - ranges
-  - reg
-  - "#address-cells"
-  - "#size-cells"
+  - compatible
+
+additionalProperties: false
+
+examples:
+  - |
+      /dts-v1/;
+      /{
+              model = "ARM Juno development board (r0)";
+              compatible = "arm,juno", "arm,vexpress";
+              interrupt-parent = <&gic>;
+              #address-cells = <2>;
+              #size-cells = <2>;
+
+                      cpus {
+                      #address-cells = <2>;
+                      #size-cells = <0>;
+                      A57_0: cpu@0 {
+                              compatible = "arm,cortex-a57","arm,armv8";
+                              reg = <0x0 0x0>;
+                              device_type = "cpu";
+                              enable-method = "psci";
+                      };
+
+                      .....
+
+                      A53_0: cpu@100 {
+                              compatible = "arm,cortex-a53","arm,armv8";
+                              reg = <0x0 0x100>;
+                              device_type = "cpu";
+                              enable-method = "psci";
+                      };
 
-dependentRequired:
-  msi-map-mask: [ msi-map ]
+                      .....
+              };
 
-additionalProperties: true
+      };
```

### Comparing `dtschema-2023.1/dtschema/schemas/pci/pci-iommu.yaml` & `dtschema-2023.4/dtschema/schemas/pci/pci-iommu.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/phy/phy-consumer.yaml` & `dtschema-2023.4/dtschema/schemas/phy/phy-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/phy/phy-provider.yaml` & `dtschema-2023.4/dtschema/schemas/phy/phy-provider.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/pinctrl/pinctrl-consumer.yaml` & `dtschema-2023.4/dtschema/schemas/pinctrl/pinctrl-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/power-domain/power-domain-consumer.yaml` & `dtschema-2023.4/dtschema/schemas/power-domain/power-domain-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/property-units.yaml` & `dtschema-2023.4/dtschema/schemas/property-units.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/pwm/pwm-consumer.yaml` & `dtschema-2023.4/dtschema/schemas/pwm/pwm-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/reset/reset.yaml` & `dtschema-2023.4/dtschema/schemas/reset/reset.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/root-node.yaml` & `dtschema-2023.4/dtschema/schemas/root-node.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/simple-bus.yaml` & `dtschema-2023.4/dtschema/schemas/simple-bus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema/schemas/types.yaml` & `dtschema-2023.4/dtschema/schemas/types.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/dtschema.egg-info/PKG-INFO` & `dtschema-2023.4/dtschema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtschema
-Version: 2023.1
+Version: 2023.4
 Summary: DeviceTree validation schema and tools
 Home-page: https://github.com/devicetree-org/dt-schema
 Author: Rob Herring
 Author-email: robh@kernel.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dtschema-2023.1/dtschema.egg-info/SOURCES.txt` & `dtschema-2023.4/dtschema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/example-schema.yaml` & `dtschema-2023.4/example-schema.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/setup.py` & `dtschema-2023.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'tools/dtb2py'
     ],
 
     python_requires='>=3.5',
 
     install_requires=[
         'ruamel.yaml>0.15.69',
-        'jsonschema>=4.1.2',
+        'jsonschema >=4.1.2, <4.18',
         'rfc3987',
         'pylibfdt',
     ],
 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
```

### Comparing `dtschema-2023.1/test/child-node-fail.dts` & `dtschema-2023.4/test/child-node-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/test/child-node.dts` & `dtschema-2023.4/test/child-node.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/test/conditionals-allof-fail.dts` & `dtschema-2023.4/test/conditionals-allof-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/test/conditionals-allof-pass.dts` & `dtschema-2023.4/test/conditionals-allof-pass.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/test/conditionals-single-fail.dts` & `dtschema-2023.4/test/conditionals-single-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/test/device-fail.dts` & `dtschema-2023.4/test/device-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/test/device.dts` & `dtschema-2023.4/test/device.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/test/schemas/bad-example.yaml` & `dtschema-2023.4/test/schemas/bad-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/test/schemas/child-node-example.yaml` & `dtschema-2023.4/test/schemas/child-node-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/test/schemas/conditionals-allof-example.yaml` & `dtschema-2023.4/test/schemas/conditionals-allof-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/test/schemas/conditionals-single-example.yaml` & `dtschema-2023.4/test/schemas/conditionals-single-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/test/simple-bus-pass.dts` & `dtschema-2023.4/test/simple-bus-pass.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/test/test-dt-validate.py` & `dtschema-2023.4/test/test-dt-validate.py`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/tools/dt-check-compatible` & `dtschema-2023.4/tools/dt-check-compatible`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/tools/dt-doc-validate` & `dtschema-2023.4/tools/dt-doc-validate`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/tools/dt-extract-example` & `dtschema-2023.4/tools/dt-extract-example`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,19 @@
 import os
 import re
 import sys
 import ruamel.yaml
 import argparse
 
 interrupt_template = """
-        interrupt-controller;
-        #interrupt-cells = < {int_cells} >;
+        interrupt-parent = <&fake_intc{index}>;
+        fake_intc{index}: fake-interrupt-controller {{
+            interrupt-controller;
+            #interrupt-cells = < {int_cells} >;
+        }};
 """
 
 example_template = """
     example-{example_num} {{
         #address-cells = <1>;
         #size-cells = <1>;
 
@@ -77,15 +80,15 @@
                     int_val = re.sub(r'\(.+|\)', r'0', int_val)
                     int_cells = len(int_val.strip().split())
                 except:
                     int_cells = 0
                 example_dts += example_start
                 ex = '        '.join(ex.splitlines(True))
                 if int_cells > 0:
-                    int_props = interrupt_template.format(int_cells=int_cells)
+                    int_props = interrupt_template.format(int_cells=int_cells, index=idx)
                 else:
                     int_props = ""
                 example_dts += example_template.format(example=ex, example_num=idx, interrupt=int_props)
             else:
                 example_dts += ex
     else:
         example_dts += example_start
```

### Comparing `dtschema-2023.1/tools/dt-extract-props` & `dtschema-2023.4/tools/dt-extract-props`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/tools/dt-mk-schema` & `dtschema-2023.4/tools/dt-mk-schema`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/tools/dt-prop-populate` & `dtschema-2023.4/tools/dt-prop-populate`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/tools/dt-validate` & `dtschema-2023.4/tools/dt-validate`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/tools/dtb2py` & `dtschema-2023.4/tools/dtb2py`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/tools/extract-compatibles` & `dtschema-2023.4/tools/extract-compatibles`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/tools/yaml-format` & `dtschema-2023.4/tools/yaml-format`

 * *Files identical despite different names*

### Comparing `dtschema-2023.1/tools/yaml2json` & `dtschema-2023.4/tools/yaml2json`

 * *Files identical despite different names*

