# Notes for Decomposition of Differentials in Health Expectancies from Multistate Life Tables
***Wanying Ling***

This is a code note for the decomposition approach to healthy life expectancy based on multistate life tables (Shen et.al, [*2023*](https://doi.org/10.1215/00703370-11058373)).

## Functions

It contains seven functions:

### Function 1: l0_func

**l0_func** : Function for obtaining baseline population health structure.

### Function 2: lx_func

**lx_func** : Function for obtaining $l_x$

### Function 3: P_func

**P_func** : Function for obtaining the matrix of transition probabilities.

### Function 4: All_P_func

**All_P_func** : Function for obtaining \$ \prod\_{k=x}\^{\beta-1} \mathbf{P}\_k}\$.

### Function 5: SUM_func

**SUM_func** : Function for obtaining $\mathbb{e}_x$ (Status­Based­HLE­and­ULE).

### Function 6: HLE_func

**HLE_func** : Function for obtaining $e_x$ (Popualtion­Based LE,­HLE­and­ULE).

### Function 7: Decom_func

**Decom_func** : Function for obtaining component from the initial population $\dot{\mathbf{l}}_\alpha \cdot{ }_{\beta-\alpha} \mathbb{e}_\alpha$.

### Function 8: DecomByTrans_func

**DecomByTrans_func** : Function for decomposition of differences in transition probabilities.

## Dataset

The dataset **BASELINE.csv** includes the initial health structure of the population. It contains four variables:

-   **state**: health state (with 1 and 2, healthy and unhealthy respectively)

-   **ragender**: gender

-   **pro**: proportion of the population in that health state (they are rescaled to 1 by sex and iteration to calculated the HLE for male and female separately)

-   **iter**: bootstrap iteration number

The dataset **PROB.csv** includes the transition probabilities by age. It contains seven variables:

-   **pre_state**: the initial state

-   **ragender**: gender

-   **age**: age

-   **iter**: bootstrap iteration number

-   **A**: probability to "Healthy" given the initial state

-   **L**: probability to "Unhealthy" given the initial state

-   **H**: probability to "Death" given the initial state

## Table 1 - Panel A : Baseline population health structure­(Table 1 - Panel A)

## Table 1 - Panel B : Status Based HLE and ULE­(Table 1 - Panel B)

## Table 1 - Panel C : Population Based HLE and ULE

## Table 2 - Panel A: Difference in Expectancies

## Table 2 - Panel B: From Initial Population

## Table 2 - Panel C: From Transitions

## Table 2 - Panel D: From Each Transition Probability

For other enquiries related to the note and codes, please email lingwany@connect.hku.hk
