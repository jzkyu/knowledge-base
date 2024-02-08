A *signal* is a form of inter-process communication ([[IPC]]) - effectively the software notification system. It may stem from the process' ([[process]]) own actions (`SIGSEGV`) or from external events (`SIGINT`). 

With a *signal*, you can choose to handle it with a signal handler, or ignore it with a mask. 