# Comparing `tmp/waymore-4.2.tar.gz` & `tmp/waymore-4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waymore-4.2.tar", last modified: Tue Apr 16 12:51:10 2024, max compression
+gzip compressed data, was "waymore-4.3.tar", last modified: Wed May  8 23:17:25 2024, max compression
```

## Comparing `waymore-4.2.tar` & `waymore-4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-16 12:51:10.357043 waymore-4.2/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-03-20 18:00:02.000000 waymore-4.2/LICENSE
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47245 2024-04-16 12:51:10.338303 waymore-4.2/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    46794 2024-04-16 12:25:53.000000 waymore-4.2/README.md
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-04-16 12:51:10.359349 waymore-4.2/setup.cfg
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2142 2024-04-01 16:43:41.000000 waymore-4.2/setup.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-16 12:51:10.094560 waymore-4.2/waymore/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-04-16 12:25:47.000000 waymore-4.2/waymore/__init__.py
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)   167332 2024-04-16 12:32:29.000000 waymore-4.2/waymore/waymore.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-16 12:51:10.319250 waymore-4.2/waymore.egg-info/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47245 2024-04-16 12:51:09.000000 waymore-4.2/waymore.egg-info/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)      253 2024-04-16 12:51:09.000000 waymore-4.2/waymore.egg-info/SOURCES.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-16 12:51:09.000000 waymore-4.2/waymore.egg-info/dependency_links.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       49 2024-04-16 12:51:09.000000 waymore-4.2/waymore.egg-info/entry_points.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       63 2024-04-16 12:51:09.000000 waymore-4.2/waymore.egg-info/requires.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        8 2024-04-16 12:51:09.000000 waymore-4.2/waymore.egg-info/top_level.txt
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-08 23:17:25.817201 waymore-4.3/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-05-08 20:42:52.000000 waymore-4.3/LICENSE
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47245 2024-05-08 23:17:25.805375 waymore-4.3/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    46794 2024-05-08 21:49:16.000000 waymore-4.3/README.md
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-05-08 23:17:25.820218 waymore-4.3/setup.cfg
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2142 2024-05-08 20:42:52.000000 waymore-4.3/setup.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-08 23:17:25.446064 waymore-4.3/waymore/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-05-08 21:49:24.000000 waymore-4.3/waymore/__init__.py
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)   168145 2024-05-08 23:08:08.000000 waymore-4.3/waymore/waymore.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-08 23:17:25.779233 waymore-4.3/waymore.egg-info/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47245 2024-05-08 23:17:25.000000 waymore-4.3/waymore.egg-info/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)      253 2024-05-08 23:17:25.000000 waymore-4.3/waymore.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-05-08 23:17:25.000000 waymore-4.3/waymore.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       49 2024-05-08 23:17:25.000000 waymore-4.3/waymore.egg-info/entry_points.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       63 2024-05-08 23:17:25.000000 waymore-4.3/waymore.egg-info/requires.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        8 2024-05-08 23:17:25.000000 waymore-4.3/waymore.egg-info/top_level.txt
```

### Comparing `waymore-4.2/LICENSE` & `waymore-4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `waymore-4.2/PKG-INFO` & `waymore-4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waymore
-Version: 4.2
+Version: 4.3
 Summary: Find way more from the Wayback Machine, Common Crawl, Alien Vault OTX, URLScan & VirusTotal!
 Home-page: https://github.com/xnl-h4ck3r/waymore
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: requests
@@ -12,15 +12,15 @@
 Requires-Dist: termcolor
 Requires-Dist: psutil
 Requires-Dist: urlparse3
 Requires-Dist: tldextract
 
 <center><img src="https://github.com/xnl-h4ck3r/waymore/blob/main/waymore/images/title.png"></center>
 
-## About - v4.2
+## About - v4.3
 
 The idea behind **waymore** is to find even more links from the Wayback Machine than other existing tools.
 
 👉 The biggest difference between **waymore** and other tools is that it can also **download the archived responses** for URLs on wayback machine so that you can then search these for even more links, developer comments, extra parameters, etc. etc.
 👉 Also, other tools do not currenrtly deal with the rate limiting now in place by the sources, and will often just stop with incomplete results and not let you know they are incomplete.
 
 Anyone who does bug bounty will have likely used the amazing [waybackurls](https://github.com/tomnomnom/waybackurls) by @TomNomNoms. This tool gets URLs from [web.archive.org](https://web.archive.org) and additional links (if any) from one of the index collections on [index.commoncrawl.org](http://index.commoncrawl.org/).
```

### Comparing `waymore-4.2/README.md` & `waymore-4.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <center><img src="https://github.com/xnl-h4ck3r/waymore/blob/main/waymore/images/title.png"></center>
 
-## About - v4.2
+## About - v4.3
 
 The idea behind **waymore** is to find even more links from the Wayback Machine than other existing tools.
 
 👉 The biggest difference between **waymore** and other tools is that it can also **download the archived responses** for URLs on wayback machine so that you can then search these for even more links, developer comments, extra parameters, etc. etc.
 👉 Also, other tools do not currenrtly deal with the rate limiting now in place by the sources, and will often just stop with incomplete results and not let you know they are incomplete.
 
 Anyone who does bug bounty will have likely used the amazing [waybackurls](https://github.com/tomnomnom/waybackurls) by @TomNomNoms. This tool gets URLs from [web.archive.org](https://web.archive.org) and additional links (if any) from one of the index collections on [index.commoncrawl.org](http://index.commoncrawl.org/).
```

### Comparing `waymore-4.2/setup.py` & `waymore-4.3/setup.py`

 * *Files identical despite different names*

### Comparing `waymore-4.2/waymore/waymore.py` & `waymore-4.3/waymore/waymore.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 checkAlienVault = 0
 checkURLScan = 0
 checkVirusTotal = 0
 argsInputHostname = ''
 responseOutputDirectory = ''
 
 # Source Provider URLs
-WAYBACK_URL = 'https://web.archive.org/cdx/search/cdx?url={DOMAIN}&collapse={COLLAPSE}&fl=timestamp,original,mimetype,statuscode,digest'
+WAYBACK_URL = 'https://web.archive.org/cdx/search/cdx?url={DOMAIN}{COLLAPSE}&fl=timestamp,original,mimetype,statuscode,digest'
 CCRAWL_INDEX_URL = 'https://index.commoncrawl.org/collinfo.json'
 ALIENVAULT_URL = 'https://otx.alienvault.com/api/v1/indicators/{TYPE}/{DOMAIN}/url_list?limit=500'
 URLSCAN_URL = 'https://urlscan.io/api/v1/search/?q=domain:{DOMAIN}&size=10000'
 VIRUSTOTAL_URL = 'https://www.virustotal.com/vtapi/v2/domain/report?apikey={APIKEY}&domain={DOMAIN}'
 
 # User Agents to use when making requests, chosen at random
 USER_AGENT  = [
@@ -1847,19 +1847,23 @@
                 write(colored('\rGetting the number of Wayback Machine (archive.org) pages to search...\r','cyan'))
             # Choose a random user agent string to use for any requests
             userAgent = random.choice(USER_AGENT)
             session = requests.Session()
             session.mount('https://', HTTP_ADAPTER)
             session.mount('http://', HTTP_ADAPTER)
             resp = session.get(url+'&showNumPages=True', headers={"User-Agent":userAgent}) 
-            totalPages = int(resp.text.strip())
-            
-            # If the argument to limit the requests was passed and the total pages is larger than that, set to the limit
-            if args.limit_requests != 0 and totalPages > args.limit_requests:
-                totalPages = args.limit_requests
+            # Try to get the total number of pages. If there is a problem, we'll return totalPages = 0 which means we'll get everything back in one request 
+            try:
+                totalPages = int(resp.text.strip())
+                
+                # If the argument to limit the requests was passed and the total pages is larger than that, set to the limit
+                if args.limit_requests != 0 and totalPages > args.limit_requests:
+                    totalPages = args.limit_requests
+            except:
+                totalPages = -1
         except Exception as e:
             try:
                 # If the rate limit was reached end now
                 if resp.status_code == 429:
                     writerr(colored(getSPACER('[ 429 ] Wayback Machine (Archive.org) rate limit reached so unable to get links.'),'red'))
                     return
                 
@@ -1876,39 +1880,47 @@
                 if str(e).lower().find('alert access denied'):
                     writerr(colored(getSPACER('[ ERR ] Unable to get links from Wayback Machine (archive.org): Access Denied. Are you able to manually visit https://web.archive.org/? Your ISP may be blocking you, e.g. your adult content filter is on (why it triggers that filter I don\'t know, but it has happened!)'), 'red'))
                 elif str(e).lower().find('connection refused'):
                     writerr(colored(getSPACER('[ ERR ] Unable to get links from Wayback Machine (archive.org): Connection Refused. Are you able to manually visit https://web.archive.org/? Your ISP may be blocking your IP)'), 'red'))
                 else:
                     writerr(colored(getSPACER('[ ERR ] Unable to get links from Wayback Machine (archive.org): ' + str(e)), 'red'))
             return
-
+        
         if args.check_only:
-            checkWayback = totalPages
-            write(colored('Get URLs from Wayback Machine: ','cyan')+colored(str(checkWayback)+' requests','white'))
+            if totalPages < 0:
+                write(colored('Due to a change in Wayback Machine API, all URLs will be retrieved in one request and it is not possible to determine how long it will take, so please ignore this.','cyan'))
+            else:
+                checkWayback = totalPages
+                write(colored('Get URLs from Wayback Machine: ','cyan')+colored(str(checkWayback)+' requests','white'))
         else:
             if verbose():
                 write(colored('The archive URL requested to get links: ','magenta')+colored(url+'\n','white'))
             
-            # if the page number was found then display it, but otherwise we will just try to increment until we have everything       
-            write(colored('\rGetting links from ' + str(totalPages) + ' Wayback Machine (archive.org) API requests (this can take a while for some domains)...\r','cyan'))
+            if totalPages < 0:
+                write(colored('\rGetting links from Wayback Machine (archive.org) with one request (this can take a while for some domains)...\r','cyan'))
 
-            # Get a list of all the page URLs we need to visit
-            pages = []
-            if totalPages == 1:
-                pages.append(url)
+                processWayBackPage(url)
             else:
-                for page in range(0, totalPages):
-                    pages.append(url+str(page))
-            
-            # Process the URLs from web archive
-            if stopProgram is None:
-                p = mp.Pool(args.processes)
-                p.map(processWayBackPage, pages)
-                p.close()
-                p.join()
+                # if the page number was found then display it, but otherwise we will just try to increment until we have everything  
+                write(colored('\rGetting links from ' + str(totalPages) + ' Wayback Machine (archive.org) API requests (this can take a while for some domains)...\r','cyan'))
+
+                # Get a list of all the page URLs we need to visit
+                pages = []
+                if totalPages == 1:
+                    pages.append(url)
+                else:
+                    for page in range(0, totalPages):
+                        pages.append(url+str(page))
+                
+                # Process the URLs from web archive
+                if stopProgram is None:
+                    p = mp.Pool(args.processes)
+                    p.map(processWayBackPage, pages)
+                    p.close()
+                    p.join()
                 
             # Show the MIME types found (in case user wants to exclude more)
             if verbose() and len(linkMimes) > 0 :
                 linkMimes.discard('warc/revisit')
                 write(getSPACER(colored('MIME types found: ','magenta')+colored(str(linkMimes),'white'))+'\n')
                 linkMimes = None
             
@@ -2427,19 +2439,19 @@
             # Set the collapse parameter value in the archive.org URL. From the Wayback API docs:
             # "A new form of filtering is the option to 'collapse' results based on a field, or a substring of a field.
             # Collapsing is done on adjacent cdx lines where all captures after the first one that are duplicate are filtered out.
             # This is useful for filtering out captures that are 'too dense' or when looking for unique captures."
             if args.capture_interval == 'none': # get all
                 collapse = ''
             elif args.capture_interval == 'h': # get at most 1 capture per URL per hour
-                collapse = 'timestamp:10,original'
+                collapse = '&collapse=timestamp:10'
             elif args.capture_interval == 'd': # get at most 1 capture per URL per day
-                collapse = 'timestamp:8,original'
+                collapse = '&collapse=timestamp:8'
             elif args.capture_interval == 'm': # get at most 1 capture per URL per month
-                collapse = 'timestamp:6,original'
+                collapse = '&collapse=timestamp:6'
 
             url = WAYBACK_URL.replace('{DOMAIN}',subs + quote(argsInput) + path).replace('{COLLAPSE}',collapse) + filterMIME + filterCode + filterLimit + filterFrom + filterTo + filterKeywords
                 
             if verbose():
                 write(colored('The archive URL requested to get responses: ','magenta')+colored(url+'\n','white'))
             
             if args.check_only:
```

### Comparing `waymore-4.2/waymore.egg-info/PKG-INFO` & `waymore-4.3/waymore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waymore
-Version: 4.2
+Version: 4.3
 Summary: Find way more from the Wayback Machine, Common Crawl, Alien Vault OTX, URLScan & VirusTotal!
 Home-page: https://github.com/xnl-h4ck3r/waymore
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: requests
@@ -12,15 +12,15 @@
 Requires-Dist: termcolor
 Requires-Dist: psutil
 Requires-Dist: urlparse3
 Requires-Dist: tldextract
 
 <center><img src="https://github.com/xnl-h4ck3r/waymore/blob/main/waymore/images/title.png"></center>
 
-## About - v4.2
+## About - v4.3
 
 The idea behind **waymore** is to find even more links from the Wayback Machine than other existing tools.
 
 👉 The biggest difference between **waymore** and other tools is that it can also **download the archived responses** for URLs on wayback machine so that you can then search these for even more links, developer comments, extra parameters, etc. etc.
 👉 Also, other tools do not currenrtly deal with the rate limiting now in place by the sources, and will often just stop with incomplete results and not let you know they are incomplete.
 
 Anyone who does bug bounty will have likely used the amazing [waybackurls](https://github.com/tomnomnom/waybackurls) by @TomNomNoms. This tool gets URLs from [web.archive.org](https://web.archive.org) and additional links (if any) from one of the index collections on [index.commoncrawl.org](http://index.commoncrawl.org/).
```

