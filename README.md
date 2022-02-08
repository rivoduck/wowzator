# wowzator
### Configuration Manager for Wowza Streaming Engine

This tool is an interactive commandline Configuration Manager, it has been created to help keeping the configuration aligned across multiple Wowza servers.

This tool uses a shell-like syntax to list and compare configuration information about vhosts, applications, smil files, transcoding templates, mediacache items and other parameters.

It has no database, it just lazy-fetches configuration information through the Wowza REST APIs to show and compare configuration info.

![Wowzator Screenshot](wowzator-screenshot.png)

### Installation
`pip install -r requirements.txt`

Create config.json file in the same dir of wowzator executable

Example:

	{
        	"secure_mode": "true",
        	"servers": [
			{
				"name": "or01",
				"address": "10.0.0.99",
				"user": "admin",
				"pw": "mysecret",
				"auth": "digest"
			},
			{
				[details of other server(s)...]
			}
		]
	}



Setting "secure_mode" to "false" enables redirection to file and piping of output (eg. "`ls all/apps | grep myapp`" or "`ls all/apps > application_list.txt`").

Note about the "auth" configuration parameter: Wowza after 4.8.5 uses basic authentication while Wowza 4.8.5 and earlier uses digest!!



  
