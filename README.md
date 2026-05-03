# Attention as Linear Algebra

Deck 10 of the [Linear Algebra for AI / ML](https://github.com/BrendanJamesLynskey/LLM_Hub_Linear_Algebra) series.

**Live presentation:** https://brendanjameslynskey.github.io/Linear_Algebra_AI_10_Attention_as_Linear_Algebra/

Q, K, V are learned projections. The attention matrix is row-stochastic. The output is a row-by-row weighted average of value vectors. Read this way, attention loses its mystery and becomes a piece of crystallised linear algebra. Includes an interactive attention playground with mask, temperature and pattern presets.

## What's inside

- Scaled dot-product attention in one equation
- Q, K, V as learned down-projections of the residual stream
- $QK^\top$ as a rank-$\le d_h$ score matrix; the low-rank bottleneck and why multi-head solves it
- Softmax-rowwise as a row-stochastic matrix; the convex-combination interpretation
- $AV$ as a row-by-row weighted average of value rows &mdash; attention as routing, not creation
- Multi-head attention as block-diagonal projection; standard head-count regimes
- $W_O$ decomposition into $H$ sub-blocks; one-head-writes-one-direction interpretation
- QK circuit and OV circuit (Anthropic's mechanistic-interpretability framework)
- Causal, padding, sliding-window masks; bi-directional and prefix-LM variants
- GQA and MQA &mdash; sharing K and V across heads to cut KV cache by 8&ndash;$H\times$
- Interactive attention playground (induction-head pattern, previous-token pattern, mask switching, temperature)

Single-page HTML, KaTeX-rendered maths, no build step. Open `index.html` directly.
