# Demonstration of autoware_universe splitting workflow

This repository is a mirror of a selected packages in https://github.com/autowarefoundation/autoware_universe and CI demonstration.

## How to create this repository

```bash
$ cd /path/to/workspace
$ git clone git@github.com:autowarefoundation/autoware_universe.git .
$ git switch -c mirror
$ git filter-repo --path planning/autoware_trajectory_validator --path .github/ --path docs/ --path-regex '^[^/]*$' --force
```
