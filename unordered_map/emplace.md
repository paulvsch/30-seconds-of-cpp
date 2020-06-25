# emplace

**Description :** This function creates a new element in the unordered map and increases the size by 1 provided the key does not already exist. After creating the key, the function returns a pair consisting of an iterator to the created or existing element, and a boolean. The boolean is true if emplace created a new element the value is false if the element already existed.

**Example** :

```cpp
// Demonstrates emplace() 
#include <iostream>
#include <unordered_map>

int main(){
    //declares an empty map. O(1)
    std::unordered_map<char, int> mymap; 
    
    
    // inserting in to unordered_map with O(1) time on average
    mymap.emplace('A', 1);
    mymap.emplace('b', 2);
    mymap.emplace('c', 3);
    //print unordered_map elements
    for (auto it = mymap.begin(); it != mymap.end(); ++it){ 
        std::cout << it->first << " = "<< it->second << '\n'; 
    }
    return 0;
}

```
**[Run Code](https://rextester.com/DZMBR10084)**
