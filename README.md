# Hands-on--10
This is a repository of "UTA ID:1002201193". With student email "mxo1193@mavs.uta.edu".



This code implements a hash table data structure, which is a way to store key-value pairs for efficient retrieval. Think of it like a dictionary where you can look up a word and find its definition quickly.

Working:

When we insert a key-value pair into the hash table using the insert_item method, the code calculates a hash value for the key. This hash value determines where in the hash table the key-value pair will be stored.
If there's already a key-value pair stored at that location (i.e., a collision), the new pair is added to a linked list at that location.
The code also keeps track of how full the hash table is. If it gets too full (more than 75% full), it automatically doubles its size to accommodate more items. This helps maintain efficiency by keeping the load factor low.
When we remove a key-value pair using the remove_item method, the code finds the pair based on the key and removes it from the hash table. If the hash table becomes less than 25% full after removals, it automatically halves its size to conserve memory.
Finally, the retrieve_value method allows you to look up the value associated with a given key.

output:

The output "20" indicates that when we looked up the key "15" in the hash table using the retrieve_value method, it returned the corresponding value "20". This means that the key "15" was successfully inserted into the hash table earlier.
The output "None" indicates that after removing the key "15" from the hash table using the remove_item method, when we tried to retrieve its value again, it returned "None". This confirms that the key "15" was indeed removed from the hash table.
