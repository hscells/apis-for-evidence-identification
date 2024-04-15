# 2.1 Data Formats

When you access an API, you usually get back a response in a machine-readable format like JSON or XML. These formats are used to structure and transmit data between different software applications. In this section, we'll learn more about these data formats and how they are used in APIs.

## JSON

JSON (JavaScript Object Notation, pronounced /ˈdʒeɪsən/; also /ˈdʒeɪˌsɒn/) is an open standard file format and data interchange format that uses human-readable text to store and transmit data objects consisting of attribute–value pairs and arrays (or other serializable values). It is a commonly used data format with diverse uses in electronic data interchange, including that of web applications with servers. [[wikipedia](https://en.wikipedia.org/wiki/JSON)]

This is the main data format used in APIs because it is easy to read and write, lightweight, and easy to parse. Almost all the APIs we'll be using in this workshop return data in JSON format.

### Example

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "isAlive": true,
  "age": 27,
  "address": {
    "streetAddress": "21 2nd Street",
    "city": "New York",
    "state": "NY",
    "postalCode": "10021-3100"
  },
  "phoneNumbers": [
    {
      "type": "home",
      "number": "212 555-1234"
    },
    {
      "type": "office",
      "number": "646 555-4567"
    }
  ],
  "children": [],
  "spouse": null
}
```

## XML

Extensible Markup Language (XML) is a markup language and file format for storing, transmitting, and reconstructing arbitrary data. It defines a set of rules for encoding documents in a format that is both human-readable and machine-readable. The World Wide Web Consortium's XML 1.0 Specification of 1998 and several other related specifications —all of them free open standards—define XML. [[wikipedia](https://en.wikipedia.org/wiki/XML)]

### Example

```xml
<person>
  <firstName>John</firstName>
  <lastName>Smith</lastName>
  <isAlive>true</isAlive>
  <age>27</age>
  <address>
    <streetAddress>21 2nd Street</streetAddress>
    <city>New York</city>
    <state>NY</state>
    <postalCode>10021-3100</postalCode>
  </address>
  <phoneNumbers>
    <phoneNumber>
      <type>home</type>
      <number>212 555-1234</number>
    </phoneNumber>
    <phoneNumber>
      <type>office</type>
      <number>646 555-4567</number>
    </phoneNumber>
  </phoneNumbers>
  <children/>
  <spouse/>
</person>
```

## CSV

Comma-separated values (CSV) is a text file format that uses commas to separate values, and newlines to separate records. A CSV file stores tabular data (numbers and text) in plain text, where each line of the file typically represents one data record. Each record consists of the same number of fields, and these are separated by commas in the CSV file. If the field delimiter itself may appear within a field, fields can be surrounded with quotation marks. [[wikipedia](https://en.wikipedia.org/wiki/Comma-separated_values)]

### Example

```csv
firstName,lastName,isAlive,age,streetAddress,city,state,postalCode,phoneNumbers
John,Smith,true,27,21 2nd Street,New York,NY,10021-3100,"home: 212 555-1234, office: 646 555-4567"
``` 

---
[top](../README.md)<br/>
[previous: Finding APIs](../1-what/1-3-finding-apis.md)<br/>
[next: Authentication and Rate limits](2-2-authentication-and-rate-limits.md)<br/>

