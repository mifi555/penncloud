**

# CIS 5050 Final Project Team 11

**

**Team Members and Emails**
 1. Akanksha Ashok: aashok@seas.upenn.edu
 2. Bilal Ali: bilalali@seas.upenn.edu
 3. Milan Filo: mfilo@seas.upenn.edu
 4. Peter Akioyamen: peterai@seas.upenn.edu


**Instructions for Compilation**
Dependencies:
 - [ ] Open ssl [https://github.com/openssl/openssl/blob/master/README.md](https://github.com/openssl/openssl/blob/master/README.md)
 - [ ] lldns  (brew install dns)
 - [ ] update config files to includes necessary paths to downloads
 - [ ] install tmux using brew [https://github.com/tmux/tmux/wiki](https://github.com/tmux/tmux/wiki) 

**Compiling and Running**
*Each of the following should be run in a new terminal*

1. ./startup.sh (this runs admin, coordinator, loadbalancer and relay)
2. cd front_end
	./run_fe_group.sh
3. cd backend_server
	./run_be_cluster_G0.sh
4. cd backend_server
	./run_be_cluster_G1.sh
5. cd backend_server
	./run_be_cluster_G2.sh

This runs 3 server groups with 3 secondaries (4 servers in each server group). 

*To run PennCloud:*
1. Open localhost:7500 in browser (this will redirect you to the relevant front end server)
2. Open another tab for localhost:8082/admin/dashboard to see admin dashboard
3. To send emails, open another browser or thunderbird to send emails to and from registered users.