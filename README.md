
# Terraria API

Terraria API was created to allow anyone access the most up to date Terraria data on the below things
- Items

## TODO
1. Research/Document project

	- What might people want to search for?
		- all new 1.44 items
		- all ds items
		- all ds recipes

	- How should the data be provided?
		- JSON via API
		- CSV in Source code
		- JSON in Source code

	- How far to be nested?
		Limit nesting depth by locating resources at the root path.

	- Log as much as I can
		([Requests Per Minute (RPM), Latency, Failure Rate, API Uptime, Time to First Hello World, Memory & CPU Usage](!https://sematext.com/blog/api-monitoring/#what-api-metrics-should-you-track))

	- What are items that are most likely overkill?
		- Authentication
		- Caching
		- **Pagination?**

3. Build API that responds to requests with proper status codes
4. Deploy to AWS
5. Collect data locally
6.  Load data to database
7. Create new endpoints as needed
8.  Go through this [Restful Guide](!https://www.vinaysahni.com/best-practices-for-a-pragmatic-restful-api) and implement as much as reasonable


## *In Progress*
- Item Categories
- Biomes
- Mechanics
- NPCs
- Bosses
- Events


## Responses
Many API endpoints return the JSON representation of the resource requested. However, if an invalid request is submitted, or some other error occurs, Terraria API returns a JSON response in the following format:

    {
      "message" : string,
      "success" : bool,
      "data"    : string
    }

The message attribute contains a message commonly used to indicate errors.

The success attribute describes if the transaction was successful or not.

The data attribute contains any other metadata associated with the response. This will be an escaped string containing JSON data.

## Showcase
website like https://platinumgod.co.uk/
updated website like https://terrariaitemids.com
