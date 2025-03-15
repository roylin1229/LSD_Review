# A Comprehensive Review of Image Line Segment Detection and Description: Taxonomies, Comparisons, and Challenges

This repository contains the code and supplementary materials for the paper titled **"A Comprehensive Review of Image Line Segment Detection and Description: Taxonomies, Comparisons, and Challenges"**, published in IEEE TPAMI 2024. The paper provides a comprehensive review of existing methods for detecting and describing line segments in images, along with taxonomies, comparisons, and challenges in the field.

## Links
- [IEEE TPAMI 2024 Link](https://ieeexplore.ieee.org/document/10530374)
- [arXiv Preprint Link](https://arxiv.org/abs/2305.00264)
- [GitHub Evaluation Code](https://github.com/roylin1229/line_segment_review)

## Authors
- **Xinyu Lin**<sup>1</sup> ([roylin_cv@163.com](mailto:roylin_cv@163.com))
- **Yingjie Zhou**<sup>2</sup>
- **Yipeng Liu**<sup>1</sup>
- **Ce Zhu**<sup>1*</sup>

### Affiliations
<sup>1</sup>University of Electronic Science and Technology of China  
<sup>2</sup>Sichuan University

## Abstract
An image line segment is a fundamental low-level visual feature that delineates straight, slender, and uninterrupted portions of objects and scenarios within images. Detection and description of line segments lay the basis for numerous vision tasks. Although many studies have aimed to detect and describe line segments, a comprehensive review is lacking, obstructing their progress. This study fills the gap by comprehensively reviewing related studies on detecting and describing two-dimensional image line segments to provide researchers with an overall picture and deep understanding. Based on their mechanisms, two taxonomies for line segment detection and description are presented to introduce, analyze, and summarize these studies, facilitating researchers to learn about them quickly and extensively. The key issues, core ideas, advantages and disadvantages of existing methods, and their potential applications for each category are analyzed and summarized, including previously unknown findings. The challenges in existing methods and corresponding insights for potentially solving them are also provided to inspire researchers. In addition, some state-of-the-art line segment detection and description algorithms are evaluated without bias, and the evaluation code will be publicly available. The theoretical analysis, coupled with the experimental results, can guide researchers in selecting the best method for their intended vision applications. Finally, this study provides insights for potentially interesting future research directions to attract more attention from researchers to this field.

![Figure 1: The structure of this review and high-level taxonomies of existing line segment detection and description methods.](line_segment_taxonomy.jpg)

## References
```bibtex
@ARTICLE{10530374,
  author={Lin, Xinyu and Zhou, Yingjie and Liu, Yipeng and Zhu, Ce},
  journal={IEEE Transactions on Pattern Analysis and Machine Intelligence},
  title={A Comprehensive Review of Image Line Segment Detection and Description: Taxonomies, Comparisons, and Challenges},
  year={2024},
  volume={46},
  number={12},
  pages={8074-8093},
  keywords={Image segmentation;Reviews;Task analysis;Image edge detection;Feature extraction;Taxonomy;Motion segmentation;Line segment description;line segment detection;line segment matching;low-level feature},
  doi={10.1109/TPAMI.2024.3400881}
}
```

## Citation
X. Lin, Y. Zhou, Y. Liu and C. Zhu, "A Comprehensive Review of Image Line Segment Detection and Description: Taxonomies, Comparisons, and Challenges," in *IEEE Transactions on Pattern Analysis and Machine Intelligence*, vol. 46, no. 12, pp. 8074-8093, Dec. 2024, doi: 10.1109/TPAMI.2024.3400881.

## A Collection of Line Segment Detection Algorithms
The tables below will be continuously updated as new methods and advancements emerge.

### Global Hough-based Methods
<iframe class="resizable-iframe" src="detection_global_hough.html"></iframe>

### Local-based Methods (Gradient Grouping-based Methods)
<iframe class="resizable-iframe" src="detection_gradient_grouping.html"></iframe>

### Local-based Methods (Edge Fitting-based Methods)
<iframe class="resizable-iframe" src="detection_edge_fitting.html"></iframe>

### Deep Learning-based Methods
<iframe class="resizable-iframe" src="detection_deep_learning.html"></iframe>

### Hybrid Methods
<iframe class="resizable-iframe" src="detection_hybrid.html"></iframe>

### Other Methods
<iframe class="resizable-iframe" src="detection_other.html"></iframe>

## A Collection of Line Segment Description Algorithms
The tables below will be continuously updated as new methods and advancements emerge.

### Statistic-based Methods
<iframe class="resizable-iframe" src="description_statistic.html"></iframe>

### Structure-based Methods
<iframe class="resizable-iframe" src="description_structure.html"></iframe>

### Deep Learning-based Methods
<iframe class="resizable-iframe" src="description_learning.html"></iframe>

## A Collection of Reviews and Evaluations for Line Segment Detection and Description
The tables below will be continuously updated as new methods and advancements emerge.
<iframe class="resizable-iframe" src="review_evaluation.html"></iframe>

<script>
  function resizeIframe(iframe) {
    iframe.style.height = (iframe.contentWindow.document.body.scrollHeight + 20) + 'px';
  }
  window.onload = function () {
    const iframes = document.querySelectorAll('.resizable-iframe');
    iframes.forEach(iframe => {
      iframe.onload = () => resizeIframe(iframe);
      resizeIframe(iframe); 
    });
  };
  window.addEventListener('resize', function () {
    const iframes = document.querySelectorAll('.resizable-iframe');
    iframes.forEach(iframe => resizeIframe(iframe));
  });
</script>
```