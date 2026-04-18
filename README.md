# ClientFucker (Inspired by MeowDoomsdayFucker and _legendryy_)

ClientFucker is a lightweight detection program designed to identify the presence of specific clients within a running process it mainly detects shitty skided clients

## Overview

This project focuses on basic memory inspection techniques to determine whether a target process contains identifiable traces of supported clients. It is intended as a simple and direct approach to signature-based detection.

## How It Works

The script performs the following steps:

- Enumerates running processes or targets a specific process  
- Reads accessible memory regions from the process  
- Extracts and analyzes strings from memory  
- Compares extracted data against known client-related signatures (currently Doomsday and Lagoon)  

If a match is found, the process is flagged as containing the client.

## Output

The script returns one of the following results:

- `process clean`  
  Indicates that no known client signatures were found in the scanned process  

- `client detected (Lagoon)`  
  Indicates that the Lagoon client was detected in the process memory  

- `client detected (Doomsday)`  
  Indicates that the Doomsday client was detected in the process memory  

## Future Plans

- Add detection for more clients  
- Improve signature accuracy and reduce false positives  
- Expand signature database  
- Optimize memory scanning performance  
- Add optional real-time scanning  


## Detected Clients
- Doomsday
- Lagoon
- Grim
- Old Prestige Mod & Prestige Injector
- Nova
- System - Flag the same as nova since its a nova skid that it detects mainly
- Zenith

## Acknowledgements

This project is inspired by Doomsday Fucker and follows a similar concept of detecting software through memory inspection techniques.

## Usage

Run the Detector by downloading it from the releases and run it
