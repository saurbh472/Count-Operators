// C Program to count 
#include <stdio.h> 
int main() 
{ 
	FILE *fp; 

// Character counter (result) 
	int count = 0; 
	// To store a character read from file 
  char c; 
  
  
// Open the file 
	fp = fopen("text.txt", "r"); 

// Check if file exists 
	if (fp == NULL) { 
		printf("Could not open file "); 
		return 0; 
	} 

// Extract characters from file 
	// and store in character c 
	for (c = getc(fp); c != EOF; c = getc(fp)) 

// Increment count for this character 
		 
   if( c>=40 && c<=50)
        count = count + 1;

// Close the file 
	fclose(fp); 

// Print the count of characters 
	printf("The file  has %d characters\n ", count); 

return 0; 
} 
