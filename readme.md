# lib_propertyManager v1.0

lib_propertyManager is easy to use Livecode Property Management system. Short and simple syntax prevents you from declaring and using global variables.

# Installation

######Add the library to your project.
start using stack "lib_propertyManager".

# Usage

## pmSetProp
###### Type: Command
###### Description: Stores the property in local variable scope
##### Parameters:
###### pProp: The property name
###### pVal: The property value
###### pObj: Not required, send to specify whose the property is
##### Usage:
###### pmSetProp "user_id", "123456"
###### $S "user_id", "123456"
###### pmSetProp "buttonLabel", the label of me, the long id of me
###### Short syntax: $S - $S pProp, pVal, pObj
---------------------------------------------------------------------------------------------------

## pmGetProp
###### Type: Function
###### Description: Returns the property value
##### Parameters:
###### pProp: The property name
###### pObj: Not required, send to specify whose the property is
##### Usage:
###### put pmGetProp("user_id") into tUserID
###### loginUser(pmGetProp("user_id"), pmGetProp("password"))
###### loginUser($G("user_id"), $G("password"))
###### set the label of me to pmGetProp("buttonLabel", the long id of me)
###### Short syntax: $G - $G(pProp, pObj)
---------------------------------------------------------------------------------------------------


##### Gurgen Hovhannisyan
##### g.hovhannisyan@digitalpomegranate.com
##### DIGITAL POMEGRANATE LLC
##### 2017
