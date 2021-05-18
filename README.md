# Template Matching
> really looking for a perfect match between template and image
> no real ML; works well with minimal changes between template and input
> also due to max value, won't find duplicate matches (multi-template matching)

pipeline is
- template
- image with a cup
- find the cup in the image

how? 
- sliding window
- left>right
- top>bottom
- compute a score "normalized correlation coefficient"
    - how well did the pixels match between template and target

In this notebook
- bright regions = higher matches
- darker regions = lower matches