# Excel Password Cracker - Seclists

A simple brute-force attack password cracker for Excel files with multi-threaded implementation optimizing performance.

The original tool simply generates a sequence of words (including numbers) following the predefined character combination, and attempts to decrypt Excel file with each password until the correct one is found.

The added method use a passwords.txt instead, this files can for example be copied from Seclists (https://github.com/danielmiessler/SecLists/tree/master/Passwords)

Brute-force is not the most efficient algorithm out there, so keep in mind that this tool is limited to be functional with simple passwords.

## Usage for non Java people

- Git Clone
- Install Java and Maven
- ```mvn install```
- Put your excel file as ```input.xlsx```
- Put your password text file as ```passwords.txt```
- ```java -cp target/ExcelPasswordCracker-jar-with-dependencies.jar MainSeclists```
- The program stop when the password is found


## Todo
- [ ] Save decrypted file
- [ ] Progress info
- [ ] Easier selection of characters for generator
- [ ] Dictionary attack
- [ ] Code readability
- [ ] Heuristics
- [ ] Benchmarks
- [ ] Save last position
- [ ] Possibility to restart form last position
