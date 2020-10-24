# FiMDP Evaluations

This repository hosts notebooks that evaluate [FiMDP]. 

### FiMDP vs Stormm Comparison
The notebook [fimdp_and_storm_comparison.ipynb](fimdp_and_storm_comparison.ipynb) 
compares the performance of FiMDP with the popular open-source model checker 
[Storm]. [FiMDP] performs the analysis directly on a given consumption MDP, while 
[Storm] runs its analysis on a regular MDP with the energy constraints encoded into 
states and actions. The results from this experiment were discussed in first part of the
the *Evaluation* section of the TACAS submission. 

### Energy solvers Comparison
The [uuv_energysolvers_comparison.ipynb](uuv_energysolvers_comparison.ipynb) notebook
shows the practicality of strategies generated by sevaral variants of the energy
solvers implemented in [FiMDP]. This notebook contains a pregenerated simulation runs for each solver. In order to see them, mark the notebook as [trusted][trust] or see it at [nbviewer] using this [link](https://nbviewer.jupyter.org/github/FiMDP/FiMDP-Evaluation/blob/master/uuv_energysolvers_comparison.ipynb). 
The *Goal-leaning solvers* subsection of the *Evaluation* section in the TACAS submission. 

Both of the notebooks use environments from [FiMDPEnv].

## Requirements
In order to run these notebooks, you need the following Python libraries: 
```
pandas matplotlib numpy seaborn
```
Moreover, to run the comparison with Storm, you need to have [Stormpy] and [Storm] installed.



[FiMDP]: https://github.com/FiMDP/FiMDP
[FiMDPEnv]: https://github.com/FiMDP/FiMDPEnv 
[Storm]: https://www.stormchecker.org/
[Stormpy]: https://moves-rwth.github.io/stormpy/
[trust]: https://jupyter-notebook.readthedocs.io/en/stable/security.html#explicit-trust
[nbviewer]: https://nbviewer.jupyter.org/
