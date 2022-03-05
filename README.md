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
