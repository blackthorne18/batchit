## mbatch - A personal workload manager

For scipts that can take a long time to execute due to file size or complexity, it is helpful to run them in the background so you don't have to wait around while it is running.
`mbatch` is a simple wrapper around Linux's native `nohup` feature. It's an easy way to run processes in the background and keep track of them.

### Run an executable file in the background
	`mbatch somefile.sh`
### Pass a simple command directly to batch to run in the background
	`mbatch sed -i 's/test/string/g' somefile.fna`
### List all running processes
	`mbatch list`
Shows `mbatch` processes that are still active and their runtime. Easy way to keep track of processes without having to refer to `top`
