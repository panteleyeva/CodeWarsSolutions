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
* Day 8:
1. https://www.codewars.com/kata/random-case/train/javascript
    function randomCase(x) {
    let str = '';
      for (let i = 0; i < x.length; i++) {
        if (Math.round(Math.random()) > 0) {
        str = str + x[i].toUpperCase();
        }
      else {
      str = str + x[i].toLowerCase();
      }
      }
      return str;

    }
2. https://www.codewars.com/kata/sum-mixed-array/train/javascript
    function sumMix(x){
    let sum = 0;
      for (let i = 0; i < x.length; i++) {
         if (typeof x[i] === 'string'){
         x[i] = Number(x[i]);
         }
         sum = sum + x[i];
       }
       return sum;
     }
* Day 9:
1. https://www.codewars.com/kata/remove-string-spaces/train/javascript
    function noSpace(x){
      let str = x.replace(/ /g, '');
       return str;
    }
2. https://www.codewars.com/kata/do-i-get-a-bonus/train/javascript
    function bonusTime(salary, bonus) {
      let str = '';
      if (bonus) {
       return str = '£' + salary * 10;
       } else {
        return str = '£' + salary;
       }
    }
3. https://www.codewars.com/kata/returning-strings/train/javascript
    function greet(name){
       return `Hello, ${name} how are you doing today?`

    }
* Day 10:
1. https://www.codewars.com/kata/string-average/train/javascript
    function averageString(str) {
      if (!str) return 'n/a';
      let d = {
          'zero': 0,
          'one': 1,
          'two': 2,
          'three': 3,
          'four': 4,
          'five': 5,
          'six': 6,
          'seven': 7,
          'eight': 8,
          'nine': 9,
       }
      let n = {
          0: 'zero',
          1: 'one',
          2: 'two',
          3: 'three',
          4: 'four',
          5: 'five',
          6: 'six',
          7: 'seven',
          8: 'eigth',
          9: 'nine'
      }
      const da = str.split(' ');
      let sum = 0;


      for (let i = 0; i < da.length; i++) {
        if (d[da[i]] !== undefined) {
        sum += d[da[i]];
      } else {
        return 'n/a';
      }
    }
    const avg = Math.floor(sum/da.length);
    return n[avg];
    }
2. https://www.codewars.com/kata/58d76854024c72c3e20000de
    function reverse(str){
      return str
      .trim()
      .split(' ')
      .map((el, i) => {
       return i % 2
       ? el.split('').reverse().join('')
       : el;
       })
       .join(' ');
    }
* Day 11:
1. https://www.codewars.com/kata/square-n-sum/train/javascript
    function squareSum(num){
      let sum = 0;
      for (let i = 0; i < num.length; i++) {
        sum = sum + num[i] ** 2;
      }
      return sum;
    }
2. https://www.codewars.com/kata/grasshopper-messi-goals-function/train/javascript
    function goals (laLigaGoals, copaDelReyGoals, championsLeagueGoals) {
      total = laLigaGoals + copaDelReyGoals + championsLeagueGoals
      return total;
    }
* Day 12:
1. https://www.codewars.com/kata/isreallynan/train/javascript
    const isReallyNaN = val => Number.isNaN(val);
2. https://www.codewars.com/kata/convert-a-string-to-a-number/train/javascript
    function stringToNumber(str) {
      return Number (str);
    }
3. https://www.codewars.com/kata/sentence-smash/train/javascript
    function smash (words) {
      return words.join(' ')
    }
4. https://www.codewars.com/kata/reversing-words-in-a-string/train/javascript
    const reverse = s => s.split(' ').reverse().join(' ');
