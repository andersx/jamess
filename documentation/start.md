
# Documentation

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



