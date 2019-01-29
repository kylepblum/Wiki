###VAE Workflow
1. Get input data ready
  * Save as csv
  * Should be (TxN) where T is the number of time bins and N is the number of distinct inputs
  * Move <data.csv> from local to shrek (on local):
    * `scp ~/path/to/file/data.csv shrek:~/path/to/shrek/dir/data.csv`
  * Move <data.csv> to docker container (on shrek host):
    * `$ docker cp /path/to/file/data.csv <container>:/path/to/file/data.csv`
3. Modify VAE code for input data
  * Move code to docker container (same as data file)
5. Train NN Model on Shrek (PyTorch container)
7. Get data from Shrek to local 
  * on shrek host: `$ docker cp <container>:/path/to/file/output.csv /path/to/file/output.csv`
  * on local `scp shrek:/path/to/file/output.csv ~/path/to/file/output.csv`
9. Analyze data locally or on GOB
10. 
