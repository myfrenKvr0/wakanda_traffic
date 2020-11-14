# Wakanda Traffic Department

# A serverless Web application that hosts three distinctive cloudlets created using various IBM Cloud Services
This implementation demonstrates how to build a serverless web application where static content is hosted in a storage bucket (here it uses GitHub Pages) and the backend is implemented with Cloud Functions. 
API Gateway is used to expose the Cloud Functions for the web user interface.

Refer to [this tutorial](https://console.bluemix.net/docs/solution-tutorials/serverless-api-webapp.html) for instructions.


## The three cloudlets include:

### Customer Repository:

This cloudlet facilitates the storage of road user information (bio data, address, car color, license plate etc.) in a NoSQL database. This is useful to keep track of who owns what car, in the case of a traffic rule violation. 
This cloudlet makes use of Cloud Functions to communicate with the created Cloudant database. PUT and GET requests are sent to the API Gateway using the following apiUrl = 'https://c094c5b1.us-south.apigw.appdomain.cloud/repository'. 
Users are able to post and view customer information as well as contact the Administrator provided they are able to log into the system.

> The Public Cloud Functions along with the defined Node.js scripts saved in the actions folder were used to power this cloudlet.

### Traffic analysis and Visualization:

This cloudlet aims at identifying areas with highest traffic counts as well as traffic variation throughout the day. This could help people avoid areas with a concentrated amount of traffic.



### Identification of traffic rule violators:

This cloudlet focuses on using visual/text recognition to identify number plates of offenders who ignore the “red light”. This improves traffic safety.



### How to access the Wakanda Traffic Department system:

Visit the following path:

The username is: wakanda 		(case sensitive)
The password is: FOREVER 	(case sensitive)

After logging in users will be able to navigate to the respective cloudlets using the website user interface.

Alternatively, clone the repository and open docs/index.html using your preferred browser to interact with the site.




See [License.txt](License.txt) for license information.
