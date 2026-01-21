# Bubble-Sort-in-C
A simple C program that demonstrates the Bubble Sort algorithm for sorting an array in ascending order. Ideal for beginners learning sorting techniques in C programming.
# Bubble Sort in C

This repository contains a simple C program that implements the **Bubble Sort** algorithm.
Bubble Sort is one of the basic sorting techniques used to arrange elements in ascending order.

## 🔹 What is Bubble Sort?
Bubble Sort repeatedly compares adjacent elements and swaps them if they are in the wrong order.
This process continues until the array is completely sorted.

## 🔹 Program Features
- Uses integer array
- Sorts elements in ascending order
- Beginner-friendly logic
- Easy to understand and modify

## 🔹 Source Code
```c
#include <stdio.h>

int main() {
    int a[5] = {5, 1, 4, 2, 8};
    int temp;

    for(int i = 0; i < 4; i++) {
        for(int j = 0; j < 4 - i; j++) {
            if(a[j] > a[j + 1]) {
                temp = a[j];
                a[j] = a[j + 1];
                a[j + 1] = temp;
            }
        }
    }

    printf("Sorted array: ");
    for(int i = 0; i < 5; i++) {
        printf("%d ", a[i]);
    }

    return 0;
}
