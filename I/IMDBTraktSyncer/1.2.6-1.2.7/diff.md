# Comparing `tmp/IMDBTraktSyncer-1.2.6.tar.gz` & `tmp/IMDBTraktSyncer-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.2.6.tar", last modified: Tue May 23 23:44:42 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.2.7.tar", last modified: Wed May 24 22:06:49 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.2.6.tar` & `IMDBTraktSyncer-1.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 23:44:42.957660 IMDBTraktSyncer-1.2.6/
-drwxrwxrwx   0        0        0        0 2023-05-23 23:44:42.934671 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    21642 2023-05-23 23:30:49.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1900 2023-05-23 23:43:19.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4079 2023-05-16 01:53:33.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3845 2023-05-20 20:45:06.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     7405 2023-05-23 21:38:34.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     6981 2023-05-23 22:09:09.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:44:42.954670 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     8525 2023-05-23 23:44:42.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-05-23 23:44:42.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 23:44:42.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-23 23:44:42.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-23 23:44:42.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-23 23:44:42.000000 IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.6/LICENSE
--rw-rw-rw-   0        0        0     8525 2023-05-23 23:44:42.956660 IMDBTraktSyncer-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     7855 2023-05-23 23:42:16.000000 IMDBTraktSyncer-1.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 23:44:42.957660 IMDBTraktSyncer-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-05-23 23:37:34.000000 IMDBTraktSyncer-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 22:06:49.255229 IMDBTraktSyncer-1.2.7/
+drwxrwxrwx   0        0        0        0 2023-05-24 22:06:49.222344 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    22282 2023-05-24 22:01:23.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1900 2023-05-23 23:43:19.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4079 2023-05-16 01:53:33.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3845 2023-05-20 20:45:06.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     7752 2023-05-24 22:03:34.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     6981 2023-05-23 22:09:09.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-24 22:06:49.252344 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     8556 2023-05-24 22:06:49.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-05-24 22:06:49.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 22:06:49.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-24 22:06:49.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-24 22:06:49.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-24 22:06:49.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0     8556 2023-05-24 22:06:49.255229 IMDBTraktSyncer-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7856 2023-05-24 22:06:25.000000 IMDBTraktSyncer-1.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 22:06:49.255229 IMDBTraktSyncer-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1347 2023-05-24 22:06:09.000000 IMDBTraktSyncer-1.2.7/setup.py
```

### Comparing `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,24 +102,24 @@
             print("\nIf your login is correct then an IMDB captcha check likely the cause of this error. To fix this, simply login to the IMDB website in your browser, preferably Chrome, and from the same computer. If logged in, log out and log back in. It may ask you to fill in a captcha; complete it and finish logging in. After logging in successfully on your browser, run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues.")
             print("\nIf your IMDB login is incorrect, simply edit the credentials.txt file with the correct login or delete the credentials file and run the script again.")
             print("\nSee this GitHub link for more details: https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2")
             print("\nStopping script...")
             raise SystemExit
         
         trakt_watchlist, trakt_ratings, trakt_reviews = traktData.getTraktData()
-        imdb_watchlist, imdb_ratings, imdb_reviews = imdbData.getImdbData(imdb_username, imdb_password, driver, directory, wait)
+        imdb_watchlist, imdb_ratings, imdb_reviews, errors_found_getting_imdb_reviews = imdbData.getImdbData(imdb_username, imdb_password, driver, directory, wait)
 
-        #Get trakt and imdb ratings and filter out trakt ratings with missing imdb id
-        trakt_ratings = [rating for rating in trakt_ratings if rating['ID'] is not None]
-        imdb_ratings = [rating for rating in imdb_ratings if rating['ID'] is not None]
-        trakt_reviews = [review for review in trakt_reviews if review['ID'] is not None]
-        imdb_reviews = [review for review in imdb_reviews if review['ID'] is not None]
-        trakt_watchlist = [item for item in trakt_watchlist if item['ID'] is not None]
-        imdb_watchlist = [item for item in imdb_watchlist if item['ID'] is not None]
-        #Filter out ratings already set
+        #Get trakt and imdb data and filter out items with missing imdb id
+        trakt_ratings = [rating for rating in trakt_ratings if rating.get('ID') is not None]
+        imdb_ratings = [rating for rating in imdb_ratings if rating.get('ID') is not None]
+        trakt_reviews = [review for review in trakt_reviews if review.get('ID') is not None]
+        imdb_reviews = [review for review in imdb_reviews if review.get('ID') is not None]
+        trakt_watchlist = [item for item in trakt_watchlist if item.get('ID') is not None]
+        imdb_watchlist = [item for item in imdb_watchlist if item.get('ID') is not None]
+        #Filter out items already set
         imdb_ratings_to_set = [rating for rating in trakt_ratings if rating['ID'] not in [imdb_rating['ID'] for imdb_rating in imdb_ratings]]
         trakt_ratings_to_set = [rating for rating in imdb_ratings if rating['ID'] not in [trakt_rating['ID'] for trakt_rating in trakt_ratings]]
         imdb_reviews_to_set = [review for review in trakt_reviews if review['ID'] not in [imdb_review['ID'] for imdb_review in imdb_reviews]]
         trakt_reviews_to_set = [review for review in imdb_reviews if review['ID'] not in [trakt_review['ID'] for trakt_review in trakt_reviews]]
         imdb_watchlist_to_set = [item for item in trakt_watchlist if item['ID'] not in [imdb_item['ID'] for imdb_item in imdb_watchlist]]
         trakt_watchlist_to_set = [item for item in imdb_watchlist if item['ID'] not in [trakt_item['ID'] for trakt_item in trakt_watchlist]]
         # Remove duplicate reviews and filter by out any items for imdb_reviews_to_set where comment length is less than 600 characters
@@ -304,108 +304,112 @@
 
             print('Setting IMDB Ratings Complete')
         else:
             print('No IMDB Ratings To Set')
 
         # If sync_reviews_value is true
         if VC.sync_reviews_value:
-            # Set Trakt Reviews
-            if trakt_reviews_to_set:
-                print('Setting Trakt Reviews')
+            # Check if there was an error getting IMDB reviews
+            if not errors_found_getting_imdb_reviews:
+                # Set Trakt Reviews
+                if trakt_reviews_to_set:
+                    print('Setting Trakt Reviews')
 
-                # Count the total number of items
-                num_items = len(trakt_reviews_to_set)
-                item_count = 0
+                    # Count the total number of items
+                    num_items = len(trakt_reviews_to_set)
+                    item_count = 0
 
-                for review in trakt_reviews_to_set:
-                    item_count += 1
-                    imdb_id = review['ID']
-                    comment = review['Comment']
-                    media_type = review['Type']  # 'movie', 'show', or 'episode'
+                    for review in trakt_reviews_to_set:
+                        item_count += 1
+                        imdb_id = review['ID']
+                        comment = review['Comment']
+                        media_type = review['Type']  # 'movie', 'show', or 'episode'
 
-                    url = f"https://api.trakt.tv/comments"
+                        url = f"https://api.trakt.tv/comments"
 
-                    data = {
-                        "comment": comment
-                    }
+                        data = {
+                            "comment": comment
+                        }
 
-                    if media_type == 'movie':
-                        data['movie'] = {
-                            "ids": {
-                                "imdb": imdb_id
+                        if media_type == 'movie':
+                            data['movie'] = {
+                                "ids": {
+                                    "imdb": imdb_id
+                                }
                             }
-                        }
-                    elif media_type == 'show':
-                        data['show'] = {
-                            "ids": {
-                                "imdb": imdb_id
+                        elif media_type == 'show':
+                            data['show'] = {
+                                "ids": {
+                                    "imdb": imdb_id
+                                }
                             }
-                        }
-                    elif media_type == 'episode':
-                        data['episode'] = {
-                            "ids": {
-                                "imdb": episode_id
+                        elif media_type == 'episode':
+                            data['episode'] = {
+                                "ids": {
+                                    "imdb": episode_id
+                                }
                             }
-                        }
-                    
-                    response = EH.make_trakt_request(url, payload=data)
-                    if response:
-                        print(f"Submitted comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt")
-                    else:
-                        print(f"Failed to submit comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt")
-                        print("Error Response:", response.content, response.status_code)
-
-                print('Trakt Reviews Set Successfully')
-            else:
-                print('No Trakt Reviews To Set')
+                        
+                        response = EH.make_trakt_request(url, payload=data)
+                        if response:
+                            print(f"Submitted comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt")
+                        else:
+                            print(f"Failed to submit comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt")
+                            print("Error Response:", response.content, response.status_code)
 
-            # Set IMDB Reviews
-            if imdb_reviews_to_set:
-                # Call the check_last_run() function
-                if VC.check_imdb_reviews_last_submitted():
-                    print('Setting IMDB Reviews')
-                    
-                    # Count the total number of items
-                    num_items = len(trakt_reviews_to_set)
-                    item_count = 0
-                    
-                    for review in imdb_reviews_to_set:
-                        item_count += 1
-                        try:
-                            print(f"Submitting review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB")
-                            driver.get(f'https://contribute.imdb.com/review/{review["ID"]}/add?bus=imdb')
-                            
-                            review_title_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input.klondike-input")))
-                            review_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "textarea.klondike-textarea")))
-                            
-                            review_title_input.send_keys("My Review")
-                            review_input.send_keys(review["Comment"])
-                            
-                            no_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "ul.klondike-userreview-spoiler li:nth-child(2)")))
-                            yes_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "ul.klondike-userreview-spoiler li:nth-child(1)")))
-                            
-                            if review["Spoiler"]:
-                                yes_element.click()                        
-                            else:
-                                no_element.click()
-                                                    
-                            submit_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input.a-button-input[type='submit']")))
+                    print('Trakt Reviews Set Successfully')
+                else:
+                    print('No Trakt Reviews To Set')
 
-                            submit_button.click()
-                            
-                            time.sleep(1)
-                        except (NoSuchElementException, TimeoutException):
-                            print(f"Failed to submit review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB ({item['ID']})")
-                            pass
-                    
-                    print('Setting IMDB Reviews Complete')
+                # Set IMDB Reviews
+                if imdb_reviews_to_set:
+                    # Call the check_last_run() function
+                    if VC.check_imdb_reviews_last_submitted():
+                        print('Setting IMDB Reviews')
+                        
+                        # Count the total number of items
+                        num_items = len(trakt_reviews_to_set)
+                        item_count = 0
+                        
+                        for review in imdb_reviews_to_set:
+                            item_count += 1
+                            try:
+                                print(f"Submitting review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB")
+                                driver.get(f'https://contribute.imdb.com/review/{review["ID"]}/add?bus=imdb')
+                                
+                                review_title_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input.klondike-input")))
+                                review_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "textarea.klondike-textarea")))
+                                
+                                review_title_input.send_keys("My Review")
+                                review_input.send_keys(review["Comment"])
+                                
+                                no_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "ul.klondike-userreview-spoiler li:nth-child(2)")))
+                                yes_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "ul.klondike-userreview-spoiler li:nth-child(1)")))
+                                
+                                if review["Spoiler"]:
+                                    yes_element.click()                        
+                                else:
+                                    no_element.click()
+                                                        
+                                submit_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input.a-button-input[type='submit']")))
+
+                                submit_button.click()
+                                
+                                time.sleep(1)
+                            except (NoSuchElementException, TimeoutException):
+                                print(f"Failed to submit review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB ({item['ID']})")
+                                pass
+                        
+                        print('Setting IMDB Reviews Complete')
+                    else:
+                        print('IMDB reviews were submitted within the last 7 days. Skipping IMDB review submission.')
                 else:
-                    print('IMDB reviews were submitted within the last 7 days. Skipping IMDB review submission.')
+                    print('No IMDB Reviews To Set')
             else:
-                print('No IMDB Reviews To Set')
+                print('There was an error getting IMDB reviews. See exception. Skipping reviews submissions.')
 
         #Close web driver
         print("Closing webdriver...")
         driver.quit()
         service.stop()
     
     except Exception as e:
```

### Comparing `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/imdbData.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,22 +39,22 @@
                 reader = csv.reader(file)
                 header = next(reader)  # skip the header row
                 for row in reader:
                     title = row[5]
                     year = row[10]
                     imdb_id = row[1]
                     if "tvSeries" in row[7] or "tvMiniSeries" in row[7]:
-                        type = "show"
+                        media_type = "show"
                     elif "tvEpisode" in row[7]:
-                        type = "episode"
+                        media_type = "episode"
                     elif "movie" in row[7]:
-                        type = "movie"
+                        media_type = "movie"
                     else:
-                        type = "unknown"
-                    imdb_watchlist.append({'Title': title, 'Year': year, 'ID': imdb_id, 'Type': type})
+                        media_type = "unknown"
+                    imdb_watchlist.append({'Title': title, 'Year': year, 'ID': imdb_id, 'Type': media_type})
         except FileNotFoundError:
             print('Ratings file not found')
             
         # Delete csv files
         for file in os.listdir(directory):
             if file.endswith('.csv') and 'WATCHLIST' in file:
                 os.remove(os.path.join(directory, file))
@@ -88,22 +88,22 @@
                 header = next(reader)  # skip the header row
                 for row in reader:
                     title = row[3]
                     year = row[8]
                     rating = row[1]
                     imdb_id = row[0]
                     if "tvSeries" in row[5] or "tvMiniSeries" in row[5]:
-                        type = "show"
+                        media_type = "show"
                     elif "tvEpisode" in row[5]:
-                        type = "episode"
+                        media_type = "episode"
                     elif "movie" in row[5]:
-                        type = "movie"
+                        media_type = "movie"
                     else:
-                        type = "unknown"
-                    imdb_ratings.append({'Title': title, 'Year': year, 'Rating': rating, 'ID': imdb_id, 'Type': type})
+                        media_type = "unknown"
+                    imdb_ratings.append({'Title': title, 'Year': year, 'Rating': rating, 'ID': imdb_id, 'Type': media_type})
         except FileNotFoundError:
             print('Ratings file not found')
             
         # Delete csv files
         for file in os.listdir(directory):
             if file.endswith('.csv') and 'ratings' in file:
                 os.remove(os.path.join(directory, file))
@@ -124,20 +124,22 @@
 
     #Get IMDB Reviews
     driver.get('https://www.imdb.com/profile')
     reviews_link = driver.find_element(By.CSS_SELECTOR, "div.aux-content-widget-2 div.subNavItem a[href*='comments-index']")
     reviews_link.click()
 
     reviews = []
-
+    errors_found_getting_imdb_reviews = False
     while True:
         try:
-            review_elements = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".imdb-user-review")))
-            if not review_elements:
-                break  # No review elements found, exit the loop
+            try:
+                review_elements = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".imdb-user-review")))
+            except (NoSuchElementException, TimeoutException):
+                # No review elements found. There are no reviews. Exit the loop without an error.
+                break
             
             for element in review_elements:
                 review = {}
                 # Extract review details
                 review['Title'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header a").text
                 review['Year'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header span").text.strip('()').split('–')[0].strip()
                 review['ID'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header a").get_attribute("href").split('/')[4]
@@ -165,17 +167,18 @@
                 # Wait until the URL changes
                 wait.until(EC.url_changes(current_url))
                 
                 # Refresh review_elements
                 review_elements = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".imdb-user-review")))
 
             except (NoSuchElementException, TimeoutException):
-                break  # "Next" link not found or timed out waiting for the 'Next' link, exit the loop
+                break  # "Next" link not found or timed out waiting for the 'Next' link, exit the loop without error.
         except Exception as e:
-            print(f"Exception occurred: {e}")
+            errors_found_getting_imdb_reviews = True
+            print(f"Exception occurred while getting IMDB reviews: {type(e)}")
             break
 
     imdb_reviews = reviews
 
     print('Processing IMDB Data Complete')
     
-    return imdb_watchlist, imdb_ratings, imdb_reviews
+    return imdb_watchlist, imdb_ratings, imdb_reviews, errors_found_getting_imdb_reviews
```

### Comparing `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.2.6
-Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
+Version: 1.2.7
+Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDB-Trakt-Syncer
-This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Data already set will not be overwritten. Ratings are synced by default. Watchlist and comment/review sync is optional. The user will be prompted to enter their settings and credentials on first run.
+This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Data already set will not be overwritten. Ratings are synced by default, watchlist and comment/review sync are optional. The user will be prompted to enter their settings and credentials on first run.
 
 The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
```

### Comparing `IMDBTraktSyncer-1.2.6/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.6/LICENSE` & `IMDBTraktSyncer-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.6/PKG-INFO` & `IMDBTraktSyncer-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.2.6
-Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
+Version: 1.2.7
+Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDB-Trakt-Syncer
-This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Data already set will not be overwritten. Ratings are synced by default. Watchlist and comment/review sync is optional. The user will be prompted to enter their settings and credentials on first run.
+This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Data already set will not be overwritten. Ratings are synced by default, watchlist and comment/review sync are optional. The user will be prompted to enter their settings and credentials on first run.
 
 The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
```

### Comparing `IMDBTraktSyncer-1.2.6/README.md` & `IMDBTraktSyncer-1.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # IMDB-Trakt-Syncer
-This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Data already set will not be overwritten. Ratings are synced by default. Watchlist and comment/review sync is optional. The user will be prompted to enter their settings and credentials on first run.
+This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Data already set will not be overwritten. Ratings are synced by default, watchlist and comment/review sync are optional. The user will be prompted to enter their settings and credentials on first run.
 
 The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
```

### Comparing `IMDBTraktSyncer-1.2.6/setup.py` & `IMDBTraktSyncer-1.2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.2.6'
-DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.'
+VERSION = '1.2.7'
+DESCRIPTION = 'This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
```

