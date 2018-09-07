# ASCOM Perseus Commander :telescope:

[![ASCOM DOWNLOAD](https://img.shields.io/badge/Optec-Perseus%20Driver%20Download-blue.svg?longCache=true&style=for-the-badge&&colorA=242958&colorB=88a8be&logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz48c3ZnIHZlcnNpb249IjEuMSIgaWQ9IkxheWVyXzEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHg9IjBweCIgeT0iMHB4IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHN0eWxlPSJlbmFibGUtYmFja2dyb3VuZDpuZXcgMCAwIDI0IDI0OyIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSI+PHN0eWxlIHR5cGU9InRleHQvY3NzIj4uc3Qwe2ZpbGw6I0ZGRkZGRjt9PC9zdHlsZT48dGl0bGUgIGlkPSJzaW1wbGVpY29ucy1kaXNjb3Zlci1pY29uIj5EaXNjb3ZlciBpY29uPC90aXRsZT48Y2lyY2xlIGNsYXNzPSJzdDAiIGN4PSIxMiIgY3k9IjEyIiByPSIxMiIvPjwvc3ZnPg==)](https://www.optecinc.com/astronomy/software/download/older_versions/OptecPerseusSetup(1.0.5).zip) [![ASCOM DOWNLOAD](https://img.shields.io/badge/ASCOM%206.4-Download-blue.svg?longCache=true&colorA=002157&colorb=0061FF&style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz48c3ZnIHZlcnNpb249IjEuMSIgaWQ9IkxheWVyXzEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHg9IjBweCIgeT0iMHB4IiB2aWV3Qm94PSIwIDAgMTIgMTEiIHN0eWxlPSJlbmFibGUtYmFja2dyb3VuZDpuZXcgMCAwIDEyIDExOyIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSI%2BPHN0eWxlIHR5cGU9InRleHQvY3NzIj4uc3Qwe2ZpbGw6I0ZGRkZGRjt9PC9zdHlsZT48Zz48Zz48cGF0aCBjbGFzcz0ic3QwIiBkPSJNOSwxMWMtMC4yLDAtMC41LTAuMS0wLjctMC4yQzcuOSwxMC42LDcuNywxMCw3LjksOS41QzgsOS40LDguMSw5LjMsOC4xLDkuMmMwLjEtMC4xLDAuMS0wLjMsMC4xLTAuNWMtMC4zLTAuNy0wLjYtMS4zLTAuOS0yQzcuMiw2LjUsNy4yLDYuNSw2LjksNi42Yy0wLjcsMC4zLTEuNCwwLjctMi4xLDFDNC4yLDgsMy41LDguMywyLjcsOC43QzIuNSw4LjgsMi4zLDksMi4zLDkuM2MwLDAuMi0wLjIsMC40LTAuMywwLjVjLTAuNiwwLjUtMS4zLDAuMy0xLjctMC4yYy0wLjMtMC4zLTAuMy0wLjgsMC0xLjJDMC40LDguMiwwLjcsOCwxLDhjMC40LDAsMC42LTAuMiwwLjctMC41YzAuNy0xLjUsMS40LTMsMi4yLTQuNUM0LDIuOSw0LjEsMi42LDQuMywyLjRjMC4xLTAuMywwLjEtMC41LTAuMS0wLjdDMy43LDEuMiwzLjksMC40LDQuNSwwLjFDNS4xLTAuMSw1LjcsMCw2LjEsMC41YzAuMiwwLjMsMC4yLDAuNiwwLDFDNi4xLDEuNiw2LDEuNyw1LjksMS44QzUuNywxLjksNS43LDEuOSw1LjgsMi4xYzAuMywwLjcsMC42LDEuNCwwLjksMi4xYzAuMiwwLjQsMC40LDAuOSwwLjYsMS4zYzAuMSwwLjIsMC4yLDAuMywwLjQsMC4yQzguMyw1LjUsOC44LDUuMiw5LjMsNWMwLjEsMCwwLjItMC4xLDAuMi0wLjFjMC4xLTAuMSwwLjItMC4yLDAuMi0wLjNjLTAuMS0wLjYsMC40LTEsMC45LTEuMWMwLjQtMC4xLDAuNywwLDEsMC4zYzAuNSwwLjQsMC42LDEuMy0wLjIsMS43Yy0wLjMsMC4xLTAuNSwwLjItMC44LDAuMWMtMC4xLDAtMC4xLDAtMC4yLTAuMWMtMC4zLTAuMi0wLjUtMC4yLTAuOC0wLjFDOS4zLDUuNCw5LjEsNS41LDguOCw1LjdDOC41LDUuOCw4LjEsNiw3LjgsNi4yQzcuNiw2LjMsNy42LDYuMyw3LjcsNi41QzgsNy4yLDguMyw3LjksOC42LDguNmMwLjEsMC4yLDAuMiwwLjMsMC41LDAuM2MwLjMsMCwwLjUsMC4xLDAuOCwwLjRjMC40LDAuNCwwLjQsMS4yLTAuMSwxLjVDOS41LDEwLjksOS4yLDExLDksMTF6IE0yLjMsOC40YzAuMSwwLDAuMy0wLjEsMC40LTAuMmMxLjQtMC43LDIuOC0xLjMsNC4xLTJDNyw2LjEsNyw2LjEsNi45LDUuOEM2LjcsNS4zLDYuNSw0LjcsNi4yLDQuMkM1LjksMy42LDUuNywyLjksNS40LDIuM0M1LjMsMi4yLDUuMiwyLjEsNS4xLDIuMWMtMC4yLDAtMC4zLDAuMS0wLjMsMC4yYzAsMC4xLTAuMSwwLjItMC4xLDAuM0M0LjEsMy44LDMuNSw0LjksMi45LDYuMUMyLjYsNi43LDIuMyw3LjQsMiw4LjFDMS45LDguMywyLDguNCwyLjMsOC40eiIvPjwvZz48L2c%2BPC9zdmc%2B)](https://github.com/ASCOMInitiative/ASCOMPlatform/releases/download/Platform6.4Release/ASCOMPlatform64.exe) [![ASCOM DOWNLOAD](https://img.shields.io/badge/ASCOM%20DEVELOPER%20TOOLS-Download-blue.svg?longCache=true&colorA=002157&colorb=0061FF&style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz48c3ZnIHZlcnNpb249IjEuMSIgaWQ9IkxheWVyXzEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHg9IjBweCIgeT0iMHB4IiB2aWV3Qm94PSIwIDAgMTIgMTEiIHN0eWxlPSJlbmFibGUtYmFja2dyb3VuZDpuZXcgMCAwIDEyIDExOyIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSI%2BPHN0eWxlIHR5cGU9InRleHQvY3NzIj4uc3Qwe2ZpbGw6I0ZGRkZGRjt9PC9zdHlsZT48Zz48Zz48cGF0aCBjbGFzcz0ic3QwIiBkPSJNOSwxMWMtMC4yLDAtMC41LTAuMS0wLjctMC4yQzcuOSwxMC42LDcuNywxMCw3LjksOS41QzgsOS40LDguMSw5LjMsOC4xLDkuMmMwLjEtMC4xLDAuMS0wLjMsMC4xLTAuNWMtMC4zLTAuNy0wLjYtMS4zLTAuOS0yQzcuMiw2LjUsNy4yLDYuNSw2LjksNi42Yy0wLjcsMC4zLTEuNCwwLjctMi4xLDFDNC4yLDgsMy41LDguMywyLjcsOC43QzIuNSw4LjgsMi4zLDksMi4zLDkuM2MwLDAuMi0wLjIsMC40LTAuMywwLjVjLTAuNiwwLjUtMS4zLDAuMy0xLjctMC4yYy0wLjMtMC4zLTAuMy0wLjgsMC0xLjJDMC40LDguMiwwLjcsOCwxLDhjMC40LDAsMC42LTAuMiwwLjctMC41YzAuNy0xLjUsMS40LTMsMi4yLTQuNUM0LDIuOSw0LjEsMi42LDQuMywyLjRjMC4xLTAuMywwLjEtMC41LTAuMS0wLjdDMy43LDEuMiwzLjksMC40LDQuNSwwLjFDNS4xLTAuMSw1LjcsMCw2LjEsMC41YzAuMiwwLjMsMC4yLDAuNiwwLDFDNi4xLDEuNiw2LDEuNyw1LjksMS44QzUuNywxLjksNS43LDEuOSw1LjgsMi4xYzAuMywwLjcsMC42LDEuNCwwLjksMi4xYzAuMiwwLjQsMC40LDAuOSwwLjYsMS4zYzAuMSwwLjIsMC4yLDAuMywwLjQsMC4yQzguMyw1LjUsOC44LDUuMiw5LjMsNWMwLjEsMCwwLjItMC4xLDAuMi0wLjFjMC4xLTAuMSwwLjItMC4yLDAuMi0wLjNjLTAuMS0wLjYsMC40LTEsMC45LTEuMWMwLjQtMC4xLDAuNywwLDEsMC4zYzAuNSwwLjQsMC42LDEuMy0wLjIsMS43Yy0wLjMsMC4xLTAuNSwwLjItMC44LDAuMWMtMC4xLDAtMC4xLDAtMC4yLTAuMWMtMC4zLTAuMi0wLjUtMC4yLTAuOC0wLjFDOS4zLDUuNCw5LjEsNS41LDguOCw1LjdDOC41LDUuOCw4LjEsNiw3LjgsNi4yQzcuNiw2LjMsNy42LDYuMyw3LjcsNi41QzgsNy4yLDguMyw3LjksOC42LDguNmMwLjEsMC4yLDAuMiwwLjMsMC41LDAuM2MwLjMsMCwwLjUsMC4xLDAuOCwwLjRjMC40LDAuNCwwLjQsMS4yLTAuMSwxLjVDOS41LDEwLjksOS4yLDExLDksMTF6IE0yLjMsOC40YzAuMSwwLDAuMy0wLjEsMC40LTAuMmMxLjQtMC43LDIuOC0xLjMsNC4xLTJDNyw2LjEsNyw2LjEsNi45LDUuOEM2LjcsNS4zLDYuNSw0LjcsNi4yLDQuMkM1LjksMy42LDUuNywyLjksNS40LDIuM0M1LjMsMi4yLDUuMiwyLjEsNS4xLDIuMWMtMC4yLDAtMC4zLDAuMS0wLjMsMC4yYzAsMC4xLTAuMSwwLjItMC4xLDAuM0M0LjEsMy44LDMuNSw0LjksMi45LDYuMUMyLjYsNi43LDIuMyw3LjQsMiw4LjFDMS45LDguMywyLDguNCwyLjMsOC40eiIvPjwvZz48L2c%2BPC9zdmc%2B)](http://download.ascom-standards.org/devtools/ConformSetup.exe)


ASCOM external driver control for Optec's Perseus Commander. 
  [Perseus 4-Port Instrument Selector](https://www.optecinc.com/astronomy/catalog/perseus/perseus_4-port.htm)
  [PDF Documentation](https://www.optecinc.com/astronomy/catalog/perseus/pdf/Perseus%20Commander%20Help%20File.pdf)

![alt text](https://www.optecinc.com/astronomy/catalog/perseus/images/Perseus_Commander.png "Perseus 4-Port Instrument Selector")

### Control API
```JavaScript
supportedActions.Add("GetPort1Name");
supportedActions.Add("GetPort2Name");
supportedActions.Add("GetPort3Name");
supportedActions.Add("GetPort4Name");
supportedActions.Add("SetPort1Name");
supportedActions.Add("SetPort2Name");
supportedActions.Add("SetPort3Name");
supportedActions.Add("SetPort4Name");
supportedActions.Add("GetFWVersion");

supportedActions.Add("IsHomed");
supportedActions.Add("Home");
 ```
 
 # License
 ![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg?style=for-the-badge) 
