# Comparing `tmp/recipe_scrapers_ap_fork-14.24.1.tar.gz` & `tmp/recipe_scrapers_ap_fork-14.24.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recipe_scrapers_ap_fork-14.24.1.tar", last modified: Sat Dec 10 14:23:01 2022, max compression
+gzip compressed data, was "recipe_scrapers_ap_fork-14.24.2.tar", last modified: Thu May 25 18:15:25 2023, max compression
```

## Comparing `recipe_scrapers_ap_fork-14.24.1.tar` & `recipe_scrapers_ap_fork-14.24.2.tar`

### file list

```diff
@@ -1,252 +1,481 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2022-12-10 14:23:01.349166 recipe_scrapers_ap_fork-14.24.1/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1080 2021-08-25 16:01:34.000000 recipe_scrapers_ap_fork-14.24.1/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)    20397 2022-12-10 14:23:01.349166 recipe_scrapers_ap_fork-14.24.1/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)    19735 2022-11-30 23:56:17.000000 recipe_scrapers_ap_fork-14.24.1/README.rst
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1172 2022-11-30 23:53:13.000000 recipe_scrapers_ap_fork-14.24.1/pyproject.toml
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2022-12-10 14:23:01.349166 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)    19899 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       24 2022-12-10 14:22:16.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/__version__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     5968 2022-12-10 14:21:35.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/_abstract.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1358 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/_exceptions.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1347 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/_factory.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     9849 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/_schemaorg.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     6110 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/_utils.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      561 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/abril.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      564 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/acouplecooks.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1775 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/afghankitchenrecipes.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2579 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/akispetretzikis.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1429 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/albertheijn.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     5920 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/allrecipes.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      676 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/alltomat.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      873 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/altonbrown.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      802 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/amazingribs.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      633 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/ambitiouskitchen.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      574 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/archanaskitchen.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      925 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/arla.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      648 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/atelierdeschefs.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      623 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/averiecooks.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bakingmischeif.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      624 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bakingsense.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1757 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bbcfood.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      631 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bbcgoodfood.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2146 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bettybossi.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      809 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bettycrocker.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1440 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bigoven.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      619 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/blueapron.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2296 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bodybuilding.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      483 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bonappetit.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      631 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bowlofdelicious.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      566 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/budgetbytes.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      625 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/castironketo.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      558 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cdkitchen.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      685 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/chefkoch.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1010 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/closetcooking.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      692 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/comidinhasdochef.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      485 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cookeatshare.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1270 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cookieandkate.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1886 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cookingcircle.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1101 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cookinglight.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      615 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cookpad.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1542 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cookstr.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1241 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/coop.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      971 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/copykat.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      501 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/countryliving.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      490 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cucchiaio.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      678 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cuisineaz.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      622 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cybercook.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      568 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/davidlebovitz.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      552 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/delish.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/ditchthecarbs.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      628 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/domesticateme.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      688 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/downshiftology.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      769 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/dr.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      688 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/eatingbirdfood.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1222 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/eatingwell.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      642 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/eatsmarter.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      568 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/eatwhattonight.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      875 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/emmikochteinfach.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/epicurious.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      894 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/ethanchlebowski.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     4132 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/farmhousedelivery.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      631 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/fifteenspatulas.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      727 2022-11-30 23:29:18.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/finedininglovers.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1427 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/fitmencook.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      548 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/food.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1145 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/food52.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      562 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/foodandwine.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      564 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/foodnetwork.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1112 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/foodrepublic.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1288 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/forksoverknives.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      874 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/franzoesischkochen.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1386 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/fredriksfikaallas.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      610 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/g750g.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      570 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/geniuskitchen.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      581 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/giallozafferano.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/gimmesomeoven.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      559 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/globo.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      641 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/gonnawantseconds.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      671 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/gousto.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2003 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/goustojson.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      644 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/greatbritishchefs.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      633 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/halfbakedharvest.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      581 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/handletheheat.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      680 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/hassanchef.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      696 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/headbangerskitchen.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/heb.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1015 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/heinzbrasil.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1579 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/hellofresh.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      915 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/homechef.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      625 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/hostthetoast.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      517 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/hundredandonecookbooks.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      923 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/ica.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1665 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/ig.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      870 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/imworthy.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      700 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/indianhealthyrecipes.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      810 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/innit.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      547 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/inspiralized.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1162 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/jamieoliver.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      692 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/jimcooksfoodgood.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1572 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/joyfoodsunshine.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      621 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/justataste.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1783 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/justbento.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1341 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/justonecookbook.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1124 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/kennymcgovern.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1341 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/kingarthur.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1623 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/kitchenstories.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      553 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/kochbar.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      669 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/koket.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     3601 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/kptncook.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      649 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/kuchniadomowa.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1182 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/kwestiasmaku.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2016 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/latelierderoxane.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1377 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/leanandgreenrecipes.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1763 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/lecker.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      633 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/lecremedelacrumb.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1119 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/lekkerensimpel.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      629 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/littlespicejar.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      623 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/livelytable.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/lovingitvegan.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1440 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/maangchi.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1071 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/madensverden.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1736 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/madewithlau.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     4346 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/marleyspoon.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      617 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/marmiton.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      943 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/marthastewart.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      683 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/matprat.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2445 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/meljoulwan.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      631 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/melskitchencafe.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1987 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/mindmegette.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      631 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/minimalistbaker.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      612 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/misya.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1325 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/mobkitchen.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1365 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/momswithcrockpots.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2329 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/monsieurcuisine.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      566 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/motherthyme.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      578 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/mybakingaddiction.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1358 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/mykitchen101.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      560 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/mykitchen101en.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      558 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/myrecipes.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2372 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/nhshealthierfamilies.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     7324 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/nihhealthyeating.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      641 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/nourishedbynutrition.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1273 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/nutritionbynathalie.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      623 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/nytimes.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      621 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/ohsheglows.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1125 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/omnivorescookbook.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1137 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/onehundredonecookbooks.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      595 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/owenhan.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      694 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/paleorunningmomma.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1607 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/panelinha.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1091 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/paninihappy.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      847 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/pingodoce.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2022-12-10 14:23:01.349166 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      435 2022-04-06 21:27:02.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      910 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/_interface.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2069 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/exception_handling.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2354 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/html_tags_stripper.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1037 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/normalize_string.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1598 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/opengraph_image_fetch.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1755 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/schemaorg_fill.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1189 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/template.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1947 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/popsugar.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      597 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/practicalselfreliance.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      633 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/primaledgehealth.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1093 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/przepisy.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      621 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/purelypope.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      684 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/purplecarrot.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        0 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/py.typed
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1002 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/rachlmansfield.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      692 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/rainbowplantlife.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      687 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/realfoodtesco.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      687 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/realsimple.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/recipetineats.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      686 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/redhousespice.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2157 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/reishunger.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1623 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/rezeptwelt.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1273 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/rosannapansino.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      643 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/sallysbakingaddiction.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      566 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/saveur.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      625 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/seriouseats.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2022-12-10 14:23:01.349166 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/settings/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2810 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/settings/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1164 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/settings/default.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      274 2021-08-25 16:01:34.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/settings/template.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      876 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/simpleveganista.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1244 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/simplycookit.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      569 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/simplyquinoa.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1384 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/simplyrecipes.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/simplywhisked.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      623 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/skinnytaste.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1025 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/smulweb.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      587 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/southerncastiron.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      638 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/southernliving.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      684 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/spendwithpennies.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      937 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/springlane.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      822 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/steamykitchen.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1394 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/streetkitchen.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2277 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/sunbasket.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1030 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/sundpaabudget.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      629 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/sweetcsdesigns.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1953 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/sweetpeasandsaffron.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1090 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/tasteofhome.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      647 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/tastesbetterfromscratch.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      512 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/tastesoflizzyt.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      543 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/tasty.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1264 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/tastykitchen.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      682 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/theclevercarrot.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1472 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thehappyfoodie.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      633 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thekitchenmagpie.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      619 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thekitchn.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      579 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thenutritiouskitchen.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1013 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thepioneerwoman.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      566 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thespruceeats.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1302 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thevintagemixer.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thewoksoflife.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1093 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/timesofindia.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2526 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/tineno.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      934 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/tudogostoso.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      576 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/twopeasandtheirpod.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     3305 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/usdamyplate.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     3081 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/valdemarsro.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      629 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/vanillaandbean.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2185 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/vegolosi.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      694 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/vegrecipesofindia.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/watchwhatueat.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     5141 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/weightwatchers.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2292 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/weightwatcherspublic.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      515 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/whatsgabycooking.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      648 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/wholefoods.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2059 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/wikicookbook.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1907 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/woolworths.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1525 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/woop.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      670 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/yemek.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1595 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/yummly.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1711 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/zeitwochenmarkt.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      617 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/zenbelly.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2022-12-10 14:23:01.349166 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers_ap_fork.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)    20397 2022-12-10 14:23:01.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers_ap_fork.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     7906 2022-12-10 14:23:01.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers_ap_fork.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2022-12-10 14:23:01.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers_ap_fork.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2022-12-10 14:23:01.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers_ap_fork.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       16 2022-12-10 14:23:01.000000 recipe_scrapers_ap_fork-14.24.1/recipe_scrapers_ap_fork.egg-info/top_level.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2022-12-10 14:23:01.349166 recipe_scrapers_ap_fork-14.24.1/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-05-25 18:15:25.157905 recipe_scrapers_ap_fork-14.24.2/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1080 2021-08-25 16:01:34.000000 recipe_scrapers_ap_fork-14.24.2/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)    20397 2023-05-25 18:15:25.157905 recipe_scrapers_ap_fork-14.24.2/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)    19735 2022-11-30 23:56:17.000000 recipe_scrapers_ap_fork-14.24.2/README.rst
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1172 2022-11-30 23:53:13.000000 recipe_scrapers_ap_fork-14.24.2/pyproject.toml
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-05-25 18:15:25.101904 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)    19899 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/__init__.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       24 2023-05-25 18:14:22.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/__version__.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     6043 2023-05-25 13:27:33.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/_abstract.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1358 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/_exceptions.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1347 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/_factory.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     9849 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/_schemaorg.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     6110 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/_utils.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      561 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/abril.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      564 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/acouplecooks.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1775 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/afghankitchenrecipes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2579 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/akispetretzikis.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1429 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/albertheijn.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5920 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/allrecipes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      676 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/alltomat.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      873 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/altonbrown.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      802 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/amazingribs.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      633 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/ambitiouskitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      574 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/archanaskitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      925 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/arla.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      648 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/atelierdeschefs.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      623 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/averiecooks.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bakingmischeif.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      624 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bakingsense.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1757 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bbcfood.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      631 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bbcgoodfood.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2146 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bettybossi.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      809 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bettycrocker.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1440 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bigoven.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      619 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/blueapron.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2296 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bodybuilding.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      483 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bonappetit.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      631 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bowlofdelicious.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      566 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/budgetbytes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      625 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/castironketo.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      558 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cdkitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      685 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/chefkoch.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1010 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/closetcooking.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      692 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/comidinhasdochef.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      485 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cookeatshare.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1270 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cookieandkate.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1886 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cookingcircle.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1101 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cookinglight.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      615 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cookpad.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1542 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cookstr.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1241 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/coop.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      971 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/copykat.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      501 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/countryliving.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      490 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cucchiaio.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      678 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cuisineaz.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      622 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cybercook.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      568 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/davidlebovitz.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      552 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/delish.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/ditchthecarbs.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      628 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/domesticateme.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      688 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/downshiftology.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      769 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/dr.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      688 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/eatingbirdfood.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1222 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/eatingwell.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      642 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/eatsmarter.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      568 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/eatwhattonight.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      875 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/emmikochteinfach.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/epicurious.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      894 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/ethanchlebowski.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4132 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/farmhousedelivery.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      631 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/fifteenspatulas.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      727 2022-11-30 23:29:18.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/finedininglovers.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1427 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/fitmencook.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      548 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/food.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1145 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/food52.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      562 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/foodandwine.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      564 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/foodnetwork.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1112 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/foodrepublic.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1288 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/forksoverknives.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      874 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/franzoesischkochen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1386 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/fredriksfikaallas.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      610 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/g750g.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      570 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/geniuskitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      581 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/giallozafferano.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/gimmesomeoven.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      559 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/globo.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      641 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/gonnawantseconds.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      671 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/gousto.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2003 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/goustojson.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      644 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/greatbritishchefs.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      633 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/halfbakedharvest.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      581 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/handletheheat.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      680 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/hassanchef.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      696 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/headbangerskitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/heb.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1015 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/heinzbrasil.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1579 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/hellofresh.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      915 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/homechef.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      625 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/hostthetoast.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      517 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/hundredandonecookbooks.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      923 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/ica.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1665 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/ig.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      870 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/imworthy.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      700 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/indianhealthyrecipes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      810 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/innit.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      547 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/inspiralized.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1162 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/jamieoliver.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      692 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/jimcooksfoodgood.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1572 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/joyfoodsunshine.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      621 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/justataste.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1783 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/justbento.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1341 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/justonecookbook.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1124 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/kennymcgovern.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1341 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/kingarthur.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1623 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/kitchenstories.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      553 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/kochbar.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      669 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/koket.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3601 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/kptncook.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      649 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/kuchniadomowa.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1182 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/kwestiasmaku.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2016 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/latelierderoxane.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1377 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/leanandgreenrecipes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1763 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/lecker.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      633 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/lecremedelacrumb.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1119 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/lekkerensimpel.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      629 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/littlespicejar.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      623 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/livelytable.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/lovingitvegan.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1440 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/maangchi.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1071 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/madensverden.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1736 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/madewithlau.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4346 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/marleyspoon.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      617 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/marmiton.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      943 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/marthastewart.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      683 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/matprat.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2445 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/meljoulwan.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      631 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/melskitchencafe.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1987 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/mindmegette.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      631 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/minimalistbaker.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      612 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/misya.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1325 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/mobkitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1365 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/momswithcrockpots.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2329 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/monsieurcuisine.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      566 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/motherthyme.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      578 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/mybakingaddiction.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1358 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/mykitchen101.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      560 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/mykitchen101en.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      558 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/myrecipes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2372 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/nhshealthierfamilies.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     7324 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/nihhealthyeating.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      641 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/nourishedbynutrition.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1273 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/nutritionbynathalie.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      623 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/nytimes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      621 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/ohsheglows.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1125 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/omnivorescookbook.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1137 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/onehundredonecookbooks.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      595 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/owenhan.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      694 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/paleorunningmomma.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1607 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/panelinha.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1091 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/paninihappy.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      847 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/pingodoce.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-05-25 18:15:25.105904 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      435 2022-04-06 21:27:02.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/__init__.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      910 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/_interface.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2069 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/exception_handling.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2354 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/html_tags_stripper.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1037 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/normalize_string.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1598 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/opengraph_image_fetch.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1755 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/schemaorg_fill.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1189 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/template.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1947 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/popsugar.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      597 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/practicalselfreliance.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      633 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/primaledgehealth.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1093 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/przepisy.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      621 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/purelypope.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      684 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/purplecarrot.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        0 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/py.typed
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1002 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/rachlmansfield.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      692 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/rainbowplantlife.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      687 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/realfoodtesco.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      687 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/realsimple.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/recipetineats.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      686 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/redhousespice.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2157 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/reishunger.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1623 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/rezeptwelt.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1273 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/rosannapansino.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      643 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/sallysbakingaddiction.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      566 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/saveur.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      625 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/seriouseats.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-05-25 18:15:25.105904 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/settings/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2810 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/settings/__init__.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1164 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/settings/default.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      274 2021-08-25 16:01:34.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/settings/template.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      876 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/simpleveganista.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1244 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/simplycookit.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      569 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/simplyquinoa.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1384 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/simplyrecipes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/simplywhisked.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      623 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/skinnytaste.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1025 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/smulweb.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      587 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/southerncastiron.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      638 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/southernliving.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      684 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/spendwithpennies.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      937 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/springlane.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      822 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/steamykitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1394 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/streetkitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2277 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/sunbasket.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1030 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/sundpaabudget.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      629 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/sweetcsdesigns.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1953 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/sweetpeasandsaffron.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1090 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/tasteofhome.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      647 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/tastesbetterfromscratch.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      512 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/tastesoflizzyt.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      543 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/tasty.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1264 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/tastykitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      682 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/theclevercarrot.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1472 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thehappyfoodie.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      633 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thekitchenmagpie.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      619 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thekitchn.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      579 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thenutritiouskitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1013 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thepioneerwoman.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      566 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thespruceeats.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1302 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thevintagemixer.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thewoksoflife.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1093 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/timesofindia.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2526 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/tineno.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      934 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/tudogostoso.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      576 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/twopeasandtheirpod.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3305 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/usdamyplate.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3081 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/valdemarsro.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      629 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/vanillaandbean.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2185 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/vegolosi.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      694 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/vegrecipesofindia.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/watchwhatueat.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5141 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/weightwatchers.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2292 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/weightwatcherspublic.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      515 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/whatsgabycooking.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      648 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/wholefoods.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2059 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/wikicookbook.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1907 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/woolworths.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1525 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/woop.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      670 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/yemek.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1595 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/yummly.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1711 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/zeitwochenmarkt.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      617 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/zenbelly.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-05-25 18:15:25.105904 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers_ap_fork.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)    20397 2023-05-25 18:15:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers_ap_fork.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)    14046 2023-05-25 18:15:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers_ap_fork.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-05-25 18:15:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers_ap_fork.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-05-25 18:15:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers_ap_fork.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       16 2023-05-25 18:15:25.000000 recipe_scrapers_ap_fork-14.24.2/recipe_scrapers_ap_fork.egg-info/top_level.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-05-25 18:15:25.157905 recipe_scrapers_ap_fork-14.24.2/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-05-25 18:15:25.157905 recipe_scrapers_ap_fork-14.24.2/tests/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2190 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_750g.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2471 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_abril.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1896 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_acouplecooks.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4555 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_afghankitchenrecipes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3239 2022-04-06 21:27:02.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_akispetretzikis.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2527 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_albertheijn.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5188 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_allrecipes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2183 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_alltomat.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4307 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_altonbrown.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3065 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_amazingribs.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4643 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_ambitiouskitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2923 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_archanaskitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2885 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_arla.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3059 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_atelierdeschefs.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2465 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_averiecooks.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4321 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_bakingmischeif.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3279 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_bakingsense.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2537 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_bbc.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2848 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_bbcgoodfood.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3432 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_bettybossi.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2751 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_bettycrocker.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     6079 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_bigoven.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     7560 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_blueapron.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3120 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_bodybuilding.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3561 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_bonappetit.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3423 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_bowlofdelicious.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3177 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_budgetbytes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2408 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_castironketo.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2319 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_cdkitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3171 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_chefkoch.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1955 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_closetcooking.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2717 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_comidinhasdochef.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1873 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_cookeatshare.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3406 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_cookieandkate.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2640 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_cookingcircle.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2858 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_cookinglight.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2598 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_cookpad.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1982 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_cookstr.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2639 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_coop.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3266 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_copykat.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2582 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_countryliving.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3281 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_cucchiaio.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2305 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_cuisineaz.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2397 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_cybercook.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3360 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_davidlebovitz.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2918 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_delish.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2829 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_delishrogue.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3098 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_ditchthecarbs.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4145 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_domesticateme.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2723 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_downshiftology.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3002 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_dr.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2885 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_eatingbirdfood.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2737 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_eatingwell.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2028 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_eatsmarter.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2404 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_eatwhattonight.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5153 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_emmikochteinfach.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2207 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_epicurious.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2788 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_ethanchlebowski.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2125 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_farmhousedelivery_1.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2627 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_farmhousedelivery_2.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3712 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_fifteenspatulas.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2456 2022-12-01 00:11:02.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_finedininglovers.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5149 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_fitmencook.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2401 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_food.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3882 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_food52.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2249 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_foodandwine.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3142 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_foodnetwork.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2273 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_foodrepublic.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2911 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_forksoverknives.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2631 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_franzoesischkochen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2252 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_fredriksfikaallas.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1950 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_geniuskitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4699 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_giallozafferano.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2224 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_gimmesomeoven.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2345 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_globo.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3153 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_gonnawantseconds.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2864 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_gousto.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4361 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_goustojson.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3004 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_greatbritishchefs.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3049 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_halfbakedharvest.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2691 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_handletheheat.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5547 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_hassanchef.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2217 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_headbangerskitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2242 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_heb.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2101 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_heinzbrasil.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3810 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_hellofresh.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3777 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_hellofresh_adhoc.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3945 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_homechef.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3153 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_hostthetoast.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2536 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_hundredandonecookbooks.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3404 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_ica.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2414 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_ig.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3193 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_imworthy.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3583 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_indianhealthyrecipes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3426 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_innit.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1978 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_inspiralized.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2998 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_jamieoliver.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2485 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_jimcooksfoodgood.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2916 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_joyfoodsunshine.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3400 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_justataste.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2420 2021-08-25 16:01:34.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_justbento.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4699 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_justonecookbook.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3175 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_kennymcgovern.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     6628 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_kingarthur.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3442 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_kitchenstories.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4747 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_kochbar.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2466 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_koket.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3720 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_kptncook.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2347 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_kuchniadomowa.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2130 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_kwestiasmaku.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3402 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_latelierderoxane.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2371 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_leanandgreenrecipes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3584 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_lecker_1.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3817 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_lecker_2.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2421 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_lecremedelacrumb.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2249 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_lekkerensimpel.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3117 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_littlespicejar.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2551 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_livelytable.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1945 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_lovingitvegan.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5517 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_maangchi.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3597 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_madensverden.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5368 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_madewithlau.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5727 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_marleyspoon.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2576 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_marmiton.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2855 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_marthastewart.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3728 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_matprat.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3913 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_meljoulwan.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2989 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_melskitchencafe.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2405 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_mindmegette.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2900 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_minimalistbaker.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2638 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_misya.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3354 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_mobkitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2432 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_momswithcrockpots.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2293 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_monsieurcuisine.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2758 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_motherthyme.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3059 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_mybakingaddiction.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2466 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_mykitchen101.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2783 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_mykitchen101en.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2648 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_myrecipes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2677 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_nhshealthierfamilies.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     9685 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_nih.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3140 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_nourishedbynutrition.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2018 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_nutritionbynathalie.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5859 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_nytimes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4528 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_ohsheglows.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2937 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_omnivorescookbook.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2390 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_onehundredonecookbooks.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2368 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_owenhan.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3476 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_paleorunningmomma.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2191 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_panelinha_1.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3553 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_panelinha_2.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2730 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_paninihappy.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2458 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_pingodoce.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4541 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_popsugar.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3597 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_practicalselfreliance.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2182 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_primaledgehealth.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1968 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_przepisy.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1796 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_purelypope.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2178 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_purplecarrot.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2226 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_rachlmansfield.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3850 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_rainbowplantlife.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2809 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_realfoodtesco.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3588 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_realsimple.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2674 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_recipetineats.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3210 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_redhousespice.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2283 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_reishunger_1.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5284 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_reishunger_2.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2427 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_rezeptwelt.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2202 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_rosannapansino.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5921 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_sallysbakingaddiction.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5314 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_saveur.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1491 2021-08-25 16:01:34.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_schemaorg.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5638 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_seriouseats.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4081 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_simpleveganista.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4099 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_simplycookit.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2386 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_simplyquinoa.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3275 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_simplyrecipes.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2634 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_simplywhisked.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2544 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_skinnytaste.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3966 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_smulweb.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3076 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_southerncastiron.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5082 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_southernliving.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2383 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_spendwithpennies.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2679 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_springlane.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3508 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_steamykitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2729 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_streetkitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3690 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_sunbasket.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2981 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_sundpaabudget.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2526 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_sweetcsdesigns.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4470 2021-08-25 16:01:34.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_sweetpeasandsaffron.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3137 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_tasteofhome.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3199 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_tastesbetterfromscratch.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2135 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_tastesoflizzyt.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5066 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_tasty.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2558 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_tastykitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     7848 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_theclevercarrot.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3739 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_thehappyfoodie_1.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4155 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_thehappyfoodie_2.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2157 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_thekitchenmagpie.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3979 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_thekitchn.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2775 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_thenutritiouskitchen.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3435 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_thepioneerwoman.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3045 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_thespruceeats.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3049 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_thevintagemixer.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1808 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_thewoksoflife.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3156 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_timesofindia.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3258 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_tineno.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2274 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_tudogostoso.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3083 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_twopeasandtheirpod.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3706 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_usdamyplate.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2736 2022-04-06 21:27:02.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_valdemarsro.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     7831 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_vanillaandbean.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3369 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_vegolosi.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4037 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_vegrecipesofindia.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3148 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_watchwhatueat.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3322 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_weightwatchers.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3963 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_weightwatchers_2.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3737 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_weightwatcherspublic.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2604 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_whatsgabycooking.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2551 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_wholefoods.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2486 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_wikibooks.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4827 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_wild_mode.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3402 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_woolworths.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3000 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_woop.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3481 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_yemek.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1934 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_yummly.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2421 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_zeitwochenmarkt.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     2779 2022-11-30 23:21:25.000000 recipe_scrapers_ap_fork-14.24.2/tests/test_zenbelly.py
```

### Comparing `recipe_scrapers_ap_fork-14.24.1/LICENSE` & `recipe_scrapers_ap_fork-14.24.2/LICENSE`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/PKG-INFO` & `recipe_scrapers_ap_fork-14.24.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recipe_scrapers_ap_fork
-Version: 14.24.1
+Version: 14.24.2
 Summary: Python package, scraping recipes from all over the internet
 Author-email: Hristo Harsev <r+pypi@hharsev.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/hhursev/recipe-scrapers/
 Keywords: python,recipes,scraper,harvest,recipe-scraper,recipe-scrapers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `recipe_scrapers_ap_fork-14.24.1/README.rst` & `recipe_scrapers_ap_fork-14.24.2/README.rst`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/pyproject.toml` & `recipe_scrapers_ap_fork-14.24.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/__init__.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/__init__.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/_abstract.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/_abstract.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,23 +28,24 @@
         ] = None,  # allows us to specify optional proxy server
         timeout: Optional[
             Union[float, Tuple[float, float], Tuple[float, None]]
         ] = None,  # allows us to specify optional timeout for request
         wild_mode: Optional[bool] = False,
         html: Union[str, bytes, None] = None,
         allow_redirects: Optional[bool] = True,
+        headers: Dict[str, str] = None
     ):
         if html:
             self.page_data = html
             self.url = url
         else:
             assert url is not None, "url required for fetching recipe data"
             self.resp = requests.get(
                 url,
-                headers=HEADERS,
+                headers=headers if headers is not None else HEADERS,
                 proxies=proxies,
                 timeout=timeout,
                 allow_redirects=allow_redirects,
             )
             self.page_data = self.resp.content
             self.url = self.resp.url
```

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/_exceptions.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/_exceptions.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/_factory.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/_factory.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/_schemaorg.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/_schemaorg.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/_utils.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/_utils.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/abril.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/abril.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/acouplecooks.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/acouplecooks.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/afghankitchenrecipes.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/afghankitchenrecipes.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/akispetretzikis.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/akispetretzikis.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/albertheijn.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/albertheijn.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/allrecipes.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/allrecipes.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/alltomat.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/alltomat.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/altonbrown.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/altonbrown.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/amazingribs.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/amazingribs.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/ambitiouskitchen.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/ambitiouskitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/archanaskitchen.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/archanaskitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/arla.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/arla.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/atelierdeschefs.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/atelierdeschefs.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/averiecooks.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/averiecooks.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bakingmischeif.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bakingmischeif.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bakingsense.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bakingsense.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bbcfood.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bbcfood.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bbcgoodfood.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bbcgoodfood.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bettybossi.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bettybossi.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bettycrocker.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bettycrocker.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bigoven.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bigoven.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/blueapron.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/blueapron.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bodybuilding.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bodybuilding.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/bowlofdelicious.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/bowlofdelicious.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/budgetbytes.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/budgetbytes.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/castironketo.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/castironketo.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cdkitchen.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cdkitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/chefkoch.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/chefkoch.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/closetcooking.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/closetcooking.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/comidinhasdochef.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/comidinhasdochef.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cookieandkate.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cookieandkate.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cookingcircle.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cookingcircle.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cookinglight.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cookinglight.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cookpad.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cookpad.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cookstr.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cookstr.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/coop.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/coop.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/copykat.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/copykat.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cuisineaz.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cuisineaz.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/cybercook.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/cybercook.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/davidlebovitz.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/davidlebovitz.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/delish.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/delish.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/ditchthecarbs.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/ditchthecarbs.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/domesticateme.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/domesticateme.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/downshiftology.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/downshiftology.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/dr.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/dr.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/eatingbirdfood.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/eatingbirdfood.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/eatingwell.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/eatingwell.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/eatsmarter.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/eatsmarter.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/eatwhattonight.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/eatwhattonight.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/emmikochteinfach.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/emmikochteinfach.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/epicurious.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/epicurious.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/ethanchlebowski.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/ethanchlebowski.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/farmhousedelivery.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/farmhousedelivery.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/fifteenspatulas.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/fifteenspatulas.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/finedininglovers.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/finedininglovers.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/fitmencook.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/fitmencook.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/food.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/food.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/food52.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/food52.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/foodandwine.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/foodandwine.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/foodnetwork.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/foodnetwork.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/foodrepublic.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/foodrepublic.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/forksoverknives.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/forksoverknives.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/franzoesischkochen.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/franzoesischkochen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/fredriksfikaallas.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/fredriksfikaallas.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/g750g.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/g750g.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/geniuskitchen.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/geniuskitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/giallozafferano.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/giallozafferano.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/gimmesomeoven.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/gimmesomeoven.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/globo.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/globo.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/gonnawantseconds.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/gonnawantseconds.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/gousto.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/gousto.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/goustojson.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/goustojson.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/greatbritishchefs.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/greatbritishchefs.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/halfbakedharvest.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/halfbakedharvest.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/handletheheat.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/handletheheat.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/hassanchef.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/hassanchef.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/headbangerskitchen.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/headbangerskitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/heb.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/heb.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/heinzbrasil.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/heinzbrasil.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/hellofresh.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/hellofresh.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/homechef.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/homechef.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/hostthetoast.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/hostthetoast.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/hundredandonecookbooks.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/hundredandonecookbooks.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/ica.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/ica.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/ig.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/ig.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/imworthy.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/imworthy.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/indianhealthyrecipes.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/indianhealthyrecipes.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/innit.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/innit.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/inspiralized.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/inspiralized.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/jamieoliver.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/jamieoliver.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/jimcooksfoodgood.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/jimcooksfoodgood.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/joyfoodsunshine.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/joyfoodsunshine.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/justataste.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/justataste.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/justbento.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/justbento.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/justonecookbook.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/justonecookbook.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/kennymcgovern.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/kennymcgovern.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/kingarthur.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/kingarthur.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/kitchenstories.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/kitchenstories.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/kochbar.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/kochbar.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/koket.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/koket.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/kptncook.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/kptncook.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/kuchniadomowa.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/kuchniadomowa.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/kwestiasmaku.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/kwestiasmaku.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/latelierderoxane.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/latelierderoxane.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/leanandgreenrecipes.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/leanandgreenrecipes.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/lecker.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/lecker.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/lecremedelacrumb.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/lecremedelacrumb.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/lekkerensimpel.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/lekkerensimpel.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/littlespicejar.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/littlespicejar.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/livelytable.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/livelytable.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/lovingitvegan.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/lovingitvegan.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/maangchi.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/maangchi.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/madensverden.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/madensverden.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/madewithlau.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/madewithlau.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/marleyspoon.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/marleyspoon.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/marmiton.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/marmiton.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/marthastewart.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/marthastewart.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/matprat.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/matprat.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/meljoulwan.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/meljoulwan.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/melskitchencafe.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/melskitchencafe.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/mindmegette.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/mindmegette.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/minimalistbaker.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/minimalistbaker.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/misya.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/misya.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/mobkitchen.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/mobkitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/momswithcrockpots.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/momswithcrockpots.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/monsieurcuisine.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/monsieurcuisine.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/motherthyme.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/motherthyme.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/mybakingaddiction.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/mybakingaddiction.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/mykitchen101.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/mykitchen101.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/mykitchen101en.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/mykitchen101en.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/myrecipes.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/myrecipes.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/nhshealthierfamilies.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/nhshealthierfamilies.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/nihhealthyeating.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/nihhealthyeating.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/nourishedbynutrition.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/nourishedbynutrition.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/nutritionbynathalie.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/nutritionbynathalie.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/nytimes.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/nytimes.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/ohsheglows.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/ohsheglows.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/omnivorescookbook.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/omnivorescookbook.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/onehundredonecookbooks.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/onehundredonecookbooks.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/owenhan.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/owenhan.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/paleorunningmomma.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/paleorunningmomma.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/panelinha.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/panelinha.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/paninihappy.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/paninihappy.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/pingodoce.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/pingodoce.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/_interface.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/_interface.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/exception_handling.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/exception_handling.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/html_tags_stripper.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/html_tags_stripper.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/normalize_string.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/normalize_string.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/opengraph_image_fetch.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/opengraph_image_fetch.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/schemaorg_fill.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/schemaorg_fill.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/plugins/template.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/plugins/template.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/popsugar.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/popsugar.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/practicalselfreliance.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/practicalselfreliance.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/primaledgehealth.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/primaledgehealth.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/przepisy.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/przepisy.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/purelypope.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/purelypope.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/purplecarrot.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/purplecarrot.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/rachlmansfield.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/rachlmansfield.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/rainbowplantlife.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/rainbowplantlife.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/realfoodtesco.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/realfoodtesco.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/realsimple.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/realsimple.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/recipetineats.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/recipetineats.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/redhousespice.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/redhousespice.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/reishunger.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/reishunger.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/rezeptwelt.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/rezeptwelt.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/rosannapansino.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/rosannapansino.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/sallysbakingaddiction.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/sallysbakingaddiction.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/saveur.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/saveur.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/seriouseats.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/seriouseats.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/settings/__init__.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/settings/default.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/settings/default.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/simpleveganista.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/simpleveganista.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/simplycookit.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/simplycookit.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/simplyquinoa.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/simplyquinoa.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/simplyrecipes.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/simplyrecipes.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/simplywhisked.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/simplywhisked.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/skinnytaste.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/skinnytaste.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/smulweb.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/smulweb.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/southerncastiron.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/southerncastiron.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/southernliving.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/southernliving.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/spendwithpennies.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/spendwithpennies.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/springlane.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/springlane.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/steamykitchen.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/steamykitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/streetkitchen.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/streetkitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/sunbasket.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/sunbasket.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/sundpaabudget.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/sundpaabudget.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/sweetcsdesigns.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/sweetcsdesigns.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/sweetpeasandsaffron.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/sweetpeasandsaffron.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/tasteofhome.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/tasteofhome.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/tastesbetterfromscratch.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/tastesbetterfromscratch.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/tastesoflizzyt.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/tastesoflizzyt.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/tasty.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/tasty.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/tastykitchen.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/tastykitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/theclevercarrot.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/theclevercarrot.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thehappyfoodie.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thehappyfoodie.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thekitchenmagpie.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thekitchenmagpie.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thekitchn.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thekitchn.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thenutritiouskitchen.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thenutritiouskitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thepioneerwoman.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thepioneerwoman.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thespruceeats.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thespruceeats.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thevintagemixer.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thevintagemixer.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/thewoksoflife.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/thewoksoflife.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/timesofindia.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/timesofindia.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/tineno.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/tineno.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/tudogostoso.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/tudogostoso.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/twopeasandtheirpod.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/twopeasandtheirpod.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/usdamyplate.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/usdamyplate.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/valdemarsro.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/valdemarsro.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/vanillaandbean.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/vanillaandbean.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/vegolosi.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/vegolosi.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/vegrecipesofindia.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/vegrecipesofindia.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/watchwhatueat.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/watchwhatueat.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/weightwatchers.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/weightwatchers.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/weightwatcherspublic.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/weightwatcherspublic.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/whatsgabycooking.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/whatsgabycooking.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/wholefoods.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/wholefoods.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/wikicookbook.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/wikicookbook.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/woolworths.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/woolworths.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/woop.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/woop.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/yemek.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/yemek.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/yummly.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/yummly.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/zeitwochenmarkt.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/zeitwochenmarkt.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers/zenbelly.py` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers/zenbelly.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers_ap_fork-14.24.1/recipe_scrapers_ap_fork.egg-info/PKG-INFO` & `recipe_scrapers_ap_fork-14.24.2/recipe_scrapers_ap_fork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recipe-scrapers-ap-fork
-Version: 14.24.1
+Version: 14.24.2
 Summary: Python package, scraping recipes from all over the internet
 Author-email: Hristo Harsev <r+pypi@hharsev.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/hhursev/recipe-scrapers/
 Keywords: python,recipes,scraper,harvest,recipe-scraper,recipe-scrapers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

