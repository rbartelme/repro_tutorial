# repro_tutorial
*FOSS 2021 Reproducibility Tutorial Demo*

## Computer Setup
    1  cd /scratch
    2  ls
    3  git clone https://github.com/rbartelme/repro_tutorial.git
    4  wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
    5  bash Miniconda3-latest-Linux-x86_64.sh -b -p /opt/conda
    6  ln -s /opt/conda/pkgs/*/bin/* /bin
    7  ln -s /opt/conda/pkgs/*/lib/* /usr/lib
    8  /opt/conda/bin/conda install -c conda-forge -y jupyterlab=1.2.3
    9  /opt/conda/bin/conda install -c conda-forge -y nodejs=10.13.0
   10  /opt/conda/bin/pip install bash_kernel
   11  /opt/conda/bin/pip install ipykernel
   12  /opt/conda/bin/python3 -m bash_kernel.install
   13  /opt/conda/bin/conda search -c bioconda snakemake
   14  /opt/conda/bin/conda install -c bioconda -c conda-forge -y snakemake=5.8.1
   15  ln -s /opt/conda/bin/* /bin
   16  ln -s /opt/conda/lib/* /usr/lib
   17  snakemake --version
   18  sudo apt-get update
   19  sudo apt-get install -y apt-transport-https ca-certificates curl gnupg-agent software-properties-common
   20  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
   21  sudo add-apt-repository  "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
 $(lsb_release -cs) \
 stable"
   22  sudo apt-get update
   23  sudo apt-get install -y docker-ce docker-ce-cli containerd.io
   24  docker run hello-world
   25  cd repo_tutorial
   26  cd repro_tutorial
   27  history >> README.md
