# swap

**Description :** This function exchanges all elements of one map with another map with elements of the same type.

**Example** :

```cpp
// Demonstrates swap() 
#include <iostream>
#include <unordered_map>

int main(){
    //declares two empty maps. O(1)
    std::unordered_map<char, int> mymap; 
    std::unordered_map<char, int> yourmap;
    
    // inserting in to unordered_map with O(1) time on average
    mymap.insert({'A', 1});
    mymap.insert({'N', 3});
    yourmap.insert({'b', 2});
    mymap.swap(yourmap);
    
    //print unordered_map elements
    for (auto it = mymap.begin(); it != mymap.end(); ++it){ 
        std::cout << it->first << " = "<< it->second << '\n'; 
    }
    for (auto it = yourmap.begin(); it != yourmap.end(); ++it){ 
        std::cout << it->first << " = "<< it->second << '\n'; 
    }
    return 0;
}

```
**[Run Code](https://rextester.com/YIY83962)**
