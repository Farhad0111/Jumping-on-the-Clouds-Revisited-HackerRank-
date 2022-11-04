// Jumping-on-the-Clouds-Revisited-HackerRank-
#include <iostream>
#include<vector>
using namespace std;
class Farhad{
public:    
  int n,k;
  int c[10005];
  //vector<int>c(10005);
  public:
    int faru(){
        //int n,k;
        cin>>n>>k;
        //vector<int>c(n);
        for(int i=0;i<n;i++){
            cin>>c[i];
        }
        return 0;
    }
};
class Farhad1:public Farhad{
  public:
    int e=100,cur=0;
    public:
    int display(){
        faru();
        while(true){
            cur+=k;
            cur%=n;
            if(c[cur]){
                e-=2;
            }
            e--;
            if(cur==0){
                break;
            }
        }
        cout<<e<<endl;
        return 0;
    }
};
int main(){
    Farhad1 farhad=Farhad1();
    farhad.display();
    return 0;
}
