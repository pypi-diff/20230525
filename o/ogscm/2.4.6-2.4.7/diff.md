# Comparing `tmp/ogscm-2.4.6.tar.gz` & `tmp/ogscm-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogscm-2.4.6.tar", max compression
+gzip compressed data, was "ogscm-2.4.7.tar", max compression
```

## Comparing `ogscm-2.4.6.tar` & `ogscm-2.4.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1510 2022-06-03 08:39:37.970667 ogscm-2.4.6/LICENSE
--rw-r--r--   0        0        0    11662 2022-06-03 08:39:37.970667 ogscm-2.4.6/README.md
--rw-r--r--   0        0        0       81 2022-06-03 08:39:37.970667 ogscm-2.4.6/ogscm/__init__.py
--rw-r--r--   0        0        0      118 2022-06-03 08:39:37.970667 ogscm-2.4.6/ogscm/app/__init__.py
--rw-r--r--   0        0        0     3942 2022-06-03 08:39:37.970667 ogscm-2.4.6/ogscm/app/builder.py
--rw-r--r--   0        0        0     1600 2022-06-03 08:39:37.970667 ogscm-2.4.6/ogscm/app/deployer.py
--rw-r--r--   0        0        0      402 2022-06-03 08:39:37.970667 ogscm-2.4.6/ogscm/building_blocks/__init__.py
--rw-r--r--   0        0        0     1477 2022-06-03 08:39:37.970667 ogscm-2.4.6/ogscm/building_blocks/ccache.py
--rw-r--r--   0        0        0     3312 2022-06-03 08:39:37.970667 ogscm-2.4.6/ogscm/building_blocks/lmod.py
--rw-r--r--   0        0        0     7047 2022-06-03 08:39:37.970667 ogscm-2.4.6/ogscm/building_blocks/ogs.py
--rw-r--r--   0        0        0     3366 2022-06-03 08:39:37.970667 ogscm-2.4.6/ogscm/building_blocks/ogs_base.py
--rw-r--r--   0        0        0     4124 2022-06-03 08:39:37.970667 ogscm-2.4.6/ogscm/building_blocks/osu_benchmarks.py
--rw-r--r--   0        0        0     5228 2022-06-03 08:39:37.970667 ogscm-2.4.6/ogscm/building_blocks/paraview.py
--rw-r--r--   0        0        0     3643 2022-06-03 08:39:37.970667 ogscm-2.4.6/ogscm/building_blocks/pm_easybuild.py
--rw-r--r--   0        0        0    10299 2022-06-03 08:39:37.970667 ogscm-2.4.6/ogscm/cli.py
--rw-r--r--   0        0        0      148 2022-06-03 08:39:37.970667 ogscm-2.4.6/ogscm/common.py
--rw-r--r--   0        0        0      645 2022-06-03 08:39:37.974001 ogscm-2.4.6/ogscm/config.py
--rw-r--r--   0        0        0        0 2022-06-03 08:39:37.974001 ogscm-2.4.6/ogscm/recipes/__init__.py
--rw-r--r--   0        0        0      733 2022-06-03 08:39:37.974001 ogscm-2.4.6/ogscm/recipes/_template.py
--rw-r--r--   0        0        0     3065 2022-06-03 08:39:37.974001 ogscm-2.4.6/ogscm/recipes/compiler.py
--rw-r--r--   0        0        0      116 2022-06-03 08:39:37.974001 ogscm-2.4.6/ogscm/recipes/files/jupyterlab-gitlab_settings.json
--rw-r--r--   0        0        0     2742 2022-06-03 08:39:37.974001 ogscm-2.4.6/ogscm/recipes/mpi-entrypoint.sh
--rw-r--r--   0        0        0     6536 2022-06-03 08:39:37.974001 ogscm-2.4.6/ogscm/recipes/mpi.py
--rw-r--r--   0        0        0    21626 2022-06-03 08:39:37.974001 ogscm-2.4.6/ogscm/recipes/ogs.py
--rw-r--r--   0        0        0     3406 2022-06-03 08:39:37.974001 ogscm-2.4.6/ogscm/recipes/ogs_jupyter.py
--rw-r--r--   0        0        0      665 2022-06-03 08:39:37.974001 ogscm-2.4.6/ogscm/recipes/python_vtk.py
--rw-r--r--   0        0        0      123 2022-06-03 08:39:37.974001 ogscm-2.4.6/ogscm/version.py
--rw-r--r--   0        0        0      662 2022-06-03 08:39:37.974001 ogscm-2.4.6/pyproject.toml
--rw-r--r--   0        0        0    12808 2022-06-03 08:39:55.935660 ogscm-2.4.6/setup.py
--rw-r--r--   0        0        0    12538 2022-06-03 08:39:55.937018 ogscm-2.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1510 2023-05-22 13:15:50.275640 ogscm-2.4.7/LICENSE
+-rw-r--r--   0        0        0    11903 2023-05-22 13:15:50.275640 ogscm-2.4.7/README.md
+-rw-r--r--   0        0        0       81 2023-05-22 13:15:50.275640 ogscm-2.4.7/ogscm/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/app/__init__.py
+-rw-r--r--   0        0        0     3942 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/app/builder.py
+-rw-r--r--   0        0        0     1600 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/app/deployer.py
+-rw-r--r--   0        0        0      402 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/__init__.py
+-rw-r--r--   0        0        0     1477 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/ccache.py
+-rw-r--r--   0        0        0     3312 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/lmod.py
+-rw-r--r--   0        0        0     7047 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/ogs.py
+-rw-r--r--   0        0        0     3245 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/ogs_base.py
+-rw-r--r--   0        0        0     4124 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/osu_benchmarks.py
+-rw-r--r--   0        0        0     5228 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/paraview.py
+-rw-r--r--   0        0        0     3643 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/building_blocks/pm_easybuild.py
+-rw-r--r--   0        0        0    10303 2023-05-25 10:55:11.905500 ogscm-2.4.7/ogscm/cli.py
+-rw-r--r--   0        0        0      148 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/common.py
+-rw-r--r--   0        0        0      645 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/config.py
+-rw-r--r--   0        0        0        0 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/__init__.py
+-rw-r--r--   0        0        0      733 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/_template.py
+-rw-r--r--   0        0        0     3065 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/compiler.py
+-rw-r--r--   0        0        0      116 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/files/jupyterlab-gitlab_settings.json
+-rw-r--r--   0        0        0     2742 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/mpi-entrypoint.sh
+-rw-r--r--   0        0        0     6535 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/mpi.py
+-rw-r--r--   0        0        0    22872 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/ogs.py
+-rw-r--r--   0        0        0     3471 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/ogs_jupyter.py
+-rw-r--r--   0        0        0     1083 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/ogs_vscode.py
+-rw-r--r--   0        0        0     1090 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/ogs_web.py
+-rw-r--r--   0        0        0      665 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/recipes/python_vtk.py
+-rw-r--r--   0        0        0      123 2023-05-22 13:15:50.278973 ogscm-2.4.7/ogscm/version.py
+-rw-r--r--   0        0        0      661 2023-05-25 10:55:11.905500 ogscm-2.4.7/pyproject.toml
+-rw-r--r--   0        0        0    12827 1970-01-01 00:00:00.000000 ogscm-2.4.7/PKG-INFO
```

### Comparing `ogscm-2.4.6/LICENSE` & `ogscm-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.6/README.md` & `ogscm-2.4.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 ```bash
 virtualenv ~/.venv/ogs-container-maker
 source ~/.venv/ogs-container-maker/bin/activate
 pip install ogscm
 ```
 
+If you build images with Docker (`--build`-parameter, see below) you need to make sure that you have [setup Docker to be runnable without `sudo`](https://docs.docker.com/engine/install/linux-postinstall/#manage-docker-as-a-non-root-user)!
+
+
 Apple ARM specific:
 
 ```bash
 export DOCKER_BUILDKIT=1
 docker buildx create --use --name=qemu
 docker buildx inspect --bootstrap
 ```
```

### Comparing `ogscm-2.4.6/ogscm/app/builder.py` & `ogscm-2.4.7/ogscm/app/builder.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.6/ogscm/app/deployer.py` & `ogscm-2.4.7/ogscm/app/deployer.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.6/ogscm/building_blocks/ccache.py` & `ogscm-2.4.7/ogscm/building_blocks/ccache.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.6/ogscm/building_blocks/lmod.py` & `ogscm-2.4.7/ogscm/building_blocks/lmod.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.6/ogscm/building_blocks/ogs.py` & `ogscm-2.4.7/ogscm/building_blocks/ogs.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.6/ogscm/building_blocks/ogs_base.py` & `ogscm-2.4.7/ogscm/building_blocks/ogs_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,19 +37,14 @@
     def __instructions(self):
         """String representation of the building block"""
         self += comment(__doc__, reformat=False)
         self += python(devel=True, python2=False)
         self += pip(pip="pip3", packages=["virtualenv", "pre-commit", "cmake-format"])
         self += packages(ospackages=self.__ospackages, epel=True)
         self += shell(commands=self.__commands)
-        self += environment(
-            variables={
-                "CMAKE_GENERATOR": "Ninja",
-            }
-        )
 
     def __setup(self):
         self.__ospackages.extend(["git"])
 
         dist = "deb"
         if hpccm.config.g_linux_distro == linux_distro.CENTOS:
             dist = "rpm"
```

### Comparing `ogscm-2.4.6/ogscm/building_blocks/osu_benchmarks.py` & `ogscm-2.4.7/ogscm/building_blocks/osu_benchmarks.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.6/ogscm/building_blocks/paraview.py` & `ogscm-2.4.7/ogscm/building_blocks/paraview.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.6/ogscm/building_blocks/pm_easybuild.py` & `ogscm-2.4.7/ogscm/building_blocks/pm_easybuild.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.6/ogscm/cli.py` & `ogscm-2.4.7/ogscm/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from ogscm.version import __version__
 from ogscm.app import builder
 from ogscm.app.deployer import deployer
 import shutil
 
 
 def main():  # pragma: no cover
-
     recipe_args_parser = argparse.ArgumentParser(add_help=False)
     parser = argparse.ArgumentParser(add_help=False)
     recipe_args_parser.add_argument("recipe", nargs="+")
     parser.add_argument("recipe", nargs="+")
 
     # General args
     parser.add_argument(
@@ -187,15 +186,15 @@
 
     images_out_dir = os.path.abspath(f"{args.out}/images")
     if not os.path.exists(images_out_dir):
         os.makedirs(images_out_dir)
 
     hpccm.config.set_cpu_target(args.cpu_target)
     Stage0 = hpccm.Stage()
-    Stage0 += raw(docker="# syntax=docker/dockerfile:experimental")
+    Stage0 += raw(docker="# syntax=docker/dockerfile:1.4")
 
     if args.runtime_only:
         Stage0.name = "build"
     Stage0 += baseimage(image=args.base_image, _as="build", _arch="x86_64")
 
     Stage0 += comment(
         f"Generated with ogs-container-maker {__version__}", reformat=False
@@ -206,15 +205,15 @@
 
     # Prepare runtime stage
     Stage1 = hpccm.Stage()
     if args.runtime_base_image == "":
         Stage1.baseimage(image=args.base_image)
     else:
         Stage1.baseimage(image=args.runtime_base_image)
-        if "jupyter/base-notebook" in args.runtime_base_image:
+        if "jupyter/base-notebook-ubuntu" in args.runtime_base_image:
             Stage1 += raw(docker="USER root")
 
     cwd = os.getcwd()
     img_file = ""
     out_dir = f"{args.out}/{args.format}"
     toolchain = None
     versions = None  # versions.json
@@ -305,15 +304,15 @@
         Stage1 += Stage0.runtime(exclude=runtime_exclude)
         if (
             hasattr(args, "compiler")
             and args.compiler == "gcc"
             and args.compiler_version != None
         ):
             Stage1 += packages(apt=["libstdc++6"])
-        if "jupyter/base-notebook" in args.runtime_base_image:
+        if "jupyter/base-notebook-ubuntu" in args.runtime_base_image:
             Stage1 += raw(docker="USER ${NB_USER}")
         stages_string += "\n\n" + str(Stage1)
 
     # ---------------------------- recipe end -----------------------------
     with open(definition_file_path, "w") as f:
         print(stages_string, file=f)
     if args.print:
```

### Comparing `ogscm-2.4.6/ogscm/config.py` & `ogscm-2.4.7/ogscm/config.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.6/ogscm/recipes/_template.py` & `ogscm-2.4.7/ogscm/recipes/_template.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.6/ogscm/recipes/compiler.py` & `ogscm-2.4.7/ogscm/recipes/compiler.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.6/ogscm/recipes/mpi-entrypoint.sh` & `ogscm-2.4.7/ogscm/recipes/mpi-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.6/ogscm/recipes/mpi.py` & `ogscm-2.4.7/ogscm/recipes/mpi.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         cuda=False,
         infiniband=False,
         ldconfig=True,
         version=local_args.ompi,
         disable_oshmem=True,
         disable_static=True,
         enable_mca_no_build="btl-uct",
-        with_slurm=False,
+        with_slurm=True,
     )
 toolchain = mpicc.toolchain
 Stage0 += mpicc
 
 # OpenMPI expects this program to exist, even if it's not used.
 # Default is "ssh : rsh", but that's not installed.
 # TODO: /usr/etc/openmpi-mca-params.conf ?
```

### Comparing `ogscm-2.4.6/ogscm/recipes/ogs.py` & `ogscm-2.4.7/ogscm/recipes/ogs.py`

 * *Files 4% similar despite different names*

```diff
@@ -449,26 +449,26 @@
                 print("--gui can not be used with --insitu!")
                 exit(1)
             Stage0 += paraview(
                 cmake_args=["-DPARAVIEW_USE_PYTHON=ON"],
                 edition="CATALYST",
                 ldconfig=True,
                 toolchain=toolchain,
-                version="v5.8.1",
+                version="v5.10.1",
             )
         else:
             vtk_version = versions["minimum_version"]["vtk"]
             Stage0 += generic_cmake(
                 cmake_opts=vtk_cmake_args,
                 devel_environment={"VTK_ROOT": "/usr/local/vtk"},
-                directory=f"VTK-{vtk_version}",
+                directory=f"vtk-v{vtk_version}",
                 ldconfig=True,
                 prefix="/usr/local/vtk",
                 toolchain=toolchain,
-                url=f"https://www.vtk.org/files/release/{vtk_version[:-2]}/VTK-{vtk_version}.tar.gz",
+                url=f"https://gitlab.kitware.com/vtk/vtk/-/archive/v{vtk_version}/vtk-v{vtk_version}.tar.gz",
             )
         if toolchain.CC == "mpicc":
             Stage0 += packages(yum=["diffutils"])
             if "--download-ptscotch" in local_args.petsc_configure_args:
                 Stage0 += packages(ospackages=["bison", "flex"])
             petsc_version = versions["minimum_version"]["petsc"]
             petsc_args = local_args.petsc_configure_args.strip().split(" ")
@@ -490,14 +490,20 @@
                 directory=f"petsc-{petsc_version}",
                 ldconfig=True,
                 preconfigure=["sed -i -- 's/python/python3/g' configure"],
                 prefix="/usr/local/petsc",
                 toolchain=toolchain,
                 url=f"http://ftp.mcs.anl.gov/pub/petsc/release-snapshots/petsc-lite-{petsc_version}.tar.gz",
             )
+        # Needs to be after PETSc: superlu_dist does not work Ninja
+        Stage0 += environment(
+            variables={
+                "CMAKE_GENERATOR": "Ninja",
+            }
+        )
 
         eigen_version = versions["minimum_version"]["eigen"]
         Stage0 += generic_cmake(
             devel_environment={
                 "Eigen3_ROOT": "/usr/local/eigen",
                 "Eigen3_DIR": "/usr/local/eigen",
             },
@@ -541,15 +547,34 @@
         prefix="/usr/local/cppcheck",
         runtime_environment={"PATH": "/usr/local/cppcheck/bin:$PATH"},
         toolchain=toolchain,
         url=f"https://github.com/danmar/cppcheck/archive/refs/tags/{cppcheck_version}.tar.gz",
     )
 
 if local_args.docs:
-    Stage0 += packages(ospackages=["doxygen", "graphviz", "texlive-base"])
+    Stage0 += packages(ospackages=["graphviz", "texlive-base"])
+    # doxygen package is out-dated, install Doxygen from binary
+    Stage0 += shell(
+        chdir="/tmp",
+        commands=[
+            "wget https://www.doxygen.nl/files/doxygen-1.9.6.linux.bin.tar.gz",
+            "tar xf doxygen-1.9.6.linux.bin.tar.gz -C /usr/local --strip-components=1",
+        ],
+    )
+    Stage0 += pip(pip="pip3", packages=["lizard", "pandas"])
+    Stage0 += generic_cmake(
+        directory=f"cpp-dependencies-master",
+        cmake_opts=["-DWITH_BOOST=OFF"],
+        ldconfig=True,
+        url=f"https://github.com/tomtom-international/cpp-dependencies/archive/refs/heads/master.zip",
+        prefix="/usr/local/cpp-dependencies",
+        runtime_environment={"PATH": "/usr/local/cpp-dependencies/bin:$PATH"},
+        devel_environment={"PATH": "/usr/local/cpp-dependencies/bin:$PATH"},
+        toolchain=toolchain,
+    )
 if local_args.gcovr:
     Stage0 += pip(pip="pip3", packages=["gcovr"])
 
 if local_args.dev:
     Stage0 += packages(
         ospackages=["neovim", "gdb", "silversearcher-ag", "ssh-client", "less"]
     )
@@ -624,9 +649,16 @@
         remove_source=not local_args.keep_source,
         mount_args=mount_args,
         run_ctest=local_args.run_ctest,
     )
 
 # Required for vtk from Python (for notebooks, VTUInterface)
 # https://github.com/Kaggle/docker-python/pull/358
-Stage0 += packages(apt=["libgl1"], yum=["mesa-libGL"])
-Stage1 += packages(apt=["libgl1"], yum=["mesa-libGL"])
+# xvfb for PyVista
+Stage0 += packages(
+    apt=["libgl1", "xvfb", "libgl1-mesa-glx", "libglu1-mesa"],
+    yum=["mesa-libGL", "xorg-x11-server-Xvfb", "mesa-libGLU"],
+)
+Stage1 += packages(
+    apt=["libgl1", "xvfb", "libgl1-mesa-glx", "libglu1-mesa"],
+    yum=["mesa-libGL", "xorg-x11-server-Xvfb", "mesa-libGLU"],
+)
```

### Comparing `ogscm-2.4.6/ogscm/recipes/ogs_jupyter.py` & `ogscm-2.4.7/ogscm/recipes/ogs_jupyter.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Parse local args
 local_args = parser.parse_known_args()[0]
 
 if not "jupyter/" in local_args.runtime_base_image:
     print(
         "The ogs_jupyter.py recipe requires a Jupyter base image for the "
-        "runtime stage! E.g. --runtime_base_image jupyter/base-notebook"
+        "runtime stage! E.g. --runtime_base_image jupyter/base-notebook-ubuntu"
     )
     exit(1)
 
 img_file += f"-jupyter"
 out_dir += f"/jupyter"
 
 # Implement recipe
@@ -48,16 +48,17 @@
 vtk_rendering_backend = "osmesa"
 if local_args.pyvista_gpu:
     vtk_rendering_backend = "egl"
 else:
     conda_packages.append("mesalib")
 conda_packages.append(f"vtk=*={vtk_rendering_backend}*")
 
-for package in versions["python"]["notebook_requirements"]:
-    pip_packages.append(package)
+if "notebook_requirements" in versions["python"]:
+    for package in versions["python"]["notebook_requirements"]:
+        pip_packages.append(package)
 
 pip_packages.sort()
 conda_packages.sort()
 
 Stage1 += shell(
     commands=[
         f"mamba install --yes --quiet -c bioconda -c conda-forge  {' '.join(conda_packages)}",
```

### Comparing `ogscm-2.4.6/ogscm/recipes/python_vtk.py` & `ogscm-2.4.7/ogscm/recipes/python_vtk.py`

 * *Files identical despite different names*

### Comparing `ogscm-2.4.6/pyproject.toml` & `ogscm-2.4.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "ogscm"
-version = "2.4.6"
+version = "2.4.7"
 description = "OGS Container Maker"
 authors = ["Lars Bilke <lars.bilke@ufz.de>"]
 license = "BSD 3-clause"
 repository = "https://gitlab.opengeosys.org/ogs/container-maker"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-hpccm = "^22.2.0"
+hpccm = "^22.10.0"
 requests = "^2.24.0"
-PyYAML = "^5.3.1"
+PyYAML = "^6.0"
 packaging = "^20.4"
 
 [tool.poetry.dev-dependencies]
 black = { version = "^20.8b1", allow-prereleases = true }
 
 [tool.poetry.scripts]
 ogscm = "ogscm.cli:main"
```

### Comparing `ogscm-2.4.6/setup.py` & `ogscm-2.4.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,270 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ogscm
+Version: 2.4.7
+Summary: OGS Container Maker
+Home-page: https://gitlab.opengeosys.org/ogs/container-maker
+License: BSD 3-clause
+Author: Lars Bilke
+Author-email: lars.bilke@ufz.de
+Requires-Python: >=3.7,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: hpccm (>=22.10.0,<23.0.0)
+Requires-Dist: packaging (>=20.4,<21.0)
+Requires-Dist: requests (>=2.24.0,<3.0.0)
+Project-URL: OpenGepSys project, https://www.opengeosys.org
+Project-URL: Repository, https://gitlab.opengeosys.org/ogs/container-maker
+Description-Content-Type: text/markdown
 
-packages = \
-['ogscm', 'ogscm.app', 'ogscm.building_blocks', 'ogscm.recipes']
+# OGS Container Maker
 
-package_data = \
-{'': ['*'], 'ogscm.recipes': ['files/*']}
+[![PyPI version](https://badge.fury.io/py/ogscm.svg)](https://badge.fury.io/py/ogscm)
 
-install_requires = \
-['PyYAML>=5.3.1,<6.0.0',
- 'hpccm>=22.2.0,<23.0.0',
- 'packaging>=20.4,<21.0',
- 'requests>=2.24.0,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['ogscm = ogscm.cli:main']}
-
-setup_kwargs = {
-    'name': 'ogscm',
-    'version': '2.4.6',
-    'description': 'OGS Container Maker',
-    'long_description': "# OGS Container Maker\n\n[![PyPI version](https://badge.fury.io/py/ogscm.svg)](https://badge.fury.io/py/ogscm)\n\n## General usage\n\n### Installation\n\n```bash\nvirtualenv ~/.venv/ogs-container-maker\nsource ~/.venv/ogs-container-maker/bin/activate\npip install ogscm\n```\n\nApple ARM specific:\n\n```bash\nexport DOCKER_BUILDKIT=1\ndocker buildx create --use --name=qemu\ndocker buildx inspect --bootstrap\n```\n\n### Generate container definition\n\nOGS Container Maker has builtin *recipes*. You need to specify the recipes to use as command arguments. Each of recipes adds options to the tool. Typically you want to start with a compiler. Add the `compiler.py` recipe and the `--help`-flag to get more options:\n\n```bash\n$ ogscm compiler.py --help\n...\ncompiler.py:\n  --compiler COMPILER   The compiler to use. Possible options: off, gcc,\n                        clang (default: gcc)\n  --compiler_version COMPILER_VERSION\n                        Compiler version. (default: )\n  --iwyy                Install include-what-you-use (requires clang\n                        compiler) (default: False)\n```\n\nAfter specifying the compiler recipe (and optionally setting a non-default compiler and version) you may want to add the `ogs.py` recipe:\n\n```bash\n$ ogscm compiler.py ogs.py --help\n...\nogs.py:\n  --pm {system,off}\n                        Package manager to install third-party dependencies\n                        (default: conan)\n  --ogs OGS             OGS repo on gitlab.opengeosys.org in the form\n                        'user/repo@branch' OR 'user/repo@@commit' to\n                        checkout a specific commit OR a path to a local\n                        subdirectory to the git cloned OGS sources OR 'off'\n                        to disable OGS building OR 'clean' to disable OGS\n                        and all its dev dependencies (default:\n                        ogs/ogs@master)\n  --cmake_args CMAKE_ARGS\n                        CMake argument set has to be quoted and **must**\n                        start with a space. e.g. --cmake_args '\n                        -DFIRST=TRUE -DFOO=BAR' (default: )\n...\n```\n\nPlease note that the order of the recipes given on the command line is important. The typical order for the current builtin recipes is `compiler.py mpi.py ogs.py ogs_jupyter.py`.\n\nTo generate a Dockerfile with the default parameters:\n\n```bash\n$ ogscm compiler.py ogs.py\nEvaluating compiler.py\nEvaluating ogs.py\nCreated definition _out/docker/gcc/default/ogs-d18c786e/conan/Dockerfile\n```\n\nWith some options (and the `mpi.py`-recipe):\n\n```bash\n$ ogscm compiler.py mpi.py ogs.py --ompi 4.0.5 --cmake_args ' -DOGS_BUILD_PROCESSES=LiquidFlow'\nEvaluating compiler.py\nEvaluating mpi.py\nEvaluating ogs.py\nCreated definition _out/docker/gcc/10/openmpi/4.0.5/ogs-d18c786e/conan/cmake-702517b3/Dockerfile\n```\n\n### Build image\n\nAdd the `--build`-flag.\n\nConvert Docker image to Singularity image:\n\nAdd the `--convert`-flag (requires Singularity 3.x).\n\n### Run\n\n```bash\ndocker run --it --rm ogs-ompi-2.1.3\n# in container:\nogs --version\n```\n\n```bash\nsingularity shell ogs-ompi-2.1.3.sif\n# in container:\nogs --version\n# OR directly run from host\nsingularity exec ogs-ompi-2.1.3.sif ogs local/path/to/square_1e0.prj\n```\n\n## All options\n\nAll options for current builtin recipes:\n\n```\n$ ogscm compiler.py mpi.py ogs.py --help\nEvaluating compiler.py\nEvaluating mpi.py\nEvaluating ogs.py\nusage: ogscm [-h] [--version] [--out OUT] [--file FILE] [--print] [--format {docker,singularity}] [--base_image BASE_IMAGE] [--runtime_base_image RUNTIME_BASE_IMAGE]\n             [--cpu-target {a64fx,aarch64,arm,broadwell,bulldozer,cannonlake,cascadelake,core2,excavator,haswell,i686,icelake,ivybridge,k10,mic_knl,nehalem,nocona,pentium2,pentium3,pentium4,piledriver,power7,power8,power8le,power9,power9le,ppc,ppc64,ppc64le,ppcle,prescott,sandybridge,skylake,skylake_avx512,sparc,sparc64,steamroller,thunderx2,westmere,x86,x86_64,zen,zen2}]\n             [--build] [--build_args BUILD_ARGS] [--upload] [--registry REGISTRY] [--tag TAG] [--convert] [--sif_file SIF_FILE] [--convert-enroot] [--enroot-bundle] [--enroot_file ENROOT_FILE] [--force]\n             [--runtime-only] [--clean] [--deploy [DEPLOY]] [--pip [package ...]] [--packages [packages ...]] [--compiler COMPILER] [--compiler_version COMPILER_VERSION] [--fortran] [--iwyy] [--ompi OMPI]\n             [--mpi_benchmarks] [--mpi_no_entrypoint] [--pm {system,off}] [--ogs OGS] [--cmake_args CMAKE_ARGS] [--cmake_preset CMAKE_PRESET] [--cmake_preset_file CMAKE_PRESET_FILE] [--ccache]\n             [--cpmcache] [--parallel PARALLEL] [--gui] [--docs] [--cvode] [--cppcheck] [--gcovr] [--mfront] [--insitu] [--dev] [--mkl] [--petsc_configure_args PETSC_CONFIGURE_ARGS]\n             [--version_file VERSION_FILE] [--boost-sourceforge] [--keep-ogs-source] [--keep-ogs-build] [--run-ctest]\n             recipe [recipe ...]\n\npositional arguments:\n  recipe\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --version             show program's version number and exit\n  --out OUT             Output directory (default: _out)\n  --file FILE           Overwrite output recipe file name (default: )\n  --print, -P           Print the definition to stdout (default: False)\n\nGeneral image config:\n  --format {docker,singularity}\n  --base_image BASE_IMAGE\n                        The base image. (default: ubuntu:20.04)\n  --runtime_base_image RUNTIME_BASE_IMAGE\n                        The runtime base image. (default: )\n  --cpu-target {a64fx,aarch64,arm,broadwell,bulldozer,cannonlake,cascadelake,core2,excavator,haswell,i686,icelake,ivybridge,k10,mic_knl,nehalem,nocona,pentium2,pentium3,pentium4,piledriver,power7,power8,power8le,power9,power9le,ppc,ppc64,ppc64le,ppcle,prescott,sandybridge,skylake,skylake_avx512,sparc,sparc64,steamroller,thunderx2,westmere,x86,x86_64,zen,zen2}\n                        The CPU microarchitecture to optimize for (archspec). (default: ivybridge)\n\nImage build options:\n  --build, -B           Build the images from the definition files (default: False)\n  --build_args BUILD_ARGS\n                        Arguments to the build command. Have to be quoted and **must** start with a space. E.g. --build_args ' --no-cache' (default: )\n  --upload, -U          Upload Docker image to registry (default: False)\n  --registry REGISTRY   The docker registry the image is tagged and uploaded to. (default: registry.opengeosys.org/ogs/ogs)\n  --tag TAG             The full docker image tag. Overwrites --registry. (default: )\n  --convert, -C         Convert Docker image to Singularity image (default: False)\n  --sif_file SIF_FILE   Overwrite output singularity image file name (default: )\n  --convert-enroot, -E  Convert Docker image to enroot image (default: False)\n  --enroot-bundle       Convert enroot image to enroot bundle (default: False)\n  --enroot_file ENROOT_FILE\n                        Overwrite output enroot image file name (default: )\n  --force               Forces overwriting of image files! (default: False)\n  --runtime-only, -R    Generate multi-stage Dockerfiles for small runtime images (default: False)\n\nMaintenance:\n  --clean               Cleans up generated files in default directories. (default: False)\n\nImage deployment:\n  --deploy [DEPLOY], -D [DEPLOY]\n                        Deploys to all configured hosts (in config/deploy_hosts.yml) with no additional arguments or to the specified host. Implies --build and --convert arguments. (default: )\n\nPackages to install:\n  --pip [package ...]   Install additional Python packages (default: [])\n  --packages [packages ...]\n                        Install additional OS packages (default: [])\n\ncompiler.py:\n  --compiler COMPILER   The compiler to use. Possible options: off, gcc, clang (default: gcc)\n  --compiler_version COMPILER_VERSION\n                        Compiler version. (default: )\n  --fortran             Install fortran compiler. (default: False)\n  --iwyy                Install include-what-you-use (requires clang compiler) (default: False)\n\nmpi.py:\n  --ompi OMPI           OpenMPI version, e.g. 2.1.1, 2.1.5, 3.0.1, 3.1.2 (default: 4.0.6)\n  --mpi_benchmarks      Installs OSU MPI benchmarks and mpi_bw, mpi_ring, mpi_hello (default: False)\n  --mpi_no_entrypoint   Disables mpi entrypoint. (Use with ogs_jupyter.py recipe) (default: False)\n\nogs.py:\n  --pm {system,off}     Package manager to install third-party dependencies (default: system)\n  --ogs OGS             OGS repo on gitlab.opengeosys.org in the form 'user/repo@branch' OR 'user/repo@@commit' to checkout a specific commit OR a path to a local subdirectory to the git cloned OGS\n                        sources OR 'off' to disable OGS building OR 'clean' to disable OGS and all its dev dependencies (default: ogs/ogs@master)\n  --cmake_args CMAKE_ARGS\n                        CMake argument set has to be quoted and **must** start with a space. e.g. --cmake_args ' -DFIRST=TRUE -DFOO=BAR' (default: )\n  --cmake_preset CMAKE_PRESET\n                        A CMake configuration preset to use. (default: release)\n  --cmake_preset_file CMAKE_PRESET_FILE\n                        A CMake (user) presets file as a local file path. (default: None)\n  --ccache              Enables ccache build caching. (Docker-only) (default: False)\n  --cpmcache            Enables CPM source caching. (Docker-only) (default: False)\n  --parallel PARALLEL, -j PARALLEL\n                        The number of cores to use for compilation. (default: 8)\n  --gui                 Builds the GUI (Data Explorer) (default: False)\n  --docs                Setup documentation requirements (Doxygen) (default: False)\n  --cvode               Install and configure with cvode (default: False)\n  --cppcheck            Install cppcheck (default: False)\n  --gcovr               Install gcovr (default: False)\n  --mfront              Install tfel and build OGS with -DOGS_USE_MFRONT=ON (default: False)\n  --insitu              Builds with insitu capabilities (default: False)\n  --dev                 Installs development tools (vim, gdb) (default: False)\n  --mkl                 Use MKL. By setting this option, you agree to the [Intel End User License Agreement](https://software.intel.com/en-us/articles/end-user-license-agreement). (default: False)\n  --petsc_configure_args PETSC_CONFIGURE_ARGS\n                        PETSc configuration arguments; has to be quoted. (default: --with-fc=0 --download-f2cblaslapack=1)\n  --version_file VERSION_FILE\n                        OGS versions.json file (default: None)\n  --boost-sourceforge   Boolean flag to specify whether Boost should be downloaded from SourceForge rather than the current Boost repository. (default: False)\n  --keep-ogs-source     Boolean flag to specify whether the OGS source directory should be preserved. (default: False)\n  --keep-ogs-build      Boolean flag to specify whether the OGS build directory should be preserved. (default: False)\n  --run-ctest           Boolean flag to specify whether to run the OGS ctest-target. (default: False)\n```\n\n## Advanced usage\n\n### Build OGS from local git repo\n\nYou can use the ogs-container-maker to build a container image from your current source code on your host machine:\n\n```\nvirtualenv .venv\nsource .venv/bin/activate\npip install ogscm\nogscm compiler.py ogs.py -B -C -R --ogs [path to ogs sources]\n```\n\n### Deploy image files\n\n- Requires `rsync`\n- Rename the file `config/deploy_hosts_example.yml` to `config/deploy_hosts.yml`\n- `host` has to be a SSH host to which you have passwordless access\n- Deploy to the host with `... -D myhost`\n\n\n## PyPi Publication\n\n- Bump version in `pyproject.py` and run `poetry install`\n- Create tag\n- Push to GitLab (`git push --tags`)\n",
-    'author': 'Lars Bilke',
-    'author_email': 'lars.bilke@ufz.de',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://gitlab.opengeosys.org/ogs/container-maker',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+## General usage
 
+### Installation
+
+```bash
+virtualenv ~/.venv/ogs-container-maker
+source ~/.venv/ogs-container-maker/bin/activate
+pip install ogscm
+```
+
+If you build images with Docker (`--build`-parameter, see below) you need to make sure that you have [setup Docker to be runnable without `sudo`](https://docs.docker.com/engine/install/linux-postinstall/#manage-docker-as-a-non-root-user)!
+
+
+Apple ARM specific:
+
+```bash
+export DOCKER_BUILDKIT=1
+docker buildx create --use --name=qemu
+docker buildx inspect --bootstrap
+```
+
+### Generate container definition
+
+OGS Container Maker has builtin *recipes*. You need to specify the recipes to use as command arguments. Each of recipes adds options to the tool. Typically you want to start with a compiler. Add the `compiler.py` recipe and the `--help`-flag to get more options:
+
+```bash
+$ ogscm compiler.py --help
+...
+compiler.py:
+  --compiler COMPILER   The compiler to use. Possible options: off, gcc,
+                        clang (default: gcc)
+  --compiler_version COMPILER_VERSION
+                        Compiler version. (default: )
+  --iwyy                Install include-what-you-use (requires clang
+                        compiler) (default: False)
+```
+
+After specifying the compiler recipe (and optionally setting a non-default compiler and version) you may want to add the `ogs.py` recipe:
+
+```bash
+$ ogscm compiler.py ogs.py --help
+...
+ogs.py:
+  --pm {system,off}
+                        Package manager to install third-party dependencies
+                        (default: conan)
+  --ogs OGS             OGS repo on gitlab.opengeosys.org in the form
+                        'user/repo@branch' OR 'user/repo@@commit' to
+                        checkout a specific commit OR a path to a local
+                        subdirectory to the git cloned OGS sources OR 'off'
+                        to disable OGS building OR 'clean' to disable OGS
+                        and all its dev dependencies (default:
+                        ogs/ogs@master)
+  --cmake_args CMAKE_ARGS
+                        CMake argument set has to be quoted and **must**
+                        start with a space. e.g. --cmake_args '
+                        -DFIRST=TRUE -DFOO=BAR' (default: )
+...
+```
+
+Please note that the order of the recipes given on the command line is important. The typical order for the current builtin recipes is `compiler.py mpi.py ogs.py ogs_jupyter.py`.
+
+To generate a Dockerfile with the default parameters:
+
+```bash
+$ ogscm compiler.py ogs.py
+Evaluating compiler.py
+Evaluating ogs.py
+Created definition _out/docker/gcc/default/ogs-d18c786e/conan/Dockerfile
+```
+
+With some options (and the `mpi.py`-recipe):
+
+```bash
+$ ogscm compiler.py mpi.py ogs.py --ompi 4.0.5 --cmake_args ' -DOGS_BUILD_PROCESSES=LiquidFlow'
+Evaluating compiler.py
+Evaluating mpi.py
+Evaluating ogs.py
+Created definition _out/docker/gcc/10/openmpi/4.0.5/ogs-d18c786e/conan/cmake-702517b3/Dockerfile
+```
+
+### Build image
+
+Add the `--build`-flag.
+
+Convert Docker image to Singularity image:
+
+Add the `--convert`-flag (requires Singularity 3.x).
+
+### Run
+
+```bash
+docker run --it --rm ogs-ompi-2.1.3
+# in container:
+ogs --version
+```
+
+```bash
+singularity shell ogs-ompi-2.1.3.sif
+# in container:
+ogs --version
+# OR directly run from host
+singularity exec ogs-ompi-2.1.3.sif ogs local/path/to/square_1e0.prj
+```
+
+## All options
+
+All options for current builtin recipes:
+
+```
+$ ogscm compiler.py mpi.py ogs.py --help
+Evaluating compiler.py
+Evaluating mpi.py
+Evaluating ogs.py
+usage: ogscm [-h] [--version] [--out OUT] [--file FILE] [--print] [--format {docker,singularity}] [--base_image BASE_IMAGE] [--runtime_base_image RUNTIME_BASE_IMAGE]
+             [--cpu-target {a64fx,aarch64,arm,broadwell,bulldozer,cannonlake,cascadelake,core2,excavator,haswell,i686,icelake,ivybridge,k10,mic_knl,nehalem,nocona,pentium2,pentium3,pentium4,piledriver,power7,power8,power8le,power9,power9le,ppc,ppc64,ppc64le,ppcle,prescott,sandybridge,skylake,skylake_avx512,sparc,sparc64,steamroller,thunderx2,westmere,x86,x86_64,zen,zen2}]
+             [--build] [--build_args BUILD_ARGS] [--upload] [--registry REGISTRY] [--tag TAG] [--convert] [--sif_file SIF_FILE] [--convert-enroot] [--enroot-bundle] [--enroot_file ENROOT_FILE] [--force]
+             [--runtime-only] [--clean] [--deploy [DEPLOY]] [--pip [package ...]] [--packages [packages ...]] [--compiler COMPILER] [--compiler_version COMPILER_VERSION] [--fortran] [--iwyy] [--ompi OMPI]
+             [--mpi_benchmarks] [--mpi_no_entrypoint] [--pm {system,off}] [--ogs OGS] [--cmake_args CMAKE_ARGS] [--cmake_preset CMAKE_PRESET] [--cmake_preset_file CMAKE_PRESET_FILE] [--ccache]
+             [--cpmcache] [--parallel PARALLEL] [--gui] [--docs] [--cvode] [--cppcheck] [--gcovr] [--mfront] [--insitu] [--dev] [--mkl] [--petsc_configure_args PETSC_CONFIGURE_ARGS]
+             [--version_file VERSION_FILE] [--boost-sourceforge] [--keep-ogs-source] [--keep-ogs-build] [--run-ctest]
+             recipe [recipe ...]
+
+positional arguments:
+  recipe
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --version             show program's version number and exit
+  --out OUT             Output directory (default: _out)
+  --file FILE           Overwrite output recipe file name (default: )
+  --print, -P           Print the definition to stdout (default: False)
+
+General image config:
+  --format {docker,singularity}
+  --base_image BASE_IMAGE
+                        The base image. (default: ubuntu:20.04)
+  --runtime_base_image RUNTIME_BASE_IMAGE
+                        The runtime base image. (default: )
+  --cpu-target {a64fx,aarch64,arm,broadwell,bulldozer,cannonlake,cascadelake,core2,excavator,haswell,i686,icelake,ivybridge,k10,mic_knl,nehalem,nocona,pentium2,pentium3,pentium4,piledriver,power7,power8,power8le,power9,power9le,ppc,ppc64,ppc64le,ppcle,prescott,sandybridge,skylake,skylake_avx512,sparc,sparc64,steamroller,thunderx2,westmere,x86,x86_64,zen,zen2}
+                        The CPU microarchitecture to optimize for (archspec). (default: ivybridge)
+
+Image build options:
+  --build, -B           Build the images from the definition files (default: False)
+  --build_args BUILD_ARGS
+                        Arguments to the build command. Have to be quoted and **must** start with a space. E.g. --build_args ' --no-cache' (default: )
+  --upload, -U          Upload Docker image to registry (default: False)
+  --registry REGISTRY   The docker registry the image is tagged and uploaded to. (default: registry.opengeosys.org/ogs/ogs)
+  --tag TAG             The full docker image tag. Overwrites --registry. (default: )
+  --convert, -C         Convert Docker image to Singularity image (default: False)
+  --sif_file SIF_FILE   Overwrite output singularity image file name (default: )
+  --convert-enroot, -E  Convert Docker image to enroot image (default: False)
+  --enroot-bundle       Convert enroot image to enroot bundle (default: False)
+  --enroot_file ENROOT_FILE
+                        Overwrite output enroot image file name (default: )
+  --force               Forces overwriting of image files! (default: False)
+  --runtime-only, -R    Generate multi-stage Dockerfiles for small runtime images (default: False)
+
+Maintenance:
+  --clean               Cleans up generated files in default directories. (default: False)
+
+Image deployment:
+  --deploy [DEPLOY], -D [DEPLOY]
+                        Deploys to all configured hosts (in config/deploy_hosts.yml) with no additional arguments or to the specified host. Implies --build and --convert arguments. (default: )
+
+Packages to install:
+  --pip [package ...]   Install additional Python packages (default: [])
+  --packages [packages ...]
+                        Install additional OS packages (default: [])
+
+compiler.py:
+  --compiler COMPILER   The compiler to use. Possible options: off, gcc, clang (default: gcc)
+  --compiler_version COMPILER_VERSION
+                        Compiler version. (default: )
+  --fortran             Install fortran compiler. (default: False)
+  --iwyy                Install include-what-you-use (requires clang compiler) (default: False)
+
+mpi.py:
+  --ompi OMPI           OpenMPI version, e.g. 2.1.1, 2.1.5, 3.0.1, 3.1.2 (default: 4.0.6)
+  --mpi_benchmarks      Installs OSU MPI benchmarks and mpi_bw, mpi_ring, mpi_hello (default: False)
+  --mpi_no_entrypoint   Disables mpi entrypoint. (Use with ogs_jupyter.py recipe) (default: False)
+
+ogs.py:
+  --pm {system,off}     Package manager to install third-party dependencies (default: system)
+  --ogs OGS             OGS repo on gitlab.opengeosys.org in the form 'user/repo@branch' OR 'user/repo@@commit' to checkout a specific commit OR a path to a local subdirectory to the git cloned OGS
+                        sources OR 'off' to disable OGS building OR 'clean' to disable OGS and all its dev dependencies (default: ogs/ogs@master)
+  --cmake_args CMAKE_ARGS
+                        CMake argument set has to be quoted and **must** start with a space. e.g. --cmake_args ' -DFIRST=TRUE -DFOO=BAR' (default: )
+  --cmake_preset CMAKE_PRESET
+                        A CMake configuration preset to use. (default: release)
+  --cmake_preset_file CMAKE_PRESET_FILE
+                        A CMake (user) presets file as a local file path. (default: None)
+  --ccache              Enables ccache build caching. (Docker-only) (default: False)
+  --cpmcache            Enables CPM source caching. (Docker-only) (default: False)
+  --parallel PARALLEL, -j PARALLEL
+                        The number of cores to use for compilation. (default: 8)
+  --gui                 Builds the GUI (Data Explorer) (default: False)
+  --docs                Setup documentation requirements (Doxygen) (default: False)
+  --cvode               Install and configure with cvode (default: False)
+  --cppcheck            Install cppcheck (default: False)
+  --gcovr               Install gcovr (default: False)
+  --mfront              Install tfel and build OGS with -DOGS_USE_MFRONT=ON (default: False)
+  --insitu              Builds with insitu capabilities (default: False)
+  --dev                 Installs development tools (vim, gdb) (default: False)
+  --mkl                 Use MKL. By setting this option, you agree to the [Intel End User License Agreement](https://software.intel.com/en-us/articles/end-user-license-agreement). (default: False)
+  --petsc_configure_args PETSC_CONFIGURE_ARGS
+                        PETSc configuration arguments; has to be quoted. (default: --with-fc=0 --download-f2cblaslapack=1)
+  --version_file VERSION_FILE
+                        OGS versions.json file (default: None)
+  --boost-sourceforge   Boolean flag to specify whether Boost should be downloaded from SourceForge rather than the current Boost repository. (default: False)
+  --keep-ogs-source     Boolean flag to specify whether the OGS source directory should be preserved. (default: False)
+  --keep-ogs-build      Boolean flag to specify whether the OGS build directory should be preserved. (default: False)
+  --run-ctest           Boolean flag to specify whether to run the OGS ctest-target. (default: False)
+```
+
+## Advanced usage
+
+### Build OGS from local git repo
+
+You can use the ogs-container-maker to build a container image from your current source code on your host machine:
+
+```
+virtualenv .venv
+source .venv/bin/activate
+pip install ogscm
+ogscm compiler.py ogs.py -B -C -R --ogs [path to ogs sources]
+```
+
+### Deploy image files
+
+- Requires `rsync`
+- Rename the file `config/deploy_hosts_example.yml` to `config/deploy_hosts.yml`
+- `host` has to be a SSH host to which you have passwordless access
+- Deploy to the host with `... -D myhost`
+
+
+## PyPi Publication
+
+- Bump version in `pyproject.py` and run `poetry install`
+- Create tag
+- Push to GitLab (`git push --tags`)
 
-setup(**setup_kwargs)
```

