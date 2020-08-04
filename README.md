# Bongo-Android-Code-Test

1) Write a function that detects if two strings are anagram e.g. ‘bleat’ and ‘table’
are anagrams but ‘eat’ and ‘tar’ are not.





     
        function Anagram(char[] string1, char[] string2) { 
      
        int lenghtOfString1 = string1.length; 
        int lenghtOfString2 = string2.length;
        
        if (lenghtOfString1!= lenghtOfString2) 
        {
         return false; 
        } 
        Arrays.sort(string1); 
        Arrays.sort(string2); 
        
  
        for (int i = 0; i < lenghtOfString1; i++) 
        {
            if (string1[i] != string2[i]) 
                return false; 
        }
         
        return true; 
        
    } 
    
    
2) Explain the design pattern used in following:
interface Vehicle {
int set_num_of_wheels()
int set_num_of_passengers()
boolean has_gas()
}
a) Explain how you can use the pattern to create car and plane class?
b) Use a different design pattern for this solution.
  
