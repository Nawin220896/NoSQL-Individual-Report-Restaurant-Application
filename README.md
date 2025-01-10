# NoSQL Individual Report: Restaurant Application

**Author**: Naveen Kumar Manokaran  
**Student ID**: 1232482864  

---

## ✨ Project Overview
This project explores the application of NoSQL databases, specifically **UnQLite**, in managing restaurant data for platforms like **Uber Eats, Zomato, Swiggy**, etc. The project provided hands-on experience in handling NoSQL databases to store, retrieve, and process restaurant-related information efficiently.

---

## 📚 Reflection
### Key Steps:
1. **Technology Stack Exploration**:
   - Programming Language: Python
   - NoSQL Database: UnQLite
   - Python Libraries: `math` module (`radians`, `sin`, `cos`, `atan2`), and error handling techniques.

2. **Project Execution**:
   - Analyzed the structure of the database collection using the commands:
     ```python
     from unqlite import UnQLite
     db = UnQLite('sample.db')
     data = db.collection('data')
     ```
   - Implemented and optimized functions for data processing:
     - **FindBusinessBasedOnCity**: Filters businesses based on city.
     - **FindBusinessBasedOnLocation**: Filters businesses based on their proximity to a location.
     - **DistanceFunction**: Calculates the distance between two geographical points.

3. **Testing**:
   - Verified functionality using test cases.
   - Captured outputs in files: `output_city` and `output_loc`.

---

## 🚀 Key Functionalities

### 1. `FindBusinessBasedOnCity`
- **Purpose**: Filters businesses based on the provided city name.
- **Implementation**:
  - Opened the output file (`save_location`) in write mode.
  - Iterated through the collection to find matching cities.
  - Stored matching business details (`name$full_address$city$state`) in the file.

### 2. `FindBusinessBasedOnLocation`
- **Purpose**: Filters businesses based on proximity to a given latitude, longitude, and categories.
- **Implementation**:
  - Checked for category intersections between input and document data.
  - Calculated distances using the `DistanceFunction`.
  - Stored business names within the specified distance in the output file.

### 3. `DistanceFunction`
- **Purpose**: Computes distance between two geographical points using the Haversine formula.

---

## 📝 Lessons Learned
1. **Error Handling**:
   - Implemented robust error handling to manage exceptions like `None` values and missing data.
2. **Data Validation**:
   - Ensured efficient handling of `None` and invalid values in the dataset.
3. **NoSQL Databases**:
   - Learned how NoSQL databases like **UnQLite** efficiently store and retrieve restaurant data for applications.
4. **UnQLite Functionalities**:
   - Explored commands to read, write, and manipulate collections.
5. **Python Optimization**:
   - Improved function implementations by minimizing time and space complexities.
6. **Math Module**:
   - Utilized Python's `math` module for geospatial calculations (`radians`, `sin`, `cos`, `atan2`).

---

## 🖥️ Test Cases and Results

### Test Case 1: `FindBusinessBasedOnCity`
- Verified correct filtering of businesses based on city.
- Output saved in `output_city`.

### Test Case 2: `FindBusinessBasedOnLocation`
- Verified correct filtering of businesses based on proximity and categories.
- Output saved in `output_loc`.

---

## 📊 Results
- **All test cases passed successfully.**
- Outputs demonstrate the accurate filtering of data based on city and location.
- Optimized functions performed efficiently with minimized complexity.

---

## 🛠️ Technologies Used
- **Programming Language**: Python
- **Database**: UnQLite
- **Libraries**:
  - `math`: For geospatial calculations.
  - `unqlite`: For database operations.

---

## 📦 Output
Screenshots:
Included screenshots of output_city and output_loc files showing successful test results.

---

## 🔮 Future Enhancements
Extend functionality to include more filters (e.g., cuisine type, ratings).
Implement real-time database updates for dynamic restaurant applications.
Explore integration with REST APIs for broader application support.

---

## 💡 Key Takeaways
This project reinforced the importance of NoSQL databases in real-world applications. By implementing these functionalities, I gained valuable insights into handling unstructured data efficiently and optimizing Python code for better performance.
