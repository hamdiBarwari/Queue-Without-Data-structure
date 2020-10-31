#include <iostream>
#include<string>
using namespace std;
  #define size 4
  string queue[size];
  int front = 0;
  int rear = 0;
    void main() {
        queue[rear] = "callofduty.exe";
        rear++;//1
        queue[rear] = "LIMBO";
        rear++;//2
        queue[rear] = "GTA";
        rear++;//3
        queue[rear] = "FIFA";
          cout << "the inserting to queue is: \n";
          cout << "front is : " << queue[3] << "\n";
            for (int i = front; i <= rear; i++){
             cout << queue[i] << "        ";}

          if (size - 1 == rear) {
            cout << "\n\nqueue is full " << "\n\n";}
        front++;//1
        int l = 0;
            while (front != 4) {
              cout << "the instal: " << queue[l] << endl;
                for (int i = front; i <= rear; i++){
                    cout << queue[i] << "        ";
                  if (queue[rear] == queue[front])
                    cout << "\nqueue is empty becaouse front = rear ";
                }//end of for
              front++;
              l++;
              cout <<"\n";
            }//end of while
        system("pause");
  }//end of main

