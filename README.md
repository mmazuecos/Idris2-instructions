# Idris2 installation instructions
Instructions to install Idris2 in a Linux machine.

1. Download idris from https://www.idris-lang.org/pages/download.html.
2. Download Racket https://download.racket-lang.org/.
3. Install Racket -> ```sh racket-8.6-x86_64-linux-cs.sh```.
4. Export path to the instalation. If you chosed installing in home you can just ```cd; export PATH=$PATH:$(pwd)/bin.
5. Decompress -> ```tar xvfz idris2-X.X.X.tgz```.
6. ```cd Idris2-X.X.X```
7. ```make bootstrap-racket```
8. ```make install```, this will install in /home/USER/.idris2/.
9. Make Idris2 available in path: ```cd; export PATH=$PATH:$(pwd)/.idris2/bin```.

## Troubleshooting:

- ```gmp.h: No such file or directory```: ```apt-get install libgmp3-dev```
