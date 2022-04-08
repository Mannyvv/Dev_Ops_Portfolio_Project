# README.md
1. What are the various features you would like your project to offer? 
My project will allow a Twitch Streamer to log information stream information such as viewers, stream time, new followers, new subscribers, re-subscribers, donations,donors, game streamed, software used, data/time, etc.

2. What are the API endpoints that you would need to set up for each feature? List them along with the respective HTTP verb, endpoint URL, and any special details (query parameters, request bodies, headers). 
GET - New Subscribers - base_url/subscribers/<date>

GET - Total Subscribers - base_url/subscribers/

GET - New Followers - base_url/followers/<date>

GET - Total Followers - base_url/followers/

POST - Stream - base_url/Stream/

POST - Subscriber - base_url/subscriber/

PUT - Donor - base_user/subscriber/id


***Might include visuals***


3. Provide a description of the database tables required for your application, including column names, data types, constraints, and foreign keys. Include your database name. You can optionally include an ER diagram. 
Tables

Streams - ID, date, stream time, game streamed

Subscribers - ID, date, time, total subscription, Stream

Followers - ID, date, time, Stream

Donations - ID, date, time, Stream, Follower, Subscriber