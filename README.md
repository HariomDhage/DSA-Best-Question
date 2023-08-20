# DSA-Best-Question
DSA best quality question


Q1 rotate matrix by 90 degree?

solution 1:
#include<iostream>
using namespace std;
int main(){

   int n=4;
   int mat[4][4];
  for(int i=0 ;i<n;i++){
      for(int j=0;j<n;j++){
      
   cin >>mat[i][j];
      }
  }
   
  for(int i=0; i<n; i++){
      for(int j=0;j<n;j++){
          cout<< mat[i][j]<<" ";
          }
          cout<<endl;
          }
 
  cout<<"transpose matrix:"<<endl;
    for(int i=0; i<n; i++){
     for(int j=0; j<n; j++){
       cout<<mat[i][j]<<" ";
    }     cout<<endl; }


   for(int i=0; i<n; i++){
     for(int j=0; j<n/2; j++){
        swap(mat[i][j], mat[i][n-j-1]);
     }
   }

 
   cout<<"Rotated Matrix :\n";
   for(int i=0; i<n; i++){
     for(int j=0; j<n; j++){
       cout<<mat[i][j]<<" ";
     }
     cout<<endl;
   }
}

optimisized solution 2:

#include<iostream>
using namespace std;
int main(){

   int n=4;
   int mat[4][4];
  for(int i=0 ;i<n;i++){
      for(int j=0;j<n;j++){
           cin >>mat[i][j];
      }
  }  
  for(int i=0; i<n; i++){
      for(int j=0;j<n;j++){
          cout<< mat[i][j]<<" ";
          }
          cout<<endl;
  } 
   cout<<"Rotated Matrix :\n";
   for(int i=0; i<n; i++){
     for(int j=n-1; j>=0; j--){
       cout<<mat[j][i]<<" ";
     }
     cout<<endl;
   }
}

