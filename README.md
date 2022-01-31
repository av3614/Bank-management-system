// C program to implement

// the above approach

#include <conio.h>

#include <stdio.h>

#include <stdlib.h>

#include <string.h>

#include <windows.h>

 

// Declaring all the functions

void checkbalance(char*);

void transfermoney(void);

void display(char*);

void person(char*);

void login(void);

void loginsu(void);

void account(void);

void accountcreated(void);

void afterlogin(void);

void logout(void);

 

// Declaring gotoxy

// function for setting

// cursor position

void gotoxy(int x, int y)

{

    COORD c;

    c.X = x;

    c.Y = y;

 

    SetConsoleCursorPosition(

        GetStdHandle(STD_OUTPUT_HANDLE), c);

}

 

// Creating a structure to store

// data of the user

struct pass {

    char username[50];

    int date, month, year;

    char pnumber[15];

    char adharnum[20];

    char fname[20];

    char lname[20];

    char fathname[20];

    

