## JSON

- JavaScript Object Notation.
- JSON is text, written with JavaScript object notation.
- JSON is a syntax for storing and exchanging data.
- JSON is a lightweight data-interchange format.

> JSON uses JavaScript syntax, but the JSON format is text only.
> Text can be read and used as a data format by any programming language.

**Sending data:** If you have data stored in a JavaScript object, you can convert the object into JSON, and send it to a server.

**Example:**

```javascript
var myObj = { name: "Shruthi", age: 21, city: "New York" };
var myJSON = JSON.stringify(myObj);
```

**Receiving data:** If you receive data in JSON format, you can convert it into a JavaScript object.

**Example:**

```javascript
var myJSON = '{"name":"Shruthi", "age":21, "city":"New York"}';
var myObj = JSON.parse(myJSON);
```

- JavaScript has a built in function to convert a string, written in JSON format, into native JavaScript objects.

**JSON and JS differences:**

- In JSON, keys must be strings, written with double quotes.
- In JavaScript, keys can be strings, numbers, or identifier names.

## XML

- XML stands for eXtensible Markup Language.
- XML was designed to store and transport data.
- XML was designed to be both human- and machine-readable.
- XML was designed to be self-descriptive.

**XML syntax:**

```xml
<root>
  <child>
    <subchild>.....</subchild>
  </child>
</root>
```

- XML documents form a tree structure that starts at "the root" and branches to "the leaves".

**XML and HTML differences:**

- XML was designed to carry data - with focus on what data is.
- HTML was designed to display data - with focus on how data looks
- XML tags are not predefined like HTML tags are.

## JSON vs XML

- JSON and XML can be used to receive data from a web server.
- JSON object has a type whereas XML data is typeless.
- JSON does not provide namespace support while XML provides namespaces support.
- JSON has no display capabilities whereas XML offers the capability to display data.
- JSON is less secured whereas XML is more secure compared to JSON.
- XML has to be parsed with an XML parser. JSON can be parsed by a standard JavaScript function.

> XML is much more difficult to parse than JSON.
> JSON is parsed into a ready-to-use JavaScript object.

**JSON is Like XML Because**

- Both JSON and XML are "self describing" (human readable)
- Both JSON and XML are hierarchical (values within values)
- Both JSON and XML can be parsed and used by lots of programming languages
- Both JSON and XML can be fetched with an XMLHttpRequest

**JSON example:**

```javascript
{"employees":[
  { "firstName":"John", "lastName":"Doe" },
  { "firstName":"Anna", "lastName":"Smith" },
  { "firstName":"Peter", "lastName":"Jones" }
]}
```

**XML example:**

```xml
<employees>
  <employee> <firstName>John</firstName> <lastName>Doe</lastName> </employee>
  <employee> <firstName>Anna</firstName> <lastName>Smith</lastName> </employee>
  <employee> <firstName>Peter</firstName> <lastName>Jones</lastName> </employee>
</employees>
```
