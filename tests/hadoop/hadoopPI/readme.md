# 1. Buid and run original java files
    $ mkdir bin Origin replaceOutput
    $ ./build-origin.sh  
    $ ./run-origin.sh  

# 2. transform origin class files to new ones with SGX (only replace the conditions)
    $ ./replace-transforme.sh  
## encrypt SGXindex  
    $ ./encrypt_SXGindex.sh  
*the encrypted SGXindex file should be copy to */tmp/* on every node in the cluster.(scp)*  
## runing this new files
    $ ./run-replace.sh  

## NOTICE: BEFORE TRANSFORM THE CLASS FILES, TO CLEAN THE *SGXindex* AND *counter* IN THE */tmp*.
