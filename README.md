<div align="center">
  <h1>Password Checker</h1>
  <blockquote>Script to check if a list of passwords have been powned</blockquote>
</div>

## 📦 External libraries installation

```
// with Python 3
pip3 install requests
```

## ⚙️ Usage

- First argument: 1 to n passwords to check if they have been pwned

```
python main.py [Passwords to check]
```

## 📜 Documentation and examples

Check out the haveibeenpwned [API Documentation](https://haveibeenpwned.com/API/v2).

For more secure reasons, the API uses the K–anonymity technique, that allows to receive information about us without know who we are. It's a technique that is used a lot, especially now that a lot of people don't want to give their personal information to companies. This K-anonymity technique allow the companies track you but still not know who you are. The way this works is that we only give the first five characters of our hashed password, then the API will return all the passwords hashes that contains the same first five characters, so then we can compare them with the rest of our hash password to find our solution.

Example:

```
python main.py hello test abcdefGHIJK
```
