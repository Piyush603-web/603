#include<iostream>
using namespace std;

void reverse(int arr[], int n) {
    int start = 0;
    int end = n - 1;
    while (start <= end) {
        swap(arr[start], arr[end]);
        start++;
        end--;
    }
}

void PrintArray(int arr[], int n) {
    for (int i = 0; i < n; i++) {
        cout << arr[i] << " ";  // Add space between elements
    }
    cout << endl;
}

int main() {
    int arr[6] = {4, -4, 0, 7, 5, 2};  // Use curly braces and remove extra comma
    int brr[4] = {6, -7, 2, 1};        // Use curly braces and remove extra comma

    reverse(arr, 6);
    reverse(brr, 4);

    PrintArray(arr, 6);
    PrintArray(brr, 4);

    return 0;
}
