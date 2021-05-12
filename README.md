# P2P-Decentralized-Network
### General Description:
* Handshake is established between peer.
* Communication protocol is in progress. 
* We have no success in transferring files.
* Communication Protocol:
  ```
  {
    'headers': 
    [
      {
        'type': 'print',
        'body': 
          {
            'message': 'Hello World'
          }
      },
      {
        'type': 'input',
        'body': 
          {
            'message': 'Enter Hello World',
            'res-key': 'Hello Response',
            'res-type': 'string'
          }
      },
      {
        'type': 'ignore'
      },
      {
        'type': 'bittorrent',
        'body': self.message.choke
      },
      {
        'type': 'close'
      }
    ]
  }
  ```

### How To Run:
1. In terminal, cd in to `P2P-Decentralized-Network`
2. In terminal, make sure the machine installed according to the requirements.txt
3. In `peer.py`, change the `SERVER_PORT` to 5000
4. In terminal, run `py peer.py`
5. In terminal, when prompted `Enter role: ` input `seeder`
6. In terminal, when prompted `Enter peer ip: ` just press `ENTER`
7. In terminal, when prompted `Start broadcast ` input `False`
8. In `peer.py`, change the `SERVER_PORT` to 4998
9. In 2nd terminal, run `py peer.py`
10. In 2nd terminal, when prompted `Enter role: ` input `peer`
11. In 2nd terminal, when prompted `Enter peer ip: ` just press `ENTER`
12. In 2nd terminal, when prompted `Start broadcast ` input `True`
