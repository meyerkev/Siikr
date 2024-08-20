# Siikr

IYKYK.

# Installation

Best done on a clean Ubuntu or debian server.

0. clone this repo.
1. Copy `siikr.example.env` to `siikr.env` and fill out (at a minimum) the first three lines.
2. If not already in a terminal, switch to one and run `chmod +x setup_simple.sh`
3. Then run `sudo ./setup_simple.sh` and follow the prompts.
4. Pray.
5. Submit an issue if it fails.

# Docker installation

Docker gives you a clean server, but the install may be a little more involved.

0. clone this repo.
1. Make sure you have both Docker and `docker-compose` installed.
    1. TODO: Document how to setup the API key sanely
2. Copy `siikr.example.env` to `siikr.env` and fill out (at a minimum) the first three lines while noticing the hardcoded postgres user siikrweb.
3. `make build up && open localhost:8080 && make logs` - This will follow logs in the terminal and open the browser window
4. You'll need to do some magic with DDNS for callback reasons in your router or via some other mechanism.  This is _not_ documented.  

