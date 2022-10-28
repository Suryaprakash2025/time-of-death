# time-of-death
this is a simple project used to know the time of death of a person for investigation. the idea behind the concept is newtons law of cooling.





#include <iostream>
#include <math.h>

using namespace std;

int main()
{
    float t1,t2,r,ti;
    cout<<"DETECTOR \n";
    cout<<"enter the body temperature:\n";
    cin>>t1;
    
    cout<<"enter the body temperature after 1 hour:\n";
    cin>>t2;
   
    cout<<"enter the surrounding/room temperature:\n";
    cin>>r;
    float c=t1-r;
    float d=t2-r;
    float k=-log(d/c);
    float g=37-r;
    float t=log(g/c)/k;
    cout<<"the death happened before around:"<<t<<"hours from initial time of temperature known";
   

    return 0;
}
