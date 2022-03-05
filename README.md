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
## Is given value an array or not ?

  ```javascript
  let Arr = [1,2,3,4,5];
  console.log(typeof Arr)
  // console.log(Object.prototype.toString.call(Arr));
  console.log(toString.call(Arr));

  if(toString.call(Arr) === "[object Array]"){
      console.log("true");
   }else{
       console.log("false");
  }
 ```
 ## Remove null,undefined,0,Nan,"" from Array ? 

  ```javascript
  let Arr1 = [false,0,NaN,6,undefined,50,'','Hi'];

  let Arr2 =  Arr1.filter((v,i) => {
   // console.log(v+'---------'+i);
   if(v){
     return v;
   }
  })

 console.log(Arr2)
 ```
 ## Remove duplicate values from Array ? 

  ```javascript
  // first method
  
   let arr3 = [1,2,3,4,4,5,5,6,3]
   let newarr = arr3.filter((v,i)=>{
   // console.log(v+"-------"+arr3.indexOf(v)+"-------"+i)
               return arr3.indexOf(v) == i
        // return arr3.indexOf(v) != i
     })
  console.log(newarr)

 // second method
                
      let arr4 = ["Admin","user","Coder","Admin","Hacker"]
      let arr5 = [...new Set(arr4)]   
      console.log(arr5) 
 ```
## Prime Number

  ```javascript
                // 3/3,3/1 = prime no.
                // 5/5,5/1 = prime no.
                // 4/4,4/2,4/1 = not prime

                var checkprime = 5;
                isPrime = true;
                for(cnt=2;cnt<checkprime;cnt++){
                	if(checkprime%cnt==0){
                		isPrime=false;
                		break;
                	}
                }
                if(isPrime==true){
                	console.log("Prime No.")
                }else{
                	console.log("Not Prime No.")
                }

  ```
  ## Finding Factorial

  ```javascript
 n =5 
 fact =1;

 for (;n>=1;n--) {
 	fact = fact * n;
 }
 console.log(fact);
 ```
