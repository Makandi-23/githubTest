# githubTest
my first test
#include <stdio.h>
#include <time.h>

int main()
{
   int hour = 0;
   int minute = 0;
   int second = 0;
   while(1)
   {
   
     if(second == 60)
     {
           minute += 1;
           second = 0;
       }
    
       if(minute == 60)
       {
           hour += 1;
           minute = 0;
       }
    
       if(hour == 24) {
           hour = 0;
           minute = 0;
           second = 0;
       }

       sleep(1);  
   }
   return 0;
}
