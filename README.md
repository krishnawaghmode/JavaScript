# JS Interview

## Vowel & Consonant -Algorithm

  ```javascript
  // Vowel = a,e,i,o,u
// total = 26-5 = 21
function CheckLetter(Letter){
	Letter = Letter.toLowerCase();
	if(Letter == 'a' || Letter == 'e' || Letter == 'i' || Letter == 'o' || Letter == 'u' ){
		console.log('Vowel');
	}else{
		console.log('Consonant');
	}
}
	
console.log( CheckLetter('a') );

  ```
  
  ## Array Intersection & Union - ES6

  ```javascript
  // Intersection
let oneArr = [1,2,3,4,5,6];
let twoArr = [2,4,6,8];

let threeArr = oneArr.filter((v) =>{
	return twoArr.includes(v);
})

console.log('Intersection');
console.log(threeArr);

// Union

let fourthArr = [...oneArr,...twoArr];
console.log('Union');
console.log(fourthArr);

//Unique_Union
let Unique_Union = [...new Set(fourthArr)];
console.log(Unique_Union);

  ```
## Reverse Number

  ```javascript
  var Num = 12345;
  var reverse = 0;
   while(Num > 0){
         var reminder = Num % 10;
         reverse = (reverse * 10) + reminder; 
         Num = parseInt(Num/10);
    }

 console.log('Reverse of Number:'+ reverse);
 ```
