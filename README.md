# mysys
configurations for my system (laptop)

## getting started

* create `~/.mysys/` folder:
    ```
    mkdir ~/.mysys
    ```
* __source__ the `.mysys/include` file in your system's profile initialisation file ( `.zprofile`, `.bash_profile`, etc... )
    ```
    . ~/.mysys/include
    ```

* download `mysys.sh` script
  * ... from `~/.mysys/` folder
    ```
    cd ~/.mysys/
    wget https://raw.githubusercontent.com/jtviegas-sandbox/mysys/main/.mysys/bin/mysys.sh -o bin/mysys.sh
    ```
  * make it executable: `chmod +x bin/mysys.sh`
  * update bashutils include file: `bin/mysys.sh update`

you should now see this when running `bin/mysys.sh`:

    [WARN]  Mon Oct 30 11:46:50 CET 2023 *** we DON'T have a .variables variables file - creating it 
    [WARN]  Mon Oct 30 11:46:50 CET 2023 *** we DON'T have a .secrets secrets file - creating it 
    [DEBUG] Mon Oct 30 11:46:50 CET 2023 ... 1:  2:  3:  4:  5:  6:  7:  8:  9:  
    usage:
    mysys.sh { command }

        commands:
        - update: updates 'mysys'
        - release: packages mysys into a tar for release purposes

