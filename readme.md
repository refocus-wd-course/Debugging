<h1 style="text-align: center;">Debugging 💻🖥️</h1>

# Introduction

<p> Hello students 👋 In this repository we will check if your assignment passed the requirement. </p>

## Requirements:

<p>The code below has some bugs and we need to fix it:</p>

```javascript
const flowers = ["rose , star gazer , tulips , sun flower"];

// count the length of the strings inside the Array
for (i = 0; i <= flowers.length; i++) {
  console.log(flowers[0].lentgh);
}
```

Expected output should be like this:

```txt
4
10
6
10
```

## Steps:

### 1. First we need to create a new JS file and copy paste the code that has some bugs.

### 2. If we run this code you will notice that the output is wrong even if there are no error in your VSCode. This is because we are encountering a logical error problem. Let's disect this one line at a time.

### 3. Let's start by the array construction of the variable named "flowers". The array has only one element for now because every flower inside are enclosed on a double quote. To fix this, let's separate every flower as one string.

```javascript
const flowers = ["rose", "star gazer", "tulips", "sun flower"];
```

### 4. The next problem we have is the logic inside our `for` loop, we need to carefully debug this because loops tend to cause inifinite loop and will cause your device to freeze.

- The condition of our loop is currenlty checking if our `i` is less than or equal `<=` to the array lentgh. But when you check the result of an array lentgh it will actually count the elements inside starting to 1. This will cause a problem because we count our loop starting on 0 because we are counting as index. So to solve this we will change the less than or equal `<=` to less than only `<`.

```javascript
...
for (i = 0; i < flowers.length; i++) {
  //Code here
}
...
```

### 5. Now that our `for` loop logic is correct, let's check the code inside of it. You will notice that the `console.log()` function only checks the index 0 on our array. So we need to change this into our `i` since it's the variable that will be updated when the loop runs. Then the length spelling is also wrong, so let's fix that also.

```javascript
...
console.log(flowers[i].length);
...
```

---

# The End

<p> Don't worry if some of your approach is not the same on this repository, it doesn't mean that it is wrong. This is just a guide for you on how to make it. </p>
Happy Coding! 🧑‍💻👩‍💻
