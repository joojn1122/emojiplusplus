# Emoji++


> `Emoji++` is **enhanced** `c++`
>> Not every compiler supports **emoji macros**!

#### Sample code without emojis
```c++
#include <iostream>
#include <cstring>

int main() {
    std::string text = "Hello world!";
    
    // all of this is equivalent to std::cout << text;
    const char* text_ = text.c_str();
    auto addr = reinterpret_cast<unsigned long>(text_);

    for(int i = 0; i < strlen(text_); i++) {
        std::cout << *reinterpret_cast<char*>(addr + (i * sizeof(char)));
    }

    return 0;
}
```


#### With emojis 😎
```c++
#include "emoji.h"
#include <iostream>
#include <cstring>

🔟 🚪︵︶ ︷

    🔤 text 💾 "Hello world!" 🛑
    🧱 🅰️👉 text_ 💾 text.c_str︵︶ 🛑
    🚗 addr = 🎭︿😊 🥒﹀︵text_︶ 🛑

    🔀 ︵🔟 i 💾 0🛑 i ︿ strlen︵text_︶🛑 i➕➕︶ ︷
        📝 ︽ 👉🎭︿🅰️👉﹀︵addr ➕ ︵i 👉 📏︵🅰️︶︶︶ 🛑
    ︸

    🔙 0 🛑
︸
```


#### List of emojis
- TODO
