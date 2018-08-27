# beamerthemeKTHprofile

Include this into ``main.tex``


    \makeatletter
    \def\beamer@calltheme#1#2#3{%
    \def\beamer@themelist{#2}
    \@for\beamer@themename:=\beamer@themelist\do
    {\usepackage[{#1}]{\beamer@themelocation/#3\beamer@themename}}}

    \def\usefolder#1{
    \def\beamer@themelocation{#1}
    }
    \def\beamer@themelocation{}


    \usepackage{graphicx} %Loading the package
    \graphicspath{{beamerthemeKTHprofile/}} %Setting the graphicspath

    \usefolder{beamerthemeKTHprofile}
    \usetheme{KTHprofile}
