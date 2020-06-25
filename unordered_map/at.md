# at

**Description :** This function returns a reference to the element with the given key. If 

**Example** :

```cpp
// Demonstrates at() 
#include <iostream>
#include <unordered_map>

int main(){
    //declares an empty map. O(1)
    std::unordered_map<char, int> mymap; 
    
    // inserting in to unordered_map with O(1) time on average
    mymap.insert({'A', 1});
    mymap.insert({'C', 3});
    mymap.insert({'b', 2});
    
    // reassigning unordered_map values using at()
    mymap.at('A') = 5;
    mymap.at('b') = 0;
    
    //print unordered_map elements
    for (auto it = mymap.begin(); it != mymap.end(); ++it){ 
        std::cout << it->first << " = "<< it->second << '\n'; 
    }
    return 0;
}

```
**[Run Code](https://rextester.com/WUDJ68420)**
