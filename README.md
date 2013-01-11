# CAF (Cloud Assistant Framework)

Co-design permanent, active, stateful, reliable cloud proxies with your web app.

See http://www.cafjs.com 

## CAF Lib Properties

This repository contains a CAF lib to add statically defined properties common to all CAs.


## API

    lib/proxy_prop.js
 
## Configuration Example

### framework.json

None


### ca.json


     "proxies" : [
         {
             "module": "caf_prop/proxy",
             "name": "prop",
             "description": "Provides access to static properties defined in this env",
             "env" : {
                 "whatever" :10,
                 "orSomethingElse" : {
                         "c": "erre",
                         "d": [1,2]
                 }
            }
          }
          ...
      ]
  
  
and your code can access a property as follows:

    this.$.prop.get('orSomethingElse')
    
        
            
 
