---
layout: archive
title: ""
permalink: /research/
author_profile: true
redirect_from: 
  - /research_red/
---


# Research interets

1. High-order numerical methods for PDEs: 
   - Discontinuous Galerkin finite element methods 
   - Spectral methods 
   - Finite difference / volume methods 
2. Scientific computing: 
   - Parallel numerical solvers 

---

# Preprints 

1. Y. Wu and Y. Xu, "A high-order local discontinuous Galerkin method for the $p$-Laplace equation" (special issue in honor of Chi-Wang Shu's 65th birthday), submitted to *Beijing Journal of Pure and Applied Mathematics*, Nov. 2023. [arXiv:2311.09119 [math.NA]](https://arxiv.org/abs/2311.09119){:target="_blank"}. DOI: [10.48550/arXiv.2311.09119](https://doi.org/10.48550/arXiv.2311.09119){:target="_blank"}. 

---


# Projects

## 1. Numerical Simulation of Plasma Equilibrium Evolution in Nuclear Fusion 

*Undergraduate Research Program at USTC* 

Supervisor: [Prof. Mengping ZHANG](https://dsxt.ustc.edu.cn/zj_ywjs.asp?zzid=860){:target="_blank"} 

July 2021 --- May 2022, USTC 

Defense: Dec. 30, 2022 

The controlled nuclear fusion is one of the most prospective solution to the energy crisis and environmental problems. The tokamak has been widely investigated as the most feasible magnetically confined fusion device. Tearing mode instabilities have great influence on the fusion reaction thus worth stuying. 

In this research, in order to simulate the evolution process of tokamak plasma instability numerically, we reviewed different formulations of the MHD equations, selected a suitable type of nonconservative resistive MHD, and developed a parallel solver using hybrid finite difference-Fourier pseudo spectral method in cylindrical coordinates. Using our solver, we simulated the $(m,n)=(2,1)$ resistive tearing mode instability, and checked the results against those obtained from the CLT and M3D-C1 code with researchers from Institute of Plasma Physics, Chinese Academy of Science. Our solver exhibits satisfactory performance in conserving numerical divergence of the magnetic field, fitting the theoretical relation between logrithmic growth rate of kinetic energy and resistivity, revealing the tearing mode structure independent of initial peturbation at the linear stage, and reaching the final saturation stage. 

Below is a plot of $\widetilde{E}_{\varphi}$ (the perturbation on the toroidal component of the electric field) at time $T=7000$, which reveals the resistive tearing mode structure and should be independent of the initial perturbation, and a log-plot of kinetic energy evolution under different resistivity. Our code reveals the linear growing stage, mode structure and the logrithmic growth rate very well. 

<center>
    <img style = "
        border-radius: 0.3125em;
        box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
        src = "../files/undergraduate-research-program/cpt_13.png" 
        width = "46.5%">
    <img style = "
        border-radius: 0.3125em;
        box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
        src = "../files/undergraduate-research-program/energy.png" 
        width = "50%">
    <br>
    <div style = "
        color: orange;
        border-bottom: 1px solid #d9d9d9;
        display: inline-block;
        color: #999;
        padding: 2px;">
        left: tearing mode sturtcure; right: kinetic energy
    </div>
    <p> </p>
</center>

We virtually discussed this research with [Prof. Chi-Wang SHU](https://www.dam.brown.edu/people/shu/){:target="_blank"}. Thanks for his discussion and advice.

Research report (in Chinese) preview: [here](../files/undergraduate-research-program/main.pdf){:target="_blank"}; Defense PPT (in Chinese) preview: [here](../files/undergraduate-research-program/PPT.pdf){:target="_blank"}. 



## 2. Positivity-Preserving Conservative Low-Rank Methods for Vlasov Dynamics 

Supervisor: [Prof. Xiangxiong ZHANG](https://www.math.purdue.edu/~zhan1966/){:target="_blank"} 

June 2022 --- August 2022, Purdue University (online) 

The high-dimensionality of Vlasov dynamics makes it expenive to solve by traditional numerical methods. Utilizing the low-rank structure of the solution, people have developed cost-efficient methods using low-rank matrix/tensor approximation. However, very often a low-rank approximation of a given non-negative matrix (which corresponds to the solution) can have negative elements which results in non-physical solutions. In this research, our goal is to develop a cost-efficient positivity-preserving conservative low-rank method to solve this problem. We designed two algorithms, one is the tangent-space accelerated alternating projection algorithm, and the other is the nuclear norm optimization, both with macroscopic quantities conservation. 

We virtually discussed this research with [Prof. Jing-Mei QIU](https://jingmeiqiu.github.io/){:target="_blank"}. Thanks for her discussion and data. 

<center>
    <img style = "
        border-radius: 0.3125em;
        box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
        src = "../files/summer-research/1.png" 
        width = "90%">
    <br>
    <div style = "
        color: orange;
        border-bottom: 1px solid #d9d9d9;
        display: inline-block;
        color: #999;
        padding: 2px;">
        original data from a conservative dynamic low-rank Vlasov solver
    </div>
    <p> </p>
</center>

<center>
    <img style = "
        border-radius: 0.3125em;
        box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
        src = "../files/summer-research/2.png" 
        width = "90%">
    <br>
    <div style = "
        color: orange;
        border-bottom: 1px solid #d9d9d9;
        display: inline-block;
        color: #999;
        padding: 2px;">
        using tangent-space based alternating projection
    </div>
    <p> </p>
</center>

<center>
    <img style = "
        border-radius: 0.3125em;
        box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
        src = "../files/summer-research/3.png" 
        width = "90%">
    <br>
    <div style = "
        color: orange;
        border-bottom: 1px solid #d9d9d9;
        display: inline-block;
        color: #999;
        padding: 2px;">
        using nuclear norm minimization
    </div>
    <p> </p>
</center>

(still in progress) 


## 3. Discontinuous Galerkin Methods for the $p$-Laplace Equation 

*Bachelor's Thesis Project at USTC* 

Supervisor: [Prof. Yan XU](https://faculty.ustc.edu.cn/yxu){:target="_blank"} 

Feb 2023 --- June 2023, USTC (still in progress) 

The intrinsic singularity or degeneration of the $p$-Laplace equation, as a nonlinear elliptic equation, brings great trouble to usual LDG methods based on the weak formulation. As an alternative, the LDG method built upon the minimization formulation, which is equivalent to the primal formulation, proves to be a practical solution due to its provable convergence and numerical stability. In order to solve the resulting discrete minimization problem, we employed a preconditioner, which can be explained as either a regularized Newton-Raphson method or an first-order explicit gradient flow method, to make the convergence behavior both $hk$-independent. Besides, we provided a priori error estimates through the minimization formulation, which is, however, not optimal. 

<center>
    <img style = "
        border-radius: 0.3125em;
        box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
        src = "../files/bachelor thesis/error_u.png" 
        width = "40%">
    <img style = "
        border-radius: 0.3125em;
        box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" 
        src = "../files/bachelor thesis/error_q.png" 
        width = "40%">
    <br>
    <div style = "
        color: orange;
        border-bottom: 1px solid #d9d9d9;
        display: inline-block;
        color: #999;
        padding: 2px;">
        convergence using up to 9-th order polynomials on 2D unstructured triangular mesh, Poisson equation (errors for the potential and the electric field respectively)
    </div>
    <p> </p>
</center>


---


Numerical PDE Programming (choronological order) 
===

| PDE | method | domain | mesh | language |
| --- | --- | --- | --- | --- |
| Poisson (Dirichlet) | 2-order FD | 2D ractangle | uniform Cartesian | Matlab |
| compressible Euler | 5-order FD-WENO | 1D interval | uniform Cartesian | Fortran |
| compressible Navier-Stokes | 5-order FD-WENO | 2D ractangle | uniform Cartesian | Fortran + OpenMP |
| Hamilton-Jacobi | 5-order FD-WENO | 2D ractangle | uniform Cartesian | Fortran + OpenMP |
| compressible RMHD | 5-order FD-HJ | 2D ractangle | uniform Cartesian | Fortran + OpenMP |
| compressible RMHD | 4-order FD-HJ + Fourier | 3D toroidal with rectangular section | uniform Cylindrical | Fortran + OpenMP |
| compressible RMHD | 3-order FD-HJ + Fourier | 3D toroidal with circular section | uniform Cartesian (embedded) | Fortran + OpenMP + MPI |
| compressible MHD | arbitary-degree DG (locally div-free) | 2D ractangle | arbitary Cartesian | Fortran + OpenMP + MPI |
| Poisson | arbitary-degree FEM | 1D interval | arbitary Cartesian | Matlab |
| Poisson | 1,2-degree FEM | 2D polygon | triangular | Matlab |
| Poisson | LDG | 1D interval | arbitary Cartesian | Matlab |
| Poisson | HDG | 1D interval | arbitary Cartesian | Matlab |
| Poisson | arbitary-degree MD-LDG (good results up to $k=9$) | 2D polygon | triangular | Matlab |
| $p$-Laplace | arbitary-degree LDG | 1D interval | arbitary Cartesian | Matlab |
| $p$-Laplace | arbitary-degree LDG | 2D polygon | triangular | Matlab |
