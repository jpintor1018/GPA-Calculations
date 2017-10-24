# GPA-Calculations

#include <iostream>

using namespace std;

int main()

{

    int num,ocourse,classes,c1,c2,c3,c4,coursecrdt;
    double ogpa,g1,g2,g3,g4,honorpts;

    cout<<"Enter student number\n";
    cin>>num;
    cout<<"Enter old GPA score\n";
    cin>>ogpa;
    cout<<"Enter old course credit\n";
    cin>>ocourse;
    cout<<endl;
    cout<<"Student Number:      "<<num<<endl;
    cout<<endl;
    cout<<"Old GPA score:       "<<ogpa<<endl;
    cout<<endl;
    cout<<"Old Course Credit    "<<ocourse<<endl;
    cout<<endl;
    cout<<"How many classes are you taking this semester? (minimum 5)\n"<<endl;
    cin>>classes;
    if (classes==1)
    {
    
    cout<<"Enter number of credits for first class in new semester\n"<<endl;
    cin>>c1;
    cout<<"Enter grade for first class in new semester\n"<<endl;
    cin>>g1;
    cout<<endl;
    cout<<"New Honor Points:                    "<<c1*g1<<endl;
    cout<<"Total number of new course credit:   "<<c1<<endl;
    cout<<"Current GPA:  
    "<<c1*g1/c1<<endl;
    }
    else if (classes == 2)
    {

    cout<<"Enter number of credits for first class in new semester\n"<<endl;
    cin>>c1;
    cout<<"Enter grade for first class in new semester\n"<<endl;
    cin>>g1;
    cout<<"Enter of number of credits for second class in new semester\n"<<endl;
    cin>>c2;
    cout<<"Enter grade for second class in new semester\n"<<endl;
    cin>>g2;
    cout<<endl;
    cout<<"New Honor Points:                    "<<c1*g1+c2*g2<<endl;
    cout<<"Total number of new course credit:   "<<c1+c2<<endl;
    cout<<"Current GPA:                         "<<(c1*g1+c2*g2)/(c1+c2)<<endl;
    
    }
    else if (classes == 3)
    {
    
    cout<<"Enter number of credits for first class in new semester\n"<<endl;
    cin>>c1;
    cout<<"Enter grade for first class in new semester\n"<<endl;
    cin>>g1;
    cout<<"Enter of number of credits for second class in new semester\n"<<endl;
    cin>>c2;
    cout<<"Enter grade for second class in new semester\n"<<endl;
    cin>>g2;
    cout<<"Enter of number of credits for third class in new semester\n"<<endl;
    cin>>c3;
    cout<<"Enter grade for thrid class in new semester\n"<<endl;
    cin>>g3;
    cout<<endl;
     cout<<"New Honor Points:                    "<<c1*g1+c2*g2+c3*g3<<endl;
    cout<<"Total number of new course credit:   "<<c1+c2+c3<<endl;
    cout<<"Current GPA:                         "<<(c1*g1+c2*g2+c3*g3)/(c1+c2+c3)<<endl;
    
    }
    else if (classes >= 4)
    {
    
    cout<<"Enter number of credits for first class in new semester\n"<<endl;
    cin>>c1;
    cout<<"Enter grade for first class in new semester\n"<<endl;
    cin>>g1;
    cout<<"Enter of number of credits for second class in new semester\n"<<endl;
    cin>>c2;
    cout<<"Enter grade for second class in new semester\n"<<endl;
    cin>>g2;
    cout<<"Enter of number of credits for third class in new semester\n"<<endl;
    cin>>c3;
    cout<<"Enter grade for thrid class in new semester\n"<<endl;
    cin>>g3;
    cout<<"Enter of number of credits for fourth class in new semester\n"<<endl;
    cin>>c4;
    cout<<"Enter grade for fourth class in new semester\n"<<endl;
    cin>>g4;
        honorpts=c1*g1+c2*g2+c3*g3+c4*g4;
        coursecrdt=c1+c2+c3+c4;
    cout<<endl;

    cout<<"New Honor Points:                    "<<honorpts<<endl;
    cout<<"Total number of new course credit:   "<<coursecrdt<<endl;
    cout<<"Current GPA:                         "<<honorpts/coursecrdt<<endl;
    
    
    }


    return 0;
    

}

