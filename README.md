# wowzator
A Configuration Manager for Wowza Streaming Engine

## Installation
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
]`
  
