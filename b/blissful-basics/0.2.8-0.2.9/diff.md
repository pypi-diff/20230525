# Comparing `tmp/blissful_basics-0.2.8.tar.gz` & `tmp/blissful_basics-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blissful_basics-0.2.8.tar", last modified: Mon Sep  5 20:13:03 2022, max compression
+gzip compressed data, was "blissful_basics-0.2.9.tar", last modified: Mon Sep  5 20:19:00 2022, max compression
```

## Comparing `blissful_basics-0.2.8.tar` & `blissful_basics-0.2.9.tar`

### file list

```diff
@@ -1,376 +1,376 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.151835 blissful_basics-0.2.8/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-05-22 20:51:20.000000 blissful_basics-0.2.8/.keep
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2801 2022-09-05 20:13:03.151238 blissful_basics-0.2.8/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.649882 blissful_basics-0.2.8/blissful_basics/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.654092 blissful_basics-0.2.8/blissful_basics/__dependencies__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3451 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.660416 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/.gitignore
--rw-r--r--   0 jeffhykin   (501) staff       (20)      428 2022-08-14 16:48:27.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/.gitrepo
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1850 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/README.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.664890 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/pip
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.678185 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/project/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/project/clean
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/project/commands
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/project/local_install
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      143 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/project/publish
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/project/purge
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     3448 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/shell
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/start
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.622022 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/tools/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.681426 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/documentation/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/documentation/fornix_framework.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.694336 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/documentation/images/
--rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/documentation/images/cd_tutorial.gif
--rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/documentation/images/package_from_example.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/documentation/images/package_name.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/documentation/images/package_versions.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4187 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/documentation/setup.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.700657 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/logs/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/logs/main.py.log
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.704788 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/main/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/main/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.706689 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/main/file_system_py/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    10002 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/main/file_system_py/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/main/license.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/main/setup.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    29546 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/poetry.lock
--rw-r--r--   0 jeffhykin   (501) staff       (20)      497 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/pyproject.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.711046 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/run/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4424 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/run/tests
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4424 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/run/tests.ps1
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.713041 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.714196 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/.cache/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/.cache/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.717172 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_clean/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_clean/450_nix.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_clean/600_cache_folder.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_clean/801_python.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.720983 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_manual_start/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_manual_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_manual_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.724014 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_purge/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_purge/580_mac_library_caches.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1536 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_purge/802_remove_venv.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.754995 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/000_009__add_path_injections__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2013 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/001_000__setup_zsh__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/001_010__setup_nix_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/001_010_enable_globbing.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/004_000_add_system_bin.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/005_000__setup_ld_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/010_000__ssl_fix__.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      520 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/019_000_setup_python_venv.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5698 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/082_000_add_commands_to_path.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/090_000_run_project_commands.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/091_000_commands_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/092_000_doit_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/092_000_resume_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/093_000_customize_ll_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    12535 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/095_000_customize_tree_function.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.775103 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/010_000_setting_up_env_message.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/049_000_link_keychain.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/051_000_copy_git_config.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/089_000__sudo_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/091_000__logger_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/095_000_vim_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/096_000_vscode_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/097_000_atom_injection.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.632212 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.776412 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.626695 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.627373 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.782040 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      563 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/remove
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/storage
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.788961 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      750 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.796428 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_grep_regex
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_shell_argument
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/indent
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_doublequotes
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/unindent
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.803649 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.806490 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/commands/ignore
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2098 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/commands/mixin
--rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/during_cleaning.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.630310 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.817796 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.819717 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-merge/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-merge/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5698 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.820867 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-update/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5698 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.821723 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-applypatch/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-applypatch/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.823384 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-commit/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.825172 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.825994 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-push/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-push/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.826807 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-receive/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-receive/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.827947 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.828192 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/update/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.838670 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/cacert.pem
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.846366 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7941 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      891 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/fix_ssl
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/lib_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/long_eval
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/package_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/raw_find
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/during_start.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28076 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/installer_helper
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.847686 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/mixins/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      189 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/mixins/salt.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7469 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/nix.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.849508 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/nixpkgs/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.851144 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/packages/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/packages/salt.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13590 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/parse_dependencies.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)      217 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/settings.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)     5962 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/shell.nix
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2470 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/uninstaller_helper
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.854811 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/os_mac/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/os_mac/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/os_mac/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/os_mac/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.859395 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.862147 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/commands/add_project_to_pythonpath
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5698 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/commands/ensure_pip_modules
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/commands/refresh_ignores
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      520 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/commands/setup_venv
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1536 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/fornix_core
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.864101 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/home/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/home/.zshenv
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.866401 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/requirements/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     5962 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/requirements/advanced_system_tools.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7469 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/requirements/system_tools.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.867907 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/tests/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      525 2022-08-14 16:48:26.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/tests/main.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.877395 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/.gitignore
--rw-r--r--   0 jeffhykin   (501) staff       (20)      422 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/.gitrepo
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1304 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/README.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.883390 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/pip
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.890514 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/project/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/project/clean
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/project/commands
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/project/local_install
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      450 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/project/publish
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/project/purge
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     3448 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/shell
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/start
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/subrepo
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.634051 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/tools/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.893410 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/documentation/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/documentation/fornix_framework.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.904424 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/documentation/images/
--rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/documentation/images/cd_tutorial.gif
--rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/documentation/images/package_from_example.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/documentation/images/package_name.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/documentation/images/package_versions.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4269 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/documentation/setup.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.908366 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/main/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/main/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.909670 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/main/json_fix/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2318 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/main/json_fix/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/main/license.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1232 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/main/setup.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    27353 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/poetry.lock
--rw-r--r--   0 jeffhykin   (501) staff       (20)      516 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/pyproject.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.910851 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.911918 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/.cache/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/.cache/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.919769 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_clean/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_clean/450_nix.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_clean/600_cache_folder.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_clean/801_python.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.923698 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_manual_start/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_manual_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_manual_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.925945 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_purge/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_purge/580_mac_library_caches.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1536 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_purge/802_remove_venv.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.003046 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/000_009__add_path_injections__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/001_000__setup_zsh__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/001_010__setup_nix_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/001_010_enable_globbing.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/004_000_add_system_bin.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/005_000__setup_ld_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/010_000__ssl_fix__.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      520 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/019_000_setup_python_venv.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5764 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/021_000_ensure_pip_modules.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/081_000__ensure_all_commands_executable__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/082_000_add_commands_to_path.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/090_000_run_project_commands.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/091_000_commands_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/092_000_doit_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/092_000_resume_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/093_000_customize_ll_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13245 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/094_000_jeffs_git_shortcuts.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/095_000_customize_tree_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/099_050_finish_spaceship_setup_.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.051528 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/010_000_setting_up_env_message.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/049_000_link_keychain.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/051_000_copy_git_config.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/060_010_link_deno_store.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/060_010_link_nix_channel.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/060_010_link_tealdeer.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/089_000__sudo_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/091_000__logger_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/095_000_vim_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/096_000_vscode_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/097_000_atom_injection.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.645982 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.052536 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.637774 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.638451 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.060332 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/copy
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/relative_link
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/remove
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/storage
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.067516 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/basic_init_example
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/inject_into_path
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      750 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/trigger
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.074563 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/escape_grep_regex
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/escape_shell_argument
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/indent
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/remove_doublequotes
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/unindent
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.078535 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.080562 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/commands/ignore
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/commands/mixin
--rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/during_cleaning.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.644370 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.082118 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/fsmonitor-watchman/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/fsmonitor-watchman/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.083227 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-merge/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-merge/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5764 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-merge/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.085233 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-update/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5764 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-update/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.086694 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-applypatch/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-applypatch/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.088318 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-commit/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.089277 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-merge-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-merge-commit/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.090156 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-push/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-push/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.090873 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-receive/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-receive/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.091251 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/prepare-commit-msg/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/prepare-commit-msg/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.092051 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/update/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.102330 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/cacert.pem
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.119349 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7941 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/ensure_nix_installed
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      937 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/fix_ssl
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/lib_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/long_eval
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/package_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/raw_find
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/during_start.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28076 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/installer_helper
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.120113 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/mixins/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      189 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/mixins/salt.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7469 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/nix.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.122233 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/packages/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/packages/salt.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/parse_dependencies.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)      217 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/settings.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6165 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/shell.nix
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2470 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/uninstaller_helper
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.130547 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/os_mac/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/os_mac/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/os_mac/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/os_mac/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.139541 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/python/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/python/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.144827 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/python/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/python/commands/add_project_to_pythonpath
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5764 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/python/commands/ensure_pip_modules
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/python/commands/refresh_ignores
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      520 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/python/commands/setup_venv
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/python/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1536 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/python/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/fornix_core
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.145403 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/home/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/home/.zshenv
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:03.149037 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/requirements/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6165 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/requirements/advanced_system_tools.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7469 2022-08-14 16:08:31.000000 blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/requirements/system_tools.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)    42005 2022-09-05 20:12:40.000000 blissful_basics-0.2.8/blissful_basics/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:13:02.653578 blissful_basics-0.2.8/blissful_basics.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2801 2022-09-05 20:13:02.000000 blissful_basics-0.2.8/blissful_basics.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)    25511 2022-09-05 20:13:02.000000 blissful_basics-0.2.8/blissful_basics.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2022-09-05 20:13:02.000000 blissful_basics-0.2.8/blissful_basics.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       16 2022-09-05 20:13:02.000000 blissful_basics-0.2.8/blissful_basics.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2022-05-22 20:51:20.000000 blissful_basics-0.2.8/license.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2022-09-05 20:13:03.152010 blissful_basics-0.2.8/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3164 2022-08-14 16:46:13.000000 blissful_basics-0.2.8/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.476142 blissful_basics-0.2.9/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-05-22 20:51:20.000000 blissful_basics-0.2.9/.keep
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2801 2022-09-05 20:19:00.475217 blissful_basics-0.2.9/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.683435 blissful_basics-0.2.9/blissful_basics/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.698046 blissful_basics-0.2.9/blissful_basics/__dependencies__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3451 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.707846 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      428 2022-08-14 16:48:27.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1850 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.717643 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.728516 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      143 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     3448 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/start
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.501821 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.735307 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.761383 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4187 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.763742 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/logs/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/logs/main.py.log
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.767652 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/main/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.768638 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/main/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    10002 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/main/file_system_py/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/main/setup.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    29546 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      497 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.771981 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/run/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4424 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/run/tests
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4424 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/run/tests.ps1
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.772929 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.773961 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.784437 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.789452 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.793200 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1536 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.950687 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2013 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      520 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5698 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    12535 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/095_000_customize_tree_function.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.980034 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.600318 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.983332 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.518339 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.525192 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.003699 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      563 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.017535 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      750 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.027257 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.034325 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.037421 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2098 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.572823 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.038885 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.039615 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5698 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.041064 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5698 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.042046 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.043197 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.044648 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.045028 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.045379 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.045734 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.046080 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.057862 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.066027 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7941 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      891 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28076 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/installer_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.068054 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/mixins/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      189 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/mixins/salt.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7469 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/nix.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.069919 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/nixpkgs/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.070784 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/packages/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/packages/salt.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13590 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      217 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5962 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2470 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.073082 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.080566 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.083849 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5698 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      520 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1536 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.084574 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/home/.zshenv
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.087432 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5962 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7469 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/requirements/system_tools.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.088925 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/tests/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      525 2022-08-14 16:48:26.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/tests/main.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.099399 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      422 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1304 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.105991 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.223782 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      450 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     3448 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/start
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/subrepo
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.611022 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.227269 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.234963 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4269 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.240340 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/main/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.241998 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/main/json_fix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2318 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/main/json_fix/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1232 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/main/setup.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    27353 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      516 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.243533 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.244594 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.248809 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.281126 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.289766 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1536 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.343287 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      520 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5764 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13245 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/095_000_customize_tree_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/099_050_finish_spaceship_setup_.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.363826 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.664454 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.365446 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.632824 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.638020 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.373070 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.383116 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      750 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.397496 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.403644 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.406515 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.652849 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.407526 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.408402 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5764 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.415339 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5764 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.416259 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.418450 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.419566 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.421702 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.423994 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.425777 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.426321 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.445417 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.452807 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7941 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      937 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28076 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/installer_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.454476 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/mixins/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      189 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/mixins/salt.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7469 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/nix.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.456361 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/packages/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/packages/salt.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      217 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6165 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2470 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.461216 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.466032 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.469441 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5764 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      520 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1536 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.470342 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/home/.zshenv
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:19:00.473321 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6165 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7469 2022-08-14 16:08:31.000000 blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/requirements/system_tools.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    42017 2022-09-05 20:18:19.000000 blissful_basics-0.2.9/blissful_basics/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-09-05 20:18:59.692326 blissful_basics-0.2.9/blissful_basics.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2801 2022-09-05 20:18:58.000000 blissful_basics-0.2.9/blissful_basics.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    25511 2022-09-05 20:18:59.000000 blissful_basics-0.2.9/blissful_basics.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2022-09-05 20:18:58.000000 blissful_basics-0.2.9/blissful_basics.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       16 2022-09-05 20:18:58.000000 blissful_basics-0.2.9/blissful_basics.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2022-05-22 20:51:20.000000 blissful_basics-0.2.9/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2022-09-05 20:19:00.477440 blissful_basics-0.2.9/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3164 2022-08-14 16:46:13.000000 blissful_basics-0.2.9/setup.py
```

### Comparing `blissful_basics-0.2.8/PKG-INFO` & `blissful_basics-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blissful_basics
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tools I need in every python project
 Home-page: https://github.com/jeff-hykin/blissful_basics.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/__init__.py` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/__init__.py`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/.gitignore` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/.gitignore`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/README.md` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/README.md`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/project/commands` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/project/commands`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/project/purge` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/project/purge`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/shell` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/shell`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/commands/start` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/commands/start`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/documentation/fornix_framework.md` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/documentation/fornix_framework.md`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/documentation/images/cd_tutorial.gif` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/documentation/images/cd_tutorial.gif`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/documentation/images/package_from_example.png` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/documentation/images/package_from_example.png`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/documentation/images/package_name.png` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/documentation/images/package_name.png`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/documentation/images/package_versions.png` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/documentation/images/package_versions.png`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/documentation/setup.md` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/documentation/setup.md`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/main/file_system_py/__init__.py` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/main/file_system_py/__init__.py`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/main/license.txt` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/main/license.txt`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/main/setup.py` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/main/setup.py`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/poetry.lock` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/poetry.lock`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/run/tests` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/run/tests`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/run/tests.ps1` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/run/tests.ps1`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_purge/802_remove_venv.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_purge/802_remove_venv.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/001_000__setup_zsh__.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/001_000__setup_zsh__.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/019_000_setup_python_venv.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/019_000_setup_python_venv.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/091_000_commands_function.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/091_000_commands_function.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/093_000_customize_ll_function.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/093_000_customize_ll_function.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/#establish_extension.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/#establish_extension.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/commands/ignore` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/commands/ignore`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/commands/mixin` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/commands/mixin`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/#establish_extension.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/cacert.pem` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/cacert.pem`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/fix_ssl` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/fix_ssl`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/lib_path_for` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/lib_path_for`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/package_path_for` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/commands/package_path_for`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/installer_helper` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/installer_helper`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/nix.toml` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/nix.toml`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/packages/salt.nix` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/packages/salt.nix`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/parse_dependencies.nix` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/parse_dependencies.nix`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/shell.nix` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/shell.nix`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/uninstaller_helper` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/nix/uninstaller_helper`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/#establish_extension.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/commands/ensure_pip_modules` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/commands/ensure_pip_modules`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/commands/setup_venv` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/commands/setup_venv`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/during_purge.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/extensions/python/during_purge.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/fornix_core` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/fornix_core`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/home/.zshenv` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/home/.zshenv`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/requirements/advanced_system_tools.nix` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/requirements/advanced_system_tools.nix`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/settings/requirements/system_tools.toml` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/settings/requirements/system_tools.toml`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/file_system_py/tests/main.py` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/file_system_py/tests/main.py`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/.gitignore` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/.gitignore`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/README.md` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/README.md`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/project/commands` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/project/commands`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/project/purge` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/project/purge`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/shell` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/shell`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/commands/start` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/commands/start`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/documentation/fornix_framework.md` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/documentation/fornix_framework.md`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/documentation/images/cd_tutorial.gif` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/documentation/images/cd_tutorial.gif`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/documentation/images/package_from_example.png` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/documentation/images/package_from_example.png`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/documentation/images/package_name.png` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/documentation/images/package_name.png`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/documentation/images/package_versions.png` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/documentation/images/package_versions.png`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/documentation/setup.md` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/documentation/setup.md`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/main/json_fix/__init__.py` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/main/json_fix/__init__.py`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/main/license.txt` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/main/license.txt`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/main/setup.py` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/main/setup.py`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/poetry.lock` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/poetry.lock`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/pyproject.toml` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_purge/802_remove_venv.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_purge/802_remove_venv.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/001_000__setup_zsh__.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/001_000__setup_zsh__.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/019_000_setup_python_venv.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/019_000_setup_python_venv.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/021_000_ensure_pip_modules.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/021_000_ensure_pip_modules.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/081_000__ensure_all_commands_executable__.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/091_000_commands_function.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/091_000_commands_function.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/093_000_customize_ll_function.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/093_000_customize_ll_function.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start/094_000_jeffs_git_shortcuts.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start/094_000_jeffs_git_shortcuts.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/060_010_link_deno_store.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/060_010_link_deno_store.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/060_010_link_nix_channel.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/060_010_link_nix_channel.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/060_010_link_tealdeer.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/during_start_prep/060_010_link_tealdeer.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/#establish_extension.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/add_execute_permission` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/add_execute_permission`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/copy` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/copy`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/relative_link` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/file_system/relative_link`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/basic_init_example` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/basic_init_example`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/inject_into_path` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/inject_into_path`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/merge_all_templates` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/merge_all_templates`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/trigger` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/fornix/trigger`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/#establish_extension.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/commands/ignore` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/commands/ignore`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/commands/mixin` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/commands/mixin`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-merge/901_check_pip_modules` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-merge/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-update/901_check_pip_modules` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/post-update/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/#establish_extension.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/cacert.pem` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/cacert.pem`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/ensure_nix_installed` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/ensure_nix_installed`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/fix_ssl` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/fix_ssl`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/lib_path_for` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/lib_path_for`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/package_path_for` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/commands/package_path_for`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/installer_helper` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/installer_helper`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/nix.toml` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/nix.toml`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/packages/salt.nix` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/packages/salt.nix`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/parse_dependencies.nix` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/parse_dependencies.nix`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/shell.nix` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/shell.nix`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/uninstaller_helper` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/nix/uninstaller_helper`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/python/#establish_extension.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/python/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/python/commands/ensure_pip_modules` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/python/commands/ensure_pip_modules`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/python/commands/setup_venv` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/python/commands/setup_venv`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/extensions/python/during_purge.sh` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/extensions/python/during_purge.sh`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/fornix_core` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/fornix_core`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/home/.zshenv` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/home/.zshenv`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/requirements/advanced_system_tools.nix` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/requirements/advanced_system_tools.nix`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__dependencies__/json_fix/settings/requirements/system_tools.toml` & `blissful_basics-0.2.9/blissful_basics/__dependencies__/json_fix/settings/requirements/system_tools.toml`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/blissful_basics/__init__.py` & `blissful_basics-0.2.9/blissful_basics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -686,15 +686,15 @@
                 indent = print.indent.string*print.indent.size
                 # dump to string
                 output_str = print(*args, **{ **kwargs, "to_string":True})
                 # indent any contained newlines 
                 output_str = output_str.replace("\n", "\n"+indent)[0:-len(indent)]
                 # starting indent depending on previous ending
                 if len(prev_end) > 0 and prev_end[-1] in ('\n', '\r'):
-                    output_str += indent
+                    output_str = indent + output_str
                 # print it
                 return real_print(output_str, **{ "flush": print.flush.always, **kwargs, "end":""}) 
         
         return real_print(*args, **{ "flush": print.flush.always, **kwargs})
     print.prev_end = '\n'
 
     class WithNothing(object):
```

### Comparing `blissful_basics-0.2.8/blissful_basics.egg-info/PKG-INFO` & `blissful_basics-0.2.9/blissful_basics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blissful-basics
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tools I need in every python project
 Home-page: https://github.com/jeff-hykin/blissful_basics.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `blissful_basics-0.2.8/blissful_basics.egg-info/SOURCES.txt` & `blissful_basics-0.2.9/blissful_basics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/license.txt` & `blissful_basics-0.2.9/license.txt`

 * *Files identical despite different names*

### Comparing `blissful_basics-0.2.8/setup.py` & `blissful_basics-0.2.9/setup.py`

 * *Files identical despite different names*

