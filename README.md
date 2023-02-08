<h1 align="center">Javascript My Own Awesome Cheatsheet 🐱‍👤</h1>

[//]: # (Table of Content)

<a name="top"></a>

## Table of content Javascript My Own Awesome Cheatsheet 🙋‍♂️ 

> Click on any topic to go there

- [Javascript Arrays:)](#js-array)
  
  - [Array.length](#a-length)
  - [Array.push()](#a-push)
  - [Array.unshift()](#a-unshift)
  - [Array.pop()](#a-pop)
  - [Array.shift()](#a-shift)
  - [Array.indexOf()](#a-indexOf)
  - [Array.lastIndexOf()](#a-lastIndexOf)
  - [Array.includes()](#a-includes)
  - [Array.find()](#a-find)
  - [Array.findIndex()](#a-findIndex)
  - [Array.sort()](#a-sort)
  - [Array number sort()](#a-numberSort)
  - [Array.splice()](#a-splice)
  - [Array.from()](#a-from)
  - [Array.forEach()](#a-forEach)
  - [Array.filter()](#a-filter)
  - [Array.map()](#a-map)
  - [Array.reduce()](#a-reduce)



***

---

### Arrays Definiation :)

<a name="js-array"></a>
> Arrays are used to store multiple values in a single variable.This is compared to a variable that can store only one value.Each item in an array has a number attached to it, called a numeric index, that allows you to access it.In JavaScript, arrays start at index zero and can be manipulated with various methods.

```js
const Language = ['javascript', 'python', 'php', 'C#', 'java']

console.log(Language);// ['javascript', 'python', 'php', 'C#', 'java']
```

#### What is array index?

>  JavaScript arrays are zero - indexed: the first element of an array is at index 0, the second is at index 1, and so on — and the last element is at the value of the array's length property minus 1

```js
const Language = ['javascript', 'python', 'php', 'C#', 'java']
console.log(Language[1]);//'python'
```

 - [w3 schools Javascript Array References:)](https://www.w3schools.com/jsref/jsref_obj_array.asp)
 - [Developer Mozilla Javascript Array References:)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
 - [Best Bangla Language Javascript Array Learning](https://with.zonayed.me/post/js-array)

#### [Go to top:arrow_up: ](#top)



<a name="a-length"></a>

### Javascript Array.length:)

> Basically, the length of an array is the total number of the elements which is contained by all the dimensions of that array.Property Value: This property returns the total number of elements in all the dimensions of the Array.It can also return zero if there are no elements in the array.

```js
const language=['Html','Css','Js','Php','Python'];
console.log('My Array Total Length Is:',language.length);//5
```


#### [Go to top:arrow_up: ](#top)

<a name="a-push"></a>

### Javascript Array.push()

>Definition and Usage
The push() method adds new items to the end of an array.
The push() method changes the length of the array.
The push() method returns the new length.


```js
const language=['Html','Css','Js','Php','Python'];

language.push('Go')//This value add array last index
console.log(language);//[ 'javascript', 'python', 'php', 'C#', 'java', 'Go' ]
```

#### [Go to top:arrow_up: ](#top)

<a name="a-unshift"></a>

### Javascript Array.unshift()

>The unshift() method adds new elements to the beginning of an array.
The unshift() method overwrites the original array.


```js
const language=['Html','Css','Js','Php','Python'];

language.unshift('c++')//This value add array first index
console.log(language);//['c++', 'Html', 'Css', 'Js', 'Php', 'Python']
```


#### [Go to top:arrow_up: ](#top)

<a name="a-pop"></a>

### Javascript Array.pop()

>The pop() method removes(pops) the last element of an array.
The pop() method changes the original array.
The pop() method returns the removed element.

```js
const language=['Html','Css','Js','Php','Python'];

console.log(language.pop());//['Python']

console.log(language);//['Html', 'Css', 'Js', 'Php'] chack it carefully pop() method delete array last index['Python']
```

#### [Go to top:arrow_up: ](#top)

<a name="a-shift"></a>

### Javascript Array.shift()


> The shift() method removes the first item of an array.
The shift() method changes the original array.
The shift() method returns the shifted element.

```js
const language=['Html','Css','Js','Php','Python'];

console.log(language.shift());//['Html']

console.log(language);//[ 'Css', 'Js', 'Php', 'Python' ] chack it carefully shift() method delete array first index ['Html']
```


#### [Go to top:arrow_up: ](#top)

<a name="a-indexOf"></a>

### Javascript Array.indexOf()

> The indexOf() method returns the first index(position) of a specified value.
The indexOf() method returns - 1 if the value is not found.
The indexOf() method starts at a specified index and searches from left to right.
By default the search starts at the first element and ends at the last.
Negative start values counts from the last element(but still searches from left to right).

```js
const admins = [2, 4, 5, 7, 9]
const users = {name:'karim', id:7}
const user1 = { name: 'kamal', id: 12 }
console.log(admins.indexOf(users.id));//4
console.log(admins.indexOf(user1.id));//-1
const isAdmins = admins.indexOf(user1.id) > -1;
console.log(isAdmins);

const fruits = ["Banana", "Orange", "Apple", "Mango", "Apple"];
let index = fruits.indexOf("Apple", 3);//return index 4
console.log(index);
```


#### [Go to top:arrow_up: ](#top)

<a name="a-lastIndexOf"></a>

### Javascript Array.lastIndexOf()

> The lastIndexOf() method returns the last index(position) of a specified value.
The lastIndexOf() method returns - 1 if the value is not found.
The lastIndexOf() starts at a specified index and searches from right to left.
By defalt the search starts at the last element and ends at the first.
Negative start values counts from the last element(but still searches from right to left).

```js
  const fruits = ["Orange", "Apple", "Mango", "Apple", "Banana", "Apple"];
  let index = fruits.lastIndexOf("Apple",2);
  console.log(index);
  const fruites = ["Orange", "Apple", "Mango", "Apple", "Banana", "Apple"];
  let indexes = fruits.lastIndexOf("Apple", -2);//still searches from right to left
  console.log(indexes);
```  


#### [Go to top:arrow_up: ](#top)

<a name="a-includes"></a>

### Javascript Array.includes()

> The includes() method returns true if an array contains a specified value.
The includes() method returns false if the value is not found.
The includes() method is case sensitive.

```js
const admins = [2, 4, 5, 7, 9]
const users = {name:'karim', id:7}
const user1 = { name: 'kamal', id: 12 }
console.log(admins.includes(users.id));//true
console.log(admins.includes(user1.id));//false


const langs = ['Html', 'Css', 'Js', 'Php', 'Python','Css','Php','Python','Js','Html'];
const newLang = langs.includes('Html')//true
console.log(newLang);

// Simple Advanced Examples 

function findUnique(ary) {
  const unique=[]
  for (let i = 0; i < ary.length; i++){
    const name = ary[i]
    if (unique.indexOf(name) === -1) {
      unique.push(name)
    }
  }
  return unique// only return unique value [ 'Html', 'Css', 'Js', 'Php', 'Python' ]
}
const uniqueAry=findUnique(langs)
console.log(uniqueAry);
```


#### [Go to top:arrow_up: ](#top)

<a name="a-find"></a>

### Javascript Array.find()

> The find() method returns the value of the first element that passes a test.
The find() method executes a function for each array element.
The find() method returns undefined if no elements are found.
The find() method does not execute the function for empty elements.
The find() method does not change the original array.


```js
const ages = [3, 10, 18, 20];

function checkAge(age) {
  return age > 5;//10
}

// Simple And Different Example:)

console.log(ages.find(checkAge));
const allUsers = [
  { name: 'abc', id: 5 },
  { name: 'xyz', id: 10 },
  { name: 'kbc', id: 9 },
  { name: 'bcd', id: 7 },
  { name: 'axd', id: 4 }
]
const myUser = allUsers.find((user) =>user.name==='kbc')//Note that the find method will return undefinded if no value is found!
console.log(myUser);
```


#### [Go to top:arrow_up: ](#top)

<a name="a-findIndex"></a>

### Javascript Array.findIndex()

> The findIndex() method executes a function for each array element.
The findIndex() method returns the index(position) of the first element that passes a test.
The findIndex() method returns - 1 if no match is found.
The findIndex() method does not execute the function for empty array elements.
The findIndex() method does not change the original array.


```js
const ages = [3, 10, 18, 20];

let newAge=ages.findIndex(checkAge);

function checkAge(age) {
  return age > 18;//20
}
console.log('NewAge Index No Is:'+newAge);
```


#### [Go to top:arrow_up: ](#top)

<a name="a-sort"></a>

### Javascript Array.sort()

> The sort() sorts the elements of an array.
The sort() overwrites the original array.
The sort() sorts the elements as strings in alphabetical and ascending order.

```js
const language=['Html','Css','Js','Php','Python'];
console.log(language);
console.log(language.sort());//[ 'Css', 'Html', 'Js', 'Php', 'Python' ]
```


<a name="a-numberSort"></a>

### Javascript Array Number Sort:)


```js
  const number=[4,7,10,6,9];
  number.sort((min, max) => min - max)//[4,6,7,9,10]
  console.log(number);
  number.sort((min, max) => max - min)//[ 10, 9, 7, 6, 4 ]
  console.log(number);
```



#### [Go to top:arrow_up: ](#top)

<a name="a-splice"></a>

### Javascript Array.splice()

> The splice() method adds and / or removes array elements.
The splice() method overwrites the original array.

```js
  const lang = ['Html', 'Css', 'Js', 'Php', 'Python'];
  console.log(language);
  lang.splice(3,1,'go','c++')
  console.log(lang);//delete['php'] and add['go']['c++']
```


#### Simple Task 😀

```
/**
 * add a Dec of the end of a array
 * what is the return value of splice method
 * update march March (update)
 * delete the June from an array?
 */
 ```

<details>
  <summary>First You Are Try It Solve This Problem :)</summary>
  
  <p> <b><i>The Problem Is Very Easy. This Problem Solve It Very EassyLy Use Array splice() Method</i></b></p>
  
  ```js
  const months = ['Jan', 'march', 'April', 'June', 'July']
console.log('Before: '+months);
ans:1
const newMonth=months.splice(months.length,0,'Dec')
console.log('After: '+months);
ans:2
console.log(newMonth);//return [] empty array or delete elemnt
ans:3
const updateMonths = months.splice(1, 1, 'March')
console.log('Update: '+months);
console.log('Update Months: ' + updateMonths);


//Best Pactises any month updates

// const indexMonth = months.indexOf('July')
// const monthUpdate = indexMonth != -1 ? months.splice(indexMonth,1, 'Aug') : 'Search Data Not Found!';//delete july add new month
// const monthUpdate = indexMonth != -1 ? months.splice(indexMonth+1,0, 'Aug') : 'Search Data Not Found!';//not delete july and new month add after indexMonth
// console.log('Month Update: '+months);
// console.log(monthUpdate);



//ans:4
const deleteMonth = months.splice(3, 1)
console.log(months);
console.log('Delete Months: '+deleteMonth);
```

</details>















