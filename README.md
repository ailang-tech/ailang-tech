# ailang.tech

**R4 — neural networks built on quaternion algebra.** ailang.tech is the public
site for two research projects that use quaternions — four-component numbers —
as the carrier for a network's weights and activations, in place of ordinary
real-valued vectors.

### R4-Iteron — word roles learned by intervention, not correlation

Remove a piece of a sentence, re-run, and see whether the answer changes. What
changes was necessary to it, and that test is the learning signal rather than a
statistical fit to examples. There is no backpropagation — the weights are
solved for directly — and word boundaries are learned rather than looked up in
a list.

### R4-Attn — bidirectional byte infill with signed attention

Predict a missing byte from the text on both sides of it, cloze-style as in
BERT, instead of committing left to right. The scores are signed and there is
no softmax, so a negative score is a first-class "this is actively wrong" —
a softmax, whose outputs are non-negative and sum to one, can only say
"unlikely". It sits in the linear-attention family, so cost grows linearly with
sequence length rather than quadratically.

### On the site

Plain-English and technical write-ups of both projects, interactive visualizers
of the shared algebra, and in-browser demos — one of which runs a small but
genuinely trained R4-Attn model client-side, with real weights.

**[ailang.tech](https://ailang.tech)**

Both are research artifacts, not products. The research code is private, so
there is no source on this account; what is public lives on the site.
