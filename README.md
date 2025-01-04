# goit-js-hw-04

Task 1. Packing products
Perform this task in the file task-1.js
Write a function isEnoughCapacity(products, containerSize), which calculates whether all products will fit in the container when packing.

The function declares two parameters:

products — an object in which the keys contain the names of the products, and their values ​​— the number of these products. For example, { apples: 2, grapes: 4 }.
containerSize — a number, the maximum number of units of products that the container can hold.
The function should return the result of checking whether all products will fit in the container. That is, count the total number of products in the products object and return true if it is less than or equal to containerSize, and false if not.

Take the code below and insert it after the declaration of your function to check that it works correctly. The results of its calls will be displayed in the console.

console.log(
isEnoughCapacity({ apples: 2, grapes: 3, carrots: 1 }, 8)
); // true

console.log(
isEnoughCapacity({ apples: 4, grapes: 6, lime: 16 }, 12)
); // false

console.log(
isEnoughCapacity({ apples: 1, lime: 5, tomatoes: 3 }, 14)
); // true

console.log(
isEnoughCapacity({ apples: 18, potatoes: 5, oranges: 2 }, 7)
); // false

Leave this code for review by a mentor.

What the mentor will pay attention to when checking:
The declared function isEnoughCapacity(products, containerSize)
The call isEnoughCapacity({ apples: 2, grapes: 3, carrots: 1 }, 8) returns true
The call isEnoughCapacity({ apples: 4, grapes: 6, lime: 16 }, 12) returns false
The call isEnoughCapacity({ apples: 1, lime: 5, tomatoes: 3 }, 14) returns true
The call isEnoughCapacity({ apples: 18, potatoes: 5, oranges: 2 }, 7) returns false


Task 2. Calculating calories
Perform this task in the file task-2.js
Write the function calcAverageCalories(days), which returns the average daily value of the number of calories that the athlete consumed during the week. The function expects one parameter: days — an array of objects. Each object describes the day of the week and the number of calories consumed by the athlete on that day. Take the code below and insert it after the declaration of your function to check that it works correctly. The results of its calls will be displayed in the console.

console.log(
calcAverageCalories([
{ day: "monday", calories: 3010 },
{ day: "tuesday", calories: 3200 },
{ day: "wednesday", calories: 3120 },
{ day: "thursday", calories: 2900 },
{ day: "friday", calories: 3450 },
{ day: "saturday", calories: 3280 },
{ day: "sunday", calories: 3300 }
])
); // 3180

console.log(
 calcAverageCalories([
 { day: "monday", calories: 2040 },
 { day: "tuesday", calories: 2270 },
 { day: "wednesday", calories: 2420 },
 { day: "thursday", calories: 1900 },
 { day: "friday", calories: 2370 },
 { day: "saturday", calories: 2280 },
 { day: "sunday", calories: 2610 }
 ])
); // 2270

console.log(
 calcAverageCalories([])
); // 0

Leave this code for a mentor to review.

What the mentor will pay attention to when checking:
The function calcAverageCalories(days) is declared
Such a call to the function calcAverageCalories returns 3180
calcAverageCalories([
{ day: "monday", calories: 3010 },
{ day: "tuesday", calories: 3200 },
{ day: "wednesday", calories: 3120 },
{ day: "thursday", calories: 2900 },
{ day: "friday", calories: 3450 },
{ day: "saturday", calories: 3280 },
{ day: "sunday", calories: 3300 }
])

Such a call to the function calcAverageCalories returns 2270
calcAverageCalories([
{ day: "monday", calories: 2040 },
{ day: "tuesday", calories: 2270 },
{ day: "wednesday", calories: 2420 },
{ day: "thursday", calories: 1900 },
{ day: "friday", calories: 2370 },
{ day: "saturday", calories: 2280 },
{ day: "sunday", calories: 2610 }
])

This call to the calcAverageCalories function returns 0
calcAverageCalories([])

Task 3. Player Profile
Perform this task in the task-3.js file
The profile object describes the user profile on the gaming platform. Its properties store the profile name username and the number of active hours of playTime spent in the game.

const profile = {
username: "Jacob",
playTime: 300,
};

Add methods to the profile object to work with its properties.

The changeUsername(newName) method should accept a string (new name) in the newName parameter and change the value of the username property to the new one. It returns nothing.
The updatePlayTime(hours) method should accept a number (number of hours) in the hours parameter and increase the value of the playTime property by it. It returns nothing.
The getInfo() method should return a string of the format <Username> has <amount> active hours!, where <Username> is the profile name, and <amount> is the number of game hours.
Take the code below and insert it after the declaration of your function to check that it works correctly. The results of its work will be displayed in the console.

console.log(profile.getInfo()); // "Jacob has 300 active hours!"

profile.changeUsername("Marco");
console.log(profile.getInfo()); // "Marco has 300 active hours!"

profile.updatePlayTime(20);
console.log(profile.getInfo()); // "Marco has 320 active hours!"

Leave this code for the mentor to check.

What the mentor will pay attention to when checking:
The profile variable is declared
The value of the profile variable is an object with the properties username, playTime, getInfo, changeUsername and updatePlayTime
The value of the getInfo property is a function
The value of the changeUsername property is a function
The value of the updatePlayTime property is a function
To access the properties of an object in its methods, this is used
