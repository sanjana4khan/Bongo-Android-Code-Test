# Bongo-Android-Code-Test

1) Write a function that detects if two strings are anagram e.g. ‘bleat’ and ‘table’
are anagrams but ‘eat’ and ‘tar’ are not.

      function Anagram(char[] string1, char[] string2) 
       { 
        // Get lenghts of both strings 
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
  
