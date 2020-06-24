# Go-Ini

This implementation is based on these articles:
- [WikiPedia](https://en.wikipedia.org/wiki/INI_file) 
- [Apache](http://commons.apache.org/proper/commons-configuration/apidocs/org/apache/commons/configuration2/INIConfiguration.html)

## Features

- Section
- Global Properties
- Read from file

## Supported value types

- String
- Bool
- Int (0-64)
- Uint (0-64)

## Planned Features

- Section Nesting
  ```ini
  [Section]
  key=value
    [SubSection1]
    key=value
    
    [SubSection2]
    key=value
    
  [Section]
  key=value
  [Section.SubSection1]
  key=value
  [Section.SubSection2]
  key=value
  ```
- Comments above line and in-line (#) (;)
- Multi-line
- Multiple seperators (passwd : abc=def) (a:b = "value")
- Write to file
- Configuration options for features with multiple implementations (like sub-sections)

## Planned Supported value types

- Array (Types above)
