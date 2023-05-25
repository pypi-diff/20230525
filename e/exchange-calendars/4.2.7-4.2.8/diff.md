# Comparing `tmp/exchange_calendars-4.2.7.tar.gz` & `tmp/exchange_calendars-4.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchange_calendars-4.2.7.tar", last modified: Wed May 10 02:13:46 2023, max compression
+gzip compressed data, was "exchange_calendars-4.2.8.tar", last modified: Thu May 25 09:20:40 2023, max compression
```

## Comparing `exchange_calendars-4.2.7.tar` & `exchange_calendars-4.2.8.tar`

### file list

```diff
@@ -1,236 +1,239 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:46.096064 exchange_calendars-4.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    38414 2023-05-10 02:13:46.096064 exchange_calendars-4.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:45.988055 exchange_calendars-4.2.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/docs/changes_archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:45.992056 exchange_calendars-4.2.7/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    91635 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/docs/tutorials/calendar_methods.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37097 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/docs/tutorials/calendar_properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/docs/tutorials/minutes.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/docs/tutorials/sessions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   149635 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/docs/tutorials/trading_index.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:45.996056 exchange_calendars-4.2.7/etc/
--rw-r--r--   0 runner    (1001) docker     (123)   141885 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/NYSE-Historical-Closings.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/bench.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/check_holidays.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3854 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/ecal
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/factory_bounds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50169 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/lunisolar
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/make_exchange_calendar_test_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/requirements_lunisolar.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/requirements_minpandas.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/requirements_update_xkrx_holidays.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/update_xkrx_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:46.028059 exchange_calendars-4.2.7/exchange_calendars/
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 02:13:45.000000 exchange_calendars-4.2.7/exchange_calendars/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/always_open.py
--rw-r--r--   0 runner    (1001) docker     (123)    24837 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/calendar_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/calendar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/common_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/ecal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)   108025 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_aixk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_asex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_bvmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_cmes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_iepa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xams.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xasx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbkk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbud.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xcbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xcse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xdub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xfra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xhel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xhkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xice.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xidx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xjse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xkar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xkls.py
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xkrx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xlim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xlis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xlon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmad.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmil.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xnys.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xnze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xosl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xpra.py
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xses.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xsgo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13680 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xshg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xsto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xswx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtae.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xwar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xwbo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/lunisolar_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:46.032059 exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/holiday.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/korean_holiday.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/offsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/precomputed_exchange_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/tase_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/us_futures_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/us_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:46.032059 exchange_calendars-4.2.7/exchange_calendars/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/weekday_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/xbkk_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)    12755 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/xkls_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)    34830 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/xkrx_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/xtks_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:46.032059 exchange_calendars-4.2.7/exchange_calendars.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    38414 2023-05-10 02:13:45.000000 exchange_calendars-4.2.7/exchange_calendars.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-10 02:13:45.000000 exchange_calendars-4.2.7/exchange_calendars.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 02:13:45.000000 exchange_calendars-4.2.7/exchange_calendars.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 02:13:45.000000 exchange_calendars-4.2.7/exchange_calendars.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-10 02:13:45.000000 exchange_calendars-4.2.7/exchange_calendars.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 02:13:45.000000 exchange_calendars-4.2.7/exchange_calendars.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-10 02:13:46.096064 exchange_calendars-4.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:46.044060 exchange_calendars-4.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:46.096064 exchange_calendars-4.2.7/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/24-5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/24-7.csv
--rw-r--r--   0 runner    (1001) docker     (123)   110144 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/aixk.csv
--rw-r--r--   0 runner    (1001) docker     (123)   496439 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/asex.csv
--rw-r--r--   0 runner    (1001) docker     (123)   537779 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/bvmf.csv
--rw-r--r--   0 runner    (1001) docker     (123)   461924 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/cmes.csv
--rw-r--r--   0 runner    (1001) docker     (123)   461924 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/iepa.csv
--rw-r--r--   0 runner    (1001) docker     (123)   114134 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)   492279 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xams.csv
--rw-r--r--   0 runner    (1001) docker     (123)   560074 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xasx.csv
--rw-r--r--   0 runner    (1001) docker     (123)   494164 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xbkk.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486819 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xbog.csv
--rw-r--r--   0 runner    (1001) docker     (123)   418309 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xbom.csv
--rw-r--r--   0 runner    (1001) docker     (123)   492344 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xbru.csv
--rw-r--r--   0 runner    (1001) docker     (123)   530954 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xbse.csv
--rw-r--r--   0 runner    (1001) docker     (123)   499559 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xbud.csv
--rw-r--r--   0 runner    (1001) docker     (123)   498389 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xbue.csv
--rw-r--r--   0 runner    (1001) docker     (123)   547139 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xcbf.csv
--rw-r--r--   0 runner    (1001) docker     (123)   484804 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xcse.csv
--rw-r--r--   0 runner    (1001) docker     (123)   507099 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xdub.csv
--rw-r--r--   0 runner    (1001) docker     (123)   552404 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xetr.csv
--rw-r--r--   0 runner    (1001) docker     (123)   551104 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xfra.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486559 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xhel.csv
--rw-r--r--   0 runner    (1001) docker     (123)   868914 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xhkg.csv
--rw-r--r--   0 runner    (1001) docker     (123)   145764 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xice.csv
--rw-r--r--   0 runner    (1001) docker     (123)   500014 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xidx.csv
--rw-r--r--   0 runner    (1001) docker     (123)   502614 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xist.csv
--rw-r--r--   0 runner    (1001) docker     (123)   499819 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xjse.csv
--rw-r--r--   0 runner    (1001) docker     (123)   504889 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xkar.csv
--rw-r--r--   0 runner    (1001) docker     (123)   499299 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xkls.csv
--rw-r--r--   0 runner    (1001) docker     (123)   793869 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xkrx.csv
--rw-r--r--   0 runner    (1001) docker     (123)   501444 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xlim.csv
--rw-r--r--   0 runner    (1001) docker     (123)   488119 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xlis.csv
--rw-r--r--   0 runner    (1001) docker     (123)   553509 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xlon.csv
--rw-r--r--   0 runner    (1001) docker     (123)   541224 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xmad.csv
--rw-r--r--   0 runner    (1001) docker     (123)   503979 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xmex.csv
--rw-r--r--   0 runner    (1001) docker     (123)   490784 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xmil.csv
--rw-r--r--   0 runner    (1001) docker     (123)   500079 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xmos.csv
--rw-r--r--   0 runner    (1001) docker     (123)   541094 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xnys.csv
--rw-r--r--   0 runner    (1001) docker     (123)   550909 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xnze.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486299 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xosl.csv
--rw-r--r--   0 runner    (1001) docker     (123)   493059 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xpar.csv
--rw-r--r--   0 runner    (1001) docker     (123)   504694 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xphs.csv
--rw-r--r--   0 runner    (1001) docker     (123)   501184 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xpra.csv
--rw-r--r--   0 runner    (1001) docker     (123)   618964 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xses.csv
--rw-r--r--   0 runner    (1001) docker     (123)   498714 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xsgo.csv
--rw-r--r--   0 runner    (1001) docker     (123)   855469 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xshg.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486494 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xsto.csv
--rw-r--r--   0 runner    (1001) docker     (123)   485129 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xswx.csv
--rw-r--r--   0 runner    (1001) docker     (123)    79204 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xtae.csv
--rw-r--r--   0 runner    (1001) docker     (123)   548374 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xtai.csv
--rw-r--r--   0 runner    (1001) docker     (123)   617749 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xtks.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486494 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xtse.csv
--rw-r--r--   0 runner    (1001) docker     (123)   500989 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xwar.csv
--rw-r--r--   0 runner    (1001) docker     (123)   555134 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xwbo.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_aixk_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_always_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_asex_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_bvmf_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_calendar_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    69070 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_calendar_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_cmes_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)   162253 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_exchange_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_iepa_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_weekday_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xams_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xasx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xbkk_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xbog_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xbom_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xbru_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xbse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xbud_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xbue_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xcbf_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xcse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xdub_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xetr_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xfra_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xhel_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xhkg_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xice_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xidx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xist_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xjse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xkar_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xkls_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xkrx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xlim_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xlis_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xlon_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xmad_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xmex_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xmil_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xmos_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xnys_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xnze_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xosl_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xpar_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xphs_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xpra_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xses_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xsgo_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xshg_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xsto_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xswx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xtae_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xtai_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xtks_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xtse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xwar_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xwbo_calendar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:20:40.849793 exchange_calendars-4.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    38557 2023-05-25 09:20:40.849793 exchange_calendars-4.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24393 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:20:40.765793 exchange_calendars-4.2.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/docs/changes_archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:20:40.765793 exchange_calendars-4.2.8/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    91635 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/docs/tutorials/calendar_methods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37097 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/docs/tutorials/calendar_properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/docs/tutorials/minutes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/docs/tutorials/sessions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   149635 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/docs/tutorials/trading_index.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:20:40.773794 exchange_calendars-4.2.8/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)   141885 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/etc/NYSE-Historical-Closings.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/etc/bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/etc/check_holidays.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3854 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/etc/ecal
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/etc/factory_bounds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50169 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/etc/lunisolar
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/etc/make_exchange_calendar_test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/etc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/etc/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/etc/requirements_lunisolar.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/etc/requirements_minpandas.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/etc/requirements_update_xkrx_holidays.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/etc/update_xkrx_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:20:40.797793 exchange_calendars-4.2.8/exchange_calendars/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 09:20:40.000000 exchange_calendars-4.2.8/exchange_calendars/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/always_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24837 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/calendar_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/calendar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/common_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/ecal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108025 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_aixk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_asex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_bvmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_cmes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_iepa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xasx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xbkk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xbog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xbom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xbru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xbse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xbud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xbue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xcbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xcse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xdub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xfra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xhel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xhkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xjse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xkar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xkls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xkrx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xlim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xlis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xlon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xmad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xmex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xmil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xnys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xnze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xosl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xpra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xsau.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xsgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13702 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xshg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xsto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xswx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xtae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xtai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xtks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xtse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xwar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xwbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/lunisolar_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:20:40.797793 exchange_calendars-4.2.8/exchange_calendars/pandas_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/pandas_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/pandas_extensions/holiday.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/pandas_extensions/korean_holiday.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/pandas_extensions/offsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/precomputed_exchange_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/tase_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/us_futures_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/us_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:20:40.801793 exchange_calendars-4.2.8/exchange_calendars/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/weekday_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/xbkk_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12755 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/xkls_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/xkrx_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/exchange_calendars/xtks_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:20:40.797793 exchange_calendars-4.2.8/exchange_calendars.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38557 2023-05-25 09:20:40.000000 exchange_calendars-4.2.8/exchange_calendars.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-25 09:20:40.000000 exchange_calendars-4.2.8/exchange_calendars.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:20:40.000000 exchange_calendars-4.2.8/exchange_calendars.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 09:20:40.000000 exchange_calendars-4.2.8/exchange_calendars.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-25 09:20:40.000000 exchange_calendars-4.2.8/exchange_calendars.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 09:20:40.000000 exchange_calendars-4.2.8/exchange_calendars.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-25 09:20:40.849793 exchange_calendars-4.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:20:40.809793 exchange_calendars-4.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:20:40.845793 exchange_calendars-4.2.8/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/24-5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/24-7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   110144 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/aixk.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   496439 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/asex.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   537779 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/bvmf.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   461924 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/cmes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   461924 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/iepa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   114134 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   492279 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xams.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   560074 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xasx.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   494164 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xbkk.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486819 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xbog.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   418309 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xbom.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   492344 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xbru.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   530954 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xbse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   499559 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xbud.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   498389 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xbue.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   547139 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xcbf.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   484804 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xcse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   507099 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xdub.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   552404 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xetr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   551104 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xfra.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486559 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xhel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   868914 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xhkg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   145764 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xice.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   500014 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xidx.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   502614 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   499819 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xjse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   504889 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xkar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   499299 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xkls.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   821104 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xkrx.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   501444 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xlim.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   488119 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xlis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   553509 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xlon.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   541224 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xmad.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   503979 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xmex.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   490784 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xmil.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   500079 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xmos.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   541094 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xnys.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   550909 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xnze.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486299 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xosl.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   493059 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xpar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   504694 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xphs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   501184 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xpra.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    48654 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xsau.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   618964 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xses.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   498714 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xsgo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   859039 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xshg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486494 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xsto.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   485129 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xswx.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    79204 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xtae.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   548374 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xtai.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   617749 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xtks.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486494 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xtse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   500989 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xwar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   555134 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/resources/xwbo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_aixk_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_always_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_asex_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_bvmf_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_calendar_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69070 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_calendar_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_cmes_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   162253 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_exchange_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_iepa_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_weekday_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xams_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xasx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xbkk_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xbog_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xbom_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xbru_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xbse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xbud_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xbue_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xcbf_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xcse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xdub_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xetr_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xfra_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xhel_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xhkg_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xice_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xidx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xist_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xjse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xkar_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xkls_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xkrx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xlim_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xlis_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xlon_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xmad_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xmex_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xmil_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xmos_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xnys_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xnze_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xosl_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xpar_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xphs_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xpra_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xsau_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xses_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xsgo_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xshg_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xsto_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xswx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xtae_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xtai_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xtks_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xtse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xwar_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-25 09:20:27.000000 exchange_calendars-4.2.8/tests/test_xwbo_calendar.py
```

### Comparing `exchange_calendars-4.2.7/.gitignore` & `exchange_calendars-4.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/LICENSE` & `exchange_calendars-4.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/PKG-INFO` & `exchange_calendars-4.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchange_calendars
-Version: 4.2.7
+Version: 4.2.8
 Summary: Calendars for securities exchanges
 Author: Gerry Manoim
 Author-email: gerrymanoim@gmail.com
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -456,15 +456,15 @@
 `exchange_calendars` attempts to be broadly useful by considering an exchange to be open only during periods of regular trading. During any pre-trading, post-trading or auction period the exchange is treated as closed. An exchange is also treated as closed during any observed lunch break.
 
 See the [minutes tutorial](docs/tutorials/minutes.ipynb) for a detailed explanation of which minutes an exchange is considered open over. If you previously used `trading_calendars`, or `exchange_calendars` prior to release 3.4, then this is the place to look for answers to questions of how the definition of trading minutes has changed over time (and is now stable and flexible!).
 
 ## Calendars
 
 | Exchange                        | ISO Code | Country        | Version Added | Exchange Website (English)                                   |
-| ------------------------------- | -------- | -------------- | ------------- | ------------------------------------------------------------ |
+|---------------------------------|----------| -------------- |---------------| ------------------------------------------------------------ |
 | New York Stock Exchange         | XNYS     | USA            | 1.0           | https://www.nyse.com/index                                   |
 | CBOE Futures                    | XCBF     | USA            | 1.0           | https://markets.cboe.com/us/futures/overview/                |
 | Chicago Mercantile Exchange     | CMES     | USA            | 1.0           | https://www.cmegroup.com/                                    |
 | ICE US                          | IEPA     | USA            | 1.0           | https://www.theice.com/index                                 |
 | Toronto Stock Exchange          | XTSE     | Canada         | 1.0           | https://www.tsx.com/                                         |
 | BMF Bovespa                     | BVMF     | Brazil         | 1.0           | http://www.b3.com.br/en_us/                                  |
 | London Stock Exchange           | XLON     | England        | 1.0           | https://www.londonstockexchange.com/                         |
@@ -509,14 +509,15 @@
 | Taiwan Stock Exchange Corp.     | XTAI     | Taiwan         | 1.11          | https://www.twse.com.tw/en/                                  |
 | Buenos Aires Stock Exchange     | XBUE     | Argentina      | 1.11          | https://www.bcba.sba.com.ar/                                 |
 | Pakistan Stock Exchange         | XKAR     | Pakistan       | 1.11          | https://www.psx.com.pk/                                      |
 | Xetra                           | XETR     | Germany        | 2.1           | https://www.xetra.com/                                       |
 | Tel Aviv Stock Exchange         | XTAE     | Israel         | 2.1           | https://www.tase.co.il/                                      |
 | Astana International Exchange   | AIXK     | Kazakhstan     | 3.2           | https://www.aix.kz/                                          |
 | Bucharest Stock Exchange        | XBSE     | Romania        | 3.2           | https://www.bvb.ro/                                          |
+| Saudi Stock Exchange            | XSAU     | Saudi Arabia   | 4.2           | https://www.saudiexchange.sa/                                |
 
 > Note that exchange calendars are defined by their [ISO-10383](https://www.iso20022.org/10383/iso-10383-market-identifier-codes) market identifier code.
 
 ## Deprecations and Renaming
 
 ### Methods deprecated in 4.0
 | Deprecated method | Reason |
```

### Comparing `exchange_calendars-4.2.7/README.md` & `exchange_calendars-4.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
 `exchange_calendars` attempts to be broadly useful by considering an exchange to be open only during periods of regular trading. During any pre-trading, post-trading or auction period the exchange is treated as closed. An exchange is also treated as closed during any observed lunch break.
 
 See the [minutes tutorial](docs/tutorials/minutes.ipynb) for a detailed explanation of which minutes an exchange is considered open over. If you previously used `trading_calendars`, or `exchange_calendars` prior to release 3.4, then this is the place to look for answers to questions of how the definition of trading minutes has changed over time (and is now stable and flexible!).
 
 ## Calendars
 
 | Exchange                        | ISO Code | Country        | Version Added | Exchange Website (English)                                   |
-| ------------------------------- | -------- | -------------- | ------------- | ------------------------------------------------------------ |
+|---------------------------------|----------| -------------- |---------------| ------------------------------------------------------------ |
 | New York Stock Exchange         | XNYS     | USA            | 1.0           | https://www.nyse.com/index                                   |
 | CBOE Futures                    | XCBF     | USA            | 1.0           | https://markets.cboe.com/us/futures/overview/                |
 | Chicago Mercantile Exchange     | CMES     | USA            | 1.0           | https://www.cmegroup.com/                                    |
 | ICE US                          | IEPA     | USA            | 1.0           | https://www.theice.com/index                                 |
 | Toronto Stock Exchange          | XTSE     | Canada         | 1.0           | https://www.tsx.com/                                         |
 | BMF Bovespa                     | BVMF     | Brazil         | 1.0           | http://www.b3.com.br/en_us/                                  |
 | London Stock Exchange           | XLON     | England        | 1.0           | https://www.londonstockexchange.com/                         |
@@ -279,14 +279,15 @@
 | Taiwan Stock Exchange Corp.     | XTAI     | Taiwan         | 1.11          | https://www.twse.com.tw/en/                                  |
 | Buenos Aires Stock Exchange     | XBUE     | Argentina      | 1.11          | https://www.bcba.sba.com.ar/                                 |
 | Pakistan Stock Exchange         | XKAR     | Pakistan       | 1.11          | https://www.psx.com.pk/                                      |
 | Xetra                           | XETR     | Germany        | 2.1           | https://www.xetra.com/                                       |
 | Tel Aviv Stock Exchange         | XTAE     | Israel         | 2.1           | https://www.tase.co.il/                                      |
 | Astana International Exchange   | AIXK     | Kazakhstan     | 3.2           | https://www.aix.kz/                                          |
 | Bucharest Stock Exchange        | XBSE     | Romania        | 3.2           | https://www.bvb.ro/                                          |
+| Saudi Stock Exchange            | XSAU     | Saudi Arabia   | 4.2           | https://www.saudiexchange.sa/                                |
 
 > Note that exchange calendars are defined by their [ISO-10383](https://www.iso20022.org/10383/iso-10383-market-identifier-codes) market identifier code.
 
 ## Deprecations and Renaming
 
 ### Methods deprecated in 4.0
 | Deprecated method | Reason |
```

#### html2text {}

```diff
@@ -153,16 +153,16 @@
 treated as closed. An exchange is also treated as closed during any observed
 lunch break. See the [minutes tutorial](docs/tutorials/minutes.ipynb) for a
 detailed explanation of which minutes an exchange is considered open over. If
 you previously used `trading_calendars`, or `exchange_calendars` prior to
 release 3.4, then this is the place to look for answers to questions of how the
 definition of trading minutes has changed over time (and is now stable and
 flexible!). ## Calendars | Exchange | ISO Code | Country | Version Added |
-Exchange Website (English) | | ------------------------------- | -------- | ---
------------ | ------------- | -------------------------------------------------
+Exchange Website (English) | |---------------------------------|----------| ---
+----------- |---------------| -------------------------------------------------
 ----------- | | New York Stock Exchange | XNYS | USA | 1.0 | https://
 www.nyse.com/index | | CBOE Futures | XCBF | USA | 1.0 | https://
 markets.cboe.com/us/futures/overview/ | | Chicago Mercantile Exchange | CMES |
 USA | 1.0 | https://www.cmegroup.com/ | | ICE US | IEPA | USA | 1.0 | https://
 www.theice.com/index | | Toronto Stock Exchange | XTSE | Canada | 1.0 | https:/
 /www.tsx.com/ | | BMF Bovespa | BVMF | Brazil | 1.0 | http://www.b3.com.br/
 en_us/ | | London Stock Exchange | XLON | England | 1.0 | https://
@@ -210,28 +210,29 @@
 Indonesia | 1.11 | https://www.idx.co.id/ | | Taiwan Stock Exchange Corp. |
 XTAI | Taiwan | 1.11 | https://www.twse.com.tw/en/ | | Buenos Aires Stock
 Exchange | XBUE | Argentina | 1.11 | https://www.bcba.sba.com.ar/ | | Pakistan
 Stock Exchange | XKAR | Pakistan | 1.11 | https://www.psx.com.pk/ | | Xetra |
 XETR | Germany | 2.1 | https://www.xetra.com/ | | Tel Aviv Stock Exchange |
 XTAE | Israel | 2.1 | https://www.tase.co.il/ | | Astana International Exchange
 | AIXK | Kazakhstan | 3.2 | https://www.aix.kz/ | | Bucharest Stock Exchange |
-XBSE | Romania | 3.2 | https://www.bvb.ro/ | > Note that exchange calendars are
-defined by their [ISO-10383](https://www.iso20022.org/10383/iso-10383-market-
-identifier-codes) market identifier code. ## Deprecations and Renaming ###
-Methods deprecated in 4.0 | Deprecated method | Reason | | ----------------- |
------- | | sessions_closes | use `.closes[start:end]` | | sessions_opens | use
-`.opens[start:end]` | ### Methods with a parameter renamed in 4.0 | Method | --
----- | is_session | | is_open_on_minute | | minutes_in_range | | minutes_window
-| | next_close | | next_minute | | next_open | | previous_close | |
-previous_minute | | previous_open | | session_break_end | | session_break_start
-| | session_close | | session_open | | sessions_in_range | | sessions_window |
-### Methods renamed in version 3.4 and removed in 4.0 | Previous name | New
-name | | ------------- | -------- | | all_minutes | minutes | |
-all_minutes_nanos | minutes_nanos | | all_sessions | sessions | |
-break_start_and_end_for_session | session_break_start_end | |
+XBSE | Romania | 3.2 | https://www.bvb.ro/ | | Saudi Stock Exchange | XSAU |
+Saudi Arabia | 4.2 | https://www.saudiexchange.sa/ | > Note that exchange
+calendars are defined by their [ISO-10383](https://www.iso20022.org/10383/iso-
+10383-market-identifier-codes) market identifier code. ## Deprecations and
+Renaming ### Methods deprecated in 4.0 | Deprecated method | Reason | | -------
+---------- | ------ | | sessions_closes | use `.closes[start:end]` | |
+sessions_opens | use `.opens[start:end]` | ### Methods with a parameter renamed
+in 4.0 | Method | ------ | is_session | | is_open_on_minute | |
+minutes_in_range | | minutes_window | | next_close | | next_minute | |
+next_open | | previous_close | | previous_minute | | previous_open | |
+session_break_end | | session_break_start | | session_close | | session_open |
+| sessions_in_range | | sessions_window | ### Methods renamed in version 3.4
+and removed in 4.0 | Previous name | New name | | ------------- | -------- | |
+all_minutes | minutes | | all_minutes_nanos | minutes_nanos | | all_sessions |
+sessions | | break_start_and_end_for_session | session_break_start_end | |
 date_to_session_label | date_to_session | | first_trading_minute | first_minute
 | | first_trading_session | first_session | | has_breaks | sessions_has_break |
 | last_trading_minute | last_minute | | last_trading_session | last_session | |
 next_session_label | next_session | | open_and_close_for_session |
 session_open_close | | previous_session_label | previous_session | |
 market_break_ends_nanos | break_ends_nanos | | market_break_starts_nanos |
 break_starts_nanos | | market_closes_nanos | closes_nanos | |
```

### Comparing `exchange_calendars-4.2.7/docs/changes_archive.md` & `exchange_calendars-4.2.8/docs/changes_archive.md`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/docs/tutorials/calendar_methods.ipynb` & `exchange_calendars-4.2.8/docs/tutorials/calendar_methods.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/docs/tutorials/calendar_properties.ipynb` & `exchange_calendars-4.2.8/docs/tutorials/calendar_properties.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/docs/tutorials/minutes.ipynb` & `exchange_calendars-4.2.8/docs/tutorials/minutes.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/docs/tutorials/sessions.ipynb` & `exchange_calendars-4.2.8/docs/tutorials/sessions.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/docs/tutorials/trading_index.ipynb` & `exchange_calendars-4.2.8/docs/tutorials/trading_index.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/etc/NYSE-Historical-Closings.pdf` & `exchange_calendars-4.2.8/etc/NYSE-Historical-Closings.pdf`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/etc/bench.py` & `exchange_calendars-4.2.8/etc/bench.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/etc/check_holidays.py` & `exchange_calendars-4.2.8/etc/check_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/etc/ecal` & `exchange_calendars-4.2.8/etc/ecal`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/etc/factory_bounds.py` & `exchange_calendars-4.2.8/etc/factory_bounds.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/etc/lunisolar` & `exchange_calendars-4.2.8/etc/lunisolar`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/etc/make_exchange_calendar_test_csv.py` & `exchange_calendars-4.2.8/etc/make_exchange_calendar_test_csv.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/etc/requirements.txt` & `exchange_calendars-4.2.8/etc/requirements.txt`

 * *Files 27% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --output-file=etc/requirements.txt pyproject.toml
 #
 korean-lunar-calendar==0.3.1
     # via exchange-calendars (pyproject.toml)
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
-pandas==2.0.0
+pandas==2.0.1
     # via exchange-calendars (pyproject.toml)
 pyluach==2.2.0
     # via exchange-calendars (pyproject.toml)
 python-dateutil==2.8.2
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
```

### Comparing `exchange_calendars-4.2.7/etc/requirements_dev.txt` & `exchange_calendars-4.2.8/etc/requirements_dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --extra=dev --output-file=etc/requirements_dev.txt pyproject.toml
 #
-attrs==22.2.0
-    # via
-    #   hypothesis
-    #   pytest
+attrs==23.1.0
+    # via hypothesis
 build==0.10.0
     # via pip-tools
 click==8.1.3
     # via pip-tools
 colorama==0.4.6
     # via
     #   build
@@ -21,31 +19,31 @@
     # via
     #   hypothesis
     #   pytest
 execnet==1.9.0
     # via pytest-xdist
 flake8==6.0.0
     # via exchange-calendars (pyproject.toml)
-hypothesis==6.71.0
+hypothesis==6.75.3
     # via exchange-calendars (pyproject.toml)
 iniconfig==2.0.0
     # via pytest
 korean-lunar-calendar==0.3.1
     # via exchange-calendars (pyproject.toml)
 mccabe==0.7.0
     # via flake8
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
-packaging==23.0
+packaging==23.1
     # via
     #   build
     #   pytest
-pandas==2.0.0
+pandas==2.0.1
     # via exchange-calendars (pyproject.toml)
 pip-tools==6.13.0
     # via exchange-calendars (pyproject.toml)
 pluggy==1.0.0
     # via pytest
 py-cpuinfo==9.0.0
     # via pytest-benchmark
@@ -53,22 +51,22 @@
     # via flake8
 pyflakes==3.0.1
     # via flake8
 pyluach==2.2.0
     # via exchange-calendars (pyproject.toml)
 pyproject-hooks==1.0.0
     # via build
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   exchange-calendars (pyproject.toml)
     #   pytest-benchmark
     #   pytest-xdist
 pytest-benchmark==4.0.0
     # via exchange-calendars (pyproject.toml)
-pytest-xdist==3.2.1
+pytest-xdist==3.3.1
     # via exchange-calendars (pyproject.toml)
 python-dateutil==2.8.2
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
 pytz==2023.3
     # via
```

### Comparing `exchange_calendars-4.2.7/etc/requirements_minpandas.txt` & `exchange_calendars-4.2.8/etc/requirements_minpandas.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 #
 #    pip-compile --extra=dev --output-file=etc/requirements_minpandas.txt pyproject.toml
 #
 # To upgrade with pandas==1.1.0 fixed run:
 #
 #    pip-compile --upgrade --upgrade-package pandas==1.1 --extra=dev --output-file=etc/requirements_minpandas.txt pyproject.toml
 #
-attrs==22.2.0
-    # via
-    #   hypothesis
-    #   pytest
+attrs==23.1.0
+    # via hypothesis
 build==0.10.0
     # via pip-tools
 click==8.1.3
     # via pip-tools
 colorama==0.4.6
     # via
     #   build
@@ -25,27 +23,27 @@
     # via
     #   hypothesis
     #   pytest
 execnet==1.9.0
     # via pytest-xdist
 flake8==6.0.0
     # via exchange-calendars (pyproject.toml)
-hypothesis==6.71.0
+hypothesis==6.75.3
     # via exchange-calendars (pyproject.toml)
 iniconfig==2.0.0
     # via pytest
 korean-lunar-calendar==0.3.1
     # via exchange-calendars (pyproject.toml)
 mccabe==0.7.0
     # via flake8
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
-packaging==23.0
+packaging==23.1
     # via
     #   build
     #   pytest
 pandas==1.1.0
     # via exchange-calendars (pyproject.toml)
 pip-tools==6.13.0
     # via exchange-calendars (pyproject.toml)
@@ -57,22 +55,22 @@
     # via flake8
 pyflakes==3.0.1
     # via flake8
 pyluach==2.2.0
     # via exchange-calendars (pyproject.toml)
 pyproject-hooks==1.0.0
     # via build
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   exchange-calendars (pyproject.toml)
     #   pytest-benchmark
     #   pytest-xdist
 pytest-benchmark==4.0.0
     # via exchange-calendars (pyproject.toml)
-pytest-xdist==3.2.1
+pytest-xdist==3.3.1
     # via exchange-calendars (pyproject.toml)
 python-dateutil==2.8.2
     # via
     #   exchange-calendars (pyproject.toml)
     #   pandas
 pytz==2023.3
     # via
```

### Comparing `exchange_calendars-4.2.7/etc/update_xkrx_holidays.py` & `exchange_calendars-4.2.8/etc/update_xkrx_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/__init__.py` & `exchange_calendars-4.2.8/exchange_calendars/__init__.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/calendar_helpers.py` & `exchange_calendars-4.2.8/exchange_calendars/calendar_helpers.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/calendar_utils.py` & `exchange_calendars-4.2.8/exchange_calendars/calendar_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 from .exchange_calendar_xmos import XMOSExchangeCalendar
 from .exchange_calendar_xnys import XNYSExchangeCalendar
 from .exchange_calendar_xnze import XNZEExchangeCalendar
 from .exchange_calendar_xosl import XOSLExchangeCalendar
 from .exchange_calendar_xpar import XPARExchangeCalendar
 from .exchange_calendar_xphs import XPHSExchangeCalendar
 from .exchange_calendar_xpra import XPRAExchangeCalendar
+from .exchange_calendar_xsau import XSAUExchangeCalendar
 from .exchange_calendar_xses import XSESExchangeCalendar
 from .exchange_calendar_xsgo import XSGOExchangeCalendar
 from .exchange_calendar_xshg import XSHGExchangeCalendar
 from .exchange_calendar_xsto import XSTOExchangeCalendar
 from .exchange_calendar_xswx import XSWXExchangeCalendar
 from .exchange_calendar_xtae import XTAEExchangeCalendar
 from .exchange_calendar_xtai import XTAIExchangeCalendar
@@ -100,14 +101,15 @@
     "XMOS": XMOSExchangeCalendar,
     "XNYS": XNYSExchangeCalendar,
     "XNZE": XNZEExchangeCalendar,
     "XOSL": XOSLExchangeCalendar,
     "XPAR": XPARExchangeCalendar,
     "XPHS": XPHSExchangeCalendar,
     "XPRA": XPRAExchangeCalendar,
+    "XSAU": XSAUExchangeCalendar,
     "XSES": XSESExchangeCalendar,
     "XSGO": XSGOExchangeCalendar,
     "XSHG": XSHGExchangeCalendar,
     "XSTO": XSTOExchangeCalendar,
     "XSWX": XSWXExchangeCalendar,
     "XTAE": XTAEExchangeCalendar,
     "XTAI": XTAIExchangeCalendar,
```

### Comparing `exchange_calendars-4.2.7/exchange_calendars/common_holidays.py` & `exchange_calendars-4.2.8/exchange_calendars/common_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/ecal.py` & `exchange_calendars-4.2.8/exchange_calendars/ecal.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/errors.py` & `exchange_calendars-4.2.8/exchange_calendars/errors.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_aixk.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_aixk.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_asex.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_asex.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_bvmf.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_bvmf.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_cmes.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_cmes.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_iepa.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_iepa.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xams.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xams.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xasx.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xasx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbkk.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xbkk.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbog.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xbog.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbom.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xbom.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbru.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xbru.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbse.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xbse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbud.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xbud.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbue.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xbue.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xcbf.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xcbf.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xcse.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xcse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xdub.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xdub.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xetr.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xetr.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xfra.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xfra.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xhel.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xhel.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xhkg.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xhkg.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xice.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xice.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xidx.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xidx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xist.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xist.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xjse.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xjse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xkar.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xkar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xkls.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xkls.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xkrx.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xkrx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xlim.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xlim.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xlis.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xlis.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xlon.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xlon.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmad.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xmad.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmex.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xmex.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmil.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xmil.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmos.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xmos.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xnys.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xnys.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xnze.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xnze.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xosl.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xosl.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xpar.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xpar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xphs.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xphs.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xpra.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xpra.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xses.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xses.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xsgo.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xsgo.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xshg.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xshg.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,14 +544,15 @@
         "2023-01-26",
         "2023-01-27",
         "2023-04-05",
         "2023-05-01",
         "2023-05-02",
         "2023-05-03",
         "2023-06-22",
+        "2023-06-23",
         "2023-09-29",
         "2023-10-02",
         "2023-10-03",
         "2023-10-04",
         "2023-10-05",
         "2024-01-01",
         "2024-02-12",
```

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xsto.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xsto.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xswx.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xswx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtae.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xtae.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtai.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xtai.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtks.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xtks.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtse.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xtse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xwar.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xwar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xwbo.py` & `exchange_calendars-4.2.8/exchange_calendars/exchange_calendar_xwbo.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/lunisolar_holidays.py` & `exchange_calendars-4.2.8/exchange_calendars/lunisolar_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/holiday.py` & `exchange_calendars-4.2.8/exchange_calendars/pandas_extensions/holiday.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/korean_holiday.py` & `exchange_calendars-4.2.8/exchange_calendars/pandas_extensions/korean_holiday.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/offsets.py` & `exchange_calendars-4.2.8/exchange_calendars/pandas_extensions/offsets.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/precomputed_exchange_calendar.py` & `exchange_calendars-4.2.8/exchange_calendars/precomputed_exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/tase_holidays.py` & `exchange_calendars-4.2.8/exchange_calendars/tase_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/us_futures_calendar.py` & `exchange_calendars-4.2.8/exchange_calendars/us_futures_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/us_holidays.py` & `exchange_calendars-4.2.8/exchange_calendars/us_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/utils/pandas_utils.py` & `exchange_calendars-4.2.8/exchange_calendars/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/xbkk_holidays.py` & `exchange_calendars-4.2.8/exchange_calendars/xbkk_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/xkls_holidays.py` & `exchange_calendars-4.2.8/exchange_calendars/xkls_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars/xkrx_holidays.py` & `exchange_calendars-4.2.8/exchange_calendars/xkrx_holidays.py`

 * *Files 1% similar despite different names*

```diff
@@ -1100,19 +1100,27 @@
         "2022-09-12",
         "2022-10-03",
         "2022-10-10",
         "2022-12-30",
     ]
 )
 
+# This index contains holidays that were manually copied from the exchange website
+#  (https://global.krx.co.kr/contents/GLB/05/0501/0501110000/GLB0501110000.jsp)
+manually_added_holidays = pd.DatetimeIndex(
+    [
+        "2023-05-29"  # Buddha's birthday holiday in lieu
+    ]
+)
+
 
 # Merging two holidays to get full precomputed holidays list.
 precomputed_krx_holidays = original_precomputed_krx_holidays.union(
     dumped_precomputed_krx_holidays
-)
+).union(manually_added_holidays)
 
 
 # Korean regular holidays
 NewYearsDay = KoreanSolarHoliday(
     "New Years Day", month=1, day=1
 )  # New years day previously had 2 additional following holidays
 NewYearsDayAfter = KoreanSolarHoliday(
```

### Comparing `exchange_calendars-4.2.7/exchange_calendars/xtks_holidays.py` & `exchange_calendars-4.2.8/exchange_calendars/xtks_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/exchange_calendars.egg-info/PKG-INFO` & `exchange_calendars-4.2.8/exchange_calendars.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchange-calendars
-Version: 4.2.7
+Version: 4.2.8
 Summary: Calendars for securities exchanges
 Author: Gerry Manoim
 Author-email: gerrymanoim@gmail.com
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -456,15 +456,15 @@
 `exchange_calendars` attempts to be broadly useful by considering an exchange to be open only during periods of regular trading. During any pre-trading, post-trading or auction period the exchange is treated as closed. An exchange is also treated as closed during any observed lunch break.
 
 See the [minutes tutorial](docs/tutorials/minutes.ipynb) for a detailed explanation of which minutes an exchange is considered open over. If you previously used `trading_calendars`, or `exchange_calendars` prior to release 3.4, then this is the place to look for answers to questions of how the definition of trading minutes has changed over time (and is now stable and flexible!).
 
 ## Calendars
 
 | Exchange                        | ISO Code | Country        | Version Added | Exchange Website (English)                                   |
-| ------------------------------- | -------- | -------------- | ------------- | ------------------------------------------------------------ |
+|---------------------------------|----------| -------------- |---------------| ------------------------------------------------------------ |
 | New York Stock Exchange         | XNYS     | USA            | 1.0           | https://www.nyse.com/index                                   |
 | CBOE Futures                    | XCBF     | USA            | 1.0           | https://markets.cboe.com/us/futures/overview/                |
 | Chicago Mercantile Exchange     | CMES     | USA            | 1.0           | https://www.cmegroup.com/                                    |
 | ICE US                          | IEPA     | USA            | 1.0           | https://www.theice.com/index                                 |
 | Toronto Stock Exchange          | XTSE     | Canada         | 1.0           | https://www.tsx.com/                                         |
 | BMF Bovespa                     | BVMF     | Brazil         | 1.0           | http://www.b3.com.br/en_us/                                  |
 | London Stock Exchange           | XLON     | England        | 1.0           | https://www.londonstockexchange.com/                         |
@@ -509,14 +509,15 @@
 | Taiwan Stock Exchange Corp.     | XTAI     | Taiwan         | 1.11          | https://www.twse.com.tw/en/                                  |
 | Buenos Aires Stock Exchange     | XBUE     | Argentina      | 1.11          | https://www.bcba.sba.com.ar/                                 |
 | Pakistan Stock Exchange         | XKAR     | Pakistan       | 1.11          | https://www.psx.com.pk/                                      |
 | Xetra                           | XETR     | Germany        | 2.1           | https://www.xetra.com/                                       |
 | Tel Aviv Stock Exchange         | XTAE     | Israel         | 2.1           | https://www.tase.co.il/                                      |
 | Astana International Exchange   | AIXK     | Kazakhstan     | 3.2           | https://www.aix.kz/                                          |
 | Bucharest Stock Exchange        | XBSE     | Romania        | 3.2           | https://www.bvb.ro/                                          |
+| Saudi Stock Exchange            | XSAU     | Saudi Arabia   | 4.2           | https://www.saudiexchange.sa/                                |
 
 > Note that exchange calendars are defined by their [ISO-10383](https://www.iso20022.org/10383/iso-10383-market-identifier-codes) market identifier code.
 
 ## Deprecations and Renaming
 
 ### Methods deprecated in 4.0
 | Deprecated method | Reason |
```

### Comparing `exchange_calendars-4.2.7/exchange_calendars.egg-info/SOURCES.txt` & `exchange_calendars-4.2.8/exchange_calendars.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 exchange_calendars/exchange_calendar_xmos.py
 exchange_calendars/exchange_calendar_xnys.py
 exchange_calendars/exchange_calendar_xnze.py
 exchange_calendars/exchange_calendar_xosl.py
 exchange_calendars/exchange_calendar_xpar.py
 exchange_calendars/exchange_calendar_xphs.py
 exchange_calendars/exchange_calendar_xpra.py
+exchange_calendars/exchange_calendar_xsau.py
 exchange_calendars/exchange_calendar_xses.py
 exchange_calendars/exchange_calendar_xsgo.py
 exchange_calendars/exchange_calendar_xshg.py
 exchange_calendars/exchange_calendar_xsto.py
 exchange_calendars/exchange_calendar_xswx.py
 exchange_calendars/exchange_calendar_xtae.py
 exchange_calendars/exchange_calendar_xtai.py
@@ -153,14 +154,15 @@
 tests/test_xmos_calendar.py
 tests/test_xnys_calendar.py
 tests/test_xnze_calendar.py
 tests/test_xosl_calendar.py
 tests/test_xpar_calendar.py
 tests/test_xphs_calendar.py
 tests/test_xpra_calendar.py
+tests/test_xsau_calendar.py
 tests/test_xses_calendar.py
 tests/test_xsgo_calendar.py
 tests/test_xshg_calendar.py
 tests/test_xsto_calendar.py
 tests/test_xswx_calendar.py
 tests/test_xtae_calendar.py
 tests/test_xtai_calendar.py
@@ -208,14 +210,15 @@
 tests/resources/xmos.csv
 tests/resources/xnys.csv
 tests/resources/xnze.csv
 tests/resources/xosl.csv
 tests/resources/xpar.csv
 tests/resources/xphs.csv
 tests/resources/xpra.csv
+tests/resources/xsau.csv
 tests/resources/xses.csv
 tests/resources/xsgo.csv
 tests/resources/xshg.csv
 tests/resources/xsto.csv
 tests/resources/xswx.csv
 tests/resources/xtae.csv
 tests/resources/xtai.csv
```

### Comparing `exchange_calendars-4.2.7/pyproject.toml` & `exchange_calendars-4.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/setup.cfg` & `exchange_calendars-4.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/24-5.csv` & `exchange_calendars-4.2.8/tests/resources/24-5.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/24-7.csv` & `exchange_calendars-4.2.8/tests/resources/24-7.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/aixk.csv` & `exchange_calendars-4.2.8/tests/resources/aixk.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/asex.csv` & `exchange_calendars-4.2.8/tests/resources/asex.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/bvmf.csv` & `exchange_calendars-4.2.8/tests/resources/bvmf.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/cmes.csv` & `exchange_calendars-4.2.8/tests/resources/cmes.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/iepa.csv` & `exchange_calendars-4.2.8/tests/resources/iepa.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/test.csv` & `exchange_calendars-4.2.8/tests/resources/test.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xams.csv` & `exchange_calendars-4.2.8/tests/resources/xams.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xasx.csv` & `exchange_calendars-4.2.8/tests/resources/xasx.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xbkk.csv` & `exchange_calendars-4.2.8/tests/resources/xbkk.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xbog.csv` & `exchange_calendars-4.2.8/tests/resources/xbog.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xbom.csv` & `exchange_calendars-4.2.8/tests/resources/xbom.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xbru.csv` & `exchange_calendars-4.2.8/tests/resources/xbru.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xbse.csv` & `exchange_calendars-4.2.8/tests/resources/xbse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xbud.csv` & `exchange_calendars-4.2.8/tests/resources/xbud.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xbue.csv` & `exchange_calendars-4.2.8/tests/resources/xbue.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xcbf.csv` & `exchange_calendars-4.2.8/tests/resources/xcbf.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xcse.csv` & `exchange_calendars-4.2.8/tests/resources/xcse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xdub.csv` & `exchange_calendars-4.2.8/tests/resources/xdub.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xetr.csv` & `exchange_calendars-4.2.8/tests/resources/xetr.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xfra.csv` & `exchange_calendars-4.2.8/tests/resources/xfra.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xhel.csv` & `exchange_calendars-4.2.8/tests/resources/xhel.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xhkg.csv` & `exchange_calendars-4.2.8/tests/resources/xhkg.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xice.csv` & `exchange_calendars-4.2.8/tests/resources/xice.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xidx.csv` & `exchange_calendars-4.2.8/tests/resources/xidx.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xist.csv` & `exchange_calendars-4.2.8/tests/resources/xist.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xjse.csv` & `exchange_calendars-4.2.8/tests/resources/xjse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xkar.csv` & `exchange_calendars-4.2.8/tests/resources/xkar.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xkls.csv` & `exchange_calendars-4.2.8/tests/resources/xkls.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xkrx.csv` & `exchange_calendars-4.2.8/tests/resources/xkrx.csv`

 * *Files 4% similar despite different names*

```diff
@@ -9653,8 +9653,427 @@
 2022-08-29T00:00:00Z,2022-08-29T00:00:00Z,2022-08-29T06:30:00Z,,
 2022-08-30T00:00:00Z,2022-08-30T00:00:00Z,2022-08-30T06:30:00Z,,
 2022-08-31T00:00:00Z,2022-08-31T00:00:00Z,2022-08-31T06:30:00Z,,
 2022-09-01T00:00:00Z,2022-09-01T00:00:00Z,2022-09-01T06:30:00Z,,
 2022-09-02T00:00:00Z,2022-09-02T00:00:00Z,2022-09-02T06:30:00Z,,
 2022-09-05T00:00:00Z,2022-09-05T00:00:00Z,2022-09-05T06:30:00Z,,
 2022-09-06T00:00:00Z,2022-09-06T00:00:00Z,2022-09-06T06:30:00Z,,
-2022-09-07T00:00:00Z,2022-09-07T01:00:00Z,2022-09-07T06:30:00Z,,
+2022-09-07T00:00:00Z,2022-09-07T00:00:00Z,2022-09-07T06:30:00Z,,
+2022-09-08T00:00:00Z,2022-09-08T00:00:00Z,2022-09-08T06:30:00Z,,
+2022-09-13T00:00:00Z,2022-09-13T00:00:00Z,2022-09-13T06:30:00Z,,
+2022-09-14T00:00:00Z,2022-09-14T00:00:00Z,2022-09-14T06:30:00Z,,
+2022-09-15T00:00:00Z,2022-09-15T00:00:00Z,2022-09-15T06:30:00Z,,
+2022-09-16T00:00:00Z,2022-09-16T00:00:00Z,2022-09-16T06:30:00Z,,
+2022-09-19T00:00:00Z,2022-09-19T00:00:00Z,2022-09-19T06:30:00Z,,
+2022-09-20T00:00:00Z,2022-09-20T00:00:00Z,2022-09-20T06:30:00Z,,
+2022-09-21T00:00:00Z,2022-09-21T00:00:00Z,2022-09-21T06:30:00Z,,
+2022-09-22T00:00:00Z,2022-09-22T00:00:00Z,2022-09-22T06:30:00Z,,
+2022-09-23T00:00:00Z,2022-09-23T00:00:00Z,2022-09-23T06:30:00Z,,
+2022-09-26T00:00:00Z,2022-09-26T00:00:00Z,2022-09-26T06:30:00Z,,
+2022-09-27T00:00:00Z,2022-09-27T00:00:00Z,2022-09-27T06:30:00Z,,
+2022-09-28T00:00:00Z,2022-09-28T00:00:00Z,2022-09-28T06:30:00Z,,
+2022-09-29T00:00:00Z,2022-09-29T00:00:00Z,2022-09-29T06:30:00Z,,
+2022-09-30T00:00:00Z,2022-09-30T00:00:00Z,2022-09-30T06:30:00Z,,
+2022-10-04T00:00:00Z,2022-10-04T00:00:00Z,2022-10-04T06:30:00Z,,
+2022-10-05T00:00:00Z,2022-10-05T00:00:00Z,2022-10-05T06:30:00Z,,
+2022-10-06T00:00:00Z,2022-10-06T00:00:00Z,2022-10-06T06:30:00Z,,
+2022-10-07T00:00:00Z,2022-10-07T00:00:00Z,2022-10-07T06:30:00Z,,
+2022-10-11T00:00:00Z,2022-10-11T00:00:00Z,2022-10-11T06:30:00Z,,
+2022-10-12T00:00:00Z,2022-10-12T00:00:00Z,2022-10-12T06:30:00Z,,
+2022-10-13T00:00:00Z,2022-10-13T00:00:00Z,2022-10-13T06:30:00Z,,
+2022-10-14T00:00:00Z,2022-10-14T00:00:00Z,2022-10-14T06:30:00Z,,
+2022-10-17T00:00:00Z,2022-10-17T00:00:00Z,2022-10-17T06:30:00Z,,
+2022-10-18T00:00:00Z,2022-10-18T00:00:00Z,2022-10-18T06:30:00Z,,
+2022-10-19T00:00:00Z,2022-10-19T00:00:00Z,2022-10-19T06:30:00Z,,
+2022-10-20T00:00:00Z,2022-10-20T00:00:00Z,2022-10-20T06:30:00Z,,
+2022-10-21T00:00:00Z,2022-10-21T00:00:00Z,2022-10-21T06:30:00Z,,
+2022-10-24T00:00:00Z,2022-10-24T00:00:00Z,2022-10-24T06:30:00Z,,
+2022-10-25T00:00:00Z,2022-10-25T00:00:00Z,2022-10-25T06:30:00Z,,
+2022-10-26T00:00:00Z,2022-10-26T00:00:00Z,2022-10-26T06:30:00Z,,
+2022-10-27T00:00:00Z,2022-10-27T00:00:00Z,2022-10-27T06:30:00Z,,
+2022-10-28T00:00:00Z,2022-10-28T00:00:00Z,2022-10-28T06:30:00Z,,
+2022-10-31T00:00:00Z,2022-10-31T00:00:00Z,2022-10-31T06:30:00Z,,
+2022-11-01T00:00:00Z,2022-11-01T00:00:00Z,2022-11-01T06:30:00Z,,
+2022-11-02T00:00:00Z,2022-11-02T00:00:00Z,2022-11-02T06:30:00Z,,
+2022-11-03T00:00:00Z,2022-11-03T00:00:00Z,2022-11-03T06:30:00Z,,
+2022-11-04T00:00:00Z,2022-11-04T00:00:00Z,2022-11-04T06:30:00Z,,
+2022-11-07T00:00:00Z,2022-11-07T00:00:00Z,2022-11-07T06:30:00Z,,
+2022-11-08T00:00:00Z,2022-11-08T00:00:00Z,2022-11-08T06:30:00Z,,
+2022-11-09T00:00:00Z,2022-11-09T00:00:00Z,2022-11-09T06:30:00Z,,
+2022-11-10T00:00:00Z,2022-11-10T00:00:00Z,2022-11-10T06:30:00Z,,
+2022-11-11T00:00:00Z,2022-11-11T00:00:00Z,2022-11-11T06:30:00Z,,
+2022-11-14T00:00:00Z,2022-11-14T00:00:00Z,2022-11-14T06:30:00Z,,
+2022-11-15T00:00:00Z,2022-11-15T00:00:00Z,2022-11-15T06:30:00Z,,
+2022-11-16T00:00:00Z,2022-11-16T00:00:00Z,2022-11-16T06:30:00Z,,
+2022-11-17T00:00:00Z,2022-11-17T00:00:00Z,2022-11-17T06:30:00Z,,
+2022-11-18T00:00:00Z,2022-11-18T00:00:00Z,2022-11-18T06:30:00Z,,
+2022-11-21T00:00:00Z,2022-11-21T00:00:00Z,2022-11-21T06:30:00Z,,
+2022-11-22T00:00:00Z,2022-11-22T00:00:00Z,2022-11-22T06:30:00Z,,
+2022-11-23T00:00:00Z,2022-11-23T00:00:00Z,2022-11-23T06:30:00Z,,
+2022-11-24T00:00:00Z,2022-11-24T00:00:00Z,2022-11-24T06:30:00Z,,
+2022-11-25T00:00:00Z,2022-11-25T00:00:00Z,2022-11-25T06:30:00Z,,
+2022-11-28T00:00:00Z,2022-11-28T00:00:00Z,2022-11-28T06:30:00Z,,
+2022-11-29T00:00:00Z,2022-11-29T00:00:00Z,2022-11-29T06:30:00Z,,
+2022-11-30T00:00:00Z,2022-11-30T00:00:00Z,2022-11-30T06:30:00Z,,
+2022-12-01T00:00:00Z,2022-12-01T00:00:00Z,2022-12-01T06:30:00Z,,
+2022-12-02T00:00:00Z,2022-12-02T00:00:00Z,2022-12-02T06:30:00Z,,
+2022-12-05T00:00:00Z,2022-12-05T00:00:00Z,2022-12-05T06:30:00Z,,
+2022-12-06T00:00:00Z,2022-12-06T00:00:00Z,2022-12-06T06:30:00Z,,
+2022-12-07T00:00:00Z,2022-12-07T00:00:00Z,2022-12-07T06:30:00Z,,
+2022-12-08T00:00:00Z,2022-12-08T00:00:00Z,2022-12-08T06:30:00Z,,
+2022-12-09T00:00:00Z,2022-12-09T00:00:00Z,2022-12-09T06:30:00Z,,
+2022-12-12T00:00:00Z,2022-12-12T00:00:00Z,2022-12-12T06:30:00Z,,
+2022-12-13T00:00:00Z,2022-12-13T00:00:00Z,2022-12-13T06:30:00Z,,
+2022-12-14T00:00:00Z,2022-12-14T00:00:00Z,2022-12-14T06:30:00Z,,
+2022-12-15T00:00:00Z,2022-12-15T00:00:00Z,2022-12-15T06:30:00Z,,
+2022-12-16T00:00:00Z,2022-12-16T00:00:00Z,2022-12-16T06:30:00Z,,
+2022-12-19T00:00:00Z,2022-12-19T00:00:00Z,2022-12-19T06:30:00Z,,
+2022-12-20T00:00:00Z,2022-12-20T00:00:00Z,2022-12-20T06:30:00Z,,
+2022-12-21T00:00:00Z,2022-12-21T00:00:00Z,2022-12-21T06:30:00Z,,
+2022-12-22T00:00:00Z,2022-12-22T00:00:00Z,2022-12-22T06:30:00Z,,
+2022-12-23T00:00:00Z,2022-12-23T00:00:00Z,2022-12-23T06:30:00Z,,
+2022-12-26T00:00:00Z,2022-12-26T00:00:00Z,2022-12-26T06:30:00Z,,
+2022-12-27T00:00:00Z,2022-12-27T00:00:00Z,2022-12-27T06:30:00Z,,
+2022-12-28T00:00:00Z,2022-12-28T00:00:00Z,2022-12-28T06:30:00Z,,
+2022-12-29T00:00:00Z,2022-12-29T00:00:00Z,2022-12-29T06:30:00Z,,
+2023-01-02T00:00:00Z,2023-01-02T01:00:00Z,2023-01-02T06:30:00Z,,
+2023-01-03T00:00:00Z,2023-01-03T00:00:00Z,2023-01-03T06:30:00Z,,
+2023-01-04T00:00:00Z,2023-01-04T00:00:00Z,2023-01-04T06:30:00Z,,
+2023-01-05T00:00:00Z,2023-01-05T00:00:00Z,2023-01-05T06:30:00Z,,
+2023-01-06T00:00:00Z,2023-01-06T00:00:00Z,2023-01-06T06:30:00Z,,
+2023-01-09T00:00:00Z,2023-01-09T00:00:00Z,2023-01-09T06:30:00Z,,
+2023-01-10T00:00:00Z,2023-01-10T00:00:00Z,2023-01-10T06:30:00Z,,
+2023-01-11T00:00:00Z,2023-01-11T00:00:00Z,2023-01-11T06:30:00Z,,
+2023-01-12T00:00:00Z,2023-01-12T00:00:00Z,2023-01-12T06:30:00Z,,
+2023-01-13T00:00:00Z,2023-01-13T00:00:00Z,2023-01-13T06:30:00Z,,
+2023-01-16T00:00:00Z,2023-01-16T00:00:00Z,2023-01-16T06:30:00Z,,
+2023-01-17T00:00:00Z,2023-01-17T00:00:00Z,2023-01-17T06:30:00Z,,
+2023-01-18T00:00:00Z,2023-01-18T00:00:00Z,2023-01-18T06:30:00Z,,
+2023-01-19T00:00:00Z,2023-01-19T00:00:00Z,2023-01-19T06:30:00Z,,
+2023-01-20T00:00:00Z,2023-01-20T00:00:00Z,2023-01-20T06:30:00Z,,
+2023-01-25T00:00:00Z,2023-01-25T00:00:00Z,2023-01-25T06:30:00Z,,
+2023-01-26T00:00:00Z,2023-01-26T00:00:00Z,2023-01-26T06:30:00Z,,
+2023-01-27T00:00:00Z,2023-01-27T00:00:00Z,2023-01-27T06:30:00Z,,
+2023-01-30T00:00:00Z,2023-01-30T00:00:00Z,2023-01-30T06:30:00Z,,
+2023-01-31T00:00:00Z,2023-01-31T00:00:00Z,2023-01-31T06:30:00Z,,
+2023-02-01T00:00:00Z,2023-02-01T00:00:00Z,2023-02-01T06:30:00Z,,
+2023-02-02T00:00:00Z,2023-02-02T00:00:00Z,2023-02-02T06:30:00Z,,
+2023-02-03T00:00:00Z,2023-02-03T00:00:00Z,2023-02-03T06:30:00Z,,
+2023-02-06T00:00:00Z,2023-02-06T00:00:00Z,2023-02-06T06:30:00Z,,
+2023-02-07T00:00:00Z,2023-02-07T00:00:00Z,2023-02-07T06:30:00Z,,
+2023-02-08T00:00:00Z,2023-02-08T00:00:00Z,2023-02-08T06:30:00Z,,
+2023-02-09T00:00:00Z,2023-02-09T00:00:00Z,2023-02-09T06:30:00Z,,
+2023-02-10T00:00:00Z,2023-02-10T00:00:00Z,2023-02-10T06:30:00Z,,
+2023-02-13T00:00:00Z,2023-02-13T00:00:00Z,2023-02-13T06:30:00Z,,
+2023-02-14T00:00:00Z,2023-02-14T00:00:00Z,2023-02-14T06:30:00Z,,
+2023-02-15T00:00:00Z,2023-02-15T00:00:00Z,2023-02-15T06:30:00Z,,
+2023-02-16T00:00:00Z,2023-02-16T00:00:00Z,2023-02-16T06:30:00Z,,
+2023-02-17T00:00:00Z,2023-02-17T00:00:00Z,2023-02-17T06:30:00Z,,
+2023-02-20T00:00:00Z,2023-02-20T00:00:00Z,2023-02-20T06:30:00Z,,
+2023-02-21T00:00:00Z,2023-02-21T00:00:00Z,2023-02-21T06:30:00Z,,
+2023-02-22T00:00:00Z,2023-02-22T00:00:00Z,2023-02-22T06:30:00Z,,
+2023-02-23T00:00:00Z,2023-02-23T00:00:00Z,2023-02-23T06:30:00Z,,
+2023-02-24T00:00:00Z,2023-02-24T00:00:00Z,2023-02-24T06:30:00Z,,
+2023-02-27T00:00:00Z,2023-02-27T00:00:00Z,2023-02-27T06:30:00Z,,
+2023-02-28T00:00:00Z,2023-02-28T00:00:00Z,2023-02-28T06:30:00Z,,
+2023-03-02T00:00:00Z,2023-03-02T00:00:00Z,2023-03-02T06:30:00Z,,
+2023-03-03T00:00:00Z,2023-03-03T00:00:00Z,2023-03-03T06:30:00Z,,
+2023-03-06T00:00:00Z,2023-03-06T00:00:00Z,2023-03-06T06:30:00Z,,
+2023-03-07T00:00:00Z,2023-03-07T00:00:00Z,2023-03-07T06:30:00Z,,
+2023-03-08T00:00:00Z,2023-03-08T00:00:00Z,2023-03-08T06:30:00Z,,
+2023-03-09T00:00:00Z,2023-03-09T00:00:00Z,2023-03-09T06:30:00Z,,
+2023-03-10T00:00:00Z,2023-03-10T00:00:00Z,2023-03-10T06:30:00Z,,
+2023-03-13T00:00:00Z,2023-03-13T00:00:00Z,2023-03-13T06:30:00Z,,
+2023-03-14T00:00:00Z,2023-03-14T00:00:00Z,2023-03-14T06:30:00Z,,
+2023-03-15T00:00:00Z,2023-03-15T00:00:00Z,2023-03-15T06:30:00Z,,
+2023-03-16T00:00:00Z,2023-03-16T00:00:00Z,2023-03-16T06:30:00Z,,
+2023-03-17T00:00:00Z,2023-03-17T00:00:00Z,2023-03-17T06:30:00Z,,
+2023-03-20T00:00:00Z,2023-03-20T00:00:00Z,2023-03-20T06:30:00Z,,
+2023-03-21T00:00:00Z,2023-03-21T00:00:00Z,2023-03-21T06:30:00Z,,
+2023-03-22T00:00:00Z,2023-03-22T00:00:00Z,2023-03-22T06:30:00Z,,
+2023-03-23T00:00:00Z,2023-03-23T00:00:00Z,2023-03-23T06:30:00Z,,
+2023-03-24T00:00:00Z,2023-03-24T00:00:00Z,2023-03-24T06:30:00Z,,
+2023-03-27T00:00:00Z,2023-03-27T00:00:00Z,2023-03-27T06:30:00Z,,
+2023-03-28T00:00:00Z,2023-03-28T00:00:00Z,2023-03-28T06:30:00Z,,
+2023-03-29T00:00:00Z,2023-03-29T00:00:00Z,2023-03-29T06:30:00Z,,
+2023-03-30T00:00:00Z,2023-03-30T00:00:00Z,2023-03-30T06:30:00Z,,
+2023-03-31T00:00:00Z,2023-03-31T00:00:00Z,2023-03-31T06:30:00Z,,
+2023-04-03T00:00:00Z,2023-04-03T00:00:00Z,2023-04-03T06:30:00Z,,
+2023-04-04T00:00:00Z,2023-04-04T00:00:00Z,2023-04-04T06:30:00Z,,
+2023-04-05T00:00:00Z,2023-04-05T00:00:00Z,2023-04-05T06:30:00Z,,
+2023-04-06T00:00:00Z,2023-04-06T00:00:00Z,2023-04-06T06:30:00Z,,
+2023-04-07T00:00:00Z,2023-04-07T00:00:00Z,2023-04-07T06:30:00Z,,
+2023-04-10T00:00:00Z,2023-04-10T00:00:00Z,2023-04-10T06:30:00Z,,
+2023-04-11T00:00:00Z,2023-04-11T00:00:00Z,2023-04-11T06:30:00Z,,
+2023-04-12T00:00:00Z,2023-04-12T00:00:00Z,2023-04-12T06:30:00Z,,
+2023-04-13T00:00:00Z,2023-04-13T00:00:00Z,2023-04-13T06:30:00Z,,
+2023-04-14T00:00:00Z,2023-04-14T00:00:00Z,2023-04-14T06:30:00Z,,
+2023-04-17T00:00:00Z,2023-04-17T00:00:00Z,2023-04-17T06:30:00Z,,
+2023-04-18T00:00:00Z,2023-04-18T00:00:00Z,2023-04-18T06:30:00Z,,
+2023-04-19T00:00:00Z,2023-04-19T00:00:00Z,2023-04-19T06:30:00Z,,
+2023-04-20T00:00:00Z,2023-04-20T00:00:00Z,2023-04-20T06:30:00Z,,
+2023-04-21T00:00:00Z,2023-04-21T00:00:00Z,2023-04-21T06:30:00Z,,
+2023-04-24T00:00:00Z,2023-04-24T00:00:00Z,2023-04-24T06:30:00Z,,
+2023-04-25T00:00:00Z,2023-04-25T00:00:00Z,2023-04-25T06:30:00Z,,
+2023-04-26T00:00:00Z,2023-04-26T00:00:00Z,2023-04-26T06:30:00Z,,
+2023-04-27T00:00:00Z,2023-04-27T00:00:00Z,2023-04-27T06:30:00Z,,
+2023-04-28T00:00:00Z,2023-04-28T00:00:00Z,2023-04-28T06:30:00Z,,
+2023-05-02T00:00:00Z,2023-05-02T00:00:00Z,2023-05-02T06:30:00Z,,
+2023-05-03T00:00:00Z,2023-05-03T00:00:00Z,2023-05-03T06:30:00Z,,
+2023-05-04T00:00:00Z,2023-05-04T00:00:00Z,2023-05-04T06:30:00Z,,
+2023-05-08T00:00:00Z,2023-05-08T00:00:00Z,2023-05-08T06:30:00Z,,
+2023-05-09T00:00:00Z,2023-05-09T00:00:00Z,2023-05-09T06:30:00Z,,
+2023-05-10T00:00:00Z,2023-05-10T00:00:00Z,2023-05-10T06:30:00Z,,
+2023-05-11T00:00:00Z,2023-05-11T00:00:00Z,2023-05-11T06:30:00Z,,
+2023-05-12T00:00:00Z,2023-05-12T00:00:00Z,2023-05-12T06:30:00Z,,
+2023-05-15T00:00:00Z,2023-05-15T00:00:00Z,2023-05-15T06:30:00Z,,
+2023-05-16T00:00:00Z,2023-05-16T00:00:00Z,2023-05-16T06:30:00Z,,
+2023-05-17T00:00:00Z,2023-05-17T00:00:00Z,2023-05-17T06:30:00Z,,
+2023-05-18T00:00:00Z,2023-05-18T00:00:00Z,2023-05-18T06:30:00Z,,
+2023-05-19T00:00:00Z,2023-05-19T00:00:00Z,2023-05-19T06:30:00Z,,
+2023-05-22T00:00:00Z,2023-05-22T00:00:00Z,2023-05-22T06:30:00Z,,
+2023-05-23T00:00:00Z,2023-05-23T00:00:00Z,2023-05-23T06:30:00Z,,
+2023-05-24T00:00:00Z,2023-05-24T00:00:00Z,2023-05-24T06:30:00Z,,
+2023-05-25T00:00:00Z,2023-05-25T00:00:00Z,2023-05-25T06:30:00Z,,
+2023-05-26T00:00:00Z,2023-05-26T00:00:00Z,2023-05-26T06:30:00Z,,
+2023-05-30T00:00:00Z,2023-05-30T00:00:00Z,2023-05-30T06:30:00Z,,
+2023-05-31T00:00:00Z,2023-05-31T00:00:00Z,2023-05-31T06:30:00Z,,
+2023-06-01T00:00:00Z,2023-06-01T00:00:00Z,2023-06-01T06:30:00Z,,
+2023-06-02T00:00:00Z,2023-06-02T00:00:00Z,2023-06-02T06:30:00Z,,
+2023-06-05T00:00:00Z,2023-06-05T00:00:00Z,2023-06-05T06:30:00Z,,
+2023-06-07T00:00:00Z,2023-06-07T00:00:00Z,2023-06-07T06:30:00Z,,
+2023-06-08T00:00:00Z,2023-06-08T00:00:00Z,2023-06-08T06:30:00Z,,
+2023-06-09T00:00:00Z,2023-06-09T00:00:00Z,2023-06-09T06:30:00Z,,
+2023-06-12T00:00:00Z,2023-06-12T00:00:00Z,2023-06-12T06:30:00Z,,
+2023-06-13T00:00:00Z,2023-06-13T00:00:00Z,2023-06-13T06:30:00Z,,
+2023-06-14T00:00:00Z,2023-06-14T00:00:00Z,2023-06-14T06:30:00Z,,
+2023-06-15T00:00:00Z,2023-06-15T00:00:00Z,2023-06-15T06:30:00Z,,
+2023-06-16T00:00:00Z,2023-06-16T00:00:00Z,2023-06-16T06:30:00Z,,
+2023-06-19T00:00:00Z,2023-06-19T00:00:00Z,2023-06-19T06:30:00Z,,
+2023-06-20T00:00:00Z,2023-06-20T00:00:00Z,2023-06-20T06:30:00Z,,
+2023-06-21T00:00:00Z,2023-06-21T00:00:00Z,2023-06-21T06:30:00Z,,
+2023-06-22T00:00:00Z,2023-06-22T00:00:00Z,2023-06-22T06:30:00Z,,
+2023-06-23T00:00:00Z,2023-06-23T00:00:00Z,2023-06-23T06:30:00Z,,
+2023-06-26T00:00:00Z,2023-06-26T00:00:00Z,2023-06-26T06:30:00Z,,
+2023-06-27T00:00:00Z,2023-06-27T00:00:00Z,2023-06-27T06:30:00Z,,
+2023-06-28T00:00:00Z,2023-06-28T00:00:00Z,2023-06-28T06:30:00Z,,
+2023-06-29T00:00:00Z,2023-06-29T00:00:00Z,2023-06-29T06:30:00Z,,
+2023-06-30T00:00:00Z,2023-06-30T00:00:00Z,2023-06-30T06:30:00Z,,
+2023-07-03T00:00:00Z,2023-07-03T00:00:00Z,2023-07-03T06:30:00Z,,
+2023-07-04T00:00:00Z,2023-07-04T00:00:00Z,2023-07-04T06:30:00Z,,
+2023-07-05T00:00:00Z,2023-07-05T00:00:00Z,2023-07-05T06:30:00Z,,
+2023-07-06T00:00:00Z,2023-07-06T00:00:00Z,2023-07-06T06:30:00Z,,
+2023-07-07T00:00:00Z,2023-07-07T00:00:00Z,2023-07-07T06:30:00Z,,
+2023-07-10T00:00:00Z,2023-07-10T00:00:00Z,2023-07-10T06:30:00Z,,
+2023-07-11T00:00:00Z,2023-07-11T00:00:00Z,2023-07-11T06:30:00Z,,
+2023-07-12T00:00:00Z,2023-07-12T00:00:00Z,2023-07-12T06:30:00Z,,
+2023-07-13T00:00:00Z,2023-07-13T00:00:00Z,2023-07-13T06:30:00Z,,
+2023-07-14T00:00:00Z,2023-07-14T00:00:00Z,2023-07-14T06:30:00Z,,
+2023-07-17T00:00:00Z,2023-07-17T00:00:00Z,2023-07-17T06:30:00Z,,
+2023-07-18T00:00:00Z,2023-07-18T00:00:00Z,2023-07-18T06:30:00Z,,
+2023-07-19T00:00:00Z,2023-07-19T00:00:00Z,2023-07-19T06:30:00Z,,
+2023-07-20T00:00:00Z,2023-07-20T00:00:00Z,2023-07-20T06:30:00Z,,
+2023-07-21T00:00:00Z,2023-07-21T00:00:00Z,2023-07-21T06:30:00Z,,
+2023-07-24T00:00:00Z,2023-07-24T00:00:00Z,2023-07-24T06:30:00Z,,
+2023-07-25T00:00:00Z,2023-07-25T00:00:00Z,2023-07-25T06:30:00Z,,
+2023-07-26T00:00:00Z,2023-07-26T00:00:00Z,2023-07-26T06:30:00Z,,
+2023-07-27T00:00:00Z,2023-07-27T00:00:00Z,2023-07-27T06:30:00Z,,
+2023-07-28T00:00:00Z,2023-07-28T00:00:00Z,2023-07-28T06:30:00Z,,
+2023-07-31T00:00:00Z,2023-07-31T00:00:00Z,2023-07-31T06:30:00Z,,
+2023-08-01T00:00:00Z,2023-08-01T00:00:00Z,2023-08-01T06:30:00Z,,
+2023-08-02T00:00:00Z,2023-08-02T00:00:00Z,2023-08-02T06:30:00Z,,
+2023-08-03T00:00:00Z,2023-08-03T00:00:00Z,2023-08-03T06:30:00Z,,
+2023-08-04T00:00:00Z,2023-08-04T00:00:00Z,2023-08-04T06:30:00Z,,
+2023-08-07T00:00:00Z,2023-08-07T00:00:00Z,2023-08-07T06:30:00Z,,
+2023-08-08T00:00:00Z,2023-08-08T00:00:00Z,2023-08-08T06:30:00Z,,
+2023-08-09T00:00:00Z,2023-08-09T00:00:00Z,2023-08-09T06:30:00Z,,
+2023-08-10T00:00:00Z,2023-08-10T00:00:00Z,2023-08-10T06:30:00Z,,
+2023-08-11T00:00:00Z,2023-08-11T00:00:00Z,2023-08-11T06:30:00Z,,
+2023-08-14T00:00:00Z,2023-08-14T00:00:00Z,2023-08-14T06:30:00Z,,
+2023-08-16T00:00:00Z,2023-08-16T00:00:00Z,2023-08-16T06:30:00Z,,
+2023-08-17T00:00:00Z,2023-08-17T00:00:00Z,2023-08-17T06:30:00Z,,
+2023-08-18T00:00:00Z,2023-08-18T00:00:00Z,2023-08-18T06:30:00Z,,
+2023-08-21T00:00:00Z,2023-08-21T00:00:00Z,2023-08-21T06:30:00Z,,
+2023-08-22T00:00:00Z,2023-08-22T00:00:00Z,2023-08-22T06:30:00Z,,
+2023-08-23T00:00:00Z,2023-08-23T00:00:00Z,2023-08-23T06:30:00Z,,
+2023-08-24T00:00:00Z,2023-08-24T00:00:00Z,2023-08-24T06:30:00Z,,
+2023-08-25T00:00:00Z,2023-08-25T00:00:00Z,2023-08-25T06:30:00Z,,
+2023-08-28T00:00:00Z,2023-08-28T00:00:00Z,2023-08-28T06:30:00Z,,
+2023-08-29T00:00:00Z,2023-08-29T00:00:00Z,2023-08-29T06:30:00Z,,
+2023-08-30T00:00:00Z,2023-08-30T00:00:00Z,2023-08-30T06:30:00Z,,
+2023-08-31T00:00:00Z,2023-08-31T00:00:00Z,2023-08-31T06:30:00Z,,
+2023-09-01T00:00:00Z,2023-09-01T00:00:00Z,2023-09-01T06:30:00Z,,
+2023-09-04T00:00:00Z,2023-09-04T00:00:00Z,2023-09-04T06:30:00Z,,
+2023-09-05T00:00:00Z,2023-09-05T00:00:00Z,2023-09-05T06:30:00Z,,
+2023-09-06T00:00:00Z,2023-09-06T00:00:00Z,2023-09-06T06:30:00Z,,
+2023-09-07T00:00:00Z,2023-09-07T00:00:00Z,2023-09-07T06:30:00Z,,
+2023-09-08T00:00:00Z,2023-09-08T00:00:00Z,2023-09-08T06:30:00Z,,
+2023-09-11T00:00:00Z,2023-09-11T00:00:00Z,2023-09-11T06:30:00Z,,
+2023-09-12T00:00:00Z,2023-09-12T00:00:00Z,2023-09-12T06:30:00Z,,
+2023-09-13T00:00:00Z,2023-09-13T00:00:00Z,2023-09-13T06:30:00Z,,
+2023-09-14T00:00:00Z,2023-09-14T00:00:00Z,2023-09-14T06:30:00Z,,
+2023-09-15T00:00:00Z,2023-09-15T00:00:00Z,2023-09-15T06:30:00Z,,
+2023-09-18T00:00:00Z,2023-09-18T00:00:00Z,2023-09-18T06:30:00Z,,
+2023-09-19T00:00:00Z,2023-09-19T00:00:00Z,2023-09-19T06:30:00Z,,
+2023-09-20T00:00:00Z,2023-09-20T00:00:00Z,2023-09-20T06:30:00Z,,
+2023-09-21T00:00:00Z,2023-09-21T00:00:00Z,2023-09-21T06:30:00Z,,
+2023-09-22T00:00:00Z,2023-09-22T00:00:00Z,2023-09-22T06:30:00Z,,
+2023-09-25T00:00:00Z,2023-09-25T00:00:00Z,2023-09-25T06:30:00Z,,
+2023-09-26T00:00:00Z,2023-09-26T00:00:00Z,2023-09-26T06:30:00Z,,
+2023-09-27T00:00:00Z,2023-09-27T00:00:00Z,2023-09-27T06:30:00Z,,
+2023-10-02T00:00:00Z,2023-10-02T00:00:00Z,2023-10-02T06:30:00Z,,
+2023-10-04T00:00:00Z,2023-10-04T00:00:00Z,2023-10-04T06:30:00Z,,
+2023-10-05T00:00:00Z,2023-10-05T00:00:00Z,2023-10-05T06:30:00Z,,
+2023-10-06T00:00:00Z,2023-10-06T00:00:00Z,2023-10-06T06:30:00Z,,
+2023-10-10T00:00:00Z,2023-10-10T00:00:00Z,2023-10-10T06:30:00Z,,
+2023-10-11T00:00:00Z,2023-10-11T00:00:00Z,2023-10-11T06:30:00Z,,
+2023-10-12T00:00:00Z,2023-10-12T00:00:00Z,2023-10-12T06:30:00Z,,
+2023-10-13T00:00:00Z,2023-10-13T00:00:00Z,2023-10-13T06:30:00Z,,
+2023-10-16T00:00:00Z,2023-10-16T00:00:00Z,2023-10-16T06:30:00Z,,
+2023-10-17T00:00:00Z,2023-10-17T00:00:00Z,2023-10-17T06:30:00Z,,
+2023-10-18T00:00:00Z,2023-10-18T00:00:00Z,2023-10-18T06:30:00Z,,
+2023-10-19T00:00:00Z,2023-10-19T00:00:00Z,2023-10-19T06:30:00Z,,
+2023-10-20T00:00:00Z,2023-10-20T00:00:00Z,2023-10-20T06:30:00Z,,
+2023-10-23T00:00:00Z,2023-10-23T00:00:00Z,2023-10-23T06:30:00Z,,
+2023-10-24T00:00:00Z,2023-10-24T00:00:00Z,2023-10-24T06:30:00Z,,
+2023-10-25T00:00:00Z,2023-10-25T00:00:00Z,2023-10-25T06:30:00Z,,
+2023-10-26T00:00:00Z,2023-10-26T00:00:00Z,2023-10-26T06:30:00Z,,
+2023-10-27T00:00:00Z,2023-10-27T00:00:00Z,2023-10-27T06:30:00Z,,
+2023-10-30T00:00:00Z,2023-10-30T00:00:00Z,2023-10-30T06:30:00Z,,
+2023-10-31T00:00:00Z,2023-10-31T00:00:00Z,2023-10-31T06:30:00Z,,
+2023-11-01T00:00:00Z,2023-11-01T00:00:00Z,2023-11-01T06:30:00Z,,
+2023-11-02T00:00:00Z,2023-11-02T00:00:00Z,2023-11-02T06:30:00Z,,
+2023-11-03T00:00:00Z,2023-11-03T00:00:00Z,2023-11-03T06:30:00Z,,
+2023-11-06T00:00:00Z,2023-11-06T00:00:00Z,2023-11-06T06:30:00Z,,
+2023-11-07T00:00:00Z,2023-11-07T00:00:00Z,2023-11-07T06:30:00Z,,
+2023-11-08T00:00:00Z,2023-11-08T00:00:00Z,2023-11-08T06:30:00Z,,
+2023-11-09T00:00:00Z,2023-11-09T00:00:00Z,2023-11-09T06:30:00Z,,
+2023-11-10T00:00:00Z,2023-11-10T00:00:00Z,2023-11-10T06:30:00Z,,
+2023-11-13T00:00:00Z,2023-11-13T00:00:00Z,2023-11-13T06:30:00Z,,
+2023-11-14T00:00:00Z,2023-11-14T00:00:00Z,2023-11-14T06:30:00Z,,
+2023-11-15T00:00:00Z,2023-11-15T00:00:00Z,2023-11-15T06:30:00Z,,
+2023-11-16T00:00:00Z,2023-11-16T00:00:00Z,2023-11-16T06:30:00Z,,
+2023-11-17T00:00:00Z,2023-11-17T00:00:00Z,2023-11-17T06:30:00Z,,
+2023-11-20T00:00:00Z,2023-11-20T00:00:00Z,2023-11-20T06:30:00Z,,
+2023-11-21T00:00:00Z,2023-11-21T00:00:00Z,2023-11-21T06:30:00Z,,
+2023-11-22T00:00:00Z,2023-11-22T00:00:00Z,2023-11-22T06:30:00Z,,
+2023-11-23T00:00:00Z,2023-11-23T00:00:00Z,2023-11-23T06:30:00Z,,
+2023-11-24T00:00:00Z,2023-11-24T00:00:00Z,2023-11-24T06:30:00Z,,
+2023-11-27T00:00:00Z,2023-11-27T00:00:00Z,2023-11-27T06:30:00Z,,
+2023-11-28T00:00:00Z,2023-11-28T00:00:00Z,2023-11-28T06:30:00Z,,
+2023-11-29T00:00:00Z,2023-11-29T00:00:00Z,2023-11-29T06:30:00Z,,
+2023-11-30T00:00:00Z,2023-11-30T00:00:00Z,2023-11-30T06:30:00Z,,
+2023-12-01T00:00:00Z,2023-12-01T00:00:00Z,2023-12-01T06:30:00Z,,
+2023-12-04T00:00:00Z,2023-12-04T00:00:00Z,2023-12-04T06:30:00Z,,
+2023-12-05T00:00:00Z,2023-12-05T00:00:00Z,2023-12-05T06:30:00Z,,
+2023-12-06T00:00:00Z,2023-12-06T00:00:00Z,2023-12-06T06:30:00Z,,
+2023-12-07T00:00:00Z,2023-12-07T00:00:00Z,2023-12-07T06:30:00Z,,
+2023-12-08T00:00:00Z,2023-12-08T00:00:00Z,2023-12-08T06:30:00Z,,
+2023-12-11T00:00:00Z,2023-12-11T00:00:00Z,2023-12-11T06:30:00Z,,
+2023-12-12T00:00:00Z,2023-12-12T00:00:00Z,2023-12-12T06:30:00Z,,
+2023-12-13T00:00:00Z,2023-12-13T00:00:00Z,2023-12-13T06:30:00Z,,
+2023-12-14T00:00:00Z,2023-12-14T00:00:00Z,2023-12-14T06:30:00Z,,
+2023-12-15T00:00:00Z,2023-12-15T00:00:00Z,2023-12-15T06:30:00Z,,
+2023-12-18T00:00:00Z,2023-12-18T00:00:00Z,2023-12-18T06:30:00Z,,
+2023-12-19T00:00:00Z,2023-12-19T00:00:00Z,2023-12-19T06:30:00Z,,
+2023-12-20T00:00:00Z,2023-12-20T00:00:00Z,2023-12-20T06:30:00Z,,
+2023-12-21T00:00:00Z,2023-12-21T00:00:00Z,2023-12-21T06:30:00Z,,
+2023-12-22T00:00:00Z,2023-12-22T00:00:00Z,2023-12-22T06:30:00Z,,
+2023-12-26T00:00:00Z,2023-12-26T00:00:00Z,2023-12-26T06:30:00Z,,
+2023-12-27T00:00:00Z,2023-12-27T00:00:00Z,2023-12-27T06:30:00Z,,
+2023-12-28T00:00:00Z,2023-12-28T00:00:00Z,2023-12-28T06:30:00Z,,
+2024-01-02T00:00:00Z,2024-01-02T01:00:00Z,2024-01-02T06:30:00Z,,
+2024-01-03T00:00:00Z,2024-01-03T00:00:00Z,2024-01-03T06:30:00Z,,
+2024-01-04T00:00:00Z,2024-01-04T00:00:00Z,2024-01-04T06:30:00Z,,
+2024-01-05T00:00:00Z,2024-01-05T00:00:00Z,2024-01-05T06:30:00Z,,
+2024-01-08T00:00:00Z,2024-01-08T00:00:00Z,2024-01-08T06:30:00Z,,
+2024-01-09T00:00:00Z,2024-01-09T00:00:00Z,2024-01-09T06:30:00Z,,
+2024-01-10T00:00:00Z,2024-01-10T00:00:00Z,2024-01-10T06:30:00Z,,
+2024-01-11T00:00:00Z,2024-01-11T00:00:00Z,2024-01-11T06:30:00Z,,
+2024-01-12T00:00:00Z,2024-01-12T00:00:00Z,2024-01-12T06:30:00Z,,
+2024-01-15T00:00:00Z,2024-01-15T00:00:00Z,2024-01-15T06:30:00Z,,
+2024-01-16T00:00:00Z,2024-01-16T00:00:00Z,2024-01-16T06:30:00Z,,
+2024-01-17T00:00:00Z,2024-01-17T00:00:00Z,2024-01-17T06:30:00Z,,
+2024-01-18T00:00:00Z,2024-01-18T00:00:00Z,2024-01-18T06:30:00Z,,
+2024-01-19T00:00:00Z,2024-01-19T00:00:00Z,2024-01-19T06:30:00Z,,
+2024-01-22T00:00:00Z,2024-01-22T00:00:00Z,2024-01-22T06:30:00Z,,
+2024-01-23T00:00:00Z,2024-01-23T00:00:00Z,2024-01-23T06:30:00Z,,
+2024-01-24T00:00:00Z,2024-01-24T00:00:00Z,2024-01-24T06:30:00Z,,
+2024-01-25T00:00:00Z,2024-01-25T00:00:00Z,2024-01-25T06:30:00Z,,
+2024-01-26T00:00:00Z,2024-01-26T00:00:00Z,2024-01-26T06:30:00Z,,
+2024-01-29T00:00:00Z,2024-01-29T00:00:00Z,2024-01-29T06:30:00Z,,
+2024-01-30T00:00:00Z,2024-01-30T00:00:00Z,2024-01-30T06:30:00Z,,
+2024-01-31T00:00:00Z,2024-01-31T00:00:00Z,2024-01-31T06:30:00Z,,
+2024-02-01T00:00:00Z,2024-02-01T00:00:00Z,2024-02-01T06:30:00Z,,
+2024-02-02T00:00:00Z,2024-02-02T00:00:00Z,2024-02-02T06:30:00Z,,
+2024-02-05T00:00:00Z,2024-02-05T00:00:00Z,2024-02-05T06:30:00Z,,
+2024-02-06T00:00:00Z,2024-02-06T00:00:00Z,2024-02-06T06:30:00Z,,
+2024-02-07T00:00:00Z,2024-02-07T00:00:00Z,2024-02-07T06:30:00Z,,
+2024-02-08T00:00:00Z,2024-02-08T00:00:00Z,2024-02-08T06:30:00Z,,
+2024-02-13T00:00:00Z,2024-02-13T00:00:00Z,2024-02-13T06:30:00Z,,
+2024-02-14T00:00:00Z,2024-02-14T00:00:00Z,2024-02-14T06:30:00Z,,
+2024-02-15T00:00:00Z,2024-02-15T00:00:00Z,2024-02-15T06:30:00Z,,
+2024-02-16T00:00:00Z,2024-02-16T00:00:00Z,2024-02-16T06:30:00Z,,
+2024-02-19T00:00:00Z,2024-02-19T00:00:00Z,2024-02-19T06:30:00Z,,
+2024-02-20T00:00:00Z,2024-02-20T00:00:00Z,2024-02-20T06:30:00Z,,
+2024-02-21T00:00:00Z,2024-02-21T00:00:00Z,2024-02-21T06:30:00Z,,
+2024-02-22T00:00:00Z,2024-02-22T00:00:00Z,2024-02-22T06:30:00Z,,
+2024-02-23T00:00:00Z,2024-02-23T00:00:00Z,2024-02-23T06:30:00Z,,
+2024-02-26T00:00:00Z,2024-02-26T00:00:00Z,2024-02-26T06:30:00Z,,
+2024-02-27T00:00:00Z,2024-02-27T00:00:00Z,2024-02-27T06:30:00Z,,
+2024-02-28T00:00:00Z,2024-02-28T00:00:00Z,2024-02-28T06:30:00Z,,
+2024-02-29T00:00:00Z,2024-02-29T00:00:00Z,2024-02-29T06:30:00Z,,
+2024-03-04T00:00:00Z,2024-03-04T00:00:00Z,2024-03-04T06:30:00Z,,
+2024-03-05T00:00:00Z,2024-03-05T00:00:00Z,2024-03-05T06:30:00Z,,
+2024-03-06T00:00:00Z,2024-03-06T00:00:00Z,2024-03-06T06:30:00Z,,
+2024-03-07T00:00:00Z,2024-03-07T00:00:00Z,2024-03-07T06:30:00Z,,
+2024-03-08T00:00:00Z,2024-03-08T00:00:00Z,2024-03-08T06:30:00Z,,
+2024-03-11T00:00:00Z,2024-03-11T00:00:00Z,2024-03-11T06:30:00Z,,
+2024-03-12T00:00:00Z,2024-03-12T00:00:00Z,2024-03-12T06:30:00Z,,
+2024-03-13T00:00:00Z,2024-03-13T00:00:00Z,2024-03-13T06:30:00Z,,
+2024-03-14T00:00:00Z,2024-03-14T00:00:00Z,2024-03-14T06:30:00Z,,
+2024-03-15T00:00:00Z,2024-03-15T00:00:00Z,2024-03-15T06:30:00Z,,
+2024-03-18T00:00:00Z,2024-03-18T00:00:00Z,2024-03-18T06:30:00Z,,
+2024-03-19T00:00:00Z,2024-03-19T00:00:00Z,2024-03-19T06:30:00Z,,
+2024-03-20T00:00:00Z,2024-03-20T00:00:00Z,2024-03-20T06:30:00Z,,
+2024-03-21T00:00:00Z,2024-03-21T00:00:00Z,2024-03-21T06:30:00Z,,
+2024-03-22T00:00:00Z,2024-03-22T00:00:00Z,2024-03-22T06:30:00Z,,
+2024-03-25T00:00:00Z,2024-03-25T00:00:00Z,2024-03-25T06:30:00Z,,
+2024-03-26T00:00:00Z,2024-03-26T00:00:00Z,2024-03-26T06:30:00Z,,
+2024-03-27T00:00:00Z,2024-03-27T00:00:00Z,2024-03-27T06:30:00Z,,
+2024-03-28T00:00:00Z,2024-03-28T00:00:00Z,2024-03-28T06:30:00Z,,
+2024-03-29T00:00:00Z,2024-03-29T00:00:00Z,2024-03-29T06:30:00Z,,
+2024-04-01T00:00:00Z,2024-04-01T00:00:00Z,2024-04-01T06:30:00Z,,
+2024-04-02T00:00:00Z,2024-04-02T00:00:00Z,2024-04-02T06:30:00Z,,
+2024-04-03T00:00:00Z,2024-04-03T00:00:00Z,2024-04-03T06:30:00Z,,
+2024-04-04T00:00:00Z,2024-04-04T00:00:00Z,2024-04-04T06:30:00Z,,
+2024-04-05T00:00:00Z,2024-04-05T00:00:00Z,2024-04-05T06:30:00Z,,
+2024-04-08T00:00:00Z,2024-04-08T00:00:00Z,2024-04-08T06:30:00Z,,
+2024-04-09T00:00:00Z,2024-04-09T00:00:00Z,2024-04-09T06:30:00Z,,
+2024-04-10T00:00:00Z,2024-04-10T00:00:00Z,2024-04-10T06:30:00Z,,
+2024-04-11T00:00:00Z,2024-04-11T00:00:00Z,2024-04-11T06:30:00Z,,
+2024-04-12T00:00:00Z,2024-04-12T00:00:00Z,2024-04-12T06:30:00Z,,
+2024-04-15T00:00:00Z,2024-04-15T00:00:00Z,2024-04-15T06:30:00Z,,
+2024-04-16T00:00:00Z,2024-04-16T00:00:00Z,2024-04-16T06:30:00Z,,
+2024-04-17T00:00:00Z,2024-04-17T00:00:00Z,2024-04-17T06:30:00Z,,
+2024-04-18T00:00:00Z,2024-04-18T00:00:00Z,2024-04-18T06:30:00Z,,
+2024-04-19T00:00:00Z,2024-04-19T00:00:00Z,2024-04-19T06:30:00Z,,
+2024-04-22T00:00:00Z,2024-04-22T00:00:00Z,2024-04-22T06:30:00Z,,
+2024-04-23T00:00:00Z,2024-04-23T00:00:00Z,2024-04-23T06:30:00Z,,
+2024-04-24T00:00:00Z,2024-04-24T00:00:00Z,2024-04-24T06:30:00Z,,
+2024-04-25T00:00:00Z,2024-04-25T00:00:00Z,2024-04-25T06:30:00Z,,
+2024-04-26T00:00:00Z,2024-04-26T00:00:00Z,2024-04-26T06:30:00Z,,
+2024-04-29T00:00:00Z,2024-04-29T00:00:00Z,2024-04-29T06:30:00Z,,
+2024-04-30T00:00:00Z,2024-04-30T00:00:00Z,2024-04-30T06:30:00Z,,
+2024-05-02T00:00:00Z,2024-05-02T00:00:00Z,2024-05-02T06:30:00Z,,
+2024-05-03T00:00:00Z,2024-05-03T00:00:00Z,2024-05-03T06:30:00Z,,
+2024-05-07T00:00:00Z,2024-05-07T00:00:00Z,2024-05-07T06:30:00Z,,
+2024-05-08T00:00:00Z,2024-05-08T00:00:00Z,2024-05-08T06:30:00Z,,
+2024-05-09T00:00:00Z,2024-05-09T00:00:00Z,2024-05-09T06:30:00Z,,
+2024-05-10T00:00:00Z,2024-05-10T00:00:00Z,2024-05-10T06:30:00Z,,
+2024-05-13T00:00:00Z,2024-05-13T00:00:00Z,2024-05-13T06:30:00Z,,
+2024-05-14T00:00:00Z,2024-05-14T00:00:00Z,2024-05-14T06:30:00Z,,
+2024-05-16T00:00:00Z,2024-05-16T00:00:00Z,2024-05-16T06:30:00Z,,
+2024-05-17T00:00:00Z,2024-05-17T00:00:00Z,2024-05-17T06:30:00Z,,
+2024-05-20T00:00:00Z,2024-05-20T00:00:00Z,2024-05-20T06:30:00Z,,
+2024-05-21T00:00:00Z,2024-05-21T00:00:00Z,2024-05-21T06:30:00Z,,
+2024-05-22T00:00:00Z,2024-05-22T01:00:00Z,2024-05-22T06:30:00Z,,
```

### Comparing `exchange_calendars-4.2.7/tests/resources/xlim.csv` & `exchange_calendars-4.2.8/tests/resources/xlim.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xlis.csv` & `exchange_calendars-4.2.8/tests/resources/xlis.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xlon.csv` & `exchange_calendars-4.2.8/tests/resources/xlon.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xmad.csv` & `exchange_calendars-4.2.8/tests/resources/xmad.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xmex.csv` & `exchange_calendars-4.2.8/tests/resources/xmex.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xmil.csv` & `exchange_calendars-4.2.8/tests/resources/xmil.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xmos.csv` & `exchange_calendars-4.2.8/tests/resources/xmos.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xnys.csv` & `exchange_calendars-4.2.8/tests/resources/xnys.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xnze.csv` & `exchange_calendars-4.2.8/tests/resources/xnze.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xosl.csv` & `exchange_calendars-4.2.8/tests/resources/xosl.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xpar.csv` & `exchange_calendars-4.2.8/tests/resources/xpar.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xphs.csv` & `exchange_calendars-4.2.8/tests/resources/xphs.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xpra.csv` & `exchange_calendars-4.2.8/tests/resources/xpra.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xses.csv` & `exchange_calendars-4.2.8/tests/resources/xses.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xsgo.csv` & `exchange_calendars-4.2.8/tests/resources/xsgo.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xshg.csv` & `exchange_calendars-4.2.8/tests/resources/xshg.csv`

 * *Files 0% similar despite different names*

```diff
@@ -7948,15 +7948,14 @@
 2023-06-13T00:00:00Z,2023-06-13T01:30:00Z,2023-06-13T07:00:00Z,2023-06-13T03:30:00Z,2023-06-13T05:00:00Z
 2023-06-14T00:00:00Z,2023-06-14T01:30:00Z,2023-06-14T07:00:00Z,2023-06-14T03:30:00Z,2023-06-14T05:00:00Z
 2023-06-15T00:00:00Z,2023-06-15T01:30:00Z,2023-06-15T07:00:00Z,2023-06-15T03:30:00Z,2023-06-15T05:00:00Z
 2023-06-16T00:00:00Z,2023-06-16T01:30:00Z,2023-06-16T07:00:00Z,2023-06-16T03:30:00Z,2023-06-16T05:00:00Z
 2023-06-19T00:00:00Z,2023-06-19T01:30:00Z,2023-06-19T07:00:00Z,2023-06-19T03:30:00Z,2023-06-19T05:00:00Z
 2023-06-20T00:00:00Z,2023-06-20T01:30:00Z,2023-06-20T07:00:00Z,2023-06-20T03:30:00Z,2023-06-20T05:00:00Z
 2023-06-21T00:00:00Z,2023-06-21T01:30:00Z,2023-06-21T07:00:00Z,2023-06-21T03:30:00Z,2023-06-21T05:00:00Z
-2023-06-23T00:00:00Z,2023-06-23T01:30:00Z,2023-06-23T07:00:00Z,2023-06-23T03:30:00Z,2023-06-23T05:00:00Z
 2023-06-26T00:00:00Z,2023-06-26T01:30:00Z,2023-06-26T07:00:00Z,2023-06-26T03:30:00Z,2023-06-26T05:00:00Z
 2023-06-27T00:00:00Z,2023-06-27T01:30:00Z,2023-06-27T07:00:00Z,2023-06-27T03:30:00Z,2023-06-27T05:00:00Z
 2023-06-28T00:00:00Z,2023-06-28T01:30:00Z,2023-06-28T07:00:00Z,2023-06-28T03:30:00Z,2023-06-28T05:00:00Z
 2023-06-29T00:00:00Z,2023-06-29T01:30:00Z,2023-06-29T07:00:00Z,2023-06-29T03:30:00Z,2023-06-29T05:00:00Z
 2023-06-30T00:00:00Z,2023-06-30T01:30:00Z,2023-06-30T07:00:00Z,2023-06-30T03:30:00Z,2023-06-30T05:00:00Z
 2023-07-03T00:00:00Z,2023-07-03T01:30:00Z,2023-07-03T07:00:00Z,2023-07-03T03:30:00Z,2023-07-03T05:00:00Z
 2023-07-04T00:00:00Z,2023-07-04T01:30:00Z,2023-07-04T07:00:00Z,2023-07-04T03:30:00Z,2023-07-04T05:00:00Z
@@ -8142,7 +8141,42 @@
 2024-03-26T00:00:00Z,2024-03-26T01:30:00Z,2024-03-26T07:00:00Z,2024-03-26T03:30:00Z,2024-03-26T05:00:00Z
 2024-03-27T00:00:00Z,2024-03-27T01:30:00Z,2024-03-27T07:00:00Z,2024-03-27T03:30:00Z,2024-03-27T05:00:00Z
 2024-03-28T00:00:00Z,2024-03-28T01:30:00Z,2024-03-28T07:00:00Z,2024-03-28T03:30:00Z,2024-03-28T05:00:00Z
 2024-03-29T00:00:00Z,2024-03-29T01:30:00Z,2024-03-29T07:00:00Z,2024-03-29T03:30:00Z,2024-03-29T05:00:00Z
 2024-04-01T00:00:00Z,2024-04-01T01:30:00Z,2024-04-01T07:00:00Z,2024-04-01T03:30:00Z,2024-04-01T05:00:00Z
 2024-04-02T00:00:00Z,2024-04-02T01:30:00Z,2024-04-02T07:00:00Z,2024-04-02T03:30:00Z,2024-04-02T05:00:00Z
 2024-04-03T00:00:00Z,2024-04-03T01:30:00Z,2024-04-03T07:00:00Z,2024-04-03T03:30:00Z,2024-04-03T05:00:00Z
+2024-04-05T00:00:00Z,2024-04-05T01:30:00Z,2024-04-05T07:00:00Z,2024-04-05T03:30:00Z,2024-04-05T05:00:00Z
+2024-04-08T00:00:00Z,2024-04-08T01:30:00Z,2024-04-08T07:00:00Z,2024-04-08T03:30:00Z,2024-04-08T05:00:00Z
+2024-04-09T00:00:00Z,2024-04-09T01:30:00Z,2024-04-09T07:00:00Z,2024-04-09T03:30:00Z,2024-04-09T05:00:00Z
+2024-04-10T00:00:00Z,2024-04-10T01:30:00Z,2024-04-10T07:00:00Z,2024-04-10T03:30:00Z,2024-04-10T05:00:00Z
+2024-04-11T00:00:00Z,2024-04-11T01:30:00Z,2024-04-11T07:00:00Z,2024-04-11T03:30:00Z,2024-04-11T05:00:00Z
+2024-04-12T00:00:00Z,2024-04-12T01:30:00Z,2024-04-12T07:00:00Z,2024-04-12T03:30:00Z,2024-04-12T05:00:00Z
+2024-04-15T00:00:00Z,2024-04-15T01:30:00Z,2024-04-15T07:00:00Z,2024-04-15T03:30:00Z,2024-04-15T05:00:00Z
+2024-04-16T00:00:00Z,2024-04-16T01:30:00Z,2024-04-16T07:00:00Z,2024-04-16T03:30:00Z,2024-04-16T05:00:00Z
+2024-04-17T00:00:00Z,2024-04-17T01:30:00Z,2024-04-17T07:00:00Z,2024-04-17T03:30:00Z,2024-04-17T05:00:00Z
+2024-04-18T00:00:00Z,2024-04-18T01:30:00Z,2024-04-18T07:00:00Z,2024-04-18T03:30:00Z,2024-04-18T05:00:00Z
+2024-04-19T00:00:00Z,2024-04-19T01:30:00Z,2024-04-19T07:00:00Z,2024-04-19T03:30:00Z,2024-04-19T05:00:00Z
+2024-04-22T00:00:00Z,2024-04-22T01:30:00Z,2024-04-22T07:00:00Z,2024-04-22T03:30:00Z,2024-04-22T05:00:00Z
+2024-04-23T00:00:00Z,2024-04-23T01:30:00Z,2024-04-23T07:00:00Z,2024-04-23T03:30:00Z,2024-04-23T05:00:00Z
+2024-04-24T00:00:00Z,2024-04-24T01:30:00Z,2024-04-24T07:00:00Z,2024-04-24T03:30:00Z,2024-04-24T05:00:00Z
+2024-04-25T00:00:00Z,2024-04-25T01:30:00Z,2024-04-25T07:00:00Z,2024-04-25T03:30:00Z,2024-04-25T05:00:00Z
+2024-04-26T00:00:00Z,2024-04-26T01:30:00Z,2024-04-26T07:00:00Z,2024-04-26T03:30:00Z,2024-04-26T05:00:00Z
+2024-04-29T00:00:00Z,2024-04-29T01:30:00Z,2024-04-29T07:00:00Z,2024-04-29T03:30:00Z,2024-04-29T05:00:00Z
+2024-04-30T00:00:00Z,2024-04-30T01:30:00Z,2024-04-30T07:00:00Z,2024-04-30T03:30:00Z,2024-04-30T05:00:00Z
+2024-05-02T00:00:00Z,2024-05-02T01:30:00Z,2024-05-02T07:00:00Z,2024-05-02T03:30:00Z,2024-05-02T05:00:00Z
+2024-05-03T00:00:00Z,2024-05-03T01:30:00Z,2024-05-03T07:00:00Z,2024-05-03T03:30:00Z,2024-05-03T05:00:00Z
+2024-05-06T00:00:00Z,2024-05-06T01:30:00Z,2024-05-06T07:00:00Z,2024-05-06T03:30:00Z,2024-05-06T05:00:00Z
+2024-05-07T00:00:00Z,2024-05-07T01:30:00Z,2024-05-07T07:00:00Z,2024-05-07T03:30:00Z,2024-05-07T05:00:00Z
+2024-05-08T00:00:00Z,2024-05-08T01:30:00Z,2024-05-08T07:00:00Z,2024-05-08T03:30:00Z,2024-05-08T05:00:00Z
+2024-05-09T00:00:00Z,2024-05-09T01:30:00Z,2024-05-09T07:00:00Z,2024-05-09T03:30:00Z,2024-05-09T05:00:00Z
+2024-05-10T00:00:00Z,2024-05-10T01:30:00Z,2024-05-10T07:00:00Z,2024-05-10T03:30:00Z,2024-05-10T05:00:00Z
+2024-05-13T00:00:00Z,2024-05-13T01:30:00Z,2024-05-13T07:00:00Z,2024-05-13T03:30:00Z,2024-05-13T05:00:00Z
+2024-05-14T00:00:00Z,2024-05-14T01:30:00Z,2024-05-14T07:00:00Z,2024-05-14T03:30:00Z,2024-05-14T05:00:00Z
+2024-05-15T00:00:00Z,2024-05-15T01:30:00Z,2024-05-15T07:00:00Z,2024-05-15T03:30:00Z,2024-05-15T05:00:00Z
+2024-05-16T00:00:00Z,2024-05-16T01:30:00Z,2024-05-16T07:00:00Z,2024-05-16T03:30:00Z,2024-05-16T05:00:00Z
+2024-05-17T00:00:00Z,2024-05-17T01:30:00Z,2024-05-17T07:00:00Z,2024-05-17T03:30:00Z,2024-05-17T05:00:00Z
+2024-05-20T00:00:00Z,2024-05-20T01:30:00Z,2024-05-20T07:00:00Z,2024-05-20T03:30:00Z,2024-05-20T05:00:00Z
+2024-05-21T00:00:00Z,2024-05-21T01:30:00Z,2024-05-21T07:00:00Z,2024-05-21T03:30:00Z,2024-05-21T05:00:00Z
+2024-05-22T00:00:00Z,2024-05-22T01:30:00Z,2024-05-22T07:00:00Z,2024-05-22T03:30:00Z,2024-05-22T05:00:00Z
+2024-05-23T00:00:00Z,2024-05-23T01:30:00Z,2024-05-23T07:00:00Z,2024-05-23T03:30:00Z,2024-05-23T05:00:00Z
+2024-05-24T00:00:00Z,2024-05-24T01:30:00Z,2024-05-24T07:00:00Z,2024-05-24T03:30:00Z,2024-05-24T05:00:00Z
```

### Comparing `exchange_calendars-4.2.7/tests/resources/xsto.csv` & `exchange_calendars-4.2.8/tests/resources/xsto.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xswx.csv` & `exchange_calendars-4.2.8/tests/resources/xswx.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xtae.csv` & `exchange_calendars-4.2.8/tests/resources/xtae.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xtai.csv` & `exchange_calendars-4.2.8/tests/resources/xtai.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xtks.csv` & `exchange_calendars-4.2.8/tests/resources/xtks.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xtse.csv` & `exchange_calendars-4.2.8/tests/resources/xtse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xwar.csv` & `exchange_calendars-4.2.8/tests/resources/xwar.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/resources/xwbo.csv` & `exchange_calendars-4.2.8/tests/resources/xwbo.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_aixk_calendar.py` & `exchange_calendars-4.2.8/tests/test_aixk_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_always_open.py` & `exchange_calendars-4.2.8/tests/test_always_open.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_asex_calendar.py` & `exchange_calendars-4.2.8/tests/test_asex_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_bvmf_calendar.py` & `exchange_calendars-4.2.8/tests/test_bvmf_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_calendar_dispatcher.py` & `exchange_calendars-4.2.8/tests/test_calendar_dispatcher.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_calendar_helpers.py` & `exchange_calendars-4.2.8/tests/test_calendar_helpers.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_cmes_calendar.py` & `exchange_calendars-4.2.8/tests/test_cmes_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_exchange_calendar.py` & `exchange_calendars-4.2.8/tests/test_exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_iepa_calendar.py` & `exchange_calendars-4.2.8/tests/test_iepa_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_weekday_calendar.py` & `exchange_calendars-4.2.8/tests/test_weekday_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xams_calendar.py` & `exchange_calendars-4.2.8/tests/test_xams_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xasx_calendar.py` & `exchange_calendars-4.2.8/tests/test_xasx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xbkk_calendar.py` & `exchange_calendars-4.2.8/tests/test_xbkk_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xbog_calendar.py` & `exchange_calendars-4.2.8/tests/test_xbog_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xbom_calendar.py` & `exchange_calendars-4.2.8/tests/test_xbom_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xbru_calendar.py` & `exchange_calendars-4.2.8/tests/test_xbru_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xbse_calendar.py` & `exchange_calendars-4.2.8/tests/test_xbse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xbud_calendar.py` & `exchange_calendars-4.2.8/tests/test_xbud_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xbue_calendar.py` & `exchange_calendars-4.2.8/tests/test_xbue_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xcbf_calendar.py` & `exchange_calendars-4.2.8/tests/test_xcbf_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xcse_calendar.py` & `exchange_calendars-4.2.8/tests/test_xcse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xdub_calendar.py` & `exchange_calendars-4.2.8/tests/test_xdub_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xetr_calendar.py` & `exchange_calendars-4.2.8/tests/test_xetr_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xfra_calendar.py` & `exchange_calendars-4.2.8/tests/test_xfra_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xhel_calendar.py` & `exchange_calendars-4.2.8/tests/test_xhel_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xhkg_calendar.py` & `exchange_calendars-4.2.8/tests/test_xhkg_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xice_calendar.py` & `exchange_calendars-4.2.8/tests/test_xice_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xidx_calendar.py` & `exchange_calendars-4.2.8/tests/test_xidx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xist_calendar.py` & `exchange_calendars-4.2.8/tests/test_xist_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xjse_calendar.py` & `exchange_calendars-4.2.8/tests/test_xjse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xkar_calendar.py` & `exchange_calendars-4.2.8/tests/test_xkar_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xkls_calendar.py` & `exchange_calendars-4.2.8/tests/test_xkls_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xkrx_calendar.py` & `exchange_calendars-4.2.8/tests/test_xkrx_calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,17 @@
             "2021-10-11",
             # korean thanks giving day on sunday
             # so the next monday becomes alternative holiday
             "2022-09-12",
             # Hangul Proclamation Day on Saturday
             # so the next monday becomes alternative holiday
             "2022-10-10",
+            # Buddha's birthday was on 27th May (Saturday),
+            # so the next monday becomes alternative holiday
+            "2023-05-29"
         ]
 
     @pytest.fixture
     def non_holidays_sample(self):
         yield [
             # Holidays that fall on a weekend and are not made up. Ensure surrounding
             # days are not holidays.
```

### Comparing `exchange_calendars-4.2.7/tests/test_xlim_calendar.py` & `exchange_calendars-4.2.8/tests/test_xlim_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xlis_calendar.py` & `exchange_calendars-4.2.8/tests/test_xlis_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xlon_calendar.py` & `exchange_calendars-4.2.8/tests/test_xlon_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xmad_calendar.py` & `exchange_calendars-4.2.8/tests/test_xmad_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xmex_calendar.py` & `exchange_calendars-4.2.8/tests/test_xmex_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xmil_calendar.py` & `exchange_calendars-4.2.8/tests/test_xmil_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xmos_calendar.py` & `exchange_calendars-4.2.8/tests/test_xmos_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xnys_calendar.py` & `exchange_calendars-4.2.8/tests/test_xnys_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xnze_calendar.py` & `exchange_calendars-4.2.8/tests/test_xnze_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xosl_calendar.py` & `exchange_calendars-4.2.8/tests/test_xosl_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xpar_calendar.py` & `exchange_calendars-4.2.8/tests/test_xpar_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xphs_calendar.py` & `exchange_calendars-4.2.8/tests/test_xphs_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xpra_calendar.py` & `exchange_calendars-4.2.8/tests/test_xpra_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xses_calendar.py` & `exchange_calendars-4.2.8/tests/test_xses_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xsgo_calendar.py` & `exchange_calendars-4.2.8/tests/test_xsgo_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xshg_calendar.py` & `exchange_calendars-4.2.8/tests/test_xshg_calendar.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,8 +51,9 @@
             "2022-01-31",
             "2022-09-12",
             "2022-10-06",
             "2022-10-07",
 
             # 2023
             "2023-05-03",  # Part of Chinese Labor Day 2023
+            "2023-06-23",  # Part of Dragon Boat Festival 2023
         ]
```

### Comparing `exchange_calendars-4.2.7/tests/test_xsto_calendar.py` & `exchange_calendars-4.2.8/tests/test_xsto_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xswx_calendar.py` & `exchange_calendars-4.2.8/tests/test_xswx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xtae_calendar.py` & `exchange_calendars-4.2.8/tests/test_xtae_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xtai_calendar.py` & `exchange_calendars-4.2.8/tests/test_xtai_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xtks_calendar.py` & `exchange_calendars-4.2.8/tests/test_xtks_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xtse_calendar.py` & `exchange_calendars-4.2.8/tests/test_xtse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xwar_calendar.py` & `exchange_calendars-4.2.8/tests/test_xwar_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.7/tests/test_xwbo_calendar.py` & `exchange_calendars-4.2.8/tests/test_xwbo_calendar.py`

 * *Files identical despite different names*

