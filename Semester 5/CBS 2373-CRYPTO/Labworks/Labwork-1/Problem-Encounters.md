# Problem Encounters 

| **Issues**                         | **Solution**                                                      |
|------------------------------------|-------------------------------------------------------------------|
| SSH login failed (algorithm mismatch)  | Added `-oHostKeyAlgorithms=+ssh-rsa` to the SSH command to specify a matching algorithm. |
| Hydra failed on SSH                | Switched to Medusa for SSH brute-forcing, as Hydra encountered compatibility issues with SSH configurations. |
| Slow brute-forcing with Hydra      | Adjusted the number of tasks with `-t` option to improve performance (e.g., `-t 4` for reduced parallelism). |
