# count_files
GitHub Action to count the number of files in a specific directory

## Example workflow:
```yml
name: Count number of files in a given directory

on:
  push:
    branches:
      - master # Change this to your main branch name

jobs:
  check_number_of_files:
    runs-on: ubuntu-latest

    steps:
    - name: Check out code
      uses: actions/checkout@v2
    - name: test gh action
      uses: omagdy7/count_files@v1.0
      with:
        path: "./"
```
