## Files provided to us.

## TYPOS AND CHANGES

### PART A


### PART B
- Add the *\* iit018_stdcells.db and \* iit018_stdcells.lib* into ~synthesis/sta directory

- When generating the path-based timing reports, change the commands to the ones below to save the three most critical max and min paths.

  ```
  report_timing -max_paths 3 -slack_lesser_than 5 > max_paths.txt 
  report_timing -max_paths 3 -slack_lesser_than 5 -delay min > min_paths.txt 
  ```

### PART C
