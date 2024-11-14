> # Efficient content-based sparse attention with routing transformers
>
> * Our work proposes to learn dynamic sparse attention patterns that avoid allocating computation and memory to attend to content unrelated to the query of interest.
> * It combines the modeling flexibility of prior work on content-based sparse attention **with** the efficiency gains from approaches based on local, temporal sparse attention.
> * Our model, the Routing Transformer, endows self-attention with a sparse routing module based on online k-means while reducing the overall complexity of attention to O(n1.5d) from O(n2d) for sequence length n and hidden dimension d.
> * Our formulation avoids sparsemax variants and relies on clustering of attention instead. Each attention module considers a clustering of the space: The current time-step only attends to context belonging to the same cluster. In other words, the current time-step query is routed to a limited number of context elements through its cluster assignment.
> * Our proposed model, Routing Transformer, combines our efficient clustering-based sparse attention with classical local attention to reach excellent performance both for language and image generation\
> * Routing Transformer sets new state-of-the-art, while having comparable or fewer number of self-attention layers and heads, on Wikitext-103 (15.8 vs 18.3 perplexity), PG-19 (33.2 vs 33.6 perplexity), and on ImageNet-64 (3.43 vs 3.44 bits/dim). We also report competitive results on enwik-8 (0.99 vs 0.98 perplexity) and present ablations on CIFAR-10.
