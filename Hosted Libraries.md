# Usage

## Links

Use:
* cdn.library.isc
* cdn.isc
* cdn.delivr.isc

## URL Structure

### Typical usage
	//cdn.library.isc/{projectName}/{version}/{file}
	Example: //cdn.delivr.isc/jquery/1.11.0/jquery.min.js

When you want all the files in that version folder as a single compressed archive:
  //cdn.library.isc/{projectName}/{version}/{projectName}.zip
	//cdn.delivr.isc/{projectName}/{version}/{projectName}.zip

Downloads the three projects' mainfile from their latest versions as a single collated file:
	//cdn.library.isc/g/{projectName},{projectName},{projectName}
	//cdn.delivr.isc/g/{projectName},{projectName},{projectName}

You may specify a specific version or version-branch per file:
	//cdn.library.isc/g/{projectName}@{version},{projectName}@{versionAlias},{projectName}
	//cdn.delivr.isc/g/{projectName}@{version},{projectName}@{versionAlias},{projectName}

You may also select more than one file from a project (typically for plug-ins that ship with the project):
	//cdn.library.isc/g/{projectName}@{version}({filepath1}+{filepath2}),{projectName}@{versionAlias},{projectName}
	//cdn.delivr.isc/g/{projectName}@{version}({filepath1}+{filepath2}),{projectName}@{versionAlias},{projectName}



## Version aliasing

For latest version use:

	//cdn.library.isc/{projectName}/latest/{file}
	//cdn.delivr.isc/{projectName}/latest/{file}

You can also load latest versions per branch:

	//cdn.library.isc/{projectName}/3.8/{file} Latest in 3.8 branch
	//cdn.delivr.isc/{projectName}/3.8/{file} Latest in 3.8 branch

	//cdn.library.isc/{projectName}/3/{file} Latest in 3 branch
	//cdn.delivr.isc/{projectName}/3/{file} Latest in 3 branch

To automatically load the main file of a project use:

	//cdn.library.isc/{projectName}/{version}/mainfile
	//cdn.delivr.isc/{projectName}/{version}/mainfile

Depending on the project, jsDelivr will automatically load the main file as configured in info.ini with correct MIME HTTP headers. If no mainfile parameter was specified, the request will result in 404 error.






----



<h1>Hosted Libraries</h1>

The iSC Services CDN Hosted Libraries is a stable, reliable, high-speed, globally available, open source CDN that allows developers to host their own projects and anyone to link to our hosted files in their websites.

We offer a stable CDN that can be used in production even on popular websites with huge amounts of traffic. There are no bandwidth limits or premium features and its completely free to use by anybody.

All kinds of files are allowed, including JavaScript libraries, jQuery plugins, CSS frameworks, fonts and more.

You can use this repo to make your own changes and improve the contents of jsDelivr's CDN. Feel free to open issues and pull requests if you think something should be changed.

All changes made to this repo are synced to the CDN. It can take a few minutes for the changes to appear on the website.


<h2>Libraries</h2>

To load a hosted library, copy and paste the HTML snippet for that library (shown below) in your web page. For instance, to load jQuery, embed the <script src="https://cdn.isc/libs/jquery/2.1.3/jquery.min.js"></script> snippet in your web page.

We recommend that you load libraries from the CDN via HTTPS, even if your own website only uses HTTP. Nowadays, performance is fast, and caching works just the same. The CDN's files are served with CORS and Timing-Allow headers and allowed to be cached for 1 year.


<h3>AngularJS</h3>

snippet:
    <script src="https://cdn.isc/libs/angularjs/1.3.14/angular.min.js"></script> 

site:
    angularjs.org

stable versions:
	* 1.0.2
	* 1.0.1

unstable versions:
	1.4.0-beta6
