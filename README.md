*Comming soon*

Tarn is a Unix style operating system for the ESP32 S3. The kernel stays resident, and your code runs as a guest on top of it. That means you flash the OS once and then you can load scripts, Python programs, or WASM apps at runtime without reflashing or rebooting. It gives you a shell, a filesystem (PEXFS), a MicroPython REPL, ASSEMBLY compiler, tiny C++ compiler, an SSH server, and full register level access to every pin and peripheral.

Under the hood it runs a software MMU with demand paging on a chip that has no hardware MMU. That is the trick that makes virtual address spaces and process isolation possible. The whole thing fits in megabytes of RAM (still busy optimizing it to run on the original esp32 chip), leaving the rest of the ram for your applications and backround tasks.

It is designed to be operated over USB or over SSH. Plug it in and you get a console. Connect over WiFi and you get a full ssh shell. From there you can write Python, toggle GPIO, read sensors, and treat the microcontroller like a full computer. 

It is probably the most complete Unix style OS running on an ESP32 S3 today, because it gives you a real operating system enviroment with process isolation and commands that is cool like git clone or curl.
