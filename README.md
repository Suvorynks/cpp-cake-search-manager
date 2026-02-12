# Cake Inventory & Search Manager (C++)

This C++ application is a comprehensive data management tool for handling structured object records. It builds upon basic file I/O operations by introducing specific search algorithms and localized character support for Windows-based console environments.

###  Mathematical & Algorithmic Logic
The program manages a collection of objects $\{c_1, c_2, \dots, c_n\}$ where each $c_i$ has a weight $w_i$.

**Key Calculations:**
* **Average Metric:** Computes the mean weight of all items using the formula:
  $$\text{Average} = \frac{\sum_{i=1}^{n} w_i}{n}$$
* **Search Logic:** Implements a linear search algorithm to locate objects by their name attribute, allowing for efficient data retrieval from the managed collection.
* **Sorting Algorithm:** Organizes data in ascending order based on numeric weight to improve data visualization.



###  Key Features
* **Advanced Search:** Allows users to find specific records in the dataset by name, demonstrating a practical implementation of data lookup.
* **File Persistence:** Seamlessly interacts with `cakes.txt` for long-term data storage and retrieval using `<fstream>`.
* **Windows Localization:** Utilizes `SetConsoleCP(1251)` and `SetConsoleOutputCP(1251)` to ensure correct encoding and display of Cyrillic text in the terminal.
* **Data Integrity:** Features functions for clearing existing data before reloading from files to prevent duplication.

###  Technical Stack
* **Language:** C++
* **Standard Headers:** `<vector>`, `<string>`, `<algorithm>`, `<fstream>`.
* **Platform Specifics:** `<windows.h>` for character encoding management.

###  How to Use
1. Prepare a `cakes.txt` file with data formatted as `Name Weight`.
2. Compile and run the application.
3. Use the interactive menu to add cakes, calculate averages, sort the list, or search for a specific cake by name.
4. Save your changes back to the file to persist data between sessions.
