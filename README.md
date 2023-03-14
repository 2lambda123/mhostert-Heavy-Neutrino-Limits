# Heavy Neutrino Limits


This package and repo tracks the constraints on the coupling and masses of heavy neutral leptons (HNL). 

All limits are kept track in this [![Google Spreadsheets](https://img.shields.io/badge/Google_Sheets-Database-brightgreen.svg)](https://docs.google.com/spreadsheets/d/1p_fslIlThKMOThGl4leporUsogq9TmgXwILntUZOscg/edit?usp=sharing)

* We consider single flavor dominance scenarios, where the HNL mixes predominantly with either the electron, muon, or tau flavor. 

* In addition, following the [accompanying paper](www.arxiv.org/abs/XXXXXXX), we also recast limits and derived new ones on the Wilson coefficients of dimesnion-six $\nu$SMEFT operators as a function of the HNL mass $m_N$.

* So far, the code keeps track of limits in the region 1 MeV $< m_N < 100$ GeV.

Additions, comments, or suggestions should be directed to:
   
* Josu Hernández-García (garcia.josu.hernandez@ttk.elte.hu)
* Matheus Hostert (mhostert@pitp.ca)

--- 
**Citation info:**

```
@article{Fernandez-Martinez2023:xxx, 
xxx
}
```
   


---
## Limits on the mixing

Current compilation of bounds:


[<img src="https://render.githubusercontent.com/render/math?math=\color{black}{|U_{e N}|^2}">](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UeN_majorana.png#gh-light-mode-only)
[<img src="https://render.githubusercontent.com/render/math?math=\color{white}{|U_{e N}|^2}">](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UeN_majorana.png#gh-dark-mode-only)
![e flavor](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UeN_majorana.png#gh-light-mode-only)
![e flavor](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UeN_majorana_white.png#gh-dark-mode-only)

[<img src="https://render.githubusercontent.com/render/math?math=\color{black}{|U_{\mu N}|^2}">](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UmuN_majorana.png#gh-light-mode-only)
[<img src="https://render.githubusercontent.com/render/math?math=\color{white}{|U_{\mu N}|^2}">](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UmuN_majorana.png#gh-dark-mode-only)
![mu flavor](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UmuN_majorana.png#gh-light-mode-only)
![mu flavor](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UmuN_majorana_white.png#gh-dark-mode-only)

[<img src="https://render.githubusercontent.com/render/math?math=\color{black}{|U_{\tau N}|^2}">](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UtauN_majorana.png#gh-light-mode-only)
[<img src="https://render.githubusercontent.com/render/math?math=\color{white}{|U_{\tau N}|^2}">](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UtauN_majorana.png#gh-dark-mode-only)
![tau flavor](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UtauN_majorana.png#gh-light-mode-only)
![tau flavor](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UtauN_majorana_white.png#gh-dark-mode-only)


---
## Limits on the dimension-six $\nu$SMEFT operators

| Type                 | Name                                      | Operator                                                                                              | Notebook                               | Figure                                                                                                                                                                                                                                                                                                                                                 |
|----------------------|-------------------------------------------|-------------------------------------------------------------------------------------------------------|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Mixing               | $O_{\rm mixing}$                                        | $\overline{L}\tilde{H}N$                                                                              | ``0_mixing.ipynb``                     | [$U_{eN}$ dominance](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UeN_majorana.pdf)  <br />  [$U_{\mu N}$ dominance](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UmuN_majorana.pdf)  <br />  [$U_{\tau N}$ dominance](https://github.com/mhostert/N-SMEFT-Limits/blob/main/plots/mixing/UtauN_majorana.pdf) |
| Higgs-dressed Mixing | $\mathcal{O}_{\rm LNH}^\alpha$            | $\overline{L}\tilde{H}N (H^\dagger H)$                                                                | ``1_NSMEFT_LHN.ipynb``                 | [$U_{eN}$ dominance]()  <br />  [$U_{\mu N}$ dominance]()  <br />  [$U_{\tau N}$ dominance]()                                                                                                                                                                                                                                                          |
| Bosonic Currents     | $\mathcal{O}_{\rm HN}$                    | $\overline{N}\gamma^\mu N (H^\dagger i \overleftrightarrow{D}_\mu H)$                                 | ``2_NSMEFT_bosonic_NC.ipynb``          | [NC bosonic]()                                                                                                                                                                                                                                                                                                                                         |
|                      | $\mathcal{O}_{\rm HN\ell}^{\alpha}$       | $\overline{N}\gamma^\mu \ell_\alpha (\tilde{H}^\dagger i \overleftrightarrow{D}_\mu H)$               | ``3_NSMEFT_bosonic_CC.ipynb``          | [CC bosonic]()                                                                                                                                                                                                                                                                                                                                         |
| Moments              | $\mathcal{O}_{\rm NB}^\alpha$             | $\left(\overline{L}_\alpha \sigma_{\mu \nu} N\right) \widetilde{H} B^{\mu\nu}$                        | ``4_NSMEFT_moment_NB.ipynb``           | [Moment hypercharge]()                                                                                                                                                                                                                                                                                                                                 |
|                      | $\mathcal{O}_{\rm NW}^\alpha$             | $\left(\overline{L} _\alpha\sigma_{\mu \nu} N\right) \tau^a \widetilde{H} W^{\mu\nu}_a$               | ``5_NSMEFT_moment_NW.ipynb``           | [Moment W]()                                                                                                                                                                                                                                                                                                                                           |
| Neutral Currents     | $\mathcal{O}_{\rm ff}$                    | $(\overline{f} \gamma^\mu f) (\overline{N} \gamma^\mu N)$                                             | ``6_NSMEFT_4fermion_NC_ff.ipynb``      | [Four fermion ff]()                                                                                                                                                                                                                                                                                                                                    |
|                      | $\mathcal{O}_{\rm LN}^\alpha$             | $(\overline{L}_\alpha \gamma^\mu L_\alpha) (\overline{N} \gamma^\mu N)$                               | ``7_NSMEFT_4fermion_NC_LN.ipynb``      | [Four fermion LN]()                                                                                                                                                                                                                                                                                                                                    |
|                      | $\mathcal{O}_{\rm QN}$                    | $\mathcal{Z}^{\rm QN}_{ij}(\overline{Q}_i \gamma^\mu Q_j) (\overline{N} \gamma^\mu N)$                | ``8_NSMEFT_4fermion_NC_QN.ipynb``      | [Four fermion QN]()                                                                                                                                                                                                                                                                                                                                    |
| Charged Currents     | $\mathcal{O}_{\rm LNL\ell}^{\alpha\beta}$ | $(\overline{L}_\alpha N)\epsilon (\overline{L}_\alpha \ell_\beta)$                                    | ``9_NSMEFT_4fermion_CC_LNLell.ipynb``  | [Four fermion LNLell]()                                                                                                                                                                                                                                                                                                                                |
|                      | $\mathcal{O}_{\rm duN\ell}^{\alpha}$      | $\mathcal{Z}_{ij}^{\rm duN\ell}(\overline{d}_i \gamma^\mu u_j) (\overline{N} \gamma^\mu \ell_\alpha)$ | ``10_NSMEFT_4fermion_NC_duNell.ipynb`` | [Four fermion duNell]()                                                                                                                                                                                                                                                                                                                                |
|                      | $\mathcal{O}_{\rm LNQd}^\alpha$           | $\mathcal{Z}^{\rm LNQd}_{ij} (\overline{L}_\alpha N)\epsilon (\overline{Q_i} d_j)$                    | ``11_NSMEFT_4fermion_NC_LNQd.ipynb``   | [Four fermion LNQd]()                                                                                                                                                                                                                                                                                                                                  |
|                      | $\mathcal{O}_{\rm QuNL}^\alpha$           | $\mathcal{Z}^{\rm QuNL}_{ij}(\overline{Q}_i u_j)(\overline{N} L_\alpha)$                              | ``12_NSMEFT_4fermion_NC_QuNL.ipynb``   | [Four fermion QuNL]()                                                                                                                                                                                                                                                                                                                                  |

