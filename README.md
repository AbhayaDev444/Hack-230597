# Hack-230597
## Temperature Alert Agent using Fetch.ai's uAgents Library and open-meteo weather API

Two agents have been created, the temperature alert agent and the user agent. The user queries the the temperature alert agent for the current temperature at a given latitude and longitude and also provides a range of temperatures. The Temperature alert agent uses the open-meteo API to extract temperatures for the give location and alerts the user if the temperature is outside the given range. The uAgents library provided by fetch.ai is used for building the communication system between the two users. 

### Working 
While the temperature ranges and location information is currently hard coded. Modifying the Message classes for the agents would allow more interactive way to obtain the loaction and temperature ranges.
The poetry.lock and the pyproject.toml files initialize the virtual environment, this is provided by fetch.ai.
The Agents folder has initializations and attributes for the two agents. While the main calls these two agents to allow their interactions in real-time. 
This was tested out on a localhost with two different ports but can be extrapolated to communicating between two systems using their IP addresses (which is part of the parameters for each agent during initialization). 

