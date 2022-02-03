# wowzator
### Configuration Manager for Wowza Streaming Engine

This tool is a commandline interactive Configuration Manager, it has been created to help keep the configuration aligned across multiple Wowza servers.

This tool is a configuration manager that lists and compares configuration information about vhosts, applications, smil files, transcoding templates, mediacache items and other parameters.

![Wowzator Screenshot](wowzator-screenshot.png)

### Installation
pip install -r requirements.txt

Create config.json file in the same dir of wowzator executable

Example:

`[
	{
		"name": "or01",
		"address": "10.0.0.99",
		"user": "admin",
		"pw": "mysecret",
		"auth": "digest"
	},
  {
  ...
  }
]
`
  
