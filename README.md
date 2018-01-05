Sprint.Filter.OData.v4
===================

This version of the project has the purpose to implement the compatibility with the OData v4 syntax.
The backward compatibility it's not fully granted.

## Main changes

* The deserializer supports datetime in OData v4 syntax.
* The deserializer supports guid in OData v4 syntax.
* The deserializer supports the function contains (the equivalent of substringof) defined in the OData v4 syntax.

## Example

 ```csharp Filter.Deserialize<Customer>("MyDate eq 2016-12-31T23:00:00.000Z");
//result: t => (t.MyDate == Convert(12/31/2016 23:00:00))
