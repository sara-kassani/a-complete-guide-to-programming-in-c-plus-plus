***char* and *wchar_t*:**
- are used to store *character codes* (integers associated with characters (A = 65)):
    - a *character set* defines which code represents a certain character.
- *wchar_t* comprises at least 2 bytes, which allows it to store modern Unicode (a 16-bit code used in Windows NT, which contains codes for approximately 35,000 characters in 24 languages) characters.

In general, C++ uses a character set which contains the *ASCII (American Standard Code for Information Interchange) code* (a 7-bit code which defines 32 control and 96 printable characters.