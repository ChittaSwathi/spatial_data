# spatial_data - NoSQL Project

## Technology Requirements
- Python 3.10
- Cython 3.0.0
- UnQLite 0.9.6
- Jupyter Notebook

## Project Description
Through this project, one will gain experience working with NoSQL databases and understand how to use Python to conduct several fundamental operations on them. Unlike conventional relational databases, NoSQL allows data to be stored more freely without the use of rigid schemas. Additionally, they are capable of handling massive amounts of data quickly.

##Distance Algorithm
DistanceFunction(lat2, lon2, lat1, lon1)
var R = 3959; // miles
var φ1 = lat1.toRadians();
var φ2 = lat2.toRadians();
var Δφ = (lat2 - lat1).toRadians();
var Δλ = (lon2 - lon1).toRadians();
var a = Math.sin(Δφ / 2) * Math.sin(Δφ / 2) + Math.cos(φ1) * Math.cos(φ2) * Math.sin(Δλ / 2) * Math.sin(Δλ / 2);
var c = 2 * Math.atan2(Math.sqrt(a), Math.sqrt(1 - a));
var d = R * c;
// d is the distance between the given pair of latitude and longitude. The distance is in miles.

Reference: [Movable Type Scripts](http://www.movable-type.co.uk/scripts/latlong.html)
