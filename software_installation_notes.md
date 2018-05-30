1. LaTeX Error: File *algorithm.sty* not found.
sudo apt-get install texlive-science

2. If our keyboard doesn't work when we are logging in, we can crack it via clicking *switch account*, but this would not solve it utterly.

3. Installation for R and rstudio

   * add the following entry in your /etc/apt/sources.list file, because of my Ubuntu16.04 OS,
        deb https://mirrors.tuna.tsinghua.edu.cn/CRAN/bin/linux/ubuntu xenial/

    * sudo apt-get update
    * sudo apt-get install r-base
    * In the terminal, we run R, then we arrive at the R command interface, which shows that R installation is successful. We have installed R. Now we install rstudio.
    * download the rstudio package from the official web https://www.rstudio.com/ (The package I downloaded is rstudio-1.0.44-amd64.deb and you need to replace the package name in the following command according to the one that you have downloaded)
    * sudo apt-get install gdebi-core
    * sudo gdebi -n rstudio-1.0.44-amd64.deb
    * run 'rstudio' in the terminal, you will see the rstudio interface.
    * You can also add it to the Dash or lock it to the Launch.

4. Install cvx in MATLAB on Ubuntu16.04

    * open your MATLAB, follow the path: Home -> Preferences -> Matlab -> keyboard -> Shortcuts -> Active settings, choose "Windows Default set" and click OK
    * download the package as either a .zip file or .tar.gz file from the web site:http://cvxr.com/cvx/download/
    * Unpack the file anywhere you like; a directory called cvx will be created.
    * Start Matlab via the terminal in the current directory. Do not add CVX to your path by hand.
    * run the cvx_setup command
    * In some cases—usually on Linux—the cvx_setup command may instruct you to create or modify a startup.m file that allows you to use CVX without having to type cvx_setup every time you re-start Matlab. For example,
    * To solve the problem, create a new file
    /home/xifeng/Documents/MATLAB/startup.m
containing the following line:
    run /home/xifeng/kk/cvx/cvx_startup.m

    * The program below is used to test whether your installation is successful.
    * m = 20; n = 10; p = 4;
A = randn(m,n); b = randn(m,1);
C = randn(p,n); d = randn(p,1); e = rand;
cvx_begin
    variable x(n)
    minimize( norm( A * x - b, 2 ) )
    subject to
        C * x == d
        norm( x, Inf ) <= e
cvx_end

5. I am running a python script and I get this error:Intel MKL FATAL ERROR: Cannot load libmkl_avx2.so or libmkl_def.so.  \ Both files are present in the anaconda2/lib directory.
If you use conda, try with these two commands:conda install nomkl numpy scipy scikit-learn numexpr
conda remove mkl mkl-service

6. install anaconda and tensorflow, and know more about anaconda, refer to [anaconda basics](https://www.jianshu.com/p/2f3be7781451) and [installation](https://blog.csdn.net/hgdwdtt/article/details/78633232)
