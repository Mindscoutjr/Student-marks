#include <iostream> 
  
using namespace std;
class student

{
    protected:
    
        int rollnumber;
    public:
    
        void get_number(int);
        void put_number(void);
        
};
void student :: get_number(int a)

{
    rollnumber=a;
    
}
void student :: put_number()

{
    cout<<"RollNumber\n"<<rollnumber<<"\n";
    
}
class test : public student

{
    protected:
    
        int Math;
        
        int Science;
        
        int Reading;
        
        
    public:
    
    
        void get_score(float,float,float);
        
        void put_score(void);
        
};
void test :: get_score(float x,float y, float z)

{
    Math=x;
    
    Science=y;
    
    Reading=z;
    
}
void test :: put_score()

{
    cout<<"Score in Math:\n"<<Math<<"\n";
    
    
    cout<<"Score in Science:\n"<<Science<<"\n";
    
    cout<<"Score in Reading:\n"<<Reading<<"\n";
    
}
class result : public test 

{
    public:
    
        void display(void);
        
};
void result :: display(void)

{
    put_number();
    
    put_score();
    
    
};
int main()

{
   int i;
   result arjun;
   
   arjun.get_number(22);
   
   arjun.get_score(90.8987,87.46,98.3467);
   
   arjun.display();
   
   cout<<"\nEnter the score you got in Math: ";
   
   float mark, sum=0, avg;
   
   for(i=0; i<1; i++)
   
   {
       cin>>mark;
       
       sum = sum+mark;
       
   }
   
   avg = sum/1;
   
   cout<<"\nGrade in math = ";
   
   if(avg>=91 && avg<=100)
   
       cout<<"A+";
       
       
   else if(avg>=81 && avg<91)
   
       cout<<"A";
       
   else if(avg>=71 && avg<81)
   
       cout<<"B+";
       
   else if(avg>=61 && avg<71)
   
       cout<<"B";
       
   else if(avg>=51 && avg<61)
   
       cout<<"C+";
       
   else if(avg>=41 && avg<51)
   
       cout<<"C";
       
   else if(avg>=33 && avg<41)
   
       cout<<"D+";
   else if(avg>=21 && avg<33)
   
       cout<<"D";
       
   else if(avg>=0 && avg<21)
   
   
       cout<<"F";
       
   else
   
       cout<<"Invalid!";
       
   cout<<endl;
   
   cout<<"\nEnter the score you got in Science: ";
   
   float pogchamp, sum1=0, aveg;
   
   for(i=0; i<1; i++)
   
   {
       cin>>pogchamp;
       
       sum1 = sum1+pogchamp;
       
   }
   aveg = sum1/1;
   
   cout<<"\nGrade in Science = ";
   
   if(aveg>=91 && aveg<=100)
   
       cout<<"A+";
       
   else if(aveg>=81 && aveg<91)
   
       cout<<"A";
       
       
   else if(aveg>=71 && aveg<81)
   
   
       cout<<"B+";
       
   else if(aveg>=61 && aveg<71)
   
       cout<<"B";
       
   else if(aveg>=51 && aveg<61)
   
       cout<<"C+";
       
   else if(aveg>=41 && aveg<51)
   
       cout<<"C";
       
   else if(aveg>=33 && aveg<41)
   
       cout<<"D+";
       
   else if(aveg>=21 && aveg<33)
   
       cout<<"D";
       
   else if(aveg>=0 && aveg<21)
   
       cout<<"F";
       
   else
   
       cout<<"Invalid!";
       
   cout<<endl;
   
   
   cout<<"\nEnter the score you got in Reading:\n ";
   
   float marks2, sum2=0, avg2;
   
   for(i=0; i<1; i++)
   
   {
   
       cin>>marks2;
       
       sum2 = sum2+marks2;
       
   }
   avg = sum2/1;
   
   cout<<"\nGrade in Reading = ";
   
   if(avg2>=91 && avg2<=100)
   
       cout<<"A+";
       
   else if(avg2>=81 && avg2<91)
   
       cout<<"A";
       
   else if(avg2>=71 && avg2<81)
   
       cout<<"B+";
       
   else if(avg2>=61 && avg2<71)
   
       cout<<"B";
       
   else if(avg2>=51 && avg2<61)
   
       cout<<"C+";
       
   else if(avg2>=41 && avg2<51)
   
       cout<<"C";
       
   else if(avg2>=33 && avg2<41)
   
       cout<<"D+";
       
   else if(avg2>=21 && avg2<33)
   
       cout<<"D";
       
   else if(avg2>=0 && avg2<21)
   
       cout<<"F";
       
   else
   
       cout<<"\nInvalid!";
       
   cout<<endl;
   
       return 0;
       
}
