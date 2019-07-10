hello

________________________________


* first

* Day 1:
 1. https://www.codewars.com/kata/opposite-number/train/javascript
    function opposite(number) {
      return - number;
    }
* Day 2:
1. https://www.codewars.com/kata/switch-it-up/train/javascript
    function switchItUp(number){
      let arr = ['Zero', 'One', 'Two', 'Three', 'Four', 'Five', 'Six', 'Seven', 'Eight', 'Nine', 'Ten'];
      return arr[number];
    }
2. https://www.codewars.com/kata/5b077ebdaf15be5c7f000077
    function countSheep (num){
      let newString = '';
        for (let i = 1; i <= num; i++){
          newString = newString + i + ' sheep...';
        }
     return newString;
    }
3. https://www.codewars.com/kata/reverse-a-number/train/javascript
    function reverseNumber(n) {
      if (n >= 0){
      let arr = n.toString().split('').reverse();
       return +(arr.join(''))
      } else {
      n = n * ( - 1);
      let arr = n.toString().split('').reverse();
        return (-1) * (+(arr.join('')))
      }
    }
* Day 3:
1. https://www.codewars.com/kata/students-final-grade/train/javascript
    function finalGrade (exam, projects) {
      if (exam > 90 || projects > 10) return 100;
      if (exam > 75 && projects >= 5) return 90;
      if (exam > 50 && projects >= 2) return 75;
      return 0
    }
2. https://www.codewars.com/kata/get-list-sum-recursively/train/javascript
    function sumR(x) {
      if (x.length  === 0) {
      } else {
      return x.shift() + sumR(x);
      }
    }
* Day 4:
1. https://www.codewars.com/kata/array-plus-array/train/javascript
    function arrayPlusArray(arr1, arr2) {
      let sum1 = 0;
      let sum2 = 0;
        for (let i = 0; i < arr1.length; i++) {
        sum1 = sum1 + arr1[i]
        }
        for (let i = 0; i < arr2.length; i++) {
        sum2 = sum2 + arr2[i];
        }k
      return sum1 + sum2;
    }
2. https://www.codewars.com/kata/count-odd-numbers-below-n/train/javascript
     function oddCount(n){
       return Math.floor (n / 2);
     }
3. https://www.codewars.com/kata/multiples-of-3-or-5/train/javascript
    function solution(number){
      let sum = 0;
       for (let i = 3; i < number; i++){
       if (i % 3 === 0 || i % 5 === 0)
       sum = sum + i;
       }
       return sum;
    }
* Day 5:
1. https://www.codewars.com/kata/spongebob-meme/train/javascript
    function spongeMeme(sentence) {
      let str = '';
      for (let i = 0; i < sentence.length; i++) {
        if (i % 2 == 0) {
        str = str + sentence[i].toUpperCase()
        } else {
        str = str + sentence[i].toLowerCase()
        }
      }
    return str;

    }
* Day 6:
1. https://www.codewars.com/kata/valid-parentheses/train/javascript
    function validParentheses(parens){
      const arr = parens.split('');
      let a = 0;
      for (let i = 0; i < arr.length; i++) {
        if (parens[i] === '(') a = a + 1;
        else if (parens[i] === ')') a = a - 1;
        if (a < 0) return false;
      }
        if (a === 0) return true;
        else return false;
    }
2. https://www.codewars.com/kata/arrays-similar/train/javascript
    function arraysSimilar(arr1, arr2) {
      if (arr1.length !== arr2.length) return false;
      arr1.sort();
      arr2.sort();
      for (let i = 0; i < arr1.length; i++) {
        if (arr1[i] !== arr2[i]) return false;
      }
      return true
    }
3. https://www.codewars.com/kata/write-shortest-function-to-calculate-average-number-of-array/train/javascript
    const avg = a => a.reduce((a, b) => a + b) / a.length

* Day 7:
1. https://www.codewars.com/kata/who-is-going-to-pay-for-the-wall/train/javascript
    function whoIsPaying(name){
    let arr = [name];
      if(name.length > 2) {
      let str = name.substring (0, 2);
      arr.push (str);
      }
    return arr;
    }
2. https://www.codewars.com/kata/maximum-triplet-sum-array-series-number-7/train/javascript
    function maxTriSum(num){
    let sum = 0;
    let res = num.sort((a, b) => b - a);
    let arr = [];
      for (let i = 0; i < res.length; i++){
        if (arr.length >= 3){
          break
        }
        if (!arr.includes(res[i])){
          arr.push(res[i]);
          sum += res[i];
        }
      }
     return sum;
    }
3. https://www.codewars.com/kata/remove-duplicates-from-list/train/javascript
    function distinct(a) {
      return [... new Set(a)];
    }