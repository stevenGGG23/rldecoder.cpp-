* Filename: rldecoder.cpp
* Description: prompts the user to enter a filename containing the RLE pairs of count character. This will create immages of these files 
*/

#include <iostream>
#include <fstream>
#include <string>

int main() {
    // Ask for filename 
    std::string filename;
    std::cout << "Enter filename to decompress: ";
    std::cin >> filename;

    std::ifstream file(filename);

    // If the file does not exist, print an error message and end the program
    if (!file) {
        std::cout << "File " << filename << " does not exist!" << std::endl;
        return 1;
    }

    // store the count and character
    int num;
    char ch;
    // while loop to process information from the file
    file>>num;
    while (file) {
        file.ignore();
        file.get(ch);
        for (int i = 0; i < num; ++i) {
            std::cout << ch;
        }
        file>>num; 
    }

    // Close the file
    file.close();
    
    return 0;
} 
