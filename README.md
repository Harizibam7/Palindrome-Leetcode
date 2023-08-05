# Palindrome-Leetcode


Palindrome By using C++

    class Solution {
    public:
        bool isPalindrome(int x) {
           int temp =x;
           if(x<0){
               return false;
           }
           long long rem;
           long long result=0;
           while(temp!=0){
               rem = temp%10;
               result = (result*10)+rem;
               temp/=10;
           }
           return (x==result);
        }
    };
Palindrome By using C

    bool isPalindrome(int x){
        if(x<0){
            return false;
    
        }
        int temp =x;
        long long rem;
        long long result =0;
        while(temp!=0){
            rem = temp %10;
            result = (result*10)+rem;
            temp/=10;
        }
        return (x==result);
    }
