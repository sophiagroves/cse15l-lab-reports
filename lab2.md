# lab report two

## Part 1: Server
![Image](a.png)
![Image](c.png)
1. The `handleRequest` method is called. 
2. The relevant argument to the `handleRequest method` is the instance of the `URI` class, which is the URL requested by me: [http://localhost:4000/add-message?s=Hello](http://localhost:4000/add-message?s=Hello). The relevant field for the `Handler` class is the `allparameters` field, which is a `List<String>`. The value of the `allparameters` field is a list with one string element, `"Hello"`.
3. Yes, the value of the `allparameters` field changed from an empty list to a list with the string element `"Hello"`.

![Image](b.png)
1. The `handleRequest` method is called. 
2. The relevant argument to the `handleRequest method` is the instance of the `URI` class, which is the URL requested by me: [http://localhost:4000/add-message?s=How%20are%20you](http://localhost:4000/add-message?s=Hello). The relevant field for the `Handler` class is the `allparameters` field, which is a `List<String>`. The value of the `allparameters` field is a list with two string elements, `"Hello", "How Are You."`.
3. Yes, the value of the `allparameters` field changed from a list with one string element `"Hello"` to a list with two string elements `"Hello", "How Are You."`.

## Part 2: Bugs
**Failure inducing input for bug code:**
```
  public void testReverseInPlacenotworks() {
    int[] input2 = {1,2,3};
    ArrayExamples.reverseInPlace(input2);
    assertArrayEquals(new int[]{3,2,1}, input2);
  }
  
```
**Non failure inducing input for bug code:**
```
	public void testReverseInPlaceworks() {
    int[] input1 = {2,2,2};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{2,2,2}, input1);
  }
  
```
**The symptom as output of running the tests:**
![Image](three.png)

**The code before debugging:**
```
  static void reverseInPlace(int[] arr) {
      for(int i = 0; i < arr.length; i += 1) {
        arr[i] = arr[arr.length - i - 1];
      }
  }
```
**The code after debugging:**
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < (arr.length / 2); i += 1) {
      int temp = arr[i];
      arr[i] = arr[arr.length - i - 1];
      arr[arr.length - i - 1] = temp;
    }
}
## Part 3: What I Learned 
During lab in week 2, I learned how to host a local server. During lab in week 3, I learned that I can run junit tests in the terminal. 
