# Toronto Beach 
&nbsp;

The easiest way to access **The City of Toronto's** Open Data beach data API in **Node.js**.


&nbsp;

# Getting Started



### Installation

&nbsp;
Super easy, first run this:

    npm install torontobeach


Then to use:

    import torontobeach from 'torontobeach';

That's it!

 Now start using it with the functions and documentation below. 


&nbsp;

# Usage


&nbsp;

### We are fetching data here, so we're returning promises.
&nbsp;
&nbsp;
**Using promises:**


    torontobeach.getAllBeachesLatest()
	    .then(response => {
		   doCoolStuffWithData(response);
	    });


**Using Async/Await**

    const beachData = await torontobeach.getAllBeachesLatest();


&nbsp;
A sample response of a single data point.:


   
```
{
	beachID: 4,
	name: 'Gibraltar Point Beach',
	map: '43.612487,-79.382173',
	sampleDate: '2019-09-02',
	publishDate: '2019-09-04',
	eColiCount: 11,
	beachAdvisory: "E.coli levels are within the City of Toronto's established beach water quality standard of 100 E.coli per 100ml of water.",
	beachState: 'Safe'
}
```
&nbsp;


**Quick reference for the beach IDs:**

  

    Marie Curtis Park East Beach: 1
    Sunnyside Beach: 2
    Hanlan's Point Beach: 3
    Gibraltar Point Beach: 4
    Centre Island Beach: 5
    Ward's Island Beach: 6
    Cherry Beach: 7
    Woodbine Beaches: 8
    Kew Balmy Beach: 9
    Bluffer's Beach Park: 10
    Rouge Beach: 11

&nbsp;
All good? Awesome. Onto the good stuff.
&nbsp;

# Methods



**Latest reading for all beaches**

    getAllBeachesLatest();

&nbsp;

**All time data for all beaches**

    getAllBeachesAllTime();

&nbsp;

**All beaches between two dates.**


    getAllBeachesForRange('YYYY-MM-DD', 'YYYY-MM-DD');

&nbsp;

**Specific beach between two dates.**


    getSpecificBeachForRange(beachID, 'YYYY-MM-DD', 'YYYY-MM-DD');

&nbsp;


**All time data for specific beach**


    getSpecificBeachAllTime(beachID);

&nbsp;
&nbsp;
&nbsp;

Awesome! 

If you are interested in learning more, or about contributing, check out the repository at: https://github.com/mikaalnaik/TorontoBeach  


