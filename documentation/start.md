
# Documentation using MD

If documentation of QM programs was done using Markdown (MD),
the ASCII version would actually be readable.
Plus MD is so easily converted to HTML, or even PDF (Latex),
for easy readme/documentation.

## Example

How to start at calculation is very simple,
here is an example of a simple Hatree-Fock calculation.


    $calculation
        method=hf
        basis=sto-3g
    $end

    $xyz
        O  -1.551007  -0.114520   0.000000
        H  -1.934259   0.762503   0.000000
        H  -0.599677   0.040712   0.000000
        O   1.350625   0.111469   0.000000
        H   1.680398  -0.373741  -0.758561
        H   1.680398  -0.373741   0.758561
    $end

which is saved as `waterdimer.inp` and then runned simple as

    ./jamess waterdimer.inp > waterdimer.log

## Unfortunately

In-line equations does not work yet, for example $\psi$, but
this could easily be done using MathJax plugin for HTML browsers.

    $$ \mathrm{RMSD}(v,w) = \sqrt{  \frac{1}{n} \sum_{i=1}^n ((v_{ix} - w_{ix})^2 + (v_{iy} - w_{iy})^2 + (v_{iz} - w_{iz})^2 ) } $$

and this would be alot better than using images, like most journals do.

