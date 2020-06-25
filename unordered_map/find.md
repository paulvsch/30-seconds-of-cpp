# find

**Description :** This function takes in a key and searches the unordered map for that key. If it is found, it returns an iterator to the element. If it is not found it returns an iterator to the element just past the end of the data.

**Example** :

```cpp
// Demonstrates find() 
#include <iostream>
#include <unordered_map>

int main(){
    //declares an empty map. O(1)
    std::unordered_map<char, int> mymap; 
    
    // inserting in to unordered_map with O(1) time on average
    mymap.insert({'A', 1});
    mymap.insert({'C', 3});
    mymap.insert({'b', 2});
    
    
    //searches for an element in the unordered_map and prints it if found 
    auto it = mymap.find('C');
    if(it != mymap.end()){
        std::cout << it->first << " = "<< it->second << '\n';
    }
    return 0;
}

```
**[Run Code](https://rextester.com/RAKSGB77396)**
