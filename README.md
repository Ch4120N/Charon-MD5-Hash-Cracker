<head>
  <meta name="google-site-verification" content="l4gzIHopgDDt57xRYeRvJZ5DYgg4lLb-qPciUxhNxkY" />
</head>

# Charon MD5 Hash Cracker

`Charon MD5 Hash Cracker` is a specialized tool for <u>hackers</u> designed to crack MD5 hashes using brute force. This tool is specifically created for penetration testing and security activities, helping hackers recover passwords from MD5 hashes.


## Project Porgrammer
> AmirHossein Ghanami (Ch4120N) - Ch4120ni@Gmail.com

## Made For
> Cracking MD5 hashes high speed


## 💻 Supported Operating Systems
- [X] Ubuntu/Debian
- [X] Kali Linux
- [X] Arch Linux/Red Hat Linux
- [X] Windows 10/8.1/8/7


## ✨ Features

* Good Command Line Design
* Easy to use
* Very High Speed
* Advanced Error Handling

## How it Works?
The `Charon MD5 Hash Cracker` is a <u>brute force</u> tool designed to crack MD5 hashes by systematically generating potential plaintexts and comparing their MD5 hash to the target hash. Here’s a breakdown of how the tool works:

1. Input Parameters:

    * The tool accepts four main arguments:

      - setChar: Specifies the character set to use, where a includes lowercase letters, A includes uppercase letters, n includes numbers, and s includes symbols.
  
      - minChar: The minimum length of the strings to be generated.
      - maxChar: The maximum length of the strings to be generated.
      - MD5Hash: The MD5 hash that needs to be cracked.

2. Character Set Selection:

    * Based on the setChar input, the tool constructs a character set that will be used to generate possible plaintexts. This set can include any combination of lowercase letters, uppercase letters, digits, and symbols.
  
3. Hash Cracking Process:

    * The tool iterates through all possible combinations of characters within the specified length range (minChar to maxChar).
  For each combination, it generates a string and calculates its MD5 hash using Python's hashlib library.
  The generated hash is then compared to the target MD5 hash.

4. Success and Failure:

    * If a match is found, the tool prints the cracked password and exits.
    * If no match is found after testing all combinations, the tool informs the user that the bruteforce attack was completed without success.

5. Output:

    * The tool provides real-time updates on the progress of the cracking attempt, showing the current string being tested and its corresponding MD5 hash.

This process continues until either the correct password is found or all possible combinations have been exhausted.

