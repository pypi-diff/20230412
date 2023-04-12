# Comparing `tmp/torchmd-0.0.2.tar.gz` & `tmp/torchmd-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchmd-0.0.2.tar", last modified: Thu Oct 22 11:32:20 2020, max compression
+gzip compressed data, was "torchmd-0.0.4.tar", last modified: Wed Apr 12 18:04:38 2023, max compression
```

## Comparing `torchmd-0.0.2.tar` & `torchmd-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 11:32:20.941874 torchmd-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1051 2020-10-22 11:32:11.000000 torchmd-0.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)       46 2020-10-22 11:32:11.000000 torchmd-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1708 2020-10-22 11:32:20.941874 torchmd-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1084 2020-10-22 11:32:11.000000 torchmd-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       59 2020-10-22 11:32:11.000000 torchmd-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-22 11:32:20.941874 torchmd-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1212 2020-10-22 11:32:11.000000 torchmd-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 11:32:20.941874 torchmd-0.0.2/torchmd/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 11:32:20.941874 torchmd-0.0.2/torchmd/forcefields/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/forcefields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4147 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/forcefields/ff_parmed.py
--rw-r--r--   0 runner    (1001) docker     (116)     3494 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/forcefields/ff_yaml.py
--rw-r--r--   0 runner    (1001) docker     (116)     1422 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/forcefields/forcefield.py
--rw-r--r--   0 runner    (1001) docker     (116)    22685 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/forces.py
--rw-r--r--   0 runner    (1001) docker     (116)     2073 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/integrator.py
--rw-r--r--   0 runner    (1001) docker     (116)     2138 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/minimizers.py
--rw-r--r--   0 runner    (1001) docker     (116)     1807 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/mycalc.py
--rw-r--r--   0 runner    (1001) docker     (116)     1575 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/neighbourlist.py
--rw-r--r--   0 runner    (1001) docker     (116)    10497 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)     7370 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/run.py
--rw-r--r--   0 runner    (1001) docker     (116)     2796 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/systems.py
--rw-r--r--   0 runner    (1001) docker     (116)     2379 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1994 2020-10-22 11:32:11.000000 torchmd-0.0.2/torchmd/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 11:32:20.941874 torchmd-0.0.2/torchmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1708 2020-10-22 11:32:20.000000 torchmd-0.0.2/torchmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      559 2020-10-22 11:32:20.000000 torchmd-0.0.2/torchmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-22 11:32:20.000000 torchmd-0.0.2/torchmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       31 2020-10-22 11:32:20.000000 torchmd-0.0.2/torchmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2020-10-22 11:32:20.000000 torchmd-0.0.2/torchmd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:04:38.820437 torchmd-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-12 18:04:01.000000 torchmd-0.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 18:04:01.000000 torchmd-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-12 18:04:38.820437 torchmd-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-12 18:04:01.000000 torchmd-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-12 18:04:01.000000 torchmd-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:04:38.820437 torchmd-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 18:04:01.000000 torchmd-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:04:38.816437 torchmd-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20120 2023-04-12 18:04:01.000000 torchmd-0.0.4/tests/test_torchmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:04:38.820437 torchmd-0.0.4/torchmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-12 18:04:38.820437 torchmd-0.0.4/torchmd/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:04:38.820437 torchmd-0.0.4/torchmd/forcefields/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/forcefields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/forcefields/ff_parmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/forcefields/ff_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/forcefields/forcefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22744 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/forces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/minimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/mycalc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/neighbourlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-12 18:04:01.000000 torchmd-0.0.4/torchmd/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:04:38.820437 torchmd-0.0.4/torchmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-12 18:04:38.000000 torchmd-0.0.4/torchmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-12 18:04:38.000000 torchmd-0.0.4/torchmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:04:38.000000 torchmd-0.0.4/torchmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:04:38.000000 torchmd-0.0.4/torchmd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 18:04:38.000000 torchmd-0.0.4/torchmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 18:04:38.000000 torchmd-0.0.4/torchmd.egg-info/top_level.txt
```

### Comparing `torchmd-0.0.2/LICENSE.md` & `torchmd-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.2/torchmd/forcefields/ff_parmed.py` & `torchmd-0.0.4/torchmd/forcefields/ff_parmed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from torchmd.forcefields.forcefield import _ForceFieldBase
 from math import radians
 import numpy as np
 
 
 def load_parmed_parameters(fname):
-    """ Convenience method for reading parameter files with parmed
+    """Convenience method for reading parameter files with parmed
 
     Parameters
     ----------
     fname : str
         Parameter file name
 
     Returns
```

### Comparing `torchmd-0.0.2/torchmd/forcefields/ff_yaml.py` & `torchmd-0.0.4/torchmd/forcefields/ff_yaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import numpy as np
 import yaml
 
 
 class YamlForcefield(_ForceFieldBase):
     def __init__(self, mol, prm):
         self.mol = mol
-        self.prm = yaml.load(open(prm), Loader=yaml.FullLoader)
+        with open(prm, "r") as f:
+            self.prm = yaml.load(f, Loader=yaml.FullLoader)
 
     def _get_x_variants(self, atomtypes):
         from itertools import product
 
         permutations = np.array(
             sorted(
                 list(product([False, True], repeat=len(atomtypes))),
@@ -48,22 +49,22 @@
                 return termpar[atomtypestr]
         raise RuntimeError(f"{atomtypes} doesn't have {term} information in the FF")
 
     def get_atom_types(self):
         return np.unique(self.prm["atomtypes"])
 
     def get_charge(self, at):
-        params = self.get_parameters("electrostatics", [at,])
+        params = self.get_parameters("electrostatics", [at])
         return params["charge"]
 
     def get_mass(self, at):
         return self.prm["masses"][at]
 
     def get_LJ(self, at):
-        params = self.get_parameters("lj", [at,])
+        params = self.get_parameters("lj", [at])
         return params["sigma"], params["epsilon"]
 
     def get_bond(self, at1, at2):
         params = self.get_parameters("bonds", [at1, at2])
         return params["k0"], params["req"]
 
     def get_angle(self, at1, at2, at3):
@@ -82,16 +83,16 @@
     def get_14(self, at1, at2, at3, at4):
         params = self.get_parameters("dihedrals", [at1, at2, at3, at4])
 
         terms = []
         for term in params["terms"]:
             terms.append([term["phi_k"], radians(term["phase"]), term["per"]])
 
-        lj1 = self.get_parameters("lj", [at1,])
-        lj4 = self.get_parameters("lj", [at4,])
+        lj1 = self.get_parameters("lj", [at1])
+        lj4 = self.get_parameters("lj", [at4])
         return (
             params["scnb"] if "scnb" in params else 1,
             params["scee"] if "scee" in params else 1,
             lj1["sigma14"],
             lj1["epsilon14"],
             lj4["sigma14"],
             lj4["epsilon14"],
```

### Comparing `torchmd-0.0.2/torchmd/forcefields/forcefield.py` & `torchmd-0.0.4/torchmd/forcefields/forcefield.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.2/torchmd/forces.py` & `torchmd-0.0.4/torchmd/forces.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from scipy import constants as const
 import torch
-import yaml
 import numpy as np
 from math import pi
 
 
 class Forces:
     """
-        Parameters
-        ----------
-        cutoff : float
-            If set to a value it will only calculate LJ, electrostatics and bond energies for atoms which are closer
-            than the threshold
-        rfa : bool
-            Use with `cutoff` to enable the reaction field approximation for scaling of the electrostatics up to the cutoff.
-            Uses the value of `solventDielectric` to model everything beyond the cutoff distance as solvent with uniform
-            dielectric.
-        solventDielectric : float
-            Used together with `cutoff` and `rfa`
+    Parameters
+    ----------
+    cutoff : float
+        If set to a value it will only calculate LJ, electrostatics and bond energies for atoms which are closer
+        than the threshold
+    rfa : bool
+        Use with `cutoff` to enable the reaction field approximation for scaling of the electrostatics up to the cutoff.
+        Uses the value of `solventDielectric` to model everything beyond the cutoff distance as solvent with uniform
+        dielectric.
+    solventDielectric : float
+        Used together with `cutoff` and `rfa`
     """
 
     # 1-4 is nonbonded but we put it currently in bonded to not calculate all distances
     bonded = ["bonds", "angles", "dihedrals", "impropers", "1-4"]
     nonbonded = ["electrostatics", "lj", "repulsion", "repulsioncg"]
     terms = bonded + nonbonded
 
@@ -34,29 +33,24 @@
         rfa=False,
         solventDielectric=78.5,
         switch_dist=None,
         exclusions=("bonds", "angles", "1-4"),
     ):
         self.par = parameters
         if terms is None:
-            terms = (
-                "electrostatics",
-                "lj",
-                "bonds",
-                "angles",
-                "dihedrals",
-                "1-4",
-                "impropers",
+            raise RuntimeError(
+                'Set force terms or leave empty brackets [].\nAvailable options: "bonds", "angles", "dihedrals", "impropers", "1-4", "electrostatics", "lj", "repulsion", "repulsioncg".'
             )
+
         self.energies = [ene.lower() for ene in terms]
         for et in self.energies:
             if et not in Forces.terms:
                 raise ValueError(f"Force term {et} is not implemented.")
 
-        if "1-4" in self.energies and not "dihedrals" in self.energies:
+        if "1-4" in self.energies and "dihedrals" not in self.energies:
             raise RuntimeError(
                 "You cannot enable 1-4 interactions without enabling dihedrals"
             )
 
         self.natoms = len(parameters.masses)
         self.require_distances = any(f in self.nonbonded for f in self.energies)
         self.ava_idx = (
@@ -324,15 +318,18 @@
             for i in range(nsystems):
                 for ene in pot[i]:
                     if pot[i][ene].requires_grad:
                         enesum += pot[i][ene]
             forces[:] = -torch.autograd.grad(
                 enesum, pos, only_inputs=True, retain_graph=True
             )[0]
-            return enesum
+            if returnDetails:
+                return pot
+            else:
+                return [torch.sum(torch.cat(list(pp.values()))) for pp in pot]
 
         if returnDetails:
             return [{k: v.cpu().item() for k, v in pp.items()} for pp in pot]
         else:
             return [np.sum([v.cpu().item() for _, v in pp.items()]) for pp in pot]
 
     def _make_indeces(self, natoms, excludepairs, device):
@@ -359,15 +356,15 @@
     direction_vec = wrap_dist(atom_pos[atom_idx[:, 0]] - atom_pos[atom_idx[:, 1]], box)
     dist = torch.norm(direction_vec, dim=1)
     direction_unitvec = direction_vec / dist.unsqueeze(1)
     return dist, direction_unitvec, direction_vec
 
 
 ELEC_FACTOR = 1 / (4 * const.pi * const.epsilon_0)  # Coulomb's constant
-ELEC_FACTOR *= const.elementary_charge ** 2  # Convert elementary charges to Coulombs
+ELEC_FACTOR *= const.elementary_charge**2  # Convert elementary charges to Coulombs
 ELEC_FACTOR /= const.angstrom  # Convert Angstroms to meters
 ELEC_FACTOR *= const.Avogadro / (const.kilo * const.calorie)  # Convert J to kcal/mol
 
 
 def evaluate_LJ(
     dist, pair_indeces, atom_types, A, B, switch_dist, cutoff, explicit_forces=True
 ):
@@ -379,15 +376,15 @@
 
 def evaluate_LJ_internal(
     dist, aa, bb, scale, switch_dist, cutoff, explicit_forces=True
 ):
     force = None
 
     rinv1 = 1 / dist
-    rinv6 = rinv1 ** 6
+    rinv6 = rinv1**6
     rinv12 = rinv6 * rinv6
 
     pot = ((aa * rinv12) - (bb * rinv6)) / scale
     if explicit_forces:
         force = (-12 * aa * rinv12 + 6 * bb * rinv6) * rinv1 / scale
 
     # Switching function
@@ -410,15 +407,15 @@
 ):  # LJ without B
     force = None
 
     atomtype_indices = atom_types[pair_indeces]
     aa = A[atomtype_indices[:, 0], atomtype_indices[:, 1]]
 
     rinv1 = 1 / dist
-    rinv6 = rinv1 ** 6
+    rinv6 = rinv1**6
     rinv12 = rinv6 * rinv6
 
     pot = (aa * rinv12) / scale
     if explicit_forces:
         force = (-12 * aa * rinv12) * rinv1 / scale
     return pot, force
 
@@ -428,15 +425,15 @@
 ):  # Repulsion like from CGNet
     force = None
 
     atomtype_indices = atom_types[pair_indeces]
     coef = B[atomtype_indices[:, 0], atomtype_indices[:, 1]]
 
     rinv1 = 1 / dist
-    rinv6 = rinv1 ** 6
+    rinv6 = rinv1**6
 
     pot = (coef * rinv6) / scale
     if explicit_forces:
         force = (-6 * coef * rinv6) * rinv1 / scale
     return pot, force
 
 
@@ -452,23 +449,23 @@
 ):
     force = None
     if rfa:  # Reaction field approximation for electrostatics with cutoff
         # http://docs.openmm.org/latest/userguide/theory.html#coulomb-interaction-with-cutoff
         # Ilario G. Tironi, René Sperb, Paul E. Smith, and Wilfred F. van Gunsteren. A generalized reaction field method
         # for molecular dynamics simulations. Journal of Chemical Physics, 102(13):5451–5459, 1995.
         denom = (2 * solventDielectric) + 1
-        krf = (1 / cutoff ** 3) * (solventDielectric - 1) / denom
+        krf = (1 / cutoff**3) * (solventDielectric - 1) / denom
         crf = (1 / cutoff) * (3 * solventDielectric) / denom
         common = (
             ELEC_FACTOR
             * atom_charges[pair_indeces[:, 0]]
             * atom_charges[pair_indeces[:, 1]]
             / scale
         )
-        dist2 = dist ** 2
+        dist2 = dist**2
         pot = common * ((1 / dist) + krf * dist2 - crf)
         if explicit_forces:
             force = common * (2 * krf * dist - 1 / dist2)
     else:
         pot = (
             ELEC_FACTOR
             * atom_charges[pair_indeces[:, 0]]
@@ -483,15 +480,15 @@
 
 def evaluate_bonds(dist, bond_params, explicit_forces=True):
     force = None
 
     k0 = bond_params[:, 0]
     d0 = bond_params[:, 1]
     x = dist - d0
-    pot = k0 * (x ** 2)
+    pot = k0 * (x**2)
     if explicit_forces:
         force = 2 * k0 * x
     return pot, force
 
 
 def evaluate_angles(r21, r23, angle_params, explicit_forces=True):
     k0 = angle_params[:, 0]
@@ -559,29 +556,29 @@
             pot.scatter_add_(0, idx, k0 * (1 + torch.cos(angleDiff)))
             if explicit_forces:
                 coeff.scatter_add_(0, idx, -per * k0 * torch.sin(angleDiff))
         else:  # CHARMM torsions
             angleDiff = phi[idx] - phi0
             angleDiff[angleDiff < -pi] = angleDiff[angleDiff < -pi] + 2 * pi
             angleDiff[angleDiff > pi] = angleDiff[angleDiff > pi] - 2 * pi
-            pot.scatter_add_(0, idx, k0 * angleDiff ** 2)
+            pot.scatter_add_(0, idx, k0 * angleDiff**2)
             if explicit_forces:
                 coeff.scatter_add_(0, idx, 2 * k0 * angleDiff)
 
     # coeff.unsqueeze_(1)
 
     force0, force1, force2, force3 = None, None, None, None
     if explicit_forces:
         # Taken from OpenMM
         normDelta2 = torch.norm(r23, dim=1)
-        norm2Delta2 = normDelta2 ** 2
-        forceFactor0 = (-coeff * normDelta2) / (normA ** 2)
+        norm2Delta2 = normDelta2**2
+        forceFactor0 = (-coeff * normDelta2) / (normA**2)
         forceFactor1 = torch.sum(r12 * r23, dim=1) / norm2Delta2
         forceFactor2 = torch.sum(r34 * r23, dim=1) / norm2Delta2
-        forceFactor3 = (coeff * normDelta2) / (normB ** 2)
+        forceFactor3 = (coeff * normDelta2) / (normB**2)
 
         force0vec = forceFactor0.unsqueeze(1) * crossA
         force3vec = forceFactor3.unsqueeze(1) * crossB
         s = (
             forceFactor1.unsqueeze(1) * force0vec
             - forceFactor2.unsqueeze(1) * force3vec
         )
```

### Comparing `torchmd-0.0.2/torchmd/integrator.py` & `torchmd-0.0.4/torchmd/integrator.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.2/torchmd/minimizers.py` & `torchmd-0.0.4/torchmd/minimizers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import torch
 import numpy as np
 
 
 def minimize_bfgs(system, forces, fmax=0.5, steps=1000):
     from scipy.optimize import minimize
 
+    if steps == 0:
+        return
+
     if system.pos.shape[0] != 1:
         raise RuntimeError(
             "System minimization currently doesn't support replicas. Talk with Stefan to implement it."
         )
 
     def evalfunc(coords, info):
         coords = coords.reshape(1, -1, 3)
@@ -42,24 +45,30 @@
         dtype=system.pos.dtype,
         device=system.pos.device,
         requires_grad=system.pos.requires_grad,
     )
 
 
 def minimize_pytorch_bfgs(system, forces, steps=1000):
+    if steps == 0:
+        return
+
     pos = system.pos.detach().requires_grad_(True)
     opt = torch.optim.LBFGS([pos], max_iter=steps, tolerance_change=1e-09)
 
     def closure(step):
         opt.zero_grad()
-        Epot = forces.compute(pos, system.box, system.forces, explicit_forces=False)
-        Epot.backward()
-        maxforce = float(torch.max(torch.norm(pos.grad, dim=1)))
-        print("{0:4d}   {1: 3.6f}   {2: 3.6f}".format(step[0], float(Epot), maxforce))
+        Epot = forces.compute(
+            pos, system.box, system.forces, explicit_forces=False, returnDetails=False
+        )
+        Etot = torch.sum(torch.cat(Epot))
+        grad = -system.forces.detach().cpu().numpy().astype(np.float64)[0]
+        maxforce = float(torch.max(torch.norm(grad, dim=1)))
+        print("{0:4d}   {1: 3.6f}   {2: 3.6f}".format(step[0], float(Etot), maxforce))
         step[0] += 1
-        return Epot
+        return Etot
 
     print("{0:4s} {1:9s}       {2:9s}".format("Iter", " Epot", " fmax"))
     step = [0]
     opt.step(lambda: closure(step))
 
     system.pos[:] = pos.detach().requires_grad_(False)
```

### Comparing `torchmd-0.0.2/torchmd/mycalc.py` & `torchmd-0.0.4/torchmd/mycalc.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,43 +5,60 @@
 import numpy as np
 from ase.units import Bohr, Hartree, kcal, mol, Angstrom
 import os
 import torch
 
 
 class MyCalc(Calculator):
-    implemented_properties = ['energy', 'forces']
+    implemented_properties = ["energy", "forces"]
 
-    def __init__(self, evaluator, restart=None, ignore_bad_restart=False,
-                 label='mycalc', atoms=None, command=None,
-                 **kwargs):
-        Calculator.__init__(self, restart=restart,
-                            ignore_bad_restart=ignore_bad_restart, label=label,
-                            atoms=atoms, command=command, **kwargs)
+    def __init__(
+        self,
+        evaluator,
+        restart=None,
+        ignore_bad_restart=False,
+        label="mycalc",
+        atoms=None,
+        command=None,
+        **kwargs
+    ):
+        Calculator.__init__(
+            self,
+            restart=restart,
+            ignore_bad_restart=ignore_bad_restart,
+            label=label,
+            atoms=atoms,
+            command=command,
+            **kwargs
+        )
         self.evaluator = evaluator
 
-    def calculate(self, atoms=None, properties=['energy'],
-                  system_changes=all_changes, symmetry='c1'):
+    def calculate(
+        self,
+        atoms=None,
+        properties=["energy"],
+        system_changes=all_changes,
+        symmetry="c1",
+    ):
 
         Calculator.calculate(self, atoms=atoms)
         if self.atoms is None:
-            raise CalculatorSetupError('An Atoms object must be provided to '
-                                       'perform a calculation')
+            raise CalculatorSetupError(
+                "An Atoms object must be provided to " "perform a calculation"
+            )
         atoms = self.atoms
 
         pos = torch.tensor(atoms.positions).double().to("cpu")
         cell = atoms.cell.tolist()
         cell = torch.tensor([cell[0][0], cell[1][1], cell[2][2]]).double().to("cpu")
         energy = self.evaluator.compute(pos, cell)
-        
+
         # Do the calculations
-        if 'forces' in properties:
+        if "forces" in properties:
             # energy comes for free
-            self.results['energy'] = energy
+            self.results["energy"] = energy
             # convert to eV/A
             # also note that the gradient is -1 * forces
-            self.results['forces'] = self.evaluator.forces.cpu().numpy()
-        elif 'energy' in properties:
+            self.results["forces"] = self.evaluator.forces.cpu().numpy()
+        elif "energy" in properties:
             # convert to eV
-            self.results['energy'] = energy
-
-
+            self.results["energy"] = energy
```

### Comparing `torchmd-0.0.2/torchmd/neighbourlist.py` & `torchmd-0.0.4/torchmd/neighbourlist.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     cellneighbours[negvals] += nbins[negvals]
     largevals = cellneighbours > (nbins - 1)
     cellneighbours[largevals] -= nbins[largevals]
 
     return xbins, ybins, zbins, cellneighbours
 
 
-def neighbour_list(pos, box, subcell_size):
-    nsystems = coordinates.shape[0]
+# def neighbour_list(pos, box, subcell_size):
+#     nsystems = coordinates.shape[0]
 
-    for s in range(nsystems):
-        spos = pos[s]
-        sbox = box[s]
+#     for s in range(nsystems):
+#         spos = pos[s]
+#         sbox = box[s]
 
-        xbins, ybins, zbins = discretize_box(sbox, subcell_size)
+#         xbins, ybins, zbins = discretize_box(sbox, subcell_size)
 
-        xidx = torch.bucketize(spos[:, 0], xbins, out_int32=True)
-        yidx = torch.bucketize(spos[:, 1], ybins, out_int32=True)
-        zidx = torch.bucketize(spos[:, 2], zbins, out_int32=True)
+#         xidx = torch.bucketize(spos[:, 0], xbins, out_int32=True)
+#         yidx = torch.bucketize(spos[:, 1], ybins, out_int32=True)
+#         zidx = torch.bucketize(spos[:, 2], zbins, out_int32=True)
 
-        binidx = torch.stack((xidx, yidx, zidx)).T
+#         binidx = torch.stack((xidx, yidx, zidx)).T
```

### Comparing `torchmd-0.0.2/torchmd/parameters.py` & `torchmd-0.0.4/torchmd/parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import torch
 from math import sqrt
 import numpy as np
 
 
 class Parameters:
     def __init__(
-        self, ff, mol, terms=None, precision=torch.float, device="cpu",
+        self,
+        ff,
+        mol,
+        terms=None,
+        precision=torch.float,
+        device="cpu",
     ):
         self.A = None
         self.B = None
         self.bonds = None
         self.bond_params = None
         self.charges = None
         self.masses = None
@@ -21,25 +26,27 @@
         self.idx14 = None
         self.nonbonded_14_params = None
         self.impropers = None
         self.improper_params = None
 
         self.natoms = mol.numAtoms
         if terms is None:
-            terms = ("bonds", "angles", "dihedrals", "impropers", "1-4")
+            terms = ("bonds", "angles", "dihedrals", "impropers", "1-4", "lj")
         terms = [term.lower() for term in terms]
         self.build_parameters(ff, mol, terms)
         self.precision_(precision)
         self.to_(device)
 
     def to_(self, device):
-        self.A = self.A.to(device)
-        self.B = self.B.to(device)
         self.charges = self.charges.to(device)
         self.masses = self.masses.to(device)
+        if self.A is not None:
+            self.A = self.A.to(device)
+        if self.B is not None:
+            self.B = self.B.to(device)
         if self.bonds is not None:
             self.bonds = self.bonds.to(device)
             self.bond_params = self.bond_params.to(device)
         if self.angles is not None:
             self.angles = self.angles.to(device)
             self.angle_params = self.angle_params.to(device)
         if self.dihedrals is not None:
@@ -52,21 +59,25 @@
             self.idx14 = self.idx14.to(device)
             self.nonbonded_14_params = self.nonbonded_14_params.to(device)
         if self.impropers is not None:
             self.impropers = self.impropers.to(device)
             termparams = self.improper_params[0]
             termparams["idx"] = termparams["idx"].to(device)
             termparams["params"] = termparams["params"].to(device)
+        if self.mapped_atom_types is not None:
+            self.mapped_atom_types = self.mapped_atom_types.to(device)
         self.device = device
 
     def precision_(self, precision):
-        self.A = self.A.type(precision)
-        self.B = self.B.type(precision)
         self.charges = self.charges.type(precision)
         self.masses = self.masses.type(precision)
+        if self.A is not None:
+            self.A = self.A.type(precision)
+        if self.B is not None:
+            self.B = self.B.type(precision)
         if self.bonds is not None:
             self.bond_params = self.bond_params.type(precision)
         if self.angles is not None:
             self.angle_params = self.angle_params.type(precision)
         if self.dihedrals is not None:
             for j in range(len(self.dihedral_params)):
                 termparams = self.dihedral_params[j]
@@ -99,15 +110,16 @@
 
     def build_parameters(self, ff, mol, terms):
         uqatomtypes, indexes = np.unique(mol.atomtype, return_inverse=True)
 
         self.mapped_atom_types = torch.tensor(indexes)
         self.charges = torch.tensor(mol.charge.astype(np.float64))
         self.masses = self.make_masses(ff, mol.atomtype)
-        self.A, self.B = self.make_lj(ff, uqatomtypes)
+        if "lj" in terms or "LJ" in terms:
+            self.A, self.B = self.make_lj(ff, uqatomtypes)
         if "bonds" in terms and len(mol.bonds):
             uqbonds = np.unique([sorted(bb) for bb in mol.bonds], axis=0)
             self.bonds = torch.tensor(uqbonds.astype(np.int64))
             self.bond_params = self.make_bonds(ff, uqatomtypes[indexes[uqbonds]])
         if "angles" in terms and len(mol.angles):
             uqangles = np.unique(
                 [ang if ang[0] < ang[2] else ang[::-1] for ang in mol.angles], axis=0
@@ -216,27 +228,27 @@
     def make_14(self, ff, uq14atomtypes):
         nonbonded_14_params = []
         for uqdih in uq14atomtypes:
             scnb, scee, lj1_s14, lj1_e14, lj4_s14, lj4_e14 = ff.get_14(*uqdih)
             # Lorentz - Berthelot combination rule
             sig = 0.5 * (lj1_s14 + lj4_s14)
             eps = sqrt(lj1_e14 * lj4_e14)
-            s6 = sig ** 6
+            s6 = sig**6
             s12 = s6 * s6
             A = eps * 4 * s12
             B = eps * 4 * s6
             nonbonded_14_params.append([A, B, scnb, scee])
         return torch.tensor(nonbonded_14_params)
 
 
 def calculate_AB(sigma, epsilon):
     # Lorentz - Berthelot combination rule
     sigma_table = 0.5 * (sigma + sigma[:, None])
     eps_table = np.sqrt(epsilon * epsilon[:, None])
-    sigma_table_6 = sigma_table ** 6
+    sigma_table_6 = sigma_table**6
     sigma_table_12 = sigma_table_6 * sigma_table_6
     A = eps_table * 4 * sigma_table_12
     B = eps_table * 4 * sigma_table_6
     del sigma_table_12, sigma_table_6, eps_table, sigma_table
     return A, B
```

### Comparing `torchmd-0.0.2/torchmd/systems.py` & `torchmd-0.0.4/torchmd/systems.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.2/torchmd/utils.py` & `torchmd-0.0.4/torchmd/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-import glob
 import csv
 import json
 import os
 import time
 import argparse
-import torch
 import yaml
-import sys
-import numpy as np
 
 
 class LogWriter(object):
     # kind of inspired form openai.baselines.bench.monitor
     # We can add here an optional Tensorboard logger as well
     def __init__(self, path, keys, header="", name="monitor.csv"):
         self.keys = tuple(keys) + ("t",)
@@ -64,14 +60,15 @@
         if isinstance(exclude, str):
             exclude = [
                 exclude,
             ]
         args = args.__dict__.copy()
         for exl in exclude:
             del args[exl]
-        yaml.dump(args, open(filename, "w"))
+        with open(filename, "w") as fout:
+            yaml.dump(args, fout)
     else:
         with open(filename, "w") as f:
             for k, v in args.__dict__.items():
                 if k is exclude:
                     continue
                 f.write(f"{k}={v}\n")
```

### Comparing `torchmd-0.0.2/torchmd/wrapper.py` & `torchmd-0.0.4/torchmd/wrapper.py`

 * *Files identical despite different names*

### Comparing `torchmd-0.0.2/torchmd.egg-info/SOURCES.txt` & `torchmd-0.0.4/torchmd.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 LICENSE.md
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.py
+tests/test_torchmd.py
 torchmd/__init__.py
+torchmd/_version.py
 torchmd/forces.py
 torchmd/integrator.py
 torchmd/minimizers.py
 torchmd/mycalc.py
 torchmd/neighbourlist.py
 torchmd/parameters.py
 torchmd/run.py
 torchmd/systems.py
 torchmd/utils.py
 torchmd/wrapper.py
 torchmd.egg-info/PKG-INFO
 torchmd.egg-info/SOURCES.txt
 torchmd.egg-info/dependency_links.txt
+torchmd.egg-info/not-zip-safe
 torchmd.egg-info/requires.txt
 torchmd.egg-info/top_level.txt
 torchmd/forcefields/__init__.py
 torchmd/forcefields/ff_parmed.py
 torchmd/forcefields/ff_yaml.py
 torchmd/forcefields/forcefield.py
```

