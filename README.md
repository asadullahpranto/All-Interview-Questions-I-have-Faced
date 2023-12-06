# All Interview Questions I have Faced

### 1. Tell me about yourself/ give some introduction about you.
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
### 3. What are the UIViewController's lifecycle in ios?
### 4. Which delegate medhod sets the item size in a UICollectionView?
   ```swift
      UICollectionViewDelegateFlowLayout.
      It inherits from UICollectionViewDelegate
   ```
### 5. Which will be execute first?
   ```swift
      DispatchQueue.main.async {
         print("inside")
      }

      print("outside")

      // MARK: Answer
      // outside -> inside
   ```
