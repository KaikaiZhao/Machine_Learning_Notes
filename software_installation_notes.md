1. LaTeX Error: File *algorithm.sty* not found.
sudo apt-get install texlive-science

2. If our keyboard doesn't work when we are logging in, we can crack it via clicking *switch account*, but this would not solve it utterly.

3. Installation for R and rstudio

   * add the following entry in your /etc/apt/sources.list file, because of my Ubuntu16.04 OS,
        deb https://mirrors.tuna.tsinghua.edu.cn/CRAN/bin/linux/ubuntu xenial/

    * sudo apt-get update
    * sudo apt-get install r-base
    * In the terminal, we run R, then we arrive at the R command interface, which shows that R installation is successful. We have installed R. Now we install rstudio.
    * download the rstudio package from the official web https://www.rstudio.com/(The package I downloaded is rstudio-1.0.44-amd64.deb and you need to replace the package name in the following command according to the one that you have downloaded)
    * sudo apt-get install gdebi-core
    * sudo gdebi -n rstudio-1.0.44-amd64.deb
    * run 'rstudio' in the terminal, you will see the rstudio interface.
    * You can also add it to the Dash or lock it to the Launch.

    
