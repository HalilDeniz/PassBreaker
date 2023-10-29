
# PassBreaker

PassBreaker is a command-line password cracking tool developed in Python. It allows you to perform various password cracking techniques such as wordlist-based attacks and brute force attacks.
<img src="source/passbreaker">

## Features

- Wordlist-based password cracking
- Brute force password cracking
- Support for multiple hash algorithms
- Optional salt value
- Parallel processing option for faster cracking
- Password complexity evaluation
- Customizable minimum and maximum password length
- Customizable character set for brute force attacks

## Installation

1. Clone the repository:

   ```shell
   git clone https://github.com/HalilDeniz/PassBreaker.git
   ```

2. Install the required dependencies:

   ```shell
   pip install -r requirements.txt
   ```

## Usage

```bash
python passbreaker.py <password_hash> <wordlist_file> [--algorithm]
```

Replace `<password_hash>` with the target password hash and `<wordlist_file>` with the path to the wordlist file containing potential passwords.

### Options

- `--algorithm <algorithm>`: Specify the hash algorithm to use (e.g., md5, sha256, sha512).
- `-s, --salt <salt>`: Specify a salt value to use.
- `-p, --parallel`: Enable parallel processing for faster cracking.
- `-c, --complexity`: Evaluate password complexity before cracking.
- `-b, --brute-force`: Perform a brute force attack.
- `--min-length <min_length>`: Set the minimum password length for brute force attacks.
- `--max-length <max_length>`: Set the maximum password length for brute force attacks.
- `--character-set <character_set>`: Set the character set to use for brute force attacks.

Elbette! İşte İngilizce olarak yazılmış başlık ve küçük bir bilgi ile daha fazla kullanım örneği:

## Usage Examples

### Wordlist-based Password Cracking
```shell
python passbreaker.py 5f4dcc3b5aa765d61d8327deb882cf99 passwords.txt --algorithm md5
```
This command attempts to crack the password with the hash value "5f4dcc3b5aa765d61d8327deb882cf99" using the MD5 algorithm and a wordlist from the "passwords.txt" file.

### Brute Force Attack
```shell
python passbreaker.py 5f4dcc3b5aa765d61d8327deb882cf99 --brute-force --min-length 6 --max-length 8 --character-set abc123
```
This command performs a brute force attack to crack the password with the hash value "5f4dcc3b5aa765d61d8327deb882cf99" by trying all possible combinations of passwords with a length between 6 and 8 characters, using the character set "abc123".

### Password Complexity Evaluation
```shell
python passbreaker.py 5f4dcc3b5aa765d61d8327deb882cf99 passwords.txt --algorithm sha256 --complexity
```
This command evaluates the complexity of passwords in the "passwords.txt" file and attempts to crack the password with the hash value "5f4dcc3b5aa765d61d8327deb882cf99" using the SHA-256 algorithm. It only tries passwords that meet the complexity requirements.

### Using Salt Value
```shell
python passbreaker.py 5f4dcc3b5aa765d61d8327deb882cf99 passwords.txt --algorithm md5 --salt mysalt123
```
This command uses a specific salt value ("mysalt123") for the password cracking process. Salt is used to enhance the security of passwords.

### Parallel Processing
```shell
python passbreaker.py 5f4dcc3b5aa765d61d8327deb882cf99 passwords.txt --algorithm sha512 --parallel
```
This command performs password cracking with parallel processing for faster cracking. It utilizes multiple processing cores, but it may consume more system resources.

These examples demonstrate different features and use cases of the "PassBreaker" password cracking tool. Users can customize the parameters based on their needs and goals.
## Disclaimer

This tool is intended for educational and ethical purposes only. Misuse of this tool for any malicious activities is strictly prohibited. The developers assume no liability and are not responsible for any misuse or damage caused by this tool.

## Contributing
Contributions are welcome! To contribute to PassBreaker, follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your changes to your forked repository.
5. Open a pull request in the main repository.

## Contact

If you have any questions, comments, or suggestions about PassBreaker, please feel free to contact me:

- LinkedIn: [LinkedIn](https://www.linkedin.com/in/halil-ibrahim-deniz/)
- TryHackMe: [TryHackMe](https://tryhackme.com/p/halilovic)
- Instagram: [Instagram](https://www.instagram.com/deniz.halil333/)
- YouTube: [YouTube](https://www.youtube.com/c/HalilDeniz)
- Email: halildeniz313@gmail.com


## License
PassBreaker is released under the [MIT License](LICENSE). See LICENSE for more information.


