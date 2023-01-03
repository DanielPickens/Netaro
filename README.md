## NETARO
 
 `_   _      _                  
 | \ | |    | |                 
 |  \| | ___| |_ __ _ _ __ ___  
 | . ` |/ _ \ __/ _` | '__/ _ \ 
 | |\  |  __/ || (_| | | | (_) |
 |_| \_|\___|\__\__,_|_|  \___/ 
 `                            



# Netaro - a Website Analysis CLI

Netaro is a cli utility that scans live CMAP, IP's and MXFiles and reports potential issues with deployed resources and configurations. It can analayze a network based on what's inferred and not what's sitting on disc or networked locally. By scanning globally , it detects misconfigurations and helps to ensure that best practices are in place, thus preventing future headaches. It aims to reduce the cognitive *over*load one faces when operating a nmap and other reconissance tools using Go as a self-operating controller. 



---

## Installation



* Binaries for Linux, Windows and Mac are available as tarballs in
  the [release](https://github.com/DanielPickens/Netaro/releases) page.

* For OSX/Unit using Homebrew/LinuxBrew

   ```shell
   brew install unknown/netaro/netaro
   ```

* Building from source
   Netaro was built using go 1.19. In order to build Netaro from source you must:
   1. Clone the repo
   2. Add the following command in your go.mod file

      ```text
      replace (
        github.com/DanielPickens/Netaro => MY_NETARO_CLONED_GIT_REPO
      )
      ```

   3. Build and run the executable

        ```shell
        go run main.go 
        ```

   Quick recipe for the impatient:

   ```shell
   # Clone outside of GOPATH
   git clone https://github.com/DanielPickens/Netaro
   cd netaro
   # Build and install
   go install
   # Run
   go run cmd/Netaro/cli.go 
   ```



