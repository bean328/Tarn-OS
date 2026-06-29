##Comming Soon!

Tarn is a Unix style operating system for the ESP32 S3. The kernel stays resident, and your code runs as a guest on top of it. That means you flash the OS once and then you can load scripts, Python programs, or WASM apps at runtime without reflashing or rebooting. It gives you a shell, a filesystem (PEXFS), a MicroPython REPL, an SSH server, and full register level access to every pin and peripheral.

Under the hood it runs a software MMU with demand paging on a chip that has no hardware MMU. That is the trick that makes virtual address spaces and process isolation possible. The whole thing fits in about 3 to 5 megabytes of RAM, leaving the rest of the 8.5 megabytes for your applications.

It is designed to be operated by a human over USB or by an AI agent over SSH. Plug it in and you get a console. Connect over WiFi and you get a real shell. From there you can write Python, toggle GPIO, read sensors, and treat the microcontroller like a tiny Linux box.

It is probably the most complete Unix style OS running on an ESP32 S3 today. Not because it is the fastest or the biggest, but because it gives you a real operating environment without the compile flash cycle. It boots instantly, survives power loss, and costs five dollars.
