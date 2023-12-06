# All Interview Questions I have Faced

### 1. Tell me about yourself/ give some introduction about you.
### 2. What is optional in swift?
  A type that represents either a wrapped value or the absence of a value.
  ```swift
   // Optionals are declared using the "?" or "!" (aka force unwrap) symbol at the end of the Types
   var message: String?
  ```
 ```swift
   // Example
   var message: String
   print(message) // shows error

   var message: String?
   print(message) // shows nil
  ```

### 2. There is a popular method for swaping two values in swift, can you demonstrate that?
   Ohh, yes. By using **Tuple** data type we can swap values easily. **Tuple** is a native data type for Swift.
   For example, if we have two values like 
   ```swift
   // A tuple type is a comma-separated list of types, enclosed in parentheses.
   var a = 5
   var b = 7
   (a, b) = (b, a) // a = 7, b = 5
  ```
   There are some other techniques
   ```swift
   //MARK: technique 1
   var a = 5
   var b = 7
   a = a + b // 12
   b = a - b // 5
   a = a - b // 7

   //MARK: technique 2
   var a = 5
   var b = 7
   var temp = a
   a = b // 7
   b = temp // 5
  ```
### 3. What are the application lifecycle in ios?
   <img width="415" alt="scene-state@2x" src="https://github.com/asadullahpranto/All-Interview-Questions-I-have-Faced/assets/22514450/768570ea-5ef3-4112-9dd7-327f1a9191af">

### 4. What are the UIViewController's lifecycle in ios?
   - loadView()
   - loadViewIfNeeded()
   - viewDidLoad()
   - viewWillAppear(_ animated: Bool)
   - viewWillLayoutSubviews()
   - viewDidLayoutSubviews()
   - viewDidAppear(_ animated: Bool)
   - viewWillDisappear(_ animated: Bool)
   - viewDidDisappear(_ animated: Bool)
     
   ![1_hX8Jd4HG3Hw0N1oWtSHnlQ](https://github.com/asadullahpranto/All-Interview-Questions-I-have-Faced/assets/22514450/10cf841e-1ff7-4ae3-bf55-bb936cd9bd2b)

### 5. Which delegate medhod sets the item size in a UICollectionView?
   ```swift
      UICollectionViewDelegateFlowLayout.
      It inherits from UICollectionViewDelegate
   ```
### 6. Which will be execute first?
   ```swift
      DispatchQueue.main.async {
         print("inside")
      }

      print("outside")

      // MARK: Answer
      // outside -> inside
   ```
