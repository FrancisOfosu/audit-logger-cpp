/*
  Program: Audit Logger
  Author : Francis Ofosu
  Date   : [June 30, 2025]
  Purpose: This program prompts the user for their full name and an action performed.
		   It then outputs an audit-style log entry in the format:
		   [AUDIT] Francis Ofosu performed 'Logged into system'
*/


#include<iostream>
#include<string>
int main()
{
	// Declare variables to store user name and action performed
	std::string fname;
	std::string action;
	
	// Prompt user for their full name
	std::cout << "Enter your full name: ";
	std::getline(std::cin, fname);			// Read full name, including spaces
	
	
	// Prompt user for the action they performed
	std::cout << "Enter action performed: ";
	std::getline(std::cin, action);			// Read full description of the action
	
	// Output a formatted audit log entry
	std::cout << "[AUDIT] " << fname << " performed " << "'" << action << "'";
	return 0;
}