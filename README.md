# LinuxShell_ssh

* remotely connect and remotely execute cmd

       ssh [remote host name or its IP addr] cmd
       
       //
       
       echo "cmd" | ssh [remote host name or its IP addr] bash
       
 
* remotely connect running script file, and return result in local

       cat script_name.sh | ssh [remote host name or its IP addr] bash

* telnet in secure way

        ssh -R [port of local host]:[remote host name or its IP addr]:[port of remote host]

        ssh -p [port of remote host]

        ssh -l [loggin_account]

        ssh -i [identify info]
        // check version,
        // if version is 1, then private key is in path of .ssh/identify
        // if 2, then .ssh/id_rsa and .ssh/id_dsa

 * Check key is exist or not
 
         ls -al ~/.ssh //.ssh 是身份確認檔案，內容含有 private key
 
      https://help.github.com/en/github/authenticating-to-github/checking-for-existing-ssh-keys
 
 * Generate key if not exist
 
        ✗ ssh-keygen -t rsa -b 4096 -C "queeniecplusplus@gmail.com"
           
        Generating public/private rsa key pair.
        
        Enter file in which to save the key (/Users/pintred/.ssh/id_rsa): key 
        
        [ Enter passphrase (empty for no passphrase): 
        Enter same passphrase again: 
        
        Your identification has been saved in keyy.
        
        Your public key has been saved in keyy.pub.
        
        The key fingerprint is:
        
        SHA256:jH2Vo/6z1iEv0INPYMPTnRVBrWae6ErRPWqMdtYiLBO queeniecplusplus@gmail.com
        
        The key's randomart image is:
        
        +---[RSA 4096]----+
        |              .++|
        |             .  o|
        |         . .+. + |
        |       +  *+.o*  |
        |      . E.+*.=x. |
        |         =o+*o+. |
        |        o B=B=.. |
        |         = **.o  |
        |          .oo+   |
        +----[SHA256]-----+

      https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
  
  
    
    
   
