# Find-N-Unique-Integers-Sum-up-to-Zero
Leetcode Challenge - Javascript


Find N Unique Integers Sum up to Zero

// Input: n = 5
// Output: [-1,0,1]

// 0, 2, -2, 1, -1

// if n is even, then output positive and negative versions of the integer?
// if n is odd, then same thing but also add in 0

//         n/2 = 6/2 = 3
//             iterate over 3 digits, positive and negative until 0
//             so that output becomes -3, 3, 2, -2, 1, -1

var sumZero = function(n) {
    result = []
    if (n % 2 == 0) {
        let integer = n/2
        for (i = 1; i <= integer; i++) {
            result.push(-i, i)
        }
     } else {
        let integer = (n-1)/2
        for (i = 1; i <= integer; i++) {
            result.push(-i, i)
        }
        result.push(0)
    }
        return result
}
    
    
    
   
       
       

    
