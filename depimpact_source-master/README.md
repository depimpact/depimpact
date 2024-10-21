## How to run
Prior to running, a log and it's related property file should be prepared. The log files should end with ".txt" and the property files should have the same name as the related log followed by ".backward" as key word. Logs and property files should be in the same folder.
```
> cmd_inject.txt
> cmd_inject.backward.property 
```
### Through Java
Run the class "ExperimentRunnerCmd". Parameters are:
```
1. path to logs and property files

2. path to directory for results

3. names of the log file

4. mode:
    nonml           - manual projection
    clusterall      - cluster all edges
    nonoutlier      - cluster without outliers
    clusterlocal    - local cluster
    localtime       - cluster locally only by time weight
    localamount     - cluster locally only by amount weight
    localstruct     - cluster locally only by structure weight
    fanout          - cluster locally only by fanout value

E.g.,  "/logfilepath" "/resultspath" "cmd_inject.txt" "clusterall"
```
