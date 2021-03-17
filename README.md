**A tool for Slurm job submission** (Work in progress)

Example usage: `slurp ls` will submit a single job on the default node, with command `ls`

Adding the -d flag makes this a devel node job: `slurp -d ls`

Job arrays can be submitted by specifying options in square brackets:

`slurp echo [foo,bar] [1,2,3]`
will submit a job array with the following commands:

- `echo foo 1`
- `echo foo 2`
- `echo foo 3`
- `echo bar 1`
- `echo bar 2`
- `echo bar 3`
