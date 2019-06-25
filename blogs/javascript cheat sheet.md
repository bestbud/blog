```plain
// 去重
const arr = [1,2,2,3,3,4,5,5];
const uniq = [...new Set(arr)]; // [1,2,3,4,5]

//Maximus 1
var arr = [6, 89, 3, 45];
var maximus = Math.max.apply(null, arr); // 89

//Maximus 2
const arr = [6, 89, 3, 45];
const maximus = Math.max(...arr); // 89 

// ES6 Destructuring Arrays to Assign Variables
const [a, b, ...arr] = [1, 2, 3, 4, 5, 7];
console.log(a, b); // 1, 2
console.log(arr); // [3, 4, 5, 7]


// hasOwnProperty
var myObj = {
  top: "hat",
  bottom: "pants"
};

myObj.hasOwnProperty("top"); // true
myObj.hasOwnProperty("middle"); // false



// ES6 Destructuring Variables from Objects
const { x, y, z } = voxel; // x = 3.6, y = 7.4, z = 6.54
// to store the values of voxel.x into a, voxel.y into b, and voxel.z into c, you have that freedom as well
const { x: a, y: b, z: c } = voxel; // a = 3.6, b = 7.4, c = 6.54
// Destructuring Variables from Nested Objects
const a = {
  start: { x: 5, y: 6 },
  end: { x: 6, y: -9 }
};

const {
  start: { x: startX, y: startY }
} = a;

console.log(startX, startY); // 5, 6

```
