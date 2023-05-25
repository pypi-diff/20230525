# Comparing `tmp/llm_client-0.0.1.tar.gz` & `tmp/llm_client-0.1.0.tar.gz`

## Comparing `llm_client-0.0.1.tar` & `llm_client-0.1.0.tar`

### file list

```diff
@@ -1,221 +1,221 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 llm_client-0.0.1/.DS_Store
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 llm_client-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 llm_client-0.0.1/llm_client/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 llm_client-0.0.1/llm_client/base_llm_client.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 llm_client-0.0.1/llm_client/consts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/llm_client/llm_api_client/__init__.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 llm_client-0.0.1/llm_client/llm_api_client/ai21_client.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 llm_client-0.0.1/llm_client/llm_api_client/aleph_alpha_client.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 llm_client-0.0.1/llm_client/llm_api_client/base_llm_api_client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 llm_client-0.0.1/llm_client/llm_api_client/huggingface_client.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 llm_client-0.0.1/llm_client/llm_api_client/llm_api_client_factory.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 llm_client-0.0.1/llm_client/llm_api_client/openai_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/llm_client/llm_client/__init__.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_client-0.0.1/llm_client/llm_client/local_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/llm_client/sync/__init__.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 llm_client-0.0.1/llm_client/sync/sync_llm_api_client_factory.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/.gitignore
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/pyvenv.cfg
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/activate
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/activate.csh
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/activate.fish
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/activate.nu
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/activate.ps1
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/activate_this.py
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/convert-caffe2-to-onnx
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/convert-onnx-to-caffe2
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/deactivate.nu
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/docutils
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/f2py
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/f2py3
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/f2py3.11
--rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/huggingface-cli
--rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/isympy
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/keyring
--rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/markdown-it
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/normalizer
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/openai
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/pip
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/pip3
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/pip3.11
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/pkginfo
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/publish.py
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/py.test
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/pygmentize
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/pyproject-build
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/python3.11 -> python
--rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/rst2html.py
--rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/rst2html4.py
--rwxr-xr-x   0        0        0     1104 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/rst2html5.py
--rwxr-xr-x   0        0        0      846 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/rst2latex.py
--rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/rst2man.py
--rwxr-xr-x   0        0        0      835 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/rst2odt.py
--rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0        0        0      654 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0        0        0      690 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/rst2s5.py
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/rst2xetex.py
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/rst2xml.py
--rwxr-xr-x   0        0        0      723 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/rstpep2html.py
--rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/torchrun
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/tqdm
--rwxr-xr-x   0        0        0      282 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/transformers-cli
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/twine
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/wheel
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/wheel-3.11
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/wheel3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/bin/wheel3.11
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/LICENSE.txt
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/README.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/3d_drawing/README.txt
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/3d_drawing/mayavi2_spring.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/3d_drawing/plot_basic.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/README.txt
--rw-r--r--   0        0        0  1346746 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/WormNet.v3.benchmark.txt
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/hartford_drug.edgelist
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_beam_search.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_betweenness_centrality.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_blockmodel.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_circuits.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_davis_club.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_dedensification.py
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_girvan_newman.py
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_iterated_dynamical_systems.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_krackhardt_centrality.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_maximum_independent_set.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_parallel_betweenness.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_rcm.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_snap.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_subgraphs.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/basic/README.txt
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/basic/plot_properties.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/basic/plot_read_write.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/basic/plot_simple_graph.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/README.txt
--rw-r--r--   0        0        0   100224 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/chess_masters_WCC.pgn.bz2
--rw-r--r--   0        0        0    20317 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/knuth_miles.txt.gz
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_center_node.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_chess_masters.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_custom_node_icons.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_degree.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_directed.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_edge_colormap.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_ego_graph.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_eigenvalues.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_four_grids.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_house_with_colors.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_knuth_miles.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_labels_and_colors.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_multipartite_graph.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_node_colormap.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_rainbow_coloring.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_random_geometric_graph.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_sampson.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_selfloops.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_simple_path.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_spectral_grid.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_tsp.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_unix_email.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_weighted_graph.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/unix_email.mbox
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/README.txt
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_dag_layout.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_degree_sequence.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_erdos_renyi.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_expected_degree_sequence.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_football.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_karate_club.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_morse_trie.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_mst.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_napoleon_russian_campaign.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_roget.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_triad_types.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_words.py
--rw-r--r--   0        0        0    15758 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/roget_dat.txt.gz
--rw-r--r--   0        0        0    33695 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/words_dat.txt.gz
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/subclass/README.txt
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/subclass/plot_antigraph.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/subclass/plot_printgraph.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 llm_client-0.0.1/new_venv/share/man/man1/isympy.1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_api_client/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_api_client/test_llm_api_client_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_api_client/ai21_client/__init__.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_api_client/ai21_client/conftest.py
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_api_client/ai21_client/test_ai21.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_api_client/huggingface_client/__init__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_api_client/huggingface_client/conftest.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_api_client/huggingface_client/test_huggingface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_api_client/openai_client/__init__.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_api_client/openai_client/conftest.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_api_client/openai_client/test_openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_client/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_client/local_client/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_client/local_client/conftest.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/llm_client/local_client/test_local_client.py
--rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/resources/ai21/text_completion.json
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/resources/ai21/tokenize.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/resources/huggingface/text_completion.json
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/resources/openai/chat_completion.json
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/resources/openai/text_completion.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/sync/__init__.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/sync/test_sync_llm_api_client_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/test_utils/__init__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.0.1/tests/test_utils/load_json_resource.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/.gitignore
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/pyvenv.cfg
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/activate
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/activate.csh
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/activate.fish
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/activate.nu
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/activate.ps1
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/activate_this.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/deactivate.nu
--rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/normalizer
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/pip
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/pip3
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/pip3.11
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/py.test
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/python3.11 -> python
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/wheel
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/wheel-3.11
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/wheel3
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_ai21/bin/wheel3.11
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/.gitignore
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/pyvenv.cfg
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/activate
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/activate.csh
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/activate.fish
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/activate.nu
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/activate.ps1
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/activate_this.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/deactivate.nu
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/f2py
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/f2py3
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/f2py3.11
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/huggingface-cli
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/normalizer
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/pip
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/pip3
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/pip3.11
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/py.test
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/python3.11 -> python
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/tqdm
--rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/transformers-cli
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/wheel
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/wheel-3.11
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/wheel3
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.0.1/venv_local/bin/wheel3.11
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 llm_client-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 llm_client-0.0.1/LICENSE
--rw-r--r--   0        0        0     7059 2020-02-02 00:00:00.000000 llm_client-0.0.1/README.md
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 llm_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8535 2020-02-02 00:00:00.000000 llm_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 llm_client-0.1.0/.DS_Store
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 llm_client-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 llm_client-0.1.0/llm_client/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 llm_client-0.1.0/llm_client/base_llm_client.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 llm_client-0.1.0/llm_client/consts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/llm_client/llm_api_client/__init__.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 llm_client-0.1.0/llm_client/llm_api_client/ai21_client.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 llm_client-0.1.0/llm_client/llm_api_client/aleph_alpha_client.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 llm_client-0.1.0/llm_client/llm_api_client/base_llm_api_client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 llm_client-0.1.0/llm_client/llm_api_client/huggingface_client.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 llm_client-0.1.0/llm_client/llm_api_client/llm_api_client_factory.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 llm_client-0.1.0/llm_client/llm_api_client/openai_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/llm_client/llm_client/__init__.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_client-0.1.0/llm_client/llm_client/local_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/llm_client/sync/__init__.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 llm_client-0.1.0/llm_client/sync/sync_llm_api_client_factory.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/.gitignore
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/pyvenv.cfg
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/activate
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/activate.csh
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/activate.fish
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/activate.nu
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/activate.ps1
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/activate_this.py
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/convert-caffe2-to-onnx
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/convert-onnx-to-caffe2
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/deactivate.nu
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/docutils
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/f2py
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/f2py3
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/f2py3.11
+-rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/huggingface-cli
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/isympy
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/keyring
+-rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/markdown-it
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/normalizer
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/openai
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/pip
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/pip3
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/pip3.11
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/pkginfo
+-rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/publish.py
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/py.test
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/pygmentize
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/pyproject-build
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/pytest
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/rst2html.py
+-rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/rst2html4.py
+-rwxr-xr-x   0        0        0     1104 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/rst2html5.py
+-rwxr-xr-x   0        0        0      846 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/rst2latex.py
+-rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/rst2man.py
+-rwxr-xr-x   0        0        0      835 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/rst2odt.py
+-rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0        0        0      654 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0        0        0      690 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/rst2s5.py
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/rst2xetex.py
+-rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/rst2xml.py
+-rwxr-xr-x   0        0        0      723 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/rstpep2html.py
+-rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/torchrun
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/tqdm
+-rwxr-xr-x   0        0        0      282 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/transformers-cli
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/twine
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/wheel
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/wheel-3.11
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/wheel3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/bin/wheel3.11
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/LICENSE.txt
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/README.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/README.txt
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/mayavi2_spring.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/plot_basic.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/README.txt
+-rw-r--r--   0        0        0  1346746 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/WormNet.v3.benchmark.txt
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/hartford_drug.edgelist
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_beam_search.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_betweenness_centrality.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_blockmodel.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_circuits.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_davis_club.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_dedensification.py
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_girvan_newman.py
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_iterated_dynamical_systems.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_krackhardt_centrality.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_maximum_independent_set.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_parallel_betweenness.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_rcm.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_snap.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_subgraphs.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/basic/README.txt
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_properties.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_read_write.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_simple_graph.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/README.txt
+-rw-r--r--   0        0        0   100224 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/chess_masters_WCC.pgn.bz2
+-rw-r--r--   0        0        0    20317 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/knuth_miles.txt.gz
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_center_node.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_chess_masters.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_custom_node_icons.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_degree.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_directed.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_edge_colormap.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_ego_graph.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_eigenvalues.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_four_grids.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_house_with_colors.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_knuth_miles.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_labels_and_colors.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_multipartite_graph.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_node_colormap.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_rainbow_coloring.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_random_geometric_graph.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_sampson.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_selfloops.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_simple_path.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_spectral_grid.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_tsp.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_unix_email.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_weighted_graph.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/unix_email.mbox
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/README.txt
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_dag_layout.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_degree_sequence.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_erdos_renyi.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_expected_degree_sequence.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_football.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_karate_club.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_morse_trie.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_mst.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_napoleon_russian_campaign.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_roget.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_triad_types.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_words.py
+-rw-r--r--   0        0        0    15758 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/roget_dat.txt.gz
+-rw-r--r--   0        0        0    33695 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/words_dat.txt.gz
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/subclass/README.txt
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_antigraph.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_printgraph.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 llm_client-0.1.0/new_venv/share/man/man1/isympy.1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_api_client/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_api_client/test_llm_api_client_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_api_client/ai21_client/__init__.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_api_client/ai21_client/conftest.py
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_api_client/ai21_client/test_ai21.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_api_client/huggingface_client/__init__.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_api_client/huggingface_client/conftest.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_api_client/huggingface_client/test_huggingface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_api_client/openai_client/__init__.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_api_client/openai_client/conftest.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_api_client/openai_client/test_openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_client/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_client/local_client/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_client/local_client/conftest.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/llm_client/local_client/test_local_client.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/resources/ai21/text_completion.json
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/resources/ai21/tokenize.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/resources/huggingface/text_completion.json
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/resources/openai/chat_completion.json
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/resources/openai/text_completion.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/sync/__init__.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/sync/test_sync_llm_api_client_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.1.0/tests/test_utils/load_json_resource.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/.gitignore
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/pyvenv.cfg
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/activate
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/activate.csh
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/activate.fish
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/activate.nu
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/activate.ps1
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/activate_this.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/deactivate.nu
+-rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/normalizer
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/pip
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/pip3
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/pip3.11
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/py.test
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/pytest
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/wheel
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/wheel-3.11
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/wheel3
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_ai21/bin/wheel3.11
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/.gitignore
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/pyvenv.cfg
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/activate
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/activate.csh
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/activate.fish
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/activate.nu
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/activate.ps1
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/activate_this.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/deactivate.nu
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/f2py
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/f2py3
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/f2py3.11
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/huggingface-cli
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/normalizer
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/pip
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/pip3
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/pip3.11
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/py.test
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/pytest
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/tqdm
+-rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/transformers-cli
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/wheel
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/wheel-3.11
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/wheel3
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.1.0/venv_local/bin/wheel3.11
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 llm_client-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 llm_client-0.1.0/LICENSE
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 llm_client-0.1.0/README.md
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 llm_client-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 llm_client-0.1.0/PKG-INFO
```

### Comparing `llm_client-0.0.1/.DS_Store` & `llm_client-0.1.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/.github/workflows/test.yml` & `llm_client-0.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/llm_client/__init__.py` & `llm_client-0.1.0/llm_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 
 from llm_client.base_llm_client import BaseLLMClient
 
 # load api clients
 try:
     from llm_client.llm_api_client.base_llm_api_client import BaseLLMAPIClient, LLMAPIClientConfig
     from llm_client.llm_api_client.llm_api_client_factory import LLMAPIClientFactory, LLMAPIClientType
```

### Comparing `llm_client-0.0.1/llm_client/llm_api_client/ai21_client.py` & `llm_client-0.1.0/llm_client/llm_api_client/ai21_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/llm_client/llm_api_client/aleph_alpha_client.py` & `llm_client-0.1.0/llm_client/llm_api_client/aleph_alpha_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from llm_client.llm_api_client.base_llm_api_client import BaseLLMAPIClient, LLMAPIClientConfig
 from llm_client.consts import PROMPT_KEY
 
 COMPLETE_PATH = "complete"
 TOKENIZE_PATH = "tokenize"
+EMBEDDING_PATH = "semantic_embed"
 BASE_URL = "https://api.aleph-alpha.com/"
 COMPLETIONS_KEY = "completions"
 TEXT_KEY = "completion"
 TOKENS_IDS_KEY = "token_ids"
 TOKENS_KEY = "tokens"
+REPRESENTATION_KEY = "representation"
+REPRESENTATION_DEFAULT_VALUE = "symmetric"
+EMBEDDING_KEY = "embedding"
 AUTH_HEADER = "Authorization"
 BEARER_TOKEN = "Bearer "
 MAX_TOKENS_KEY = "maximum_tokens"
 
 
 class AlephAlphaClient(BaseLLMAPIClient):
     def __init__(self, config: LLMAPIClientConfig):
@@ -31,14 +35,26 @@
                                             json=kwargs,
                                             headers=self._headers,
                                             raise_for_status=True)
         response_json = await response.json()
         completions = response_json[COMPLETIONS_KEY]
         return [completion[TEXT_KEY] for completion in completions]
 
+    async def embedding(self, text: str, model: str | None = None, representation: str = REPRESENTATION_DEFAULT_VALUE,
+                        **kwargs) -> list[float]:
+        self._set_model_in_kwargs(kwargs, model)
+        kwargs[REPRESENTATION_KEY] = representation
+        kwargs[PROMPT_KEY] = text
+        response = await self._session.post(self._base_url + EMBEDDING_PATH,
+                                            json=kwargs,
+                                            headers=self._headers,
+                                            raise_for_status=True)
+        response_json = await response.json()
+        return response_json[EMBEDDING_KEY]
+
     async def get_tokens_count(self, text: str, model: str | None = None, **kwargs) -> int:
         self._set_model_in_kwargs(kwargs, model)
         kwargs[TOKENS_KEY] = False
         kwargs[TOKENS_IDS_KEY] = True
         kwargs[PROMPT_KEY] = text
         response = await self._session.post(self._base_url + TOKENIZE_PATH,
                                             json=kwargs,
```

### Comparing `llm_client-0.0.1/llm_client/llm_api_client/base_llm_api_client.py` & `llm_client-0.1.0/llm_client/llm_api_client/base_llm_api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,11 +28,14 @@
         self._default_model: str = config.default_model
         self._headers: dict[str, str] = config.headers
 
     @abstractmethod
     async def text_completion(self, prompt: str, model: str | None = None, **kwargs) -> list[str]:
         raise NotImplementedError()
 
+    async def embedding(self, text: str, model: str | None = None, **kwargs) -> list[float]:
+        raise NotImplementedError()
+
     def _set_model_in_kwargs(self, kwargs, model: str | None) -> None:
         if model is not None:
             kwargs[MODEL_KEY] = model
         kwargs.setdefault(MODEL_KEY, self._default_model)
```

### Comparing `llm_client-0.0.1/llm_client/llm_api_client/huggingface_client.py` & `llm_client-0.1.0/llm_client/llm_api_client/huggingface_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/llm_client/llm_api_client/llm_api_client_factory.py` & `llm_client-0.1.0/llm_client/llm_api_client/llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/llm_client/llm_api_client/openai_client.py` & `llm_client-0.1.0/llm_client/llm_api_client/openai_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from dataclasses_json import dataclass_json, config
 from tiktoken import Encoding
 
 from llm_client.llm_api_client.base_llm_api_client import BaseLLMAPIClient, LLMAPIClientConfig
 from llm_client.consts import PROMPT_KEY
 
 
+INPUT_KEY = "input"
+
+
 class Role(Enum):
     SYSTEM = "system"
     USER = "user"
     ASSISTANT = "assistant"
 
 
 @dataclass_json
@@ -40,14 +43,20 @@
 
     async def chat_completion(self, messages: list[ChatMessage], model: str | None = None, **kwargs) -> list[str]:
         self._set_model_in_kwargs(kwargs, model)
         kwargs["messages"] = [message.to_dict() for message in messages]
         completions = await self._client.ChatCompletion.acreate(headers=self._headers, **kwargs)
         return [choice.message.content for choice in completions.choices]
 
+    async def embedding(self, text: str, model: str | None = None, **kwargs) -> list[float]:
+        self._set_model_in_kwargs(kwargs, model)
+        kwargs[INPUT_KEY] = text
+        embeddings = await openai.Embedding.acreate(**kwargs)
+        return embeddings.data[0].embedding
+
     async def get_tokens_count(self, text: str, model: str | None = None, **kwargs) -> int:
         if model is None:
             model = self._default_model
         return len(self._get_relevant_tokeniser(model).encode(text))
 
     @staticmethod
     @lru_cache(maxsize=40)
```

### Comparing `llm_client-0.0.1/llm_client/llm_client/local_client.py` & `llm_client-0.1.0/llm_client/llm_client/local_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/llm_client/sync/sync_llm_api_client_factory.py` & `llm_client-0.1.0/llm_client/sync/sync_llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/activate` & `llm_client-0.1.0/new_venv/bin/activate`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/activate.csh` & `llm_client-0.1.0/new_venv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/activate.fish` & `llm_client-0.1.0/new_venv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/activate.nu` & `llm_client-0.1.0/new_venv/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/activate.ps1` & `llm_client-0.1.0/new_venv/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/activate_this.py` & `llm_client-0.1.0/new_venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/deactivate.nu` & `llm_client-0.1.0/new_venv/bin/deactivate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/publish.py` & `llm_client-0.1.0/new_venv/bin/publish.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/rst2html.py` & `llm_client-0.1.0/new_venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/rst2html4.py` & `llm_client-0.1.0/new_venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/rst2html5.py` & `llm_client-0.1.0/new_venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/rst2latex.py` & `llm_client-0.1.0/new_venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/rst2man.py` & `llm_client-0.1.0/new_venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/rst2odt.py` & `llm_client-0.1.0/new_venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/rst2odt_prepstyles.py` & `llm_client-0.1.0/new_venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/rst2pseudoxml.py` & `llm_client-0.1.0/new_venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/rst2s5.py` & `llm_client-0.1.0/new_venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/rst2xetex.py` & `llm_client-0.1.0/new_venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/rst2xml.py` & `llm_client-0.1.0/new_venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/bin/rstpep2html.py` & `llm_client-0.1.0/new_venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/LICENSE.txt` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/3d_drawing/mayavi2_spring.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/mayavi2_spring.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/3d_drawing/plot_basic.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/plot_basic.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/WormNet.v3.benchmark.txt` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/WormNet.v3.benchmark.txt`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/hartford_drug.edgelist` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/hartford_drug.edgelist`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_beam_search.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_beam_search.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_betweenness_centrality.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_betweenness_centrality.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_blockmodel.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_blockmodel.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_circuits.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_circuits.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_davis_club.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_davis_club.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_dedensification.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_dedensification.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_girvan_newman.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_girvan_newman.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_iterated_dynamical_systems.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_iterated_dynamical_systems.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_krackhardt_centrality.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_krackhardt_centrality.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_maximum_independent_set.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_maximum_independent_set.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_parallel_betweenness.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_parallel_betweenness.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_rcm.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_rcm.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_snap.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_snap.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_subgraphs.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_subgraphs.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/basic/plot_properties.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_properties.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/basic/plot_read_write.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_read_write.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/basic/plot_simple_graph.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_simple_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/chess_masters_WCC.pgn.bz2` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/chess_masters_WCC.pgn.bz2`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/knuth_miles.txt.gz` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/knuth_miles.txt.gz`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_center_node.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_center_node.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_chess_masters.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_chess_masters.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_custom_node_icons.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_custom_node_icons.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_degree.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_degree.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_directed.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_directed.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_ego_graph.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_ego_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_eigenvalues.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_eigenvalues.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_four_grids.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_four_grids.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_house_with_colors.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_house_with_colors.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_knuth_miles.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_knuth_miles.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_labels_and_colors.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_labels_and_colors.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_multipartite_graph.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_multipartite_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_rainbow_coloring.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_rainbow_coloring.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_random_geometric_graph.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_random_geometric_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_sampson.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_sampson.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_selfloops.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_selfloops.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_spectral_grid.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_spectral_grid.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_tsp.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_tsp.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_unix_email.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_unix_email.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/plot_weighted_graph.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_weighted_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/drawing/unix_email.mbox` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/drawing/unix_email.mbox`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_dag_layout.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_dag_layout.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_degree_sequence.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_degree_sequence.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_erdos_renyi.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_erdos_renyi.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_football.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_football.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_morse_trie.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_morse_trie.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_mst.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_mst.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_napoleon_russian_campaign.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_napoleon_russian_campaign.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_roget.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_roget.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_triad_types.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_triad_types.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/plot_words.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_words.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/roget_dat.txt.gz` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/roget_dat.txt.gz`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/graph/words_dat.txt.gz` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/graph/words_dat.txt.gz`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/subclass/plot_antigraph.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_antigraph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/doc/networkx-3.1/examples/subclass/plot_printgraph.py` & `llm_client-0.1.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_printgraph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/new_venv/share/man/man1/isympy.1` & `llm_client-0.1.0/new_venv/share/man/man1/isympy.1`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/tests/llm_api_client/test_llm_api_client_factory.py` & `llm_client-0.1.0/tests/llm_api_client/test_llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/tests/llm_api_client/ai21_client/conftest.py` & `llm_client-0.1.0/tests/llm_api_client/ai21_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/tests/llm_api_client/ai21_client/test_ai21.py` & `llm_client-0.1.0/tests/llm_api_client/ai21_client/test_ai21.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/tests/llm_api_client/huggingface_client/conftest.py` & `llm_client-0.1.0/tests/llm_api_client/huggingface_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/tests/llm_api_client/huggingface_client/test_huggingface.py` & `llm_client-0.1.0/tests/llm_api_client/huggingface_client/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/tests/llm_api_client/openai_client/conftest.py` & `llm_client-0.1.0/tests/llm_api_client/openai_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/tests/llm_api_client/openai_client/test_openai.py` & `llm_client-0.1.0/tests/llm_api_client/openai_client/test_openai.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/tests/llm_client/local_client/conftest.py` & `llm_client-0.1.0/tests/llm_client/local_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/tests/llm_client/local_client/test_local_client.py` & `llm_client-0.1.0/tests/llm_client/local_client/test_local_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/tests/resources/ai21/text_completion.json` & `llm_client-0.1.0/tests/resources/ai21/text_completion.json`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/tests/sync/test_sync_llm_api_client_factory.py` & `llm_client-0.1.0/tests/sync/test_sync_llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/venv_ai21/bin/activate` & `llm_client-0.1.0/venv_ai21/bin/activate`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/venv_ai21/bin/activate.csh` & `llm_client-0.1.0/venv_ai21/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/venv_ai21/bin/activate.fish` & `llm_client-0.1.0/venv_ai21/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/venv_ai21/bin/activate.nu` & `llm_client-0.1.0/venv_ai21/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/venv_ai21/bin/activate.ps1` & `llm_client-0.1.0/venv_ai21/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/venv_ai21/bin/activate_this.py` & `llm_client-0.1.0/venv_ai21/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/venv_ai21/bin/deactivate.nu` & `llm_client-0.1.0/venv_ai21/bin/deactivate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/venv_local/bin/activate` & `llm_client-0.1.0/venv_local/bin/activate`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/venv_local/bin/activate.csh` & `llm_client-0.1.0/venv_local/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/venv_local/bin/activate.fish` & `llm_client-0.1.0/venv_local/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/venv_local/bin/activate.nu` & `llm_client-0.1.0/venv_local/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/venv_local/bin/activate.ps1` & `llm_client-0.1.0/venv_local/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/venv_local/bin/activate_this.py` & `llm_client-0.1.0/venv_local/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/venv_local/bin/deactivate.nu` & `llm_client-0.1.0/venv_local/bin/deactivate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/.gitignore` & `llm_client-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/LICENSE` & `llm_client-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/README.md` & `llm_client-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # LLM-Client-SDK
+[![Test](https://github.com/uripeled2/llm-client-sdk/actions/workflows/test.yml/badge.svg)](https://github.com/uripeled2/llm-client-sdk/actions/workflows/test.yml)
+[![License: MIT](https://img.shields.io/github/license/uripeled2/llm-client-sdk.svg)](https://opensource.org/licenses/MIT)
+
 LLM-Client-SDK is an SDK for communicating with generative AI large language models
 (We currently support - OpenAI, AI21, HuggingfaceHub, Aleph Alpha,
 Local models with transformers - and many more soon).
 
 Our vision is to provide async native and production ready SDK while creating 
 a powerful and fast integration with different LLM without letting the user lose 
 any flexibility (API params, endpoints etc.). *We also provide sync version, see
@@ -41,14 +44,17 @@
 class BaseLLMAPIClient(BaseLLMClient, ABC):
     def __init__(self, config: LLMAPIClientConfig):
         ...
 
     @abstractmethod
     async def text_completion(self, prompt: str, model: str | None = None, **kwargs) -> list[str]:
         raise NotImplementedError()
+
+    async def embedding(self, text: str, model: str | None = None, **kwargs) -> list[float]:
+        raise NotImplementedError()
 ```
 
 ## Requirements
 
 Python 3.10+
 
 ## Installation
@@ -104,14 +110,15 @@
                                                      headers={"OpenAI-Organization": OPENAI_ORG_ID}))  # The headers are optional
         text = "This is indeed a test"
 
         print("number of tokens:", await llm_client.get_tokens_count(text))  # 5
         print("generated chat:", await llm_client.chat_completion(  
             messages=[ChatMessage(role=Role.USER, content="Hello!")], model="gpt-3.5-turbo"))  # ['Hi there! How can I assist you today?']
         print("generated text:", await llm_client.text_completion(text))  # [' string\n\nYes, this is a test string. Test strings are used to']
+        print("generated embedding:", await llm_client.embedding(text))  # [0.0023064255, -0.009327292, ...]
 ```
 Using LLMAPIClientFactory - Perfect if you want to move fast and to not handle the client session yourself
 ```python
 import os
 from llm_client import LLMAPIClientFactory, LLMAPIClientType
 
 OPENAI_API_KEY = os.environ["API_KEY"]
@@ -174,15 +181,19 @@
 
 Contributions are welcome! Please check out the todos below, and feel free to open issue or a pull request.
 
 ### Todo
 *The list is unordered*
 
 - [ ] Add support for more LLMs
-- [ ] Add support for more functions via LLMs (e.g. embeddings, list models, edits, etc.)
+- [x] Add support for more functions via LLMs 
+  - [x] embeddings
+  - [ ] list models
+  - [ ] edits
+  - [ ] more
 - [ ] Add contributing guidelines
 - [ ] Create an easy way to run multiple LLMs in parallel with the same prompts
 - [ ] Convert common models parameter (e.g. temperature, max_tokens, etc.)
 
 ### Development
 To install the package in development mode, run the following command:
 ```console
@@ -193,8 +204,8 @@
 $ pytest tests
 ```
 If you want to add a new LLMClient you need to implement BaseLLMClient or BaseLLMAPIClient.
 
 If you are adding a BaseLLMAPIClient you also need to add him in LLMAPIClientFactory.
 
 You can add dependencies to your LLMClient in [pyproject.toml](pyproject.toml) also make sure you are adding a
-matrix.flavor in [test.yml](.github%2Fworkflows%2Ftest.yml). 
+matrix.flavor in [test.yml](.github%2Fworkflows%2Ftest.yml).
```

### Comparing `llm_client-0.0.1/pyproject.toml` & `llm_client-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llm_client-0.0.1/PKG-INFO` & `llm_client-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-client
-Version: 0.0.1
+Version: 0.1.0
 Summary: SDK for using LLM
 Project-URL: Homepage, https://github.com/uripeled2/llm-client-sdk
 Author-email: Uri Peled <uripeled2@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -33,14 +33,17 @@
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-aiohttp; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-mock; extra == 'test'
 Description-Content-Type: text/markdown
 
 # LLM-Client-SDK
+[![Test](https://github.com/uripeled2/llm-client-sdk/actions/workflows/test.yml/badge.svg)](https://github.com/uripeled2/llm-client-sdk/actions/workflows/test.yml)
+[![License: MIT](https://img.shields.io/github/license/uripeled2/llm-client-sdk.svg)](https://opensource.org/licenses/MIT)
+
 LLM-Client-SDK is an SDK for communicating with generative AI large language models
 (We currently support - OpenAI, AI21, HuggingfaceHub, Aleph Alpha,
 Local models with transformers - and many more soon).
 
 Our vision is to provide async native and production ready SDK while creating 
 a powerful and fast integration with different LLM without letting the user lose 
 any flexibility (API params, endpoints etc.). *We also provide sync version, see
@@ -79,14 +82,17 @@
 class BaseLLMAPIClient(BaseLLMClient, ABC):
     def __init__(self, config: LLMAPIClientConfig):
         ...
 
     @abstractmethod
     async def text_completion(self, prompt: str, model: str | None = None, **kwargs) -> list[str]:
         raise NotImplementedError()
+
+    async def embedding(self, text: str, model: str | None = None, **kwargs) -> list[float]:
+        raise NotImplementedError()
 ```
 
 ## Requirements
 
 Python 3.10+
 
 ## Installation
@@ -142,14 +148,15 @@
                                                      headers={"OpenAI-Organization": OPENAI_ORG_ID}))  # The headers are optional
         text = "This is indeed a test"
 
         print("number of tokens:", await llm_client.get_tokens_count(text))  # 5
         print("generated chat:", await llm_client.chat_completion(  
             messages=[ChatMessage(role=Role.USER, content="Hello!")], model="gpt-3.5-turbo"))  # ['Hi there! How can I assist you today?']
         print("generated text:", await llm_client.text_completion(text))  # [' string\n\nYes, this is a test string. Test strings are used to']
+        print("generated embedding:", await llm_client.embedding(text))  # [0.0023064255, -0.009327292, ...]
 ```
 Using LLMAPIClientFactory - Perfect if you want to move fast and to not handle the client session yourself
 ```python
 import os
 from llm_client import LLMAPIClientFactory, LLMAPIClientType
 
 OPENAI_API_KEY = os.environ["API_KEY"]
@@ -212,15 +219,19 @@
 
 Contributions are welcome! Please check out the todos below, and feel free to open issue or a pull request.
 
 ### Todo
 *The list is unordered*
 
 - [ ] Add support for more LLMs
-- [ ] Add support for more functions via LLMs (e.g. embeddings, list models, edits, etc.)
+- [x] Add support for more functions via LLMs 
+  - [x] embeddings
+  - [ ] list models
+  - [ ] edits
+  - [ ] more
 - [ ] Add contributing guidelines
 - [ ] Create an easy way to run multiple LLMs in parallel with the same prompts
 - [ ] Convert common models parameter (e.g. temperature, max_tokens, etc.)
 
 ### Development
 To install the package in development mode, run the following command:
 ```console
@@ -231,8 +242,8 @@
 $ pytest tests
 ```
 If you want to add a new LLMClient you need to implement BaseLLMClient or BaseLLMAPIClient.
 
 If you are adding a BaseLLMAPIClient you also need to add him in LLMAPIClientFactory.
 
 You can add dependencies to your LLMClient in [pyproject.toml](pyproject.toml) also make sure you are adding a
-matrix.flavor in [test.yml](.github%2Fworkflows%2Ftest.yml). 
+matrix.flavor in [test.yml](.github%2Fworkflows%2Ftest.yml).
```

