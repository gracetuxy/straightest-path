In this project, our goal is to create a route planner that returns the best route with constraints in length, direction, and elevation gain. The project involves interacting with map data, implementing a basic route planning algorithm, and visualizing maps.

The map data is obtained from [OpenStreetMap](https://www.openstreetmap.org/) through [OSMnx](https://geoffboeing.com/2016/11/osmnx-python-street-networks/) and the elevation data are obtained through the [Open-Elevation API](https://www.open-elevation.com/).


# `load_map.py`
This file load the map of the UBC (University of British Columbia) area and elevation data.

# `routePlanSTU.py`
This file:
- finds any path in the UBC graph whose total distance is greater some target length using depth first search
- adds the constraint for the "straightest" direction out of any vertex
- report total elevation gain
- provide a visualization of the route in rainbow with the calculated elevation gain in the `route_graph_workout.html` file
