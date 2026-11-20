# Solutions

The `basis` directory contains Sturmian functions and the `wavefunctions` 
directory contains pseudostate wavefunctions obtained from diagonalising
the hydrogen Hamiltonian in a Sturmian-type basis.

## Exact wavefunctions

For the hydrogen atom, there exists an analytical formula for the radial
wavefunctions. Students should compare their results with both the 
pseudostates in the `wavefunctions` directory (expecting to obtain
exact agreement) and the exact wave functions. How do the pseudostate
wavefunctions compare to the exact ones, how does this correspond to the
quality of the eigenvalues (energies) obtained from the diagonalisation 
procedure?

The exact wave functions are given by the formula,
```math
R_{n\ell}(r)=\sqrt{\bigg(\frac{2}{n}\bigg)^3\frac{(n-\ell-1)!}{2n(n+\ell)!}}
{\rm e}^{-r/n}\bigg(\frac{2r}{n}\bigg)^\ell
L^{2\ell+1}_{n-\ell-1}\bigg(\frac{2r}{n}\bigg),
```
where $n$ is the principal quantum number, $\ell$ is the orbital 
angular momentum, and $L$ is the associated Laguerre polynomial. 
There will already be a subroutine/function for calculating the latter in
the code.
