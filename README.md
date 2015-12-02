# onebox-ticketing-api

## API to let an onsale channel to:
+ Search for events, sessions, venue price zones and its availability
+ Provide a complete shopping cart management capabilities
+ Book tickets in two simple steps:
  + Reserve tickets by locking its availability for a while
  + Confirm reserved tickets
+ Release Locked tickets
+ Cancel an already booked and confirmed tickets.

To do so, we have used a **API Blueprint** standard, **apiary** as an online editing and mocking tool, **aglio** to document it and **getsandbox** as a sandbox provider:
+ [API Blueprint](https://apiblueprint.org/)
+ [apiary.io](http://docs.oneboxticketingapi.apiary.io/)
+ [getsandbox.com](http://onebox-ticketing-api.getsandbox.com/)
+ [aglio](https://github.com/danielgtaylor/aglio)
+ [github](https://github.com/joliva-ob/onebox-ticketing-api)
+ [onebox-developer](http://developer.oneboxtickets.com/ticketing-api)

### Usage
1 edit the api blueprint document with apiary.io, or edit directly with Atom + blueprint plugin preview, language and lintr validation. This will provide a .md or .apib file.

2 generate the documentation from the .apib file with aglio:
```
aglio -i onebox-ticketing-api.apib -o welcome.html
```
from the command line.

3 update the online mock service by singin at https://getsandbox.com, going to onebox-ticketing-api and re-importing source from the .apib file. And finally, mock will be available for testing at: http://onebox-ticketing-api.getsandbox.com/<path_api>, ie: /dynamic-pricing-api/1.0/prices from any browser, curl -X, postman or soapui.

4 Apiary.io is already connected with github, so should be already up to date.
