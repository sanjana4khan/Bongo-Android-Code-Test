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

a)      
           
    interface Vehicle {
       int set_num_of_wheels();
       int set_num_of_passengers();
       boolean has_gas();
       }

    class Plan implements Vehicle {


    public int set_num_of_wheels() {
      return 5;
     }
  


    public int set_num_of_passengers() {
      return 200;
    }

    @Override
    public boolean has_gas() {
       return true;
    }
    }

    class Car implements Vehicle {
    public int set_num_of_wheels() {
        return 4;
    }
  

   
    public int set_num_of_passengers() {
      return 4;
    }

  
    public boolean has_gas() {
       return true;
    }
    }

    class NewClass {
     public static void main(String[] args) {
       Plan plan = new Plan();
       plan.set_num_of_wheels();
       plan.set_num_of_passengers();
       plan.has_gas();
    
       Car car = new Car();
       car.set_num_of_wheels();
       car.set_num_of_passengers();
       car.has_gas();
     }
    }
    
b)

     class NewClass {
    
     static void Vehicle(String vehicleName, int numOfWheels, int numOfPassengers, boolean hasGas)
     {
      System.out.println(""+vehicleName);
      System.out.println("Wheels:" + numOfWheels);
      System.out.println("Passengers:" + numOfPassengers);
      System.out.println("Gas:" +  hasGas);
      
     }
    
     public static void main(String[] args) {
      Vehicle("Car",4,4,true);
      Vehicle("Plan",5,200,true);
      }
     }
     
     
3) Write a video player application with ‘Play’, ‘Forward’, ‘Rewind’ functionalities. Please
write pseudocode for this program and explain the design pattern you will use to
develop these three functionalities.

         function Play(View view){
           if video is playing which will be checked by the isPlaying() method of VideoView class
              then resume the video using resume() method of VideoView class
            
           else 
              start the video using start() method of VideoView Class
           }
      
        function Rewind(View view){
          stop the video using stopPlayBack() method of VideoView Class
          set the path of the video using setVideoPath() method of VideoView Class
          start the video using start() method of VideoView Class          
         }
       
        function Forward(View view){
         get the current position by using getCurrentPostion() method of VideoView Class          
         use seekTo() method of VideoView Class by adding required milisecond to current position to forward the video.
        }
    
 I have implemented a Video Player App for design Pattern. Code has been uploaded here.   
    
          
      
  
