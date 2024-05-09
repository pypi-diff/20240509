# Comparing `tmp/iphone_backup_decrypt-0.6.0.tar.gz` & `tmp/iphone_backup_decrypt-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iphone_backup_decrypt-0.6.0.tar", last modified: Sat Feb 10 11:46:12 2024, max compression
+gzip compressed data, was "iphone_backup_decrypt-0.7.0.tar", last modified: Thu May  9 19:21:21 2024, max compression
```

## Comparing `iphone_backup_decrypt-0.6.0.tar` & `iphone_backup_decrypt-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-02-10 11:46:12.364445 iphone_backup_decrypt-0.6.0/
--rw-rw-rw-   0        0        0     2777 2019-11-13 20:01:32.000000 iphone_backup_decrypt-0.6.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4983 2024-02-10 11:46:12.363446 iphone_backup_decrypt-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     4347 2024-02-06 19:55:36.000000 iphone_backup_decrypt-0.6.0/README.md
--rw-rw-rw-   0        0        0      745 2024-02-10 11:44:29.000000 iphone_backup_decrypt-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-10 11:46:12.365444 iphone_backup_decrypt-0.6.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-10 11:46:12.299484 iphone_backup_decrypt-0.6.0/src/
-drwxrwxrwx   0        0        0        0 2024-02-10 11:46:12.324470 iphone_backup_decrypt-0.6.0/src/iphone_backup_decrypt/
--rw-rw-rw-   0        0        0      199 2024-02-03 22:46:28.000000 iphone_backup_decrypt-0.6.0/src/iphone_backup_decrypt/__init__.py
--rw-rw-rw-   0        0        0     4911 2024-02-06 19:55:41.000000 iphone_backup_decrypt-0.6.0/src/iphone_backup_decrypt/google_iphone_dataprotection.py
--rw-rw-rw-   0        0        0    22893 2024-02-10 11:36:25.000000 iphone_backup_decrypt-0.6.0/src/iphone_backup_decrypt/iphone_backup.py
-drwxrwxrwx   0        0        0        0 2024-02-10 11:46:12.361446 iphone_backup_decrypt-0.6.0/src/iphone_backup_decrypt.egg-info/
--rw-rw-rw-   0        0        0     4983 2024-02-10 11:46:12.000000 iphone_backup_decrypt-0.6.0/src/iphone_backup_decrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2024-02-10 11:46:12.000000 iphone_backup_decrypt-0.6.0/src/iphone_backup_decrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-10 11:46:12.000000 iphone_backup_decrypt-0.6.0/src/iphone_backup_decrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-02-10 11:46:12.000000 iphone_backup_decrypt-0.6.0/src/iphone_backup_decrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-02-10 11:46:12.000000 iphone_backup_decrypt-0.6.0/src/iphone_backup_decrypt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 19:21:21.355233 iphone_backup_decrypt-0.7.0/
+-rw-rw-rw-   0        0        0     2777 2019-11-13 20:01:32.000000 iphone_backup_decrypt-0.7.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5307 2024-05-09 19:21:21.353279 iphone_backup_decrypt-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4671 2024-05-09 19:07:00.000000 iphone_backup_decrypt-0.7.0/README.md
+-rw-rw-rw-   0        0        0      745 2024-05-09 19:11:00.000000 iphone_backup_decrypt-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 19:21:21.355233 iphone_backup_decrypt-0.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 19:21:21.285915 iphone_backup_decrypt-0.7.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 19:21:21.316181 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/
+-rw-rw-rw-   0        0        0      218 2024-05-09 19:06:29.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/__init__.py
+-rw-rw-rw-   0        0        0     4911 2024-05-06 13:05:23.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/google_iphone_dataprotection.py
+-rw-rw-rw-   0        0        0    20354 2024-05-09 19:19:21.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/iphone_backup.py
+-rw-rw-rw-   0        0        0     6470 2024-05-09 19:06:29.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:21:21.351326 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt.egg-info/
+-rw-rw-rw-   0        0        0     5307 2024-05-09 19:21:21.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2024-05-09 19:21:21.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 19:21:21.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-09 19:21:21.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-09 19:21:21.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt.egg-info/top_level.txt
```

### Comparing `iphone_backup_decrypt-0.6.0/LICENSE.txt` & `iphone_backup_decrypt-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iphone_backup_decrypt-0.6.0/PKG-INFO` & `iphone_backup_decrypt-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphone_backup_decrypt
-Version: 0.6.0
+Version: 0.7.0
 Summary: Decrypt and extract files from an iOS13+ encrypted local backup.
 Author: James Sharkey
 Project-URL: Homepage, https://github.com/jsharkey13/iphone_backup_decrypt
 Keywords: iPhone,backup,forensics,iOS,WhatsApp,decryption,iOS backup,iTunes Backup
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.8
@@ -12,16 +12,16 @@
 License-File: LICENSE.txt
 Requires-Dist: pycryptodome>=3.20.0
 Provides-Extra: fastpbkdf2
 Requires-Dist: fastpbkdf2>=0.2; extra == "fastpbkdf2"
 
 # iphone-backup-decrypt
 
-Decrypt an encrypted, local (i.e. non-iCloud), iPhone backup created from iOS13 or newer.
-This code is mainly a [wrapper for this StackOverflow answer](https://stackoverflow.com/a/13793043),
+Decrypt an encrypted, local iPhone backup created from iOS13 or newer.
+This code [was based on this StackOverflow answer](https://stackoverflow.com/a/13793043),
 itself based on the [iphone-dataprotection](https://code.google.com/p/iphone-dataprotection/) code.
 
 ## Install
 
 Requires [Python 3.8](https://www.python.org/) or higher.
 
 The backup decryption keys are protected using 10 million rounds of PBKDF2 with SHA256, then 10 thousand further iterations of PBKDF2 with SHA-1.
@@ -56,25 +56,30 @@
 After creating the class, use the `EncryptedBackup.save_manifest_file(...)` method to store a decrypted version.
 
 A minimal example to decrypt and extract some files might look like:
 ```python
 from iphone_backup_decrypt import EncryptedBackup, RelativePath, MatchFiles
 
 passphrase = "..."  # Or load passphrase more securely from stdin, or a file, etc.
-backup_path = "%AppData%\\Apple Computer\\MobileSync\\Backup\\[device-specific-hash]"
+backup_path = "%AppData%/Apple Computer/MobileSync/Backup/[device-specific-hash]"
+# Or MacOS: "/Users/[user]/Library/Application Support/MobileSync/Backup/[device-hash]"
 
 backup = EncryptedBackup(backup_directory=backup_path, passphrase=passphrase)
 
 # Extract the call history SQLite database:
 backup.extract_file(relative_path=RelativePath.CALL_HISTORY, 
                     output_filename="./output/call_history.sqlite")
 
 # Extract the camera roll, using MatchFiles for combined path and domain matching:
 backup.extract_files(**MatchFiles.CAMERA_ROLL, output_folder="./output/camera_roll")
 
+# Extract any iCloud camera roll images on the device (may include thumbnails for some
+# but not all images offloaded to the cloud, and have duplicates from the camera roll):
+backup.extract_files(**MatchFiles.ICLOUD_PHOTOS, output_folder="./output/icloud_photos")
+
 # Extract WhatsApp SQLite database and attachments:
 backup.extract_file(relative_path=RelativePath.WHATSAPP_MESSAGES,
                     output_filename="./output/whatsapp.sqlite")
 backup.extract_files(**MatchFiles.WHATSAPP_ATTACHMENTS,
                      output_folder="./output/whatsapp", preserve_folders=False)
 
 # Extract Strava workouts:
```

### Comparing `iphone_backup_decrypt-0.6.0/README.md` & `iphone_backup_decrypt-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # iphone-backup-decrypt
 
-Decrypt an encrypted, local (i.e. non-iCloud), iPhone backup created from iOS13 or newer.
-This code is mainly a [wrapper for this StackOverflow answer](https://stackoverflow.com/a/13793043),
+Decrypt an encrypted, local iPhone backup created from iOS13 or newer.
+This code [was based on this StackOverflow answer](https://stackoverflow.com/a/13793043),
 itself based on the [iphone-dataprotection](https://code.google.com/p/iphone-dataprotection/) code.
 
 ## Install
 
 Requires [Python 3.8](https://www.python.org/) or higher.
 
 The backup decryption keys are protected using 10 million rounds of PBKDF2 with SHA256, then 10 thousand further iterations of PBKDF2 with SHA-1.
@@ -40,25 +40,30 @@
 After creating the class, use the `EncryptedBackup.save_manifest_file(...)` method to store a decrypted version.
 
 A minimal example to decrypt and extract some files might look like:
 ```python
 from iphone_backup_decrypt import EncryptedBackup, RelativePath, MatchFiles
 
 passphrase = "..."  # Or load passphrase more securely from stdin, or a file, etc.
-backup_path = "%AppData%\\Apple Computer\\MobileSync\\Backup\\[device-specific-hash]"
+backup_path = "%AppData%/Apple Computer/MobileSync/Backup/[device-specific-hash]"
+# Or MacOS: "/Users/[user]/Library/Application Support/MobileSync/Backup/[device-hash]"
 
 backup = EncryptedBackup(backup_directory=backup_path, passphrase=passphrase)
 
 # Extract the call history SQLite database:
 backup.extract_file(relative_path=RelativePath.CALL_HISTORY, 
                     output_filename="./output/call_history.sqlite")
 
 # Extract the camera roll, using MatchFiles for combined path and domain matching:
 backup.extract_files(**MatchFiles.CAMERA_ROLL, output_folder="./output/camera_roll")
 
+# Extract any iCloud camera roll images on the device (may include thumbnails for some
+# but not all images offloaded to the cloud, and have duplicates from the camera roll):
+backup.extract_files(**MatchFiles.ICLOUD_PHOTOS, output_folder="./output/icloud_photos")
+
 # Extract WhatsApp SQLite database and attachments:
 backup.extract_file(relative_path=RelativePath.WHATSAPP_MESSAGES,
                     output_filename="./output/whatsapp.sqlite")
 backup.extract_files(**MatchFiles.WHATSAPP_ATTACHMENTS,
                      output_folder="./output/whatsapp", preserve_folders=False)
 
 # Extract Strava workouts:
```

### Comparing `iphone_backup_decrypt-0.6.0/pyproject.toml` & `iphone_backup_decrypt-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "iphone_backup_decrypt"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
   { name="James Sharkey" },
 ]
 description = "Decrypt and extract files from an iOS13+ encrypted local backup."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `iphone_backup_decrypt-0.6.0/src/iphone_backup_decrypt/google_iphone_dataprotection.py` & `iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/google_iphone_dataprotection.py`

 * *Files identical despite different names*

### Comparing `iphone_backup_decrypt-0.6.0/src/iphone_backup_decrypt/iphone_backup.py` & `iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/iphone_backup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,83 +1,18 @@
 import os.path
 import plistlib
 import shutil
 import sqlite3
 import struct
 import tempfile
+from contextlib import contextmanager
 
-from . import google_iphone_dataprotection
+from . import google_iphone_dataprotection, utils
 
-__all__ = ["EncryptedBackup", "RelativePath", "RelativePathsLike", "DomainLike", "MatchFiles"]
-
-
-class RelativePath:
-    """Relative paths for commonly accessed files."""
-
-    # Standard iOS file locations:
-    ADDRESS_BOOK = "Library/AddressBook/AddressBook.sqlitedb"
-    TEXT_MESSAGES = "Library/SMS/sms.db"
-    CALL_HISTORY = "Library/CallHistoryDB/CallHistory.storedata"
-    NOTES = "Library/Notes/notes.sqlite"
-    CALENDARS = "Library/Calendar/Calendar.sqlitedb"
-    HEALTH = "Health/healthdb.sqlite"
-    HEALTH_SECURE = "Health/healthdb_secure.sqlite"
-    SAFARI_HISTORY = "Library/Safari/History.db"
-    SAFARI_BOOKMARKS = "Library/Safari/Bookmarks.db"
-
-    # Very common external files:
-    WHATSAPP_MESSAGES = "ChatStorage.sqlite"
-    WHATSAPP_CONTACTS = "ContactsV2.sqlite"
-
-
-class RelativePathsLike:
-    """Relative path wildcards for commonly accessed groups of files."""
-
-    # A wildcard, use at own risk:
-    ALL_FILES = "%"
-
-    # Standard iOS file locations:
-    CAMERA_ROLL = "Media/DCIM/%APPLE/IMG%.%"
-    SMS_ATTACHMENTS = "Library/SMS/Attachments/%.%"
-    VOICEMAILS = "Library/Voicemail/%.amr"
-    VOICE_RECORDINGS = "Library/Recordings/%"
-    ICLOUD_LOCAL_FILES = "Library/Mobile Documents/com~apple~CloudDocs/%"
-
-    # WhatsApp makes .thumb files for every media item, so maybe specifically extract JPG or MP4:
-    WHATSAPP_ATTACHED_IMAGES = "Message/Media/%.jpg"
-    WHATSAPP_ATTACHED_VIDEOS = "Message/Media/%.mp4"
-    # But allow full export if desired:
-    WHATSAPP_ATTACHMENTS = "Message/Media/%.%"
-
-
-class DomainLike:
-    """Domain wildcards for commonly accessed apps and services."""
-
-    # Standard iOS domains:
-    HOME_DOMAIN = "HomeDomain"
-    CAMERA_ROLL = "CameraRollDomain"
-    FILES_ON_IPHONE = "AppDomainGroup-group.com.apple.FileProvider.LocalStorage"
-
-    # Third party apps:
-    WHATSAPP = "%net.whatsapp.%"  # WhatsApp has several domains, all with this common section.
-
-
-class MatchFiles:
-    """Paired relative paths and domains for more complex matching.
-
-       Use items from this class with EncryptedBackup.extract_files, e.g:
-           backup.extract_files(**MatchFiles.CAMERA_ROLL, output_folder="./output")
-    """
-
-    CAMERA_ROLL = {"relative_paths_like": RelativePathsLike.CAMERA_ROLL, "domain_like": DomainLike.CAMERA_ROLL}
-    CHROME_DOWNLOADS = {"relative_paths_like": "Documents/%", "domain_like": "AppDomain-com.google.chrome.ios"}
-    STRAVA_WORKOUTS = {"relative_paths_like": "Documents/%.fit", "domain_like": "AppDomain-com.strava.stravaride"}
-    WHATSAPP_ATTACHMENTS = {"relative_paths_like": RelativePathsLike.WHATSAPP_ATTACHMENTS,
-                            "domain_like": DomainLike.WHATSAPP}
-    WHATSAPP_CONTACT_PHOTOS = {"relative_paths_like": "Media/Profile/%.jpg", "domain_like": DomainLike.WHATSAPP}
+__all__ = ["EncryptedBackup"]
 
 
 # Based on https://stackoverflow.com/questions/1498342/how-to-decrypt-an-encrypted-apple-itunes-iphone-backup
 # and code sample provided by @andrewdotn in this answer: https://stackoverflow.com/a/13793043
 class EncryptedBackup:
 
     def __init__(self, *, backup_directory, passphrase):
@@ -102,15 +37,15 @@
             The passphrase chosen in iTunes when first choosing to encrypt backups.
             If it requires an encoding other than ASCII or UTF-8, a bytes object must be provided.
         """
         # Public state:
         self.decrypted = False
         # Keep track of the backup directory, and more dangerously, keep the backup passphrase as bytes until used:
         self._backup_directory = os.path.expandvars(backup_directory)
-        self._passphrase = passphrase if type(passphrase) is bytes else passphrase.encode("utf-8")
+        self._passphrase = passphrase if isinstance(passphrase, bytes) else passphrase.encode("utf-8")
         # Internals for unlocking the Keybag:
         self._manifest_plist_path = os.path.join(self._backup_directory, 'Manifest.plist')
         self._manifest_plist = None
         self._manifest_db_path = os.path.join(self._backup_directory, 'Manifest.db')
         self._keybag = None
         self._unlocked = False
         # We need a temporary file for the decrypted database, because SQLite can't open bytes in memory as a database:
@@ -125,15 +60,15 @@
     def _cleanup(self):
         try:
             if self._temp_manifest_db_conn is not None:
                 self._temp_manifest_db_conn.close()
             shutil.rmtree(self._temporary_folder)
         except Exception:
             print("WARN: Cleanup failed. You may want to delete the decrypted temporary file found at:")
-            print("    '{}'".format(self._temp_decrypted_manifest_db_path))
+            print(f"    '{self._temp_decrypted_manifest_db_path}'")
             raise
 
     def _read_and_unlock_keybag(self):
         if self._unlocked:
             return self._unlocked
         # Open the Manifest.plist file to access the Keybag:
         with open(self._manifest_plist_path, 'rb') as infile:
@@ -179,40 +114,72 @@
         # Write the decrypted Manifest.db temporarily to disk:
         with open(self._temp_decrypted_manifest_db_path, 'wb') as decrypted_db_filehandle:
             decrypted_db_filehandle.write(decrypted_data)
         # Open the temporary database to verify decryption success:
         if not self._open_temp_database():
             raise ConnectionError("Manifest.db file does not seem to be the right format!")
 
-    def _decrypt_inner_file(self, *, file_id, file_bplist, if_modified_since=None):
+    def _file_metadata_from_manifest(self, relative_path, domain_like=None):
+        # Check arguments:
+        if relative_path is None:
+            raise ValueError("A relative_path must be provided!")
+        # Ensure that we've initialised everything:
+        if self._temp_manifest_db_conn is None:
+            self._decrypt_manifest_db_file()
+        # Use Manifest.db to find the on-disk filename and file metadata, including the keys, for the file.
+        # The metadata is contained in the 'file' column, as a binary PList file:
+        try:
+            cur = self._temp_manifest_db_conn.cursor()
+            if domain_like is None:
+                domain_like = "%"
+            query = """
+                SELECT fileID, file
+                FROM Files
+                WHERE relativePath = ?
+                AND domain LIKE ?
+                AND flags=1
+                ORDER BY domain, relativePath
+                LIMIT 1;
+            """
+            cur.execute(query, (relative_path, domain_like))
+            result = cur.fetchone()
+        except sqlite3.Error as e:
+            raise RuntimeError("Error querying Manifest database!") from e
+        if not result:
+            raise FileNotFoundError
+        file_id, file_bplist = result
+        return file_id, file_bplist
+
+    def _decrypt_inner_file(self, *, file_id, file_bplist):
         # Ensure we've already unlocked the Keybag:
         self._read_and_unlock_keybag()
-        # Read the plist data and extract file metadata:
-        plist = plistlib.loads(file_bplist)
-        file_data = plist['$objects'][plist['$top']['root'].data]
-        file_mtime = file_data.get("LastModified")
-        # Was the file modified since the time requested?
-        if if_modified_since and file_mtime <= if_modified_since:
-            # Skip decryption, since file is unchanged.
-            return None, file_mtime
+        # Read the plist data:
+        file_plist = utils.FilePlist(file_bplist)
         # Extract the decryption key from the PList data:
-        protection_class = file_data['ProtectionClass']
-        if "EncryptionKey" not in file_data:
+        if file_plist.encryption_key is None:
             raise ValueError("Path is not an encrypted file.")  # File is not encrypted; either a directory or empty.
-        encryption_key = plist['$objects'][file_data['EncryptionKey'].data]['NS.data'][4:]
-        inner_key = self._keybag.unwrapKeyForClass(protection_class, encryption_key)
+        inner_key = self._keybag.unwrapKeyForClass(file_plist.protection_class, file_plist.encryption_key)
         # Find the encrypted version of the file on disk and decrypt it:
         filename_in_backup = os.path.join(self._backup_directory, file_id[:2], file_id)
         with open(filename_in_backup, 'rb') as encrypted_file_filehandle:
             encrypted_data = encrypted_file_filehandle.read()
         # Decrypt the file contents:
         decrypted_data = google_iphone_dataprotection.AESdecryptCBC(encrypted_data, inner_key)
         # Remove any padding introduced by the CBC encryption:
         file_bytes = google_iphone_dataprotection.removePadding(decrypted_data)
-        return file_bytes, file_mtime
+        # Check the data is as expected and return it:
+        if len(file_bytes) != file_plist.filesize:
+            raise AssertionError(f"Expected file size of {file_plist.filesize} bytes, decrypted {len(file_bytes)} bytes!")
+        return file_bytes
+
+    def _decrypt_file_to_disk(self, *, file_id, key, file_plist, output_filepath):
+        # Find the name of the file on disk:
+        filename_in_backup = os.path.join(self._backup_directory, file_id[:2], file_id)
+        # Decrypt it to the output location:
+        utils.aes_decrypt_chunked(in_filename=filename_in_backup, out_filepath=output_filepath, key=key, file_plist=file_plist)
 
     def test_decryption(self):
         """Validate that the backup can be decrypted successfully."""
         # Ensure that we've initialised everything:
         if self._temp_manifest_db_conn is None:
             self._decrypt_manifest_db_file()
         return True
@@ -223,63 +190,61 @@
         self._decrypt_manifest_db_file()
         # Copy the decrypted file to the output:
         output_directory = os.path.dirname(output_filename)
         if output_directory:
             os.makedirs(output_directory, exist_ok=True)
         shutil.copy(self._temp_decrypted_manifest_db_path, output_filename)
 
-    def _file_as_bytes(self, relative_path, domain_like=None):
-        # Check arguments:
-        if relative_path is None:
-            raise ValueError("A relative_path must be provided!")
-        # Ensure that we've initialised everything:
-        if self._temp_manifest_db_conn is None:
-            self._decrypt_manifest_db_file()
-        # Use Manifest.db to find the on-disk filename and file metadata, including the keys, for the file.
-        # The metadata is contained in the 'file' column, as a binary PList file:
-        try:
-            cur = self._temp_manifest_db_conn.cursor()
-            if domain_like is None:
-                domain_like = "%"
-            query = """
-                SELECT fileID, file
-                FROM Files
-                WHERE relativePath = ?
-                AND domain LIKE ?
-                AND flags=1
-                ORDER BY domain, relativePath
-                LIMIT 1;
-            """
-            cur.execute(query, (relative_path, domain_like))
-            result = cur.fetchone()
-        except sqlite3.Error as e:
-            raise RuntimeError("Error querying Manifest database!") from e
-        if not result:
-            raise FileNotFoundError
-        file_id, file_bplist = result
-        # Decrypt the requested file:
-        return self._decrypt_inner_file(file_id=file_id, file_bplist=file_bplist)
+    @contextmanager
+    def manifest_db_cursor(self):
+        """Get a cursor into the temporary copy of the Manifest file.
+
+        The cursor is intended only for read-only querying, since the
+        underlying connection object is not returned and will not
+        commit the changes by default.
+
+        Example usage:
+
+        with backup.manifest_db_cursor() as cur:
+            cur.execute("SELECT count(*) FROM Files;")
+            print(cur.fetchone()[0])
+        """
+        # Ensure that we've decrypted the manifest file:
+        self._decrypt_manifest_db_file()
+        # Get and yield a cursor:
+        temp_cur = self._temp_manifest_db_conn.cursor()
+        yield temp_cur
+        # Close it when we're done:
+        temp_cur.close()
 
     def extract_file_as_bytes(self, relative_path, *, domain_like=None):
         """
         Decrypt a single named file and return the bytes.
 
+        This method decrypts the file contents in-memory, and can require up to 3x the file size of free
+        memory to function. If you see errors extracting the bytes of very large files, try using extract_file
+        or extract_files to write the output to disk to avoid storing the encrypted and decrypted versions of
+        the file in-memory at the same time.
+
         :param relative_path:
             The iOS 'relativePath' of the file to be decrypted. Common relative paths are provided by the
             'RelativePath' class, otherwise these can be found by opening the decrypted Manifest.db file
             and examining the Files table.
         :param domain_like:
             Optional. The iOS 'domain' for the file to be decrypted, containing '%' or '_' SQL LIKE wildcards.
             If 'relative_path' is not globally unique, a domain can be provided to restrict matching.
             Common domain wildcards are provided by the 'DomainLike' class, otherwise these can be found by opening the
             decrypted Manifest.db file and examining the Files table.
 
         :return: decrypted bytes of the file.
         """
-        file_bytes, _file_mtime = self._file_as_bytes(relative_path, domain_like)
+        # Extract the required metadata:
+        file_id, file_bplist = self._file_metadata_from_manifest(relative_path, domain_like)
+        # Decrypt the requested file:
+        file_bytes = self._decrypt_inner_file(file_id=file_id, file_bplist=file_bplist)
         return file_bytes
 
     def extract_file(self, *, relative_path, domain_like=None, output_filename):
         """
         Decrypt a single named file and save it to disk.
 
         This is a helper method and is exactly equivalent to extract_file_as_bytes(...) and then
@@ -293,25 +258,20 @@
             Optional. The iOS 'domain' for the file to be decrypted, containing '%' or '_' SQL LIKE wildcards.
             If 'relative_path' is not globally unique, a domain can be provided to restrict matching.
             Common domain wildcards are provided by the 'DomainLike' class, otherwise these can be found by opening the
             decrypted Manifest.db file and examining the Files table.
         :param output_filename:
             The filename to write the decrypted file contents to.
         """
-        # Get the decrypted bytes of the requested file:
-        file_bytes, file_mtime = self._file_as_bytes(relative_path, domain_like)
-        # Output them to disk:
-        output_directory = os.path.dirname(output_filename)
-        if output_directory:
-            os.makedirs(output_directory, exist_ok=True)
-        with open(output_filename, 'wb') as outfile:
-            outfile.write(file_bytes)
-        # Update the file mtime data:
-        if file_mtime:
-            os.utime(output_filename, times=(file_mtime, file_mtime))
+        # Extract the required metadata:
+        file_id, file_bplist = self._file_metadata_from_manifest(relative_path, domain_like)
+        file_plist = utils.FilePlist(file_bplist)
+        inner_key = self._keybag.unwrapKeyForClass(file_plist.protection_class, file_plist.encryption_key)
+        # Decrypt the requested file:
+        self._decrypt_file_to_disk(file_id=file_id, file_plist=file_plist, key=inner_key, output_filepath=output_filename)
 
     def extract_files(self, *, relative_paths_like, domain_like=None, output_folder,
                       preserve_folders=False, domain_subfolders=False, incremental=False):
         """
         Decrypt files matching a relative path query and output them to a folder.
 
         This method is not really designed to match very loose relative paths like '%' or '%.jpg',
@@ -380,46 +340,29 @@
             results = cur.fetchall()
         except sqlite3.Error as e:
             raise RuntimeError("Error querying Manifest database!") from e
         # Ensure output destination exists then loop through matches:
         os.makedirs(output_folder, exist_ok=True)
         n_files = 0
         for file_id, domain, matched_relative_path, file_bplist in results:
-            # Do we need to create a subfolder for this file's domain?
+            # Build the output file path:
+            _output_path = [output_folder]
             if domain_subfolders:
-                subfolder = os.path.join(output_folder, domain)
-                os.makedirs(subfolder, exist_ok=True)
-            else:
-                subfolder = output_folder
-            # Do we need to preserve folders from the relativePath?
+                _output_path.append(domain)
             if preserve_folders:
-                matched_relative_folder = os.path.dirname(matched_relative_path)
-                output_folder_path = os.path.join(subfolder, matched_relative_folder)
-                os.makedirs(output_folder_path, exist_ok=True)
-                output_file_path = os.path.join(subfolder, matched_relative_path)
-            else:
-                filename = os.path.basename(matched_relative_path)
-                output_file_path = os.path.join(subfolder, filename)
+                _output_path.append(os.path.dirname(matched_relative_path))
+            filename = os.path.basename(matched_relative_path)
+            output_filepath = os.path.join(*_output_path, filename)
+            # Get the file metadata PList:
+            file_plist = utils.FilePlist(file_bplist)
             # Check if file already exists and we are doing an incremental extraction:
-            if os.path.exists(output_file_path) and incremental:
-                existing_mtime = os.path.getmtime(output_file_path)
-                # Conditionally decrypt the file, to avoid unnecessary work:
-                file_bytes, file_mtime = self._decrypt_inner_file(file_id=file_id, file_bplist=file_bplist,
-                                                                  if_modified_since=existing_mtime)
-                if file_bytes is None and file_mtime <= existing_mtime:
+            if os.path.exists(output_filepath) and incremental:
+                existing_mtime = os.path.getmtime(output_filepath)
+                if file_plist.mtime <= existing_mtime:
                     # Skip re-writing this file to disk since it has not changed.
                     continue
-                elif file_bytes is None:
-                    # This should not be possible:
-                    raise IOError("Incremental decryption issue; try again with incremental disabled!")
-            else:
-                # Else just decrypt the file:
-                file_bytes, file_mtime = self._decrypt_inner_file(file_id=file_id, file_bplist=file_bplist)
-            # Output to disk:
-            with open(output_file_path, 'wb') as outfile:
-                outfile.write(file_bytes)
-            # Update the file mtime data:
-            if file_mtime:
-                os.utime(output_file_path, times=(file_mtime, file_mtime))
+            # Decrypt the file:
+            inner_key = self._keybag.unwrapKeyForClass(file_plist.protection_class, file_plist.encryption_key)
+            self._decrypt_file_to_disk(file_id=file_id, key=inner_key, file_plist=file_plist, output_filepath=output_filepath)
             n_files += 1
         # Return how many files were extracted:
         return n_files
```

### Comparing `iphone_backup_decrypt-0.6.0/src/iphone_backup_decrypt.egg-info/PKG-INFO` & `iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphone_backup_decrypt
-Version: 0.6.0
+Version: 0.7.0
 Summary: Decrypt and extract files from an iOS13+ encrypted local backup.
 Author: James Sharkey
 Project-URL: Homepage, https://github.com/jsharkey13/iphone_backup_decrypt
 Keywords: iPhone,backup,forensics,iOS,WhatsApp,decryption,iOS backup,iTunes Backup
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.8
@@ -12,16 +12,16 @@
 License-File: LICENSE.txt
 Requires-Dist: pycryptodome>=3.20.0
 Provides-Extra: fastpbkdf2
 Requires-Dist: fastpbkdf2>=0.2; extra == "fastpbkdf2"
 
 # iphone-backup-decrypt
 
-Decrypt an encrypted, local (i.e. non-iCloud), iPhone backup created from iOS13 or newer.
-This code is mainly a [wrapper for this StackOverflow answer](https://stackoverflow.com/a/13793043),
+Decrypt an encrypted, local iPhone backup created from iOS13 or newer.
+This code [was based on this StackOverflow answer](https://stackoverflow.com/a/13793043),
 itself based on the [iphone-dataprotection](https://code.google.com/p/iphone-dataprotection/) code.
 
 ## Install
 
 Requires [Python 3.8](https://www.python.org/) or higher.
 
 The backup decryption keys are protected using 10 million rounds of PBKDF2 with SHA256, then 10 thousand further iterations of PBKDF2 with SHA-1.
@@ -56,25 +56,30 @@
 After creating the class, use the `EncryptedBackup.save_manifest_file(...)` method to store a decrypted version.
 
 A minimal example to decrypt and extract some files might look like:
 ```python
 from iphone_backup_decrypt import EncryptedBackup, RelativePath, MatchFiles
 
 passphrase = "..."  # Or load passphrase more securely from stdin, or a file, etc.
-backup_path = "%AppData%\\Apple Computer\\MobileSync\\Backup\\[device-specific-hash]"
+backup_path = "%AppData%/Apple Computer/MobileSync/Backup/[device-specific-hash]"
+# Or MacOS: "/Users/[user]/Library/Application Support/MobileSync/Backup/[device-hash]"
 
 backup = EncryptedBackup(backup_directory=backup_path, passphrase=passphrase)
 
 # Extract the call history SQLite database:
 backup.extract_file(relative_path=RelativePath.CALL_HISTORY, 
                     output_filename="./output/call_history.sqlite")
 
 # Extract the camera roll, using MatchFiles for combined path and domain matching:
 backup.extract_files(**MatchFiles.CAMERA_ROLL, output_folder="./output/camera_roll")
 
+# Extract any iCloud camera roll images on the device (may include thumbnails for some
+# but not all images offloaded to the cloud, and have duplicates from the camera roll):
+backup.extract_files(**MatchFiles.ICLOUD_PHOTOS, output_folder="./output/icloud_photos")
+
 # Extract WhatsApp SQLite database and attachments:
 backup.extract_file(relative_path=RelativePath.WHATSAPP_MESSAGES,
                     output_filename="./output/whatsapp.sqlite")
 backup.extract_files(**MatchFiles.WHATSAPP_ATTACHMENTS,
                      output_folder="./output/whatsapp", preserve_folders=False)
 
 # Extract Strava workouts:
```

