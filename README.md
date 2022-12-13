# Maxwell Street Residents 1900 - 1950

#### Data Source
The base map data comes from the 1906 Sanborn Map, 1934 Sanborn Map, and 1958 Sanborn Map of E. Maxwell St. in Lexington KY made available by the [Library of Congress](https://www.loc.gov/collections/sanborn-maps/about-this-collection/?loclr=blogtea). The demographic data for these periods come from the 1900, 1930, and 1950 United State Federal Censuses made available by the [US National Archives](https://www.archives.gov/research/census), and serachable by the nonprofit [FamilySearch](https://www.familysearch.org/en/) organization.

## Backgrouund 
East Maxwell Street is just one street around the now-destroyed Adamstown community, a historic African-American community around the block of Rose St., Ave. of Champions, Martin Luther King Blvd. and Maxwell St. Since the majority of the properties in Adamstown were bought up by the University of Kentucky in the mid-20th century, a mjority of the residences were destroyed for the contruction of Memorial Colleseum and the parking accomodations behind it. East Maxwell St. is the only portion of the block that still holds many of the original structures form this historic neighborhood. By charting the residents of East Maxwell St. throughout the 20th century through its destruction, the changes in how spaces were used on this section of the block will be visualized as the University of Kentucky grew larger and larger.

## Methods
To create this visualization, I gathered historic map data originally created by the Sanborn Fire Insurance Company in the 20th century and made publically available by the [Library of Congress](https://www.loc.gov/collections/sanborn-maps/about-this-collection/?loclr=blogtea). These maps show detailed information on the footprint of buildings, the materials those buildings are made out of (coded by color), and the types of full or partial walls. Looking at these maps across time, it can be very intertesting to see how the footprints of buildings in a town or neighborhood changed as expansions were added, houses were rebuilt, or whole neighborhoods were bulldozed. The maps that I chose had to be created at relatively close dates to the three censuses I used: the 1900, 1930, and 1950 censuses. Thus, the Sanborn maps I ended up choosing were the 1906 Sanborn Map, and 1934 Sanborn Map, and the 1958 Sanborn map. 

First, maps were georeference in QGIS according to features and structures visible in OpenStreetMap. Once all maps were georeferenced, the Sanborn maps were vectorized. This step proved more time-consuming than expected, as there were multiple layers of information on the maps. Empty polygon layers were created for the rectalgular property lines, yellow borderless polyon layers were created to vectorize yellow "frame buildings", pink borderless for the pink "brick buildings", green borderless for the roads,soling multi-line vectors were made for the full enclosure layer (ie, floor-to-ceiling walls), and dashed multi-line vectors for partial enclosures (ie. porches). 
