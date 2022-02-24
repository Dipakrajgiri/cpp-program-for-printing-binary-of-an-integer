# c-program-for-printing-binary-of-an-integer
c++ program for printing binary of an integer
source code:

 include<iostream>

 using namespace std;
 int main()
 {
 int n,i,j,k,l,c,z,flag;
 int a[10];
 cout<<"enter a number";
 cin>>n;
 cout<<"number is square?"<<endl;
 for(i=1;i<=n;i++)
 {
     flag=0;
     c=i;
     for(k=0;k<10;k++)
     {

         z=c%2;
         if(z==1)
         {
           a[k]=z;
         }
         else
         {
             a[k]=0;
         }


         c=c/2;

     }
     for(j=1;j<=i;j++)
     {
         if(i==j*j)
         {
             flag=1;
             cout<<i<<"     y     ";
             for(l=9;l>=0;l--)
             {
                 cout<<a[l];
             }
             cout<<endl;
             break;
         }
     }
     if(flag==0)
     {


       cout<<i<<"     n     ";
             for(l=9;l>=0;l--)
             {
                 cout<<a[l];
             }
             cout<<endl;
     }

 }


 return 0;
 }
