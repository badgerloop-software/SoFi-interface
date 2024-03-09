## SoFi Interface Data Format Specification

The SoFi Interface data format file serves as a communication protocol between software systems and firmware. It provides a structured way to encode and interpret data for seamless interaction between these components.

### Data Format Structure

The data format follows a specific structure for each data element, defined as follows:

```"name":
"name": [bytesize, datatype, minimum value, maximum value]
```

Where:

* `"name"`: Represents the name of the signal.
* `bytesize`: Indicates the size of the data element in bytes.
* `datatype`: Specifies the type of data for the element.
* `minimum value`: Defines the minimum allowable value for the data element.
* `maximum value`: Specifies the maximum allowable value for the data element.

### Encoding Data

Data encoded using this data format should adhere to the following rules:

* Encode data into a bytearray.
* Use little endian encoding.
* Maintain the same order of fields as defined in the dataformat.

This encoding scheme ensures consistency and compatibility between software systems and firmware, ensuring smooth communication and data exchange.
