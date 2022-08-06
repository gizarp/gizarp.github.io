---
layout: page
title: projects
permalink: /projects/
description: Here are some things I have been working on.
nav: true
---

<!---
To have side-by-side pictures and text blocks, use the following template:
(see https://talk.jekyllrb.com/t/inclusion-image-on-left-side-and-text-on-the-right-side-using-markdown-in-jekyll-site/3413/9)
<div style="clear: both;">
  <div style="float: left; margin-right 1em; padding-right: 25px">
    <img src="/assets/img/sq-land-doig-tree.png" alt="" width="150px" height="200px">
  </div>
  <div>
    <h5>Parameterizing Branch-and-Bound Search Trees to Learn Branching Policies</h5>
    <p>
        We tackle variable selection in Branch-and-Bound (B&B) for Mixed-Integer Linear Programming (MILP) problems, 
seeking policies that generalize across heterogeneous MILPs.
We develop new parameterizations of the candidate variables and of the search trees, and design DNN architectures to handle them.
Our results show that incorporating a search-tree context to modulate branching aids generalization, with better test accuracy and smaller B&B trees.
        <br><br>
        <a href="https://github.com/ds4dm/branch-search-trees" target="_blank"> [code] </a>
        <a href="https://ojs.aaai.org/index.php/AAAI/article/view/16512" target="_blank"> [paper] </a>
        <a href="/assets/pdf/AAAI21-poster-gzarpellon.pdf" target="_blank" > [poster] </a>
    </p>
  </div>
</div>
-->

- **Learning to Cut by Looking Ahead: Cutting Plane Selection via Imitation Learning**<br>
    <small style="font-size: 85%; color:gray">Joint with Max B. Paulus, Andreas Krause, Laurent Charlin and Chris J. Maddison. ICML 2022.</small>
    <br>
        <a href="https://proceedings.mlr.press/v162/paulus22a.html" target="_blank"> [paper] </a>
    <br>
    We propose a new neural architecture (NeuralCut) for cut selection in Mixed-Integer Linear Programming (MILP). 
    We train our model by imitation of a novel "lookahead" expert rule, which explicitly measures which cuts yield the best bound improvement.
    Our model outperforms standard baselines for cut selection on several synthetic MILP benchmarks and shows its full potential when
    deployed in a realistic MILP solver.
  
- **A Classifier to Decide on the Linearization of MIQPs in CPLEX** +<br>
  **Learning a Classification of Mixed-Integer Quadratic Programming Problems**<br>
    <small style="font-size: 85%; color:gray">Joint with Pierre Bonami and Andrea Lodi. Operations Research 2022 + CPAIOR 2018.</small>
    <br>
        <a href="https://github.com/ds4dm/miqp-clf2lin" target="_blank"> [code] </a>
        <a href="https://pubsonline.informs.org/doi/abs/10.1287/opre.2022.2267" target="_blank"> [2022 paper] </a>
        <a href="https://link.springer.com/chapter/10.1007/978-3-319-93031-2_43" target="_blank"> [2018 paper] </a>
    <br>
    We translate the algorithmic question of whether to linearize convex Mixed-Integer Quadratic Programming problems (MIQPs) into a classification task, 
    and use machine learning techniques to tackle it. We represent MIQPs and the linearization decision by careful target and feature engineering, 
    designing learning experiments and evaluation metrics. As a practical result, we deploy a SVM regression+classification pipeline deciding on MIQP 
    linearization in the IBM-CPLEX 12.10.0 commercial solver.

- **Parameterizing Branch-and-Bound Search Trees to Learn Branching Policies**<br>
    <small style="font-size: 85%; color:gray">Joint with Jason Jo, Andrea Lodi and Yoshua Bengio. AAAI 2021.</small>
    <br>
        <a href="https://github.com/ds4dm/branch-search-trees" target="_blank"> [code] </a>
        <a href="https://ojs.aaai.org/index.php/AAAI/article/view/16512" target="_blank"> [paper] </a>
        <a href="/assets/pdf/AAAI21-poster-gzarpellon.pdf" target="_blank" > [poster] </a>
    <br>
    We tackle variable selection in Branch-and-Bound (B&B) for Mixed-Integer Linear Programming (MILP) problems, 
    seeking policies that generalize across heterogeneous MILPs.
    We develop new parameterizations of the candidate variables and of the search trees, and design DNN architectures to handle them.
    Our results show that incorporating a search-tree context to modulate branching aids generalization, with better test accuracy and smaller B&B trees.
  
- **Learning MILP Resolution Outcomes Before Reaching Time-Limit**<br>
    <small style="font-size: 85%; color:gray">Joint with Martina Fischetti and Andrea Lodi. CPAIOR 2019.</small>
    <br>
        <a href="https://github.com/ds4dm/milp-outcome" target="_blank"> [code] </a>
        <a href="https://link.springer.com/chapter/10.1007/978-3-030-19212-9_18" target="_blank"> [paper] </a>
    <br>
    Looking at the evolution of a partial branch-and-bound (B&B) tree for a MILP instance, we aim to predict whether the problem will be solved 
    to proven optimality before timing out. We exploit machine learning tools, and summarize time-series information from the 
    MILP resolution process to cast a prediction within a classification framework. Experiments show that a valuable statistical pattern can indeed be learned during B&B optimization, 
    with key predictive features reflecting the know-how and experience of field’s practitioners.
  
- **On learning and branching: a survey**<br>
    <small style="font-size: 85%; color:gray">Joint with Andrea Lodi. TOP 2017.</small>
    <br>
        <a href="https://link.springer.com/article/10.1007/s11750-017-0451-6" target="_blank"> [paper] </a>
    <br>
    We survey learning techniques to deal with the two most crucial decisions in the branch-and-bound algorithm for Mixed-Integer Linear Programming, 
    namely variable and node selections. We interpret some early contributions in the light of modern learning techniques, 
    and give the details of the recent algorithms that instead explicitly incorporate machine learning paradigms.
  