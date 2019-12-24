# KnTL
Kompile 'n Terminal Launch

A Competitive Programming tool for transpiling C++ codes

<h3>Installation</h3>

simply compile `` KnTL.cpp ``

<h3>Commands</h3>

``<kntl_executable> <cpp_file> [crRiI]``

Explanation:
  
``[crRpP]`` is optional
<ul>
  <li> <code>c</code> = compile </li>
  <li> <code>r</code> = run </li>
  <li> <code>R</code> = compile and run </li>
  <li> <code>i</code> = run with IN </li>
  <li> <code>I</code> = compile and run with IN </li>
</ul>

<h3>Usage</h3>

put
``#define DEBUG(...)``
In your source code

Stdout generated from DEBUG() will be colored for easier debugging

<h4>Example</h4>

Code.cpp:
```cpp
#include<iostream>
#define DEBUG(...)

using namespace std;

int main() {
  cout << "Konnichi wa World-kun" << endl;

  DEBUG(cout << "I just said hello to world-kun (blushes)" << endl;)

  string str;
  getline(cin, str);

  cout << str << endl;
  
  return 0;
}
```
IN:
```
H-h-how are you?
```

Command: ``` kntl.exe Code.cpp I ```
Output:
![image](https://user-images.githubusercontent.com/43501223/71398500-33b71900-2653-11ea-8178-b6bfdc809278.png)

Now everything you say and do, it all sparkles so brightly

<h3>Configuration</h3>

The default code compiles using ``g++`` with the flag ``-std=c++11``

If you would like to change the flag, simply replace ``string GPP = "g++ -stdc++11"`` in ``KnTL.cpp`` with whatever flag you want, and the recompile it

For example: ``string GPP = "g++ -std=c++14 -O2"``
