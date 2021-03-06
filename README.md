#  OSM objects counter 

Prepare your OSM file using [osm-extract](https://github.com/Rub21/osm-objects-counter/tree/master/osm-extract)

```
https://github.com/Rub21/osm-objects-counter.git
cd osm-objects-counter
npm install

```

#### Counter all objects for all users

```
node index.js --osmfile osm-extract/osm.osm.bz

```


#### Counter objects by specific users

note:
If you filter your OSM file per user in `osm-extract` is necessary to filter again as next command line because we use ` --complete-ways`, the osm file contain nodes as a part of ways which are not made or update by the specific users.


```
node index.js --osmfile osm-extract/osm.osm.bz --usersfile osm-extract/users

```

In both cases the output files are  in markdown tables: 

- [osm_objects.md](https://github.com/Rub21/osm-objects-counter/blob/master/osm_objects.md)
- [users.md](https://github.com/Rub21/osm-objects-counter/blob/master/users.md)
- [tags.md](https://github.com/Rub21/osm-objects-counter/blob/master/tags.md)
- [roads_distance.md](https://github.com/Rub21/osm-objects-counter/blob/master/roads-distance.md)
 

 