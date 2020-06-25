# clear

**Description :** This function is used to remove all elements within a specified unordered map.

**Example** :

```cpp
// Demonstrates clear() 
#include <iostream>
#include <unordered_map>

int main(){
    //declares an empty map. O(1)
    std::unordered_map<char, int> mymap; 
    
    
    // inserting in to unordered_map with O(1) time on average
    mymap.insert({'A', 1});
    mymap.insert({'b', 2});
    mymap.insert({'c', 3});
    std::cout << "Is mymap is empty? " << mymap.empty() << '\n'; //confirming that the map is not empty
    mymap.clear(); 
    std::cout << "Is mymap is empty? " << mymap.empty(); //confirming that the map IS empty after calling clear
    return 0;
}

```
**[Run Code](https://rextester.com/BLCEB24267)**
