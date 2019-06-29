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
      return 0;
      } else {
      return x.shift() + sumR(x);
      }
    }
