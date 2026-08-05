# bbosa
THE bbosa MODULE IN PYTHON

# bbosa

**A versatile Python utility module that makes common tasks simple.**

File operations • Network tools • Colors • Math helpers • YouTube downloading • Remote mouse control • Android/Termux support

[![PyPI version](https://img.shields.io/pypi/v/bbosa.svg)](https://pypi.org/project/bbosa/)
[![Python](https://img.shields.io/pypi/pyversions/bbosa.svg)](https://pypi.org/project/bbosa/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## ✨ Features

- **File operations** — read, write, append, delete, list directories
- **Network tools** — get IP, check ports, fetch website source
- **YouTube downloader** — download videos easily
- **Colored terminal output** — red, green, blue, bold, etc.
- **Math helpers** — add, multiply, power, comparisons, count
- **System utilities** — run commands, typewriter effect, wait
- **Remote mouse control** — control PC mouse over WiFi/USB (optional)
- **Android / Termux support** — properties, toast notifications
- **Extra helpers** — date/time, email/URL validation, JSON save/load

---

## 📦 Installation

### Basic (core features only)
```bash
pip install bbosa
With optional features
Bash# With mouse control support
pip install bbosa[mouse]

# Full installation (all optional features)
pip install bbosa[full]
Requirements: Python ≥ 3.7

🚀 Quick Start
Pythonfrom bbosa import Bbosa

b = Bbosa()

# See all available functions
print(b.get_help())
Examples
File operations
Pythonb.write_file("hello.txt", "Hello from bbosa!")
print(b.read_file("hello.txt"))
b.append_file("hello.txt", "\nSecond line")
print(b.file_exists("hello.txt"))   # True
b.delete_file("hello.txt")
Colors
Pythonprint(b.red("Error message"))
print(b.green("Success!"))
print(b.bold(b.cyan("Important note")))
Math helpers
Pythonprint(b.add(10, 5))          # 15
print(b.power(2, 8))         # 256
print(b.count("hello"))      # 5
print(b.more(10, 3))         # True
Network
Pythonprint(b.get_ip("google.com"))
print(b.check_port("127.0.0.1", 80))
YouTube download
Pythonb.download_video("https://www.youtube.com/watch?v=xxxxx")
Typewriter effect
Pythonb.type_effect("Hello, this appears slowly...", delay=0.05)
System
Pythonprint(b.get_current_dir())
print(b.get_date())
print(b.get_time())
b.run_command("ls -la")      # careful with this
Remote mouse (requires bbosa[mouse])
Pythonb.mouse(port=5000)   # starts remote control server

📚 Full Function Reference
File Operations









































MethodDescriptionwrite_file(file, content)Write content to a fileappend_file(file, content)Append content to a fileread_file(file)Read and return file contentdelete_file(file)Delete a filefile_exists(file)Check if file existslist_directory(path)List contents of a directorylist_current_dir()List current working directoryget_current_dir()Return current working directory
Colors

























MethodDescriptionred(text), green(text), yellow(text)Colored textblue(text), purple(text), cyan(text)Colored textbold(text)Bold textcolorize(text, color)Custom color
Network

























MethodDescriptionget_ip(hostname)Resolve hostname to IPcheck_port(ip, port)Check if a port is openget_source(url)Fetch HTML source of a URLdownload_video(url)Download YouTube video
Math





























MethodDescriptionadd(a, b), sub(a, b), mult(a, b), div(a, b)Basic arithmeticpower(a, b)Exponentiationfloor_div(a, b)Integer divisionless(a, b), more(a, b)Comparisonscount(item)Length of string / list / dict
System & Utilities









































MethodDescriptionrun_command(cmd)Run a system commandtype_effect(text, delay)Typewriter effectwait(seconds)Sleep / delayget_date(), get_time()Current date / timeis_valid_email(email)Validate emailis_valid_url(url)Validate URLjson_save(data, file)Save dict to JSONjson_load(file)Load JSON file
Android / Termux





















MethodDescriptionget_android_properties()Get device propertiesandroid_find()Android find helpershow_toast(message)Show toast notification
Remote Control













MethodDescriptionmouse(port=5000)Start remote mouse server (PC only)

🛠️ Development
Bashgit clone https://github.com/tokayasurecah-stack/bbosa.git
cd bbosa
pip install -e ".[full]"

📄 License
MIT License © Tony Bbosa Kamandwa

👨‍💻 Author
Tony Bbosa Kamandwa
Uganda

GitHub: tokayasurecah-stack
Email: tokayasurecah@gmail.com


🤝 Contributing
Contributions, issues and feature requests are welcome!
Feel free to open an issue or submit a pull request.

⭐ Show your support
If this project helped you, give it a ⭐ on GitHub!
text
