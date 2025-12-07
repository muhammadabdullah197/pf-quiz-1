#include <iostreamn>
using namespace std;
int main () {
int N , fine = 0 , totalfine = 0 , dayslate = 0;
cout << "Enter total users";
cin >> N;
for (int i = 1; i<=N; i++) {
cout << "enter the dayslate for user " <<i << " : ";
cin >> dayslate; 
if (dayslate == 0) {
fine = 0; 
} else if (dayslate >= 1 && dayslate <= 5) {
fine = dayslate * 20;
} else { 
fine = dayslate * 30
}
cout << "total fine for user" <<i "=" <<fine;
totalfine = totalfine + fine;
}
cout << "total fine collected = " <<totalfine;
return 0;
}
