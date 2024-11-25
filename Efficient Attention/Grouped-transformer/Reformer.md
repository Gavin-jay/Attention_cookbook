> # Reformer: The Efficient Transformer
>
> * Training typical transformer models can usually be prohibitively costly, epecially on long sequences. The time complexity is O(L*L).
> * So the authors propose a novel model, which referring to Reformer. They introduce two techniques to improve the efficiency of the Transformers.
> * For one, they replace dot-product attention by one that uses locality-sensitive hashing.
> * Approximate attention computation based on locality-sensitive hashing replaces the O(L2) factor in attention layers with O(L log L) and so allows operating on long sequences.
>
> [http://arxiv.org/abs/2001.04451](https://)
>
