# Comparing `tmp/haloop-0.0.7.tar.gz` & `tmp/haloop-0.0.8.tar.gz`

## Comparing `haloop-0.0.7.tar` & `haloop-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 haloop-0.0.7/.github/workflows/release.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/__init__.py
--rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/attention.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/beam.py
--rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/ctc.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/data.py
--rw-r--r--   0        0        0    14041 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/loop.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/model.py
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/resnet.py
--rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/rnnlm.py
--rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/scan.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/star.py
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/symbol_tape.py
--rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/transducer.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/xen.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 haloop-0.0.7/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 haloop-0.0.7/LICENSE
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 haloop-0.0.7/README.md
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 haloop-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 haloop-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 haloop-0.0.8/.github/workflows/release.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/__init__.py
+-rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/attention.py
+-rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/beam.py
+-rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/ctc.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/data.py
+-rw-r--r--   0        0        0    14572 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/loop.py
+-rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/lora.py
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/model.py
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/resnet.py
+-rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/rnnlm.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/scan.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/star.py
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/symbol_tape.py
+-rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/transducer.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 haloop-0.0.8/ha/xen.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 haloop-0.0.8/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 haloop-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 haloop-0.0.8/README.md
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 haloop-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 haloop-0.0.8/PKG-INFO
```

### Comparing `haloop-0.0.7/.github/workflows/release.yml` & `haloop-0.0.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `haloop-0.0.7/ha/attention.py` & `haloop-0.0.8/ha/attention.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import sys
 
 import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+from . import lora
 
 def new_gelu(x):
     """
     Implementation of the GELU activation function currently in Google BERT repo (identical to OpenAI GPT).
     Reference: Gaussian Error Linear Units (GELU) paper: https://arxiv.org/abs/1606.08415
     """
     return 0.5 * x * (1.0 + torch.tanh(math.sqrt(2.0 / math.pi) * (x + 0.044715 * torch.pow(x, 3.0))))
@@ -42,23 +43,27 @@
         self.c_proj = nn.Linear(config.n_embd, config.n_embd, bias=config.bias)
         # regularization
         self.resid_dropout = nn.Dropout(config.dropout)
         self.n_head = config.n_head
         self.n_embd = config.n_embd
         self.dropout = config.dropout
 
-    def forward(self, x):
+    def forward(self, x, past=None):
         B, T, C = x.size() # batch size, sequence length, embedding dimensionality (n_embd)
 
         # calculate query, key, values for all heads in batch and move head forward to be the batch dim
-        q, k ,v  = self.c_attn(x).split(self.n_embd, dim=2)
+        q, k, v  = self.c_attn(x).split(self.n_embd, dim=2)
         k = k.view(B, T, self.n_head, C // self.n_head).transpose(1, 2) # (B, nh, T, hs)
         q = q.view(B, T, self.n_head, C // self.n_head).transpose(1, 2) # (B, nh, T, hs)
         v = v.view(B, T, self.n_head, C // self.n_head).transpose(1, 2) # (B, nh, T, hs)
 
+        if past is not None:
+            k_cache, v_cache = past
+            k, v = torch.cat([k_cache, k], dim=2), torch.cat([v_cache, v], dim=-2)
+
         # causal self-attention; Self-attend: (B, nh, T, hs) x (B, nh, hs, T) -> (B, nh, T, T)
         bias = torch.tril(x.new_ones(T, T)).view(1, 1, T, T)
 
         att = (q @ k.transpose(-2, -1)) * (1.0 / (k.size(-1)**0.5))
         att = att.masked_fill(bias == 0, float('-inf'))
         att = att.softmax(dim=-1) # (B, nh, T, T)
 
@@ -68,15 +73,15 @@
         # attend
         y = att @ v # (B, nh, T, T) x (B, nh, T, hs) -> (B, nh, T, hs)
 
         y = y.transpose(1, 2).contiguous().view(B, T, C) # re-assemble all head outputs side by side
 
         # output projection
         y = self.resid_dropout(self.c_proj(y))
-        return y, att_entropy
+        return y, att_entropy, torch.stack([k, v])
 
 
 class MLP(nn.Module):
     def __init__(self, config):
         super().__init__()
         self.c_fc    = nn.Linear(config.n_embd, 4 * config.n_embd, bias=config.bias)
         self.c_proj  = nn.Linear(4 * config.n_embd, config.n_embd, bias=config.bias)
@@ -94,19 +99,19 @@
     def __init__(self, config):
         super().__init__()
         self.ln_1 = LayerNorm(config.n_embd, bias=config.bias)
         self.attn = MonitoredCausalSelfAttention(config)
         self.ln_2 = LayerNorm(config.n_embd, bias=config.bias)
         self.mlp = MLP(config)
 
-    def forward(self, x):
-        x_attn, att_entropy = self.attn(self.ln_1(x))
+    def forward(self, x, past=None):
+        x_attn, att_entropy, present = self.attn(self.ln_1(x), past=past)
         x = x + x_attn
         x = x + self.mlp(self.ln_2(x))
-        return x
+        return x, att_entropy, present
 
 
 class GPT(nn.Module):
     def __init__(self, config):
         super().__init__()
         self.config = config
 
@@ -128,139 +133,177 @@
             h = nn.ModuleList([Block(config) for _ in range(config.n_layer)]),
             ln_f = LayerNorm(config.n_embd, bias=config.bias),
         ))
 
         self.lm_head = nn.Linear(config.n_embd, config.vocab_size, bias=False)
         self.transformer.wte.weight = self.lm_head.weight # https://paperswithcode.com/method/weight-tying
 
-    def forward(self, input_ids):
+    def forward(self,
+                input_ids, # (B, T)
+                past=None # (nlayers, 2, B, nh, T, hs)
+                ):
         device = input_ids.device
         b, t = input_ids.size()
+        if past is None:
+            t0 = 0
+            past = torch.zeros(self.config.n_layer, 2, b, self.config.n_head, t0, self.config.n_embd // self.config.n_head, device=device)
+        else:
+            t0 = past.size(-2)
+            t = t0 + t
         assert t <= self.config.block_size, f"Cannot forward sequence of length {t}, block size is only {self.config.block_size}"
-        pos = torch.arange(0, t, dtype=torch.long, device=device).unsqueeze(0) # shape (1, t)
+
+        pos = torch.arange(t0, t, dtype=torch.long, device=device).unsqueeze(0) # shape (1, t)
 
         tok_emb = self.transformer.wte(input_ids) # token embeddings of shape (b, t, n_embd)
         pos_emb = self.transformer.wpe(pos) # position embeddings of shape (1, t, n_embd)
         x = self.transformer.drop(tok_emb + pos_emb)
-        for block in self.transformer.h:
-            x = block(x)
+
+        present = past.new_empty((self.config.n_layer, 2, b, self.config.n_head, t, self.config.n_embd // self.config.n_head))
+        for i, block in enumerate(self.transformer.h):
+            x, _att_entropy, present[i] = block(x, past=past[i])
         x = self.transformer.ln_f(x)
 
         logits = self.lm_head(x[:, [-1], :]) # note: using list [-1] to preserve the time dim
 
-        return logits
+        return logits, present
 
 
 @torch.inference_mode()
 def generate(self, input_ids, max_new_tokens, temperature=1.0, top_k=None, stop_token=50256):
     """
     Take a conditioning sequence of indices input_ids (LongTensor of shape (b,t)) and complete
     the sequence max_new_tokens times, feeding the predictions back into the model each time.
     Most likely you'll want to make sure to be in model.eval() mode of operation for this.
     """
+    past = None
     for _ in range(max_new_tokens):
-        # if the sequence context is growing too long we must crop it at block_size
-        input_ids_cond = input_ids if input_ids.size(1) <= self.config.block_size else input_ids[:, -self.config.block_size:]
-        # forward the model to get the logits for the index in the sequence
-        logits = self(input_ids_cond)
+        if input_ids.size(1) >= self.config.block_size:
+            # kv cache becomes useless here, we stop using and updating it
+            past = None
+            # if the past context is growing too long we must crop it at block_size
+            input_ids_cond = input_ids[:, -self.config.block_size:]
+            # forward the model to get the logits for the index in the sequence
+            logits, _ = self(input_ids_cond, past=None)
+        elif past is None:
+            # forward the condition for the first time and warm up the cache
+            logits, past = self(input_ids, past=None)
+        else:
+            # forward the last token in the sequence along with the cache
+            logits, past = self(input_ids[:, [-1]], past=past)
+
         # pluck the logits at the final step and scale by desired temperature
         logits = logits[:, -1, :] / temperature
         # optionally crop the logits to only the top k options
         if top_k is not None:
             v, _ = torch.topk(logits, min(top_k, logits.size(-1)))
             logits[logits < v[:, [-1]]] = -float('Inf')
         # apply softmax to convert logits to (normalized) probabilities
         probs = F.softmax(logits, dim=-1)
         # sample from the distribution
         input_ids_next = torch.multinomial(probs, num_samples=1)
+
         if input_ids_next == stop_token:
             # time to stop
             break
         else:
             # append sampled index to the running sequence and continue
             input_ids = torch.cat((input_ids, input_ids_next), dim=1)
 
-    return input_ids
+        yield input_ids_next
 
 
 @dataclass
 class GPTConfig:
     block_size: int = 1024
     vocab_size: int = 50304 # GPT-2 vocab_size of 50257, padded up to nearest multiple of 64 for efficiency
     n_layer: int = 12
     n_head: int = 12
     n_embd: int = 768
     dropout: float = 0.0
     bias: bool = False
     stable_embedding: bool = False
 
 
+def load_model(ckpt_path, *, map_location):
+    checkpoint = torch.load(ckpt_path, map_location=map_location)
+
+    if not 'vocab_size' in checkpoint['model_args']:
+        # assume checkpoint for a large model
+
+        checkpoint['model_args']['stable_embedding'] = True
+        checkpoint['model_args']['vocab_size'] = 50257
+        checkpoint['model_args']['bias'] = True
+
+        gptconf = GPTConfig(**checkpoint['model_args'])
+        model = nn.ModuleDict({'_orig_mod': GPT(gptconf)})
+        model.load_state_dict(checkpoint['model'], strict=False)
+    elif '_orig_mod.transformer.h.0.attn.c_attn.lora_A.weight' in checkpoint['model']:
+        gptconf = GPTConfig(**checkpoint['model_args'])
+        model = nn.ModuleDict({'_orig_mod': GPT(gptconf)})
+        lora.attach_to_c_attn(model)
+        model.load_state_dict(checkpoint['model'])
+    else:
+        gptconf = GPTConfig(**checkpoint['model_args'])
+        model = nn.ModuleDict({'_orig_mod': GPT(gptconf)})
+        model.load_state_dict(checkpoint['model'])
+
+    model.eval()
+    model.to(map_location)
+    model = model._orig_mod
+
+    return model
+
+
 @torch.inference_mode()
 def main():
     import argparse
     from rich.prompt import Prompt
 
     try:
         import sentencepiece as spm
     except ImportError:
         print("Please install sentencepiece with: pip install sentencepiece", file=sys.stderr)
         raise
 
     parser = argparse.ArgumentParser('GPT REPL')
     parser.add_argument('--device', type=str, default='cuda')
     parser.add_argument('--seed', type=int, default=1337)
-    parser.add_argument('--steps', type=int, default=1024)
+    parser.add_argument('--steps', type=int, default=10)
     parser.add_argument('--spm', type=str, required=True)
-    parser.add_argument('--top-k', type=int, default=5)
-    parser.add_argument('--temperature', type=float, default=0.8)
+    parser.add_argument('--top-k', type=int, default=1)
+    parser.add_argument('--temperature', type=float, default=1.0)
     parser.add_argument('ckpt_path')
     args = parser.parse_args()
 
     device = args.device
     torch.manual_seed(args.seed)
     torch.backends.cuda.matmul.allow_tf32 = True # allow tf32 on matmul
     torch.backends.cudnn.allow_tf32 = True # allow tf32 on cudnn
 
-    checkpoint = torch.load(args.ckpt_path, map_location=device)
-
-    if not 'vocab_size' in checkpoint['model_args']:
-        # assume checkpoint for a large model
-
-        checkpoint['model_args']['stable_embedding'] = True
-        checkpoint['model_args']['vocab_size'] = 50257
-        checkpoint['model_args']['bias'] = True
-
-        gptconf = GPTConfig(**checkpoint['model_args'])
-        model = nn.ModuleDict({'_orig_mod': GPT(gptconf)})
-        model.load_state_dict(checkpoint['model'], strict=False)
-    else:        
-        gptconf = GPTConfig(**checkpoint['model_args'])
-        model = nn.ModuleDict({'_orig_mod': GPT(gptconf)})
-        model.load_state_dict(checkpoint['model'])
-
-    model.eval()
-    model.to(device)
-    model = model._orig_mod
+    model = load_model(args.ckpt_path, map_location=device)
 
     sp = spm.SentencePieceProcessor(model_file=args.spm)
 
+    import time
+
     while True:
         prompt = Prompt.ask('prompt>-')
         start = [50256] + sp.encode(prompt)
         x = (torch.tensor(start, dtype=torch.long, device=device)[None, ...])
 
-        with torch.amp.autocast(device_type="cuda", dtype=torch.bfloat16):
-            y = generate(model, x, args.steps, temperature=args.temperature, top_k=args.top_k)
+        t0 = time.time()
 
-        y = y[0].tolist()
-        _prefix, gen = y[:len(start)], y[len(start):]
-        try:
-            eot = gen.index(50256)
-            gen = gen[:eot]
-        except ValueError:
-            pass
+        with torch.amp.autocast(device_type="cuda", dtype=torch.bfloat16):
+            for i, token_id in enumerate(generate(model, x, args.steps, temperature=args.temperature, top_k=args.top_k)):
+                token_id = token_id.item()
+                piece = sp.id_to_piece(token_id)
+                if piece.startswith('▁'):
+                    print(' ', end='')
+                    piece = piece[1:]
+                print(piece, end='', flush=True)
 
-        print(sp.decode(gen))
+        t1 = time.time()
+        print(f' ({i+1} tokens in {t1-t0:.2f}s)', file=sys.stderr)
 
 
 if __name__ == '__main__':
-    main()
+    main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `haloop-0.0.7/ha/beam.py` & `haloop-0.0.8/ha/beam.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.7/ha/ctc.py` & `haloop-0.0.8/ha/ctc.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.7/ha/data.py` & `haloop-0.0.8/ha/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,57 +4,73 @@
 import torchaudio
 from kaldialign import align
 
 
 def make_frames(wav):
     frames = torchaudio.compliance.kaldi.mfcc(wav)
 
+    # utterance-level CMVN
+    frames -= frames.mean(dim=0)
+    frames /= frames.std(dim=0)
+
     # frames = torchaudio.compliance.kaldi.fbank(wav, num_mel_bins=80)
     # frames += 8.
     # frames /= 4.
+
     return frames # (T, F)
 
 
 class Directory(torch.utils.data.Dataset):
     def __init__(self, path: Path):
         super().__init__()
         self.files = list(path.glob("*.wav"))
 
     def __len__(self):
         return len(self.files)
 
+    def utt_id(self, index):
+        return self.files[index].stem
+
     def __getitem__(self, index):
         wav, sr = torchaudio.load(self.files[index])
         assert sr == 16000
-        return make_frames(wav), "the quick brown fox jumps over the lazy dog"
+        return index, make_frames(wav), "the quick brown fox jumps over the lazy dog"
 
 
 class LibriSpeech(torch.utils.data.Dataset):
     def __init__(self, url='train-clean-100'):
         super().__init__()
         self.librispeech = torchaudio.datasets.LIBRISPEECH('.', url=url, download=True)
 
     def __len__(self):
         return len(self.librispeech)
 
+    def utt_id(self, index):
+        wav, sr, text, speaker_id, chapter_id, utterance_id = self.librispeech[index]
+        utt_id = f'{speaker_id}-{chapter_id}-{utterance_id}'
+        return utt_id
+
     def __getitem__(self, index):
         wav, sr, text, speaker_id, chapter_id, utterance_id = self.librispeech[index]
-        return make_frames(wav), text
+        return index, make_frames(wav), text
 
 
 class Mask(torch.utils.data.Dataset):
     def __init__(self, dataset):
         super().__init__()
         self.dataset = dataset
 
     def __len__(self):
         return len(self.dataset)
 
+    def utt_id(self, index):
+        return self.dataset.utt_id(index)
+
     def __getitem__(self, index):
-        frames, text = self.dataset[index]
+        index, frames, text = self.dataset[index]
 
         frames = frames[None,None,:]
 
         frames = torchaudio.functional.mask_along_axis_iid(
             frames,
             mask_param=2, # mask a little bit as we have only 13 components
             mask_value=0,
@@ -64,36 +80,39 @@
         frames = torchaudio.functional.mask_along_axis_iid(
             frames,
             mask_param=7,
             mask_value=0,   
             axis=2 # time
         )
 
-        return frames[0, 0, :], text
+        return index, frames[0, 0, :], text
 
 
 class WordDrop(torch.utils.data.Dataset):
     def __init__(self, dataset, p_drop_words=0.4):
         super().__init__()
         self.dataset = dataset
         self.p_drop_words = p_drop_words
 
     def __len__(self):
         return len(self.dataset)
 
+    def utt_id(self, index):
+        return self.dataset.utt_id(index)
+
     def __getitem__(self, index):
-        frames, original_text = self.dataset[index]
+        index, frames, original_text = self.dataset[index]
         generator = torch.Generator().manual_seed(index)
         text = ' '.join(w for w in original_text.split(' ') if torch.rand(1, generator=generator) > self.p_drop_words)
         if not text:
             text = original_text
         if False:
             hyp, _ref = list(zip(*align(text.split(), original_text.split(), '*')))
             print(index, ' '.join(h.replace(' ', '_') for h in hyp))
-        return frames, text
+        return index, frames, text
 
 
 def make_dataset(s):
     match s.split(':', maxsplit=1):
         case [subset]:
             return LibriSpeech(subset)
         case ['head', subset]:
```

### Comparing `haloop-0.0.7/ha/loop.py` & `haloop-0.0.8/ha/loop.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import time
 from itertools import chain
 from pathlib import Path
+import sys
 
-from rich.console import Console
 import torch
 import torch.nn as nn
 import torch.utils.data
 from kaldialign import edit_distance, align
 import wandb
 
 from .data import concat_datasets
@@ -16,30 +16,31 @@
 from .resnet import FixupResNet, FixupBasicBlock
 from .xen import Vocabulary
 from . import symbol_tape
 from .rnnlm import LM
 from .transducer import transducer_forward_score
 from .ctc import ctc_reduce_mean
 
-console = Console()
-def print(*args, flush=False, **kwargs):
-    console.log(*args, **kwargs)
+
+def log(*args, flush=False, **kwargs):
+    print(*args, **kwargs, flush=flush, file=sys.stderr)
 
 
 class Collator:
     def __init__(self, vocabulary):
         self.vocabulary = vocabulary
 
     def __call__(self, batch):
-        input_lengths = torch.tensor([len(b[0]) for b in batch])
-        inputs = torch.nn.utils.rnn.pad_sequence([b[0] for b in batch], batch_first=True)
-        targets = [self.vocabulary.encode(b[1]) for b in batch]
+        batch_indices = torch.tensor([b[0] for b in batch])
+        input_lengths = torch.tensor([len(b[1]) for b in batch])
+        inputs = torch.nn.utils.rnn.pad_sequence([b[1] for b in batch], batch_first=True)
+        targets = [self.vocabulary.encode(b[2]) for b in batch]
         target_lengths = torch.tensor([len(t) for t in targets])
-        targets = torch.nn.utils.rnn.pad_sequence(targets, batch_first=True, padding_value=0)
-        return inputs, targets, input_lengths, target_lengths
+        targets = torch.nn.utils.rnn.pad_sequence(targets, batch_first=True, padding_value=-100)
+        return batch_indices, inputs, targets, input_lengths, target_lengths
 
 
 class System(nn.Module):
     def __init__(self, args):
         super().__init__()
         self.args = args
 
@@ -48,14 +49,16 @@
                 self.encoder = Encoder().to(args.device)
             case "r9":
                 self.encoder = FixupResNet(FixupBasicBlock, [5,5,5]).to(args.device)
 
         match args.vocab:
             case "bytes":
                 self.vocab = symbol_tape.Vocabulary.bytes()
+            case "ascii":
+                self.vocab = symbol_tape.Vocabulary.ascii()
             case "cmu":
                 self.vocab = Vocabulary(add_closures=False)
             case "xen":
                 self.vocab = Vocabulary(add_closures=True)
 
         match args.star_penalty:
             case None:
@@ -87,15 +90,15 @@
     def load_state_dict(self, checkpoint):
         self.encoder.load_state_dict(checkpoint['encoder'])
         self.recognizer.load_state_dict(checkpoint['recognizer'])
         self.scaler.load_state_dict(checkpoint['scaler'])
         self.optimizer.load_state_dict(checkpoint['optimizer'])
         self.vocab.load_state_dict(checkpoint['vocab'])
         if self.lm is not None:
-            print('loading transducer lm')
+            log('loading transducer lm')
             self.lm.load_state_dict(checkpoint['lm'])
 
     def make_state_dict(self, **extra):
         return {
             'encoder': self.encoder.state_dict(),
             'recognizer': self.recognizer.state_dict(),
             'scaler': self.scaler.state_dict(),
@@ -110,15 +113,15 @@
 
         N, _, _ = inputs.shape
         inputs = inputs.to(device) # (N, T, C)
         targets = targets.to(device) # (N, U)
         input_lengths = input_lengths.to(device) # (N,)
         target_lengths = target_lengths.to(device) # (N,)
 
-        #print(inputs, targets) # works best with --batch-size 1
+        #log(inputs, targets) # works best with --batch-size 1
 
         input_lengths = self.encoder.subsampled_lengths(input_lengths)
 
         with torch.autocast(device_type='cuda', dtype=torch.float16):
             outputs = self.encoder(inputs) # (N1, T, C)
 
             if self.lm is not None:
@@ -138,121 +141,123 @@
                 joint = outputs[:, :, None, :] + lm_outputs[:, None, :, :] # (N, T, U1, C)
                 #joint = joint.log_softmax(dim=-1)
 
                 #loss = ctc_reduce_mean(transducer_forward_score(joint, targets, input_lengths, target_lengths), target_lengths)
 
                 from torchaudio.functional import rnnt_loss
                 loss = rnnt_loss(joint,
-                                    targets.to(torch.int32),
-                                    input_lengths.to(torch.int32),
-                                    target_lengths.to(torch.int32),
-                                    blank=0, reduction='mean', fused_log_softmax=True)
+                                 targets.to(torch.int32),
+                                 input_lengths.to(torch.int32),
+                                 target_lengths.to(torch.int32),
+                                 blank=0, reduction='mean', fused_log_softmax=True)
+                logits = joint # FIXME:
             else:
                 #
                 # All outputs are independent
                 #
-                loss = self.recognizer(outputs, targets, input_lengths, target_lengths)
+                loss, logits = self.recognizer(outputs, targets, input_lengths, target_lengths)
 
-        return loss, outputs
+        return loss, outputs, logits
 
     def train_one_epoch(self, epoch, train_loader):
         encoder, recognizer, optimizer, scaler = self.encoder, self.recognizer, self.optimizer, self.scaler
 
         optimizer.zero_grad()
         encoder.train()
         recognizer.train()
 
         train_loss = 0.
         t0 = time.time()
-        for i, (inputs, targets, input_lengths, target_lengths) in enumerate(train_loader):
-            loss, _ = self.forward(inputs, targets, input_lengths, target_lengths)
+        for i, (_batch_indices, inputs, targets, input_lengths, target_lengths) in enumerate(train_loader):
+            loss, _, _ = self.forward(inputs, targets, input_lengths, target_lengths)
 
             if torch.isnan(loss):
-                print(f'[{epoch + 1}, {i + 1:5d}], loss is nan, skipping batch', flush=True)
+                log(f'[{epoch + 1}, {i + 1:5d}], loss is nan, skipping batch', flush=True)
                 scaler.update()
                 continue
 
             if torch.isinf(loss):
-                print(f'[{epoch + 1}, {i + 1:5d}], loss is inf, skipping batch, skipping scaler update', flush=True)
+                log(f'[{epoch + 1}, {i + 1:5d}], loss is inf, skipping batch, skipping scaler update', flush=True)
                 continue
 
             scaler.scale(loss).backward()
             scaler.unscale_(optimizer)
-            grad_norm = torch.nn.utils.clip_grad_norm_(chain(encoder.parameters(), recognizer.parameters()), 0.1)
+            grad_norm = torch.nn.utils.clip_grad_norm_(chain(encoder.parameters(), recognizer.parameters()), self.args.clip_grad_norm)
             if self.lm:
-                grad_norm = 0.5*(grad_norm + torch.nn.utils.clip_grad_norm_(self.lm.parameters(), 0.1))
+                grad_norm = 0.5*(grad_norm + torch.nn.utils.clip_grad_norm_(self.lm.parameters(), self.args.clip_grad_norm))
             if torch.isinf(grad_norm) or torch.isnan(grad_norm):
-                print(f'[{epoch + 1}, {i + 1:5d}], grad_norm is inf or nan, skipping batch', flush=True)
+                log(f'[{epoch + 1}, {i + 1:5d}], grad_norm is inf or nan, skipping batch', flush=True)
                 scaler.update()
                 optimizer.zero_grad(set_to_none=True)
                 continue
 
             scaler.step(optimizer)
             scaler.update()
             optimizer.zero_grad(set_to_none=True)
 
             train_loss += loss.item()
             if i and i % self.args.log_interval == 0:
                 train_loss = train_loss / self.args.log_interval
                 t1 = time.time()
-                print(f'[{epoch + 1}, {i + 1:5d}] time: {t1-t0:.3f} loss: {train_loss:.3f} grad_norm: {grad_norm:.3f}', flush=True)
+                log(f'[{epoch + 1}, {i + 1:5d}] time: {t1-t0:.3f} loss: {train_loss:.3f} grad_norm: {grad_norm:.3f}', flush=True)
                 wandb.log({'train/loss': train_loss, 'train/grad_norm': grad_norm})
                 t0 = t1
                 train_loss = 0.
 
     @torch.inference_mode()
     def evaluate(self, epoch, valid_loader):
         encoder, recognizer, vocabulary = self.encoder, self.recognizer, self.vocab
 
         valid_loss = 0.
         lers = []
 
         encoder.eval()
         recognizer.eval()
-        for i, (inputs, targets, input_lengths, target_lengths) in enumerate(valid_loader):
-            loss, outputs = self.forward(inputs, targets, input_lengths, target_lengths)
+        for i, (dataset_indices, inputs, targets, input_lengths, target_lengths) in enumerate(valid_loader):
+            loss, outputs, logits = self.forward(inputs, targets, input_lengths, target_lengths)
 
             valid_loss += loss.item()
 
-            if i < 10:
-                for ref, ref_len, seq, hyp_len in zip(targets, target_lengths, outputs, input_lengths):
-                    seq = seq[:hyp_len].cpu()
-                    ref = ref[:ref_len].cpu().tolist()
-                    #print('greedy', seq.argmax(dim=-1).tolist())
-                    decoded = ctc_beam_search_decode_logits(seq)
-                    hyp1 = vocabulary.decode(filter(None, decoded[0][0]))
-                    ref1 = vocabulary.decode(ref)
-
-                    dist = edit_distance(hyp1, ref1)
-                    dist['length'] = len(ref1)
-                    dist['ler'] = round(dist['total'] / dist['length'], 2)
-                    lers.append(dist['ler'])
-
-                    if isinstance(ref1, str):
-                        star = '*'
-                        hyp, ref = list(zip(*align(hyp1, ref1, star)))
-
-                        if i == 0:
-                            console.print('hyp', ' '.join(h.replace(' ', '_') for h in hyp), overflow='crop')
-                            console.print('ref', ' '.join(r.replace(' ', '_') for r in ref), overflow='crop')
-                            print(dist)
-                    else:
-                        star = 42 # b'*'
-                        hyp, ref = list(zip(*align(hyp1, ref1, star)))
-                        hyp, ref = bytes(hyp), bytes(ref)
-
-                        if i == 0:
-                            console.print('hyp', hyp)
-                            console.print('ref', ref)
-                            print(dist)
-
+            for dataset_index, ref, ref_len, seq, hyp_len in zip(dataset_indices, targets, target_lengths, logits, input_lengths):
+                seq = seq[:hyp_len].cpu()
+                ref = ref[:ref_len].cpu().tolist()
+                ali = seq.argmax(dim=-1)
+
+                greedy = [i for i in torch.unique_consecutive(ali, dim=-1).tolist() if i]
+                hyp1 = vocabulary.decode(greedy)
+
+                #decoded_seqs, _decoded_logits = ctc_beam_search_decode_logits(seq) # FIXME: too slow
+                #hyp1 = vocabulary.decode(filter(None, decoded_seqs[0]))
+
+                ref1 = vocabulary.decode(ref)
+                ali = vocabulary.decode(ali.tolist())
+
+                dist = edit_distance(hyp1, ref1)
+                dist['length'] = len(ref1)
+                dist['ler'] = round(dist['total'] / dist['length'], 2)
+                lers.append(dist['ler'])
+
+                if isinstance(ref1, str):
+                    star = '␣'
+                    hyp, ref = list(zip(*align(hyp1, ref1, star)))
+                    hyp, ref = ''.join(hyp), ''.join(ref)
+                else:
+                    star = 42 # b'*'
+                    hyp, ref = list(zip(*align(hyp1, ref1, star)))
+                    hyp, ref = bytes(hyp), bytes(ref)
+
+                dataset_index = dataset_index.item()
+                print(epoch, dataset_index, 'hyp', self.vocab.format(hyp), sep="\t", flush=True)
+                print(epoch, dataset_index, 'ref', self.vocab.format(ref), sep="\t", flush=True)
+                print(epoch, dataset_index, 'ali', self.vocab.format(ali), sep="\t", flush=True)
+                print(epoch, dataset_index, 'stat', dist, sep="\t", flush=True)
 
         count = i + 1
         ler = round(sum(lers) / len(lers), 3)
-        print(f'valid [{epoch + 1}, {i + 1:5d}] loss: {valid_loss / count:.3f} sample ler: {ler:.3f}', flush=True)
+        log(f'valid [{epoch + 1}, {i + 1:5d}] loss: {valid_loss / count:.3f} ler: {ler:.3f}', flush=True)
         if wandb.run is not None:
             wandb.log({'valid/loss': valid_loss / count, 'valid/ler': ler})
         return valid_loss / count
 
 
 def make_parser():
     class Formatter(argparse.ArgumentDefaultsHelpFormatter,
@@ -269,22 +274,23 @@
     parser.add_argument('--lr', type=float, default=3e-4, help="Adam learning rate")
     parser.add_argument('--train', type=str, help="Datasets to train on, comma separated")
     parser.add_argument('--eval', type=str, default='dev-clean', help="Datasets to evaluate on, comma separated")
     parser.add_argument('--encoder', type=str, default='lstm', choices=['lstm', 'r9'], help="Encoder to use: unidirectional LSTM or ResNet")
     parser.add_argument('--compile', action='store_true', help="torch.compile the model (produces incompatible checkpoints)")
     parser.add_argument('--star-penalty', type=float, default=None, help="Star penalty for Star CTC. If None, train with regular CTC")
     parser.add_argument('--num-workers', type=int, default=32, help="Number of workers for data loading")
-    parser.add_argument('--vocab', type=str, default='bytes', choices=['bytes', 'cmu', 'xen'], help="Vocabulary to use: raw bytes, CMUdict, Xen (CMUdict + glottal closures)")
+    parser.add_argument('--vocab', type=str, default='ascii', choices=['bytes', 'ascii', 'cmu', 'xen'], help="Vocabulary to use: raw bytes, ascii, CMUdict, Xen (CMUdict + glottal closures)")
     parser.add_argument('--lm', type=Path, help="Path to language model checkpoint trained with hal.")
+    parser.add_argument('--clip-grad-norm', type=float, default=0.1, help="Clip gradient norm to this value")
     return parser
 
 
 def main():
     args = make_parser().parse_args()
-    print(args)
+    log(args)
 
     torch.manual_seed(3407)
 
     system = System(args)
 
     valid_loader = torch.utils.data.DataLoader(
         concat_datasets(args.eval),
@@ -294,20 +300,20 @@
         num_workers=args.num_workers,
     )
 
     if args.init:
         checkpoint = torch.load(args.init, map_location=args.device)
         system.load_state_dict(checkpoint)
     else:
-        print('initializing randomly')
+        log('initializing randomly')
 
     if args.compile:
         system = torch.compile(system, mode='reduce-overhead')
 
-    print('model parameters', sum(p.numel() for p in system.parameters() if p.requires_grad))
+    log('model parameters', sum(p.numel() for p in system.parameters() if p.requires_grad))
 
     if args.train:
         wandb.init(project='ha', config=args)
 
         train_loader = torch.utils.data.DataLoader(
             concat_datasets(args.train),
             collate_fn=Collator(system.vocab),
@@ -320,14 +326,14 @@
         best_valid_loss = float('inf')
         for epoch in range(args.num_epochs):
             system.train_one_epoch(epoch, train_loader)
 
             valid_loss = system.evaluate(epoch, valid_loader)
             if valid_loss < best_valid_loss:
                 best_valid_loss = valid_loss
-                print('saving model', args.save)
+                log('saving model', args.save)
                 torch.save(system.make_state_dict(best_valid_loss=best_valid_loss, epoch=epoch), args.save)
     else:
         system.evaluate(-100, valid_loader)
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `haloop-0.0.7/ha/model.py` & `haloop-0.0.8/ha/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         x = self.dropout(x)
         x, _ = self.lstm(x)
         return x.relu()
 
 
 
 class CTCRecognizer(nn.Module):
-    def __init__(self, feat_dim=1024, vocab_size=55+1):
+    def __init__(self, feat_dim=1024, vocab_size=256):
         super().__init__()
         self.ctc = nn.CTCLoss(blank=0)
         self.classifier = nn.Linear(feat_dim, vocab_size)
         self.dropout = nn.Dropout(0.2)
 
     def log_probs(self, features):
         features = self.dropout(features)
@@ -45,19 +45,19 @@
     def forward(self, features, targets, input_lengths=None, target_lengths=None):
         if input_lengths is None:
             input_lengths = torch.full((features.shape[0],), features.shape[1], dtype=torch.long)
         if target_lengths is None:
             target_lengths = torch.full((features.shape[0],), len(targets), dtype=torch.long)
 
         with torch.autocast(device_type='cuda', dtype=torch.float32):
-            logits = self.log_probs(features).to(torch.float32)
-            logits = logits.permute(1, 0, 2) # T, N, C
-            loss = self.ctc(logits, targets, input_lengths=input_lengths, target_lengths=target_lengths)
+            logits = self.log_probs(features)
+            logits1 = logits.to(torch.float32).permute(1, 0, 2) # T, N, C
+            loss = self.ctc(logits1, targets, input_lengths=input_lengths, target_lengths=target_lengths)
             #loss = ctc_reduce_mean(ctc_forward_score3(logits, targets, input_lengths, target_lengths), target_lengths)
-            return loss
+            return loss, logits
 
 
 class StarRecognizer(nn.Module):
     def __init__(self, feat_dim=1024, vocab_size=55+1, star_penalty=-1):
         super().__init__()
         self.classifier = nn.Linear(feat_dim, vocab_size)
         self.dropout = nn.Dropout(0.2)
```

### Comparing `haloop-0.0.7/ha/resnet.py` & `haloop-0.0.8/ha/resnet.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.7/ha/rnnlm.py` & `haloop-0.0.8/ha/rnnlm.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.7/ha/scan.py` & `haloop-0.0.8/ha/scan.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.7/ha/star.py` & `haloop-0.0.8/ha/star.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.7/ha/symbol_tape.py` & `haloop-0.0.8/ha/symbol_tape.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 from pathlib import Path
 import sys
 import math
 
 
 class Vocabulary:
-    def __init__(self, pad_token="<pad>", unk_token='<unk>'):
+    def __init__(self, pad_token="·", unk_token="∞"):
         self.id_to_string = {}
         self.string_to_id = {}
 
         # add the default pad token
         self.id_to_string[0] = pad_token
         self.string_to_id[pad_token] = 0
 
@@ -36,54 +36,85 @@
 
     def __len__(self):
         return len(self.id_to_string)
 
     def add_new_word(self, string):
         self.string_to_id[string] = len(self.string_to_id)
         self.id_to_string[len(self.id_to_string)] = string
+        return self.string_to_id[string]
 
     # Given a string, return ID
     def get_idx(self, string, extend_vocab=False):
-        byte = bytes([ord(string)])
+        try:
+            byte = bytes([ord(string)])
+            if byte in self.string_to_id:
+                return self.string_to_id[byte]
+        except ValueError:
+            pass
+
         if string in self.string_to_id:
             return self.string_to_id[string]
-        elif byte in self.string_to_id:
-            return self.string_to_id[byte]
         elif extend_vocab:  # add the new word
-            self.add_new_word(string)
-            return self.string_to_id[string]
+            return self.add_new_word(string)
         else:
             return self.unk_id
 
     def encode(self, text, extend_vocab=False):
-        return torch.LongTensor([self.get_idx(char, extend_vocab=extend_vocab) for char in text])
+        try:
+            return torch.LongTensor([self.get_idx(char, extend_vocab=extend_vocab) for char in text])
+        except:
+            import ipdb; ipdb.set_trace()
 
     def decode(self, ids):
         if isinstance(self.id_to_string[0], bytes):
             return b''.join([self.id_to_string[id] for id in ids])
         else:
             return ''.join([self.id_to_string[id] for id in ids])
 
     @classmethod
-    def bytes(cls):
+    def bytes(cls, n=256):
         self = Vocabulary(pad_token=0, unk_token=7)
         self.id_to_string = {}
         self.string_to_id = {}
 
-        for x in range(256):
+        for x in range(n):
             byte = bytes([x])
-            y = self.get_idx(byte, extend_vocab=True)
+            y = self.add_new_word(byte)
             assert x == y
             if x == 0: # nul
                 self.pad_id = x
             elif x == 7: # bel
                 self.unk_id = x
 
         return self
 
+    @classmethod
+    def ascii(cls):
+        self = Vocabulary(pad_token=0, unk_token=7)
+        self.id_to_string = {}
+        self.string_to_id = {}
+
+        for i, x in enumerate("""ε␁␂␃␄␅␆␇␈␉␤⇥␌␍␎␏␐␑␒␓␔␕␖␗␘␙␚␛␜␝␞␟ !"#$%&'()*+,-./0123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\ ]^_`abcdefghijklmnopqrstuvwxyz{|}~␡"""):
+            y = self.add_new_word(x)
+            assert y == i
+            if i == 0: # nul
+                self.pad_id = x
+            elif i == 7: # bel
+                self.unk_id = x
+
+        return self
+
+    def format(self, s):
+        if isinstance(s, bytes):
+            try:
+                s = s.decode('utf-8')
+            except UnicodeDecodeError:
+                pass
+        return s
+
 
 def tokenize_bytes(text_file, vocab, extend_vocab=False, device='cpu'):
     if vocab is None:
         vocab = Vocabulary.bytes()
 
     print(f"Memory mapping bytes from: {text_file}", file=sys.stderr)
     s = torch.ByteStorage.from_file(str(text_file), size=Path(text_file).stat().st_size, shared=False)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `haloop-0.0.7/ha/transducer.py` & `haloop-0.0.8/ha/transducer.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.7/ha/xen.py` & `haloop-0.0.8/ha/xen.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,7 +62,9 @@
                   for phoneme in self.closures.get(c, [c])]
         targets = torch.LongTensor([self.dictionary[phoneme] for phoneme in labels])
         return targets
 
     def decode(self, labels):
         return ['' if l == 0 else self.rdictionary[l-1] for l in labels]
 
+    def format(self, string):
+        return ' '.join(c.replace(' ', '_') for c in string)
```

### Comparing `haloop-0.0.7/LICENSE` & `haloop-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `haloop-0.0.7/README.md` & `haloop-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `haloop-0.0.7/pyproject.toml` & `haloop-0.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 dependencies = [
   "click",
   "g2p-en",
   "kaldialign",
   "rich",
   "torch",
   "torchaudio",
+  "wandb",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/proger/ha1#readme"
 Issues = "https://github.com/proger/ha1/issues"
 Source = "https://github.com/proger/ha1"
```

### Comparing `haloop-0.0.7/PKG-INFO` & `haloop-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haloop
-Version: 0.0.7
+Version: 0.0.8
 Summary: speech agent for 100 hours
 Project-URL: Documentation, https://github.com/proger/ha1#readme
 Project-URL: Issues, https://github.com/proger/ha1/issues
 Project-URL: Source, https://github.com/proger/ha1
 Author-email: Volodymyr Kyrylov <vol@wilab.org.ua>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
@@ -17,14 +17,15 @@
 Requires-Python: >=3.9
 Requires-Dist: click
 Requires-Dist: g2p-en
 Requires-Dist: kaldialign
 Requires-Dist: rich
 Requires-Dist: torch
 Requires-Dist: torchaudio
+Requires-Dist: wandb
 Description-Content-Type: text/markdown
 
 # haloop
 
 [![PyPI Version](https://img.shields.io/pypi/v/haloop.svg)](https://pypi.python.org/pypi/haloop)
 
 Haloop is a speech agent toolkit. Haloop provides `hac` program for acoustic model training, `hal` for RNN language model training and evaluation and `hat` for attention decoder LM. The package is available on PyPI:
```

