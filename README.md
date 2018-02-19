# Advanced-Computing
Linux, Parallel computing with FLUX and Spark

# Linux 
#### Command
```
cp source destination
chmod -change the permission
```

#### Shell programming


# Flux
Flux is a parallel computing system. 

#### How to write PBS file to submit the job 
Changing parameters about the resources and some other information and run the program

#### How to submit, check the job (job level)
```
qsub name.psb  #submit the file
qstat -u uniquename/ job ID #check the status of job submitted
qdel
```

#### How to know more about the account group that you can use (user level/ account level)
```
mdiag -u #show the account that can use
mdiag -a account #show the detail information of an account
showq -w acct=account name #show the job running on a certain account
```

#### How to run the code
Load the module
```
module keyword name #check the module on the flux
module load python #load the module
```
Load the data
```
scp source flux-xfer.arc-ts.umich.edu:/scratch/..
```

write it on the PBS file. For example
```
python a.py
```

