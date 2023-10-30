# mysys
configurations for my system (laptop)

## getting started

* create `~/.mysys/bin` folder:
    ```
    mkdir -p ~/.mysys/bin
    ```

* download `mysys.sh` script
  * ... from `~/.mysys/bin` folder
    ```
    cd ~/.mysys/bin
    wget https://raw.githubusercontent.com/jtviegas-sandbox/mysys/main/.mysys/bin/mysys.sh
    ```
  * make it executable: `chmod +x mysys.sh`
  * update __mysys__ with latest version from the github repo: `./mysys.sh update`

you should now see this when running `./mysys.sh`:

    [WARN]  Mon Oct 30 11:46:50 CET 2023 *** we DON'T have a .variables variables file - creating it 
    [WARN]  Mon Oct 30 11:46:50 CET 2023 *** we DON'T have a .secrets secrets file - creating it 
    [DEBUG] Mon Oct 30 11:46:50 CET 2023 ... 1:  2:  3:  4:  5:  6:  7:  8:  9:  
    usage:
    mysys.sh { command }

        commands:
        - update: updates 'mysys'
        - release: packages mysys into a tar for release purposes

* __source__ the `.mysys/include` file in your system's profile initialisation file ( `.zprofile`, `.bash_profile`, etc... )
    ```
    . ~/.mysys/include
    ```
* restart the system
* you should now invoke `mysys.sh` from everywhere in your terminal
  ```
  ~ % mysys.sh
  [DEBUG] Mon Oct 30 15:41:51 CET 2023 ... 1:  2:  3:  4:  5:  6:  7:  8:  9:
   usage:
   mysys.sh { command }

     commands:
       - update: updates 'mysys'
       - release: packages mysys into a tar for release purposes
  ```

* you can always override the variables and secrets in your local files:
  * `~/.mysys/.variables`
  * `~/.mysys/.secrets`

