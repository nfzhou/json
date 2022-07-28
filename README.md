# json
A JSON <-> Picat converter based mbionchi's JSON module at at: https://github.com/mbionchi/json-picat

* json_read(File): reads a JSON file into Picat. 
* json_read(): same as json_read(stdin).
* json_write(T): Write Picat term T into JSON format to stdout.

This version incorporates the following improvements:

1. A difference list is used to represent a queue so that it takes constant time to add an element to the queue.

2. It uses Picat's built-in function, to_number(String), to convert a string to a number.

3. The predicate whitespace(Char) uses pattern-matching rules, rather than the built-in predicate member, to check if a character is a whites pace.
