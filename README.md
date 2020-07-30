# Tourist Program
This project involves two parts: the first recommends certain tourist locations
based on what keyword interests a user has.  The second uses graph search
algorithms to recommend a route to get from one location to another using
some train stations from Vancouver.

## Tourist Locations
The file `script.py` contains two lists.  

`destinations` is a list consisting of several locations.

`attractions` is a list whose indices correspond to a destination in `destinations`.  Each attraction in this list is 
a list with 2 elements, the first being the name of the attraction and the second being a list of interests that describe
that attraction / the activities that might occur there.

`script.py` works by recommending the attraction in a specific destination that aligns with most
of your interests.

## Route Finder
`landmark_choices`: This file is a dictionary of letters corresponding to 
specific landmarks in Vancouver.

`vc_landmarks.py`: This file contains a dictionary of these landmarks as keys, mapped to
metro stations that you can take to get there.  

`vc_metro.py`: This file represents the graph, with each metro station in Vancouver as a node and edges connecting
two stations that have a route between them.

`graph_search.py`: Contains the BFS and DFS algorithms.

`skyroute.py`: Main level program, takes in the To and From landmarks and produces a route between them.

The data used comes from CodeCademy's Computer Science 30 Day Challenge.