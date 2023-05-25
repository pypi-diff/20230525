# Comparing `tmp/haloop-0.0.8.tar.gz` & `tmp/haloop-0.0.9.tar.gz`

## Comparing `haloop-0.0.8.tar` & `haloop-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 haloop-0.0.8/.github/workflows/release.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/__init__.py
--rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/attention.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/beam.py
--rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/ctc.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/data.py
--rw-r--r--   0        0        0    14572 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/loop.py
--rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/lora.py
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/model.py
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/resnet.py
--rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/rnnlm.py
--rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/scan.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/star.py
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/symbol_tape.py
--rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/transducer.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/xen.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 haloop-0.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 haloop-0.0.8/LICENSE
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 haloop-0.0.8/README.md
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 haloop-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 haloop-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 haloop-0.0.9/.github/workflows/release.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/__init__.py
+-rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/attention.py
+-rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/beam.py
+-rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/ctc.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/data.py
+-rw-r--r--   0        0        0    15016 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/loop.py
+-rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/lora.py
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/model.py
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/resnet.py
+-rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/rnnlm.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/scan.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/star.py
+-rw-r--r--   0        0        0     7617 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/symbol_tape.py
+-rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/transducer.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 haloop-0.0.9/ha/xen.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 haloop-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 haloop-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 haloop-0.0.9/README.md
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 haloop-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 haloop-0.0.9/PKG-INFO
```

### Comparing `haloop-0.0.8/.github/workflows/release.yml` & `haloop-0.0.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `haloop-0.0.8/ha/attention.py` & `haloop-0.0.9/ha/attention.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.8/ha/beam.py` & `haloop-0.0.9/ha/beam.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.8/ha/ctc.py` & `haloop-0.0.9/ha/ctc.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.8/ha/data.py` & `haloop-0.0.9/ha/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,33 @@
     # frames = torchaudio.compliance.kaldi.fbank(wav, num_mel_bins=80)
     # frames += 8.
     # frames /= 4.
 
     return frames # (T, F)
 
 
+class LabelFile(torch.utils.data.Dataset):
+    def __init__(self, path: Path):
+        super().__init__()
+        with open(path) as f:
+            self.ark = dict(line.strip().split(maxsplit=1) for line in f)
+            self.filenames = list(self.ark.keys())
+
+    def __len__(self):
+        return len(self.filenames)
+
+    def utt_id(self, index):
+        return self.filenames[index]
+
+    def __getitem__(self, index):
+        wav, sr = torchaudio.load(self.filenames[index])
+        assert sr == 16000
+        return index, make_frames(wav), self.ark[self.filenames[index]]
+
+
 class Directory(torch.utils.data.Dataset):
     def __init__(self, path: Path):
         super().__init__()
         self.files = list(path.glob("*.wav"))
 
     def __len__(self):
         return len(self.files)
@@ -111,16 +130,18 @@
         return index, frames, text
 
 
 def make_dataset(s):
     match s.split(':', maxsplit=1):
         case [subset]:
             return LibriSpeech(subset)
+        case ['labels', label_file]:
+            return LabelFile(Path(label_file))
         case ['head', subset]:
-            return torch.utils.data.Subset(LibriSpeech(subset), range(16))
+            return torch.utils.data.Subset(make_dataset(subset), range(16))
         case ['wdrop.4', subset]:
             return WordDrop(make_dataset(subset), p_drop_words=0.4)
         case ['wdrop.1', subset]:
             return WordDrop(make_dataset(subset), p_drop_words=0.1)
         case ['mask', subset]:
             return Mask(make_dataset(subset))
```

### Comparing `haloop-0.0.8/ha/loop.py` & `haloop-0.0.9/ha/loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,34 +35,43 @@
         inputs = torch.nn.utils.rnn.pad_sequence([b[1] for b in batch], batch_first=True)
         targets = [self.vocabulary.encode(b[2]) for b in batch]
         target_lengths = torch.tensor([len(t) for t in targets])
         targets = torch.nn.utils.rnn.pad_sequence(targets, batch_first=True, padding_value=-100)
         return batch_indices, inputs, targets, input_lengths, target_lengths
 
 
+def make_vocab(vocab_descriptor):
+    match vocab_descriptor.split(':', maxsplit=1):
+        case ["bytes"]:
+            return symbol_tape.Vocabulary.bytes()
+        case ["ascii"]:
+            return symbol_tape.Vocabulary.ascii()
+        case ["cmu"]:
+            return Vocabulary(add_closures=False)
+        case ["xen"]:
+            return Vocabulary(add_closures=True)
+        case ["words", path]:
+            _, vocab = symbol_tape.tokenize_words(path, None)
+            return vocab
+        case _:
+            raise ValueError("Unknown vocabulary descriptor. Possible values: bytes|ascii|cmu|xen|words:path/to/vocab/words.txt")
+
+
 class System(nn.Module):
     def __init__(self, args):
         super().__init__()
         self.args = args
 
         match args.encoder:
             case "lstm":
                 self.encoder = Encoder().to(args.device)
             case "r9":
                 self.encoder = FixupResNet(FixupBasicBlock, [5,5,5]).to(args.device)
 
-        match args.vocab:
-            case "bytes":
-                self.vocab = symbol_tape.Vocabulary.bytes()
-            case "ascii":
-                self.vocab = symbol_tape.Vocabulary.ascii()
-            case "cmu":
-                self.vocab = Vocabulary(add_closures=False)
-            case "xen":
-                self.vocab = Vocabulary(add_closures=True)
+        self.vocab = make_vocab(args.vocab)
 
         match args.star_penalty:
             case None:
                 self.recognizer = CTCRecognizer(vocab_size=len(self.vocab)).to(args.device)
             case star_penalty:
                 self.recognizer = StarRecognizer(star_penalty=star_penalty,
                                                  vocab_size=len(self.vocab)).to(args.device)    
@@ -232,15 +241,19 @@
                 ali = vocabulary.decode(ali.tolist())
 
                 dist = edit_distance(hyp1, ref1)
                 dist['length'] = len(ref1)
                 dist['ler'] = round(dist['total'] / dist['length'], 2)
                 lers.append(dist['ler'])
 
-                if isinstance(ref1, str):
+                if isinstance(ref1, list):
+                    star = '␣'
+                    hyp, ref = list(zip(*align(hyp1, ref1, star)))
+                    ali = tuple(ali)
+                elif isinstance(ref1, str):
                     star = '␣'
                     hyp, ref = list(zip(*align(hyp1, ref1, star)))
                     hyp, ref = ''.join(hyp), ''.join(ref)
                 else:
                     star = 42 # b'*'
                     hyp, ref = list(zip(*align(hyp1, ref1, star)))
                     hyp, ref = bytes(hyp), bytes(ref)
@@ -274,15 +287,15 @@
     parser.add_argument('--lr', type=float, default=3e-4, help="Adam learning rate")
     parser.add_argument('--train', type=str, help="Datasets to train on, comma separated")
     parser.add_argument('--eval', type=str, default='dev-clean', help="Datasets to evaluate on, comma separated")
     parser.add_argument('--encoder', type=str, default='lstm', choices=['lstm', 'r9'], help="Encoder to use: unidirectional LSTM or ResNet")
     parser.add_argument('--compile', action='store_true', help="torch.compile the model (produces incompatible checkpoints)")
     parser.add_argument('--star-penalty', type=float, default=None, help="Star penalty for Star CTC. If None, train with regular CTC")
     parser.add_argument('--num-workers', type=int, default=32, help="Number of workers for data loading")
-    parser.add_argument('--vocab', type=str, default='ascii', choices=['bytes', 'ascii', 'cmu', 'xen'], help="Vocabulary to use: raw bytes, ascii, CMUdict, Xen (CMUdict + glottal closures)")
+    parser.add_argument('--vocab', type=str, default='ascii', help="Vocabulary to use: bytes|ascii|cmu|xen|words:path/to/words.txt")
     parser.add_argument('--lm', type=Path, help="Path to language model checkpoint trained with hal.")
     parser.add_argument('--clip-grad-norm', type=float, default=0.1, help="Clip gradient norm to this value")
     return parser
 
 
 def main():
     args = make_parser().parse_args()
```

### Comparing `haloop-0.0.8/ha/lora.py` & `haloop-0.0.9/ha/lora.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.8/ha/model.py` & `haloop-0.0.9/ha/model.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.8/ha/resnet.py` & `haloop-0.0.9/ha/resnet.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.8/ha/rnnlm.py` & `haloop-0.0.9/ha/rnnlm.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.8/ha/scan.py` & `haloop-0.0.9/ha/scan.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.8/ha/star.py` & `haloop-0.0.9/ha/star.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.8/ha/symbol_tape.py` & `haloop-0.0.9/ha/symbol_tape.py`

 * *Files 9% similar despite different names*

```diff
@@ -108,14 +108,33 @@
             try:
                 s = s.decode('utf-8')
             except UnicodeDecodeError:
                 pass
         return s
 
 
+class WordVocabulary(Vocabulary):
+    def get_idx(self, string, extend_vocab=False):
+        if string in self.string_to_id:
+            return self.string_to_id[string]
+        elif extend_vocab:  # add the new word
+            return self.add_new_word(string)
+        else:
+            return self.unk_id
+
+    def encode(self, text, extend_vocab=False):
+        return torch.LongTensor([self.get_idx(char, extend_vocab=extend_vocab) for char in text.split()])
+
+    def decode(self, ids):
+        return [self.id_to_string[id] for id in ids]
+
+    def format(self, s):
+        return s
+
+
 def tokenize_bytes(text_file, vocab, extend_vocab=False, device='cpu'):
     if vocab is None:
         vocab = Vocabulary.bytes()
 
     print(f"Memory mapping bytes from: {text_file}", file=sys.stderr)
     s = torch.ByteStorage.from_file(str(text_file), size=Path(text_file).stat().st_size, shared=False)
     data = torch.ByteTensor(s)
@@ -134,14 +153,28 @@
             for token in tokens:
                 full_text.append(vocab.get_idx(token, extend_vocab=extend_vocab))
 
     data = torch.tensor(full_text, device=device, dtype=torch.int16)
     return data, vocab
 
 
+def tokenize_words(text_file, vocab, extend_vocab=True, device='cpu'):
+    if vocab is None:
+        vocab = WordVocabulary()
+
+    full_text = []
+    print(f"Using word vocabulary from: {text_file}", file=sys.stderr)
+    with open(text_file, 'r') as text:
+        for line in text:
+            for token in line.strip().split():
+                full_text.append(vocab.get_idx(token, extend_vocab=extend_vocab))
+    print(f"Vocabulary size: {len(vocab)}", file=sys.stderr)
+    data = torch.tensor(full_text, device=device, dtype=torch.int16)
+    return data, vocab
+
 
 class SymbolTape:
     def __init__(self, data, batch_size, bptt_len, pad_id):
         self.batch_size = batch_size
         self.bptt_len = bptt_len
         self.pad_id = pad_id
         self.tape_len = math.ceil(len(data) / batch_size + 1)
```

### Comparing `haloop-0.0.8/ha/transducer.py` & `haloop-0.0.9/ha/transducer.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.8/ha/xen.py` & `haloop-0.0.9/ha/xen.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.8/LICENSE` & `haloop-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `haloop-0.0.8/README.md` & `haloop-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # haloop
 
 [![PyPI Version](https://img.shields.io/pypi/v/haloop.svg)](https://pypi.python.org/pypi/haloop)
 
-Haloop is a speech agent toolkit. Haloop provides `hac` program for acoustic model training, `hal` for RNN language model training and evaluation and `hat` for attention decoder LM. The package is available on PyPI:
+Haloop is an agent toolkit. It provides `hac` program for acoustic model training, `hal` program for language model training, and `hat` for agent testing. The package is available on PyPI:
 
 ```
 pip install haloop
 ```
 
-Currently, `hat` is a REPL for Ukrainian GPT-2 models from the paper [GPT-2 Metadata Pretraining Towards Instruction Finetuning for Ukrainian](https://github.com/proger/uk4b).
+By default, `hat` operates as a REPL for Ukrainian GPT-2 models from the paper [GPT-2 Metadata Pretraining Towards Instruction Finetuning for Ukrainian](https://github.com/proger/uk4b).
 
 To use `hat`, install some additional dependencies and models:
 
 ```
 pip install bitsandbytes sentencepiece
 
 wget https://a.wilab.org.ua/gpt/wiki.model  # sentencepiece tokenizer
```

### Comparing `haloop-0.0.8/pyproject.toml` & `haloop-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `haloop-0.0.8/PKG-INFO` & `haloop-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haloop
-Version: 0.0.8
+Version: 0.0.9
 Summary: speech agent for 100 hours
 Project-URL: Documentation, https://github.com/proger/ha1#readme
 Project-URL: Issues, https://github.com/proger/ha1/issues
 Project-URL: Source, https://github.com/proger/ha1
 Author-email: Volodymyr Kyrylov <vol@wilab.org.ua>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
@@ -24,21 +24,21 @@
 Requires-Dist: wandb
 Description-Content-Type: text/markdown
 
 # haloop
 
 [![PyPI Version](https://img.shields.io/pypi/v/haloop.svg)](https://pypi.python.org/pypi/haloop)
 
-Haloop is a speech agent toolkit. Haloop provides `hac` program for acoustic model training, `hal` for RNN language model training and evaluation and `hat` for attention decoder LM. The package is available on PyPI:
+Haloop is an agent toolkit. It provides `hac` program for acoustic model training, `hal` program for language model training, and `hat` for agent testing. The package is available on PyPI:
 
 ```
 pip install haloop
 ```
 
-Currently, `hat` is a REPL for Ukrainian GPT-2 models from the paper [GPT-2 Metadata Pretraining Towards Instruction Finetuning for Ukrainian](https://github.com/proger/uk4b).
+By default, `hat` operates as a REPL for Ukrainian GPT-2 models from the paper [GPT-2 Metadata Pretraining Towards Instruction Finetuning for Ukrainian](https://github.com/proger/uk4b).
 
 To use `hat`, install some additional dependencies and models:
 
 ```
 pip install bitsandbytes sentencepiece
 
 wget https://a.wilab.org.ua/gpt/wiki.model  # sentencepiece tokenizer
```

