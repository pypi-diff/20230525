# Comparing `tmp/numpy_io-0.0.2-py3-none-any.whl.zip` & `tmp/numpy_io-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,32 @@
-Zip file size: 22779 bytes, number of entries: 28
--rw-rw-rw-  2.0 fat       77 b- defN 23-Apr-27 10:42 numpy_io/__init__.py
--rw-rw-rw-  2.0 fat      637 b- defN 23-Apr-27 12:23 numpy_io/setup.py
--rw-rw-rw-  2.0 fat       80 b- defN 23-Apr-27 10:42 numpy_io/core/__init__.py
--rw-rw-rw-  2.0 fat    12381 b- defN 23-Apr-27 12:31 numpy_io/core/numpyadapter.py
--rw-rw-rw-  2.0 fat     5457 b- defN 23-Apr-27 10:42 numpy_io/core/parallel.py
--rw-rw-rw-  2.0 fat     1894 b- defN 23-Apr-27 10:42 numpy_io/core/reader.py
--rw-rw-rw-  2.0 fat     1366 b- defN 23-Apr-27 10:42 numpy_io/core/writer.py
--rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-27 10:42 numpy_io/examples/__init__.py
--rw-rw-rw-  2.0 fat     2708 b- defN 23-Apr-27 10:42 numpy_io/examples/auto_parallel_writer.py
--rw-rw-rw-  2.0 fat     3241 b- defN 23-Apr-27 10:42 numpy_io/examples/auto_writer.py
--rw-rw-rw-  2.0 fat     1778 b- defN 23-Apr-27 10:42 numpy_io/examples/leveldb_readwriter_example.py
--rw-rw-rw-  2.0 fat     2218 b- defN 23-Apr-27 12:26 numpy_io/examples/lmdb_readwriter_example.py
--rw-rw-rw-  2.0 fat     1198 b- defN 23-Apr-27 10:42 numpy_io/examples/memory_raw_readwriter_example.py
--rw-rw-rw-  2.0 fat     1285 b- defN 23-Apr-27 10:42 numpy_io/examples/memory_readwriter_example.py
--rw-rw-rw-  2.0 fat     1586 b- defN 23-Apr-27 10:42 numpy_io/examples/record_numpywriter_example.py
--rw-rw-rw-  2.0 fat     1353 b- defN 23-Apr-27 10:42 numpy_io/examples/record_reader_example.py
--rw-rw-rw-  2.0 fat     1398 b- defN 23-Apr-27 10:42 numpy_io/examples/record_shuffle_example.py
--rw-rw-rw-  2.0 fat     3056 b- defN 23-Apr-27 10:42 numpy_io/examples/record_writer_example.py
--rw-rw-rw-  2.0 fat       56 b- defN 23-Apr-27 10:42 numpy_io/examples/testing/__init__.py
--rw-rw-rw-  2.0 fat     2658 b- defN 23-Apr-27 10:42 numpy_io/examples/testing/lmdb_test.py
--rw-rw-rw-  2.0 fat      613 b- defN 23-Apr-27 10:42 numpy_io/examples/testing/test_mem.py
--rw-rw-rw-  2.0 fat     2907 b- defN 23-Apr-27 10:42 numpy_io/examples/testing/test_mutiprocess.py
--rw-rw-rw-  2.0 fat       73 b- defN 23-Apr-27 12:37 numpy_io/pytorch_loader/__init__.py
--rw-rw-rw-  2.0 fat    10268 b- defN 23-Apr-27 12:59 numpy_io/pytorch_loader/dataloaders.py
--rw-rw-rw-  2.0 fat      364 b- defN 23-Apr-27 13:08 numpy_io-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-27 13:08 numpy_io-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-27 13:08 numpy_io-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2513 b- defN 23-Apr-27 13:08 numpy_io-0.0.2.dist-info/RECORD
-28 files, 61320 bytes uncompressed, 18655 bytes compressed:  69.6%
+Zip file size: 25278 bytes, number of entries: 30
+-rw-rw-rw-  2.0 fat       77 b- defN 23-Apr-26 15:07 numpy_io/__init__.py
+-rw-rw-rw-  2.0 fat      623 b- defN 23-May-25 13:30 numpy_io/setup.py
+-rw-rw-rw-  2.0 fat       80 b- defN 23-Apr-26 14:34 numpy_io/core/__init__.py
+-rw-rw-rw-  2.0 fat    12381 b- defN 23-Apr-29 16:46 numpy_io/core/numpyadapter.py
+-rw-rw-rw-  2.0 fat     5457 b- defN 23-Feb-18 01:47 numpy_io/core/parallel.py
+-rw-rw-rw-  2.0 fat     1894 b- defN 23-Apr-26 14:48 numpy_io/core/reader.py
+-rw-rw-rw-  2.0 fat     1366 b- defN 23-Apr-26 14:49 numpy_io/core/writer.py
+-rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-26 14:27 numpy_io/examples/__init__.py
+-rw-rw-rw-  2.0 fat     2708 b- defN 23-Apr-26 15:08 numpy_io/examples/auto_parallel_writer.py
+-rw-rw-rw-  2.0 fat     3241 b- defN 23-Apr-26 15:11 numpy_io/examples/auto_writer.py
+-rw-rw-rw-  2.0 fat     1778 b- defN 23-Apr-26 14:27 numpy_io/examples/leveldb_readwriter_example.py
+-rw-rw-rw-  2.0 fat     2218 b- defN 23-Apr-29 16:46 numpy_io/examples/lmdb_readwriter_example.py
+-rw-rw-rw-  2.0 fat     1198 b- defN 23-Apr-26 14:27 numpy_io/examples/memory_raw_readwriter_example.py
+-rw-rw-rw-  2.0 fat     1285 b- defN 23-Apr-26 14:27 numpy_io/examples/memory_readwriter_example.py
+-rw-rw-rw-  2.0 fat     1586 b- defN 23-Apr-26 14:27 numpy_io/examples/record_numpywriter_example.py
+-rw-rw-rw-  2.0 fat     1353 b- defN 23-Apr-26 14:27 numpy_io/examples/record_reader_example.py
+-rw-rw-rw-  2.0 fat     1398 b- defN 23-Apr-26 14:27 numpy_io/examples/record_shuffle_example.py
+-rw-rw-rw-  2.0 fat     3056 b- defN 23-Apr-26 14:27 numpy_io/examples/record_writer_example.py
+-rw-rw-rw-  2.0 fat       56 b- defN 23-Apr-29 16:46 numpy_io/examples/testing/__init__.py
+-rw-rw-rw-  2.0 fat     2658 b- defN 23-Apr-29 16:46 numpy_io/examples/testing/lmdb_test.py
+-rw-rw-rw-  2.0 fat      613 b- defN 23-Apr-29 16:46 numpy_io/examples/testing/test_mem.py
+-rw-rw-rw-  2.0 fat     2907 b- defN 23-Apr-29 16:46 numpy_io/examples/testing/test_mutiprocess.py
+-rw-rw-rw-  2.0 fat       73 b- defN 23-Apr-29 16:46 numpy_io/pytorch_loader/__init__.py
+-rw-rw-rw-  2.0 fat     4528 b- defN 23-May-25 13:57 numpy_io/pytorch_loader/data_helper.py
+-rw-rw-rw-  2.0 fat     8631 b- defN 23-May-25 13:37 numpy_io/pytorch_loader/dataloaders.py
+-rw-rw-rw-  2.0 fat     3780 b- defN 23-May-25 13:30 numpy_io/pytorch_loader/tokenizer_config_helper.py
+-rw-rw-rw-  2.0 fat      401 b- defN 23-May-25 14:10 numpy_io-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-25 14:10 numpy_io-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-25 14:10 numpy_io-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2714 b- defN 23-May-25 14:10 numpy_io-0.0.3.dist-info/RECORD
+30 files, 68215 bytes uncompressed, 20826 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -63,23 +63,29 @@
 
 Filename: numpy_io/examples/testing/test_mutiprocess.py
 Comment: 
 
 Filename: numpy_io/pytorch_loader/__init__.py
 Comment: 
 
+Filename: numpy_io/pytorch_loader/data_helper.py
+Comment: 
+
 Filename: numpy_io/pytorch_loader/dataloaders.py
 Comment: 
 
-Filename: numpy_io-0.0.2.dist-info/METADATA
+Filename: numpy_io/pytorch_loader/tokenizer_config_helper.py
+Comment: 
+
+Filename: numpy_io-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: numpy_io-0.0.2.dist-info/WHEEL
+Filename: numpy_io-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: numpy_io-0.0.2.dist-info/top_level.txt
+Filename: numpy_io-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: numpy_io-0.0.2.dist-info/RECORD
+Filename: numpy_io-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## numpy_io/setup.py

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2023/4/24 9:15
 
 from setuptools import setup, find_packages
 
-ignore = ['test','tests']
+ignore = []
 
 setup(
     name='numpy-io',
-    version='0.0.2',
+    version='0.0.3',
     description='an easy training architecture',
     long_description='numpy-io: https://github.com/ssbuild/numpy-io.git',
     license='Apache License 2.0',
     url='https://github.com/ssbuild/numpy-io',
     author='ssbuild',
     author_email='9727464@qq.com',
     install_requires=[
```

## numpy_io/pytorch_loader/dataloaders.py

```diff
@@ -107,66 +107,28 @@
 
         if transform_fn is not None:
             dataset = dataset.map(transform_fn)
 
         dataset_ = torch_Dataset(dataset) if with_torchdataset else dataset
     return dataset_
 
-def load_random_sampler(files: typing.Union[typing.List, str],
-                        batch_size,
-                        collate_fn=None,
-                        pin_memory=False,
-                        shuffle: bool = False,
-                        infinite: bool = False,
-                        cycle_length: int = 4,
-                        block_length: int = 10,
-                        num_processes: int = 1,
-                        process_index: int = 0,
-                        backend='record',
-                        with_record_iterable_dataset: bool = False,
-                        with_load_memory: bool = False,
-                        with_torchdataset: bool = True,
-                        transform_fn: typing.Callable = None,
-                        check_dataset_file_fn=None,
-                        limit_start: typing.Optional[int] = None,
-                        limit_count: typing.Optional[int] = None,
-                        dataset_loader_filter_fn: typing.Callable = None,
-                        **kwargs
-                        ) -> typing.Optional[typing.Union[
-    DataLoader, torch.utils.data.Dataset, torch.utils.data.IterableDataset, IterableDatasetBase, RandomDatasetBase]]:
-    dataset = load_dataset(
-        files, shuffle=shuffle, infinite=infinite, cycle_length=cycle_length,
-        block_length=block_length, num_processes=num_processes, process_index=process_index,
-        backend=backend, with_record_iterable_dataset=with_record_iterable_dataset,
-        with_load_memory=with_load_memory, with_torchdataset=with_torchdataset,
-        transform_fn=transform_fn, check_dataset_file_fn=check_dataset_file_fn,
-        limit_start=limit_start,
-        limit_count=limit_count,
-        dataset_loader_filter_fn=dataset_loader_filter_fn,
-    )
-    if dataset is None:
-        return None
-    return DataLoader(dataset, batch_size=batch_size,
-                      shuffle=False if isinstance(dataset, IterableDataset) else shuffle,
-                      collate_fn=collate_fn,
-                      pin_memory=pin_memory, **kwargs)
 
 
 
 
-def load_distributed_random_sampler(
-                                    files: typing.Union[typing.List, str],
+def load_distributed_random_sampler(files: typing.Union[typing.List, str],
                                     batch_size,
                                     num_processes: int = 1,
                                     process_index: int = 0,
                                     collate_fn=None,
                                     pin_memory=False,
                                     backend='record',
                                     with_load_memory: bool = False,
                                     with_torchdataset: bool = True,
+                                    shuffle=True,
                                     transform_fn: typing.Callable = None,
                                     check_dataset_file_fn=None,
                                     limit_start: typing.Optional[int] = None,
                                     limit_count: typing.Optional[int] = None,
                                     dataset_loader_filter_fn: typing.Callable = None,
                                     **kwargs
                                     ):
@@ -178,60 +140,67 @@
         limit_start=limit_start,
         limit_count=limit_count,
         dataset_loader_filter_fn=dataset_loader_filter_fn,
     )
     if dataset is None:
         return None
 
-    sampler = torch.utils.data.distributed.DistributedSampler(dataset,num_replicas=num_processes,rank=process_index) if num_processes > 1 else None
+    sampler = torch.utils.data.distributed.DistributedSampler(dataset,
+                                                              num_replicas=num_processes,
+                                                              rank=process_index,
+                                                              shuffle=shuffle) if num_processes > 1 else None
+
+    if not shuffle:
+        do_shuffle = False
+    else:
+        do_shuffle = sampler is None
+
     return DataLoader(dataset, batch_size=batch_size,
-                      shuffle=sampler is None,
+                      shuffle=do_shuffle,
                       sampler=sampler,
                       collate_fn=collate_fn,
                       pin_memory=pin_memory, **kwargs)
 
 
 
 
 
-
-def load_sequential_sampler(files: typing.Union[typing.List, str],
-                 batch_size,
-                 collate_fn=None,
-                 pin_memory=False,
-                 shuffle: bool=False,
-                 infinite: bool=False,
-                 cycle_length: int=4,
-                 block_length: int=10,
-                 num_processes: int = 1,
-                 process_index: int = 0,
-                 backend='record',
-                 with_record_iterable_dataset: bool = False,
-                 with_load_memory: bool = False,
-                 with_torchdataset: bool = True,
-                 transform_fn : typing.Callable = None,
-                 check_dataset_file_fn=None,
-                limit_start: typing.Optional[int] = None,
-                limit_count: typing.Optional[int] = None,
-                dataset_loader_filter_fn: typing.Callable = None,
-                **kwargs
-                            ) -> typing.Optional[typing.Union[DataLoader,torch.utils.data.Dataset,torch.utils.data.IterableDataset,IterableDatasetBase,RandomDatasetBase]]:
-
+def load_random_sampler(files: typing.Union[typing.List, str],
+                        batch_size,
+                        collate_fn=None,
+                        pin_memory=False,
+                        shuffle: bool = False,
+                        infinite: bool = False,
+                        cycle_length: int = 4,
+                        block_length: int = 10,
+                        num_processes: int = 1,
+                        process_index: int = 0,
+                        backend='record',
+                        with_record_iterable_dataset: bool = False,
+                        with_load_memory: bool = False,
+                        with_torchdataset: bool = True,
+                        transform_fn: typing.Callable = None,
+                        check_dataset_file_fn=None,
+                        limit_start: typing.Optional[int] = None,
+                        limit_count: typing.Optional[int] = None,
+                        dataset_loader_filter_fn: typing.Callable = None,
+                        **kwargs
+                        ) -> typing.Optional[typing.Union[
+    DataLoader, torch.utils.data.Dataset, torch.utils.data.IterableDataset, IterableDatasetBase, RandomDatasetBase]]:
     dataset = load_dataset(
-        files,shuffle=shuffle,
-        infinite=infinite,
-        cycle_length=cycle_length,
-        block_length=block_length,num_processes=num_processes,process_index=process_index,
-        backend=backend,with_record_iterable_dataset=with_record_iterable_dataset,
-        with_load_memory=with_load_memory,with_torchdataset=with_torchdataset,
-        transform_fn=transform_fn,check_dataset_file_fn=check_dataset_file_fn,
+        files, shuffle=shuffle, infinite=infinite, cycle_length=cycle_length,
+        block_length=block_length, num_processes=num_processes, process_index=process_index,
+        backend=backend, with_record_iterable_dataset=with_record_iterable_dataset,
+        with_load_memory=with_load_memory, with_torchdataset=with_torchdataset,
+        transform_fn=transform_fn, check_dataset_file_fn=check_dataset_file_fn,
         limit_start=limit_start,
         limit_count=limit_count,
         dataset_loader_filter_fn=dataset_loader_filter_fn,
     )
     if dataset is None:
         return None
-    return DataLoader(dataset,
-                      batch_size=batch_size,
-                      shuffle=shuffle,
+    return DataLoader(dataset, batch_size=batch_size,
+                      shuffle=False if isinstance(dataset, IterableDataset) else shuffle,
                       collate_fn=collate_fn,
-                      pin_memory=pin_memory,**kwargs)
+                      pin_memory=pin_memory, **kwargs)
+
+
```

## Comparing `numpy_io-0.0.2.dist-info/RECORD` & `numpy_io-0.0.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 numpy_io/__init__.py,sha256=aCtpF76c1Jz1-xvsEqeV_ze4a40-KqaqUtIrFy3BTcU,77
-numpy_io/setup.py,sha256=jK7HyvhIBkduPyo2ITT3dQ7JJUUqJu6e0mI1W-m7QGg,637
+numpy_io/setup.py,sha256=FpSWP9evO_39j97Ojgd_T8wUYdKMwZyPdX9sxeBAbds,623
 numpy_io/core/__init__.py,sha256=gvmkt5S6jF7SlAsFM1e9qGGXV96a5yTB5lBavIVjuKo,80
 numpy_io/core/numpyadapter.py,sha256=REFrhsPVHfQmdSu73_1j1NBfA929Y9xtaxx5cNxlJxM,12381
 numpy_io/core/parallel.py,sha256=7pxBQ7w26H5wo1gHEMJwFwrkl57PDUA7rF3y8GD5kjM,5457
 numpy_io/core/reader.py,sha256=-i7NiW3s1gPFwaM03tDWT0NLVG6FEkz6fOuo_nWB3r8,1894
 numpy_io/core/writer.py,sha256=ck68384PW4RY6osFhl7XFjqszztoW0zuSN_DEhUOuqY,1366
 numpy_io/examples/__init__.py,sha256=H6PH5pOOHNUW3_RuUpgWfpv6_Pijqyy_3U1JCTLl6jg,54
 numpy_io/examples/auto_parallel_writer.py,sha256=IBxAiuxCdouZAlWVoc98U7taEnnl17iFn6y9rafYMes,2708
@@ -17,12 +17,14 @@
 numpy_io/examples/record_shuffle_example.py,sha256=TFFnJOqgtOZZ8s8j4bZ2Ju16PyAt3Q5X17anhbfI9mg,1398
 numpy_io/examples/record_writer_example.py,sha256=VtgDxRxbs-tXVbNRo78TImVe48rioqvoKtOhTmwA1F8,3056
 numpy_io/examples/testing/__init__.py,sha256=Jj2ycuBs45i9qAcrC6iCm22QOY46Xujv9lzOSbeeZ_o,56
 numpy_io/examples/testing/lmdb_test.py,sha256=rQvokJAIDW9esAesab9wHs03OcG2TPImAuybnCO-LBA,2658
 numpy_io/examples/testing/test_mem.py,sha256=gteaDLS79vwwfJETTeL-JCxn3VhRT3So59y5AV4ah9w,613
 numpy_io/examples/testing/test_mutiprocess.py,sha256=rgO758tNAycWGYxyJl2AM2jkffNQs-AjRU9peSotGzQ,2907
 numpy_io/pytorch_loader/__init__.py,sha256=oRU1cnNHyp22vA9HkEYfoPtpdQdU4D9scv9KtgxYVdE,73
-numpy_io/pytorch_loader/dataloaders.py,sha256=amz1H9mT_T2OTgbDKjOW2YgiubNwvhSINAo2aiMZsEU,10268
-numpy_io-0.0.2.dist-info/METADATA,sha256=rE8uWKaDyqonnrzyR24_LsOenrvYcwtTowUJ6QBXLys,364
-numpy_io-0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-numpy_io-0.0.2.dist-info/top_level.txt,sha256=mV0ZVKt8HA3kBLuj9iZkff1sq-cR9hE36TgSw_7Mr4E,9
-numpy_io-0.0.2.dist-info/RECORD,,
+numpy_io/pytorch_loader/data_helper.py,sha256=FOrVkAHUXml3M4rQGFXkHz9VYLlw2jY6ilxS5tLLwnw,4528
+numpy_io/pytorch_loader/dataloaders.py,sha256=Ub_ojjmjxQESDmf25ZPjCqGtIjqzz01kElLe7tvUzZk,8631
+numpy_io/pytorch_loader/tokenizer_config_helper.py,sha256=8hoofhL7uMyE8pT-U_3WNKDyy5DBOqQhDwJMZri-InY,3780
+numpy_io-0.0.3.dist-info/METADATA,sha256=3pZ1FSxw4LPkn4iFYAIBeQWxNWlXXf-yI_VbljsTUX0,401
+numpy_io-0.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+numpy_io-0.0.3.dist-info/top_level.txt,sha256=mV0ZVKt8HA3kBLuj9iZkff1sq-cR9hE36TgSw_7Mr4E,9
+numpy_io-0.0.3.dist-info/RECORD,,
```

