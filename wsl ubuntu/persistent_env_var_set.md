WSL Linux set env variable permanently from a bash terminal
Launch your wsl instance.
$ sudo vim ~/.bashrc
Enter your password.
Press i to go into edit mode. Go to the end of the file using arrow key.
Add your variable as "export API_KEY=123" at the end of the file. If your variable has spaces, use quotes. Example - API_KEY= 'My Key'
Press esc key to get out of edit mode.
Enter :wq and press enter . This will save and close the file.
$ source ~/.bashrc will load your recent changes into your current shell.
$ echo $API_KEY should print your API_KEY.
$ printenv API_KEY should print your API_KEY too.