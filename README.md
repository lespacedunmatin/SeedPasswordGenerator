# SeedPasswordGenerator

A simple Javascript form to create MD5 passwords (32 chars long)

People usually use less than 5 differents passwords for their online life, easy to remember and less than 12 char long.

This proposal aims to generate a MD5 hash (32 hex char long) of **seed + ' ' + login + ' ' + url**, wich will be way more strong against force brute attacks, and unique for each website/account combination.

The **seed** is added to preserve randomness to the password in case of database compromission. It acts as a master key.

**Login** can be any chain of characters (including email adress).

**url** is intended to be the root of the website, but can also be any chain of characters.
