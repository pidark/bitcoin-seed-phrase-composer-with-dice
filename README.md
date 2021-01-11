# Bitcoin Seed Phrase Composer With Dice
Offline bitcoin seed phrase composer tool with visual word selection verification.

Available here to test it https://n3s1us.github.io/bitcoin-seed-phrase-composer-with-dice/

<p align="center">
  <img src="./preview.gif" width="738">
</p>

# Create your own wallet seed using regular dice
If you want maximum security you should of course not rely on a 3rd party to generate your wallet seed. This is a way to do it using only regular 6-sided dice.

To be really, really sure that you have created a Bitcoin wallet that's secure you should generate the wallet seed offline and using a method that is transparent, i.e. where you can audit the process yourself and understand where the entropy/randomness comes from.

The good thing about this method is that it is completely obvious what you are doing. You want 23 random words from a list of 2048 words so you simply draw words from a hat.

# Using more dice instead of one
If you wanna speed up the process by using more dice instead of one you need to make sure that you read the results in a predetermined order (so that your own brain is not involved in the process of deciding which die should be read first). The simplest way to do this is to always read the from left to right as they land on the table. Another option would be to use differently colored dice and decide that the red one is the first one, the blue one is the second etc.

# What about the 24th word?!
The 24th word in a BIP-39 seed is not a randomly generated one. Actually, the way a seed is normally generated is by a computer generating 256 bits of random data. From this data a checksum of 8 bits is then calculated and appended to the 256 bits. The 264 resulting bits are divided into 24 parts of 11 bits each and each one of those 11 bits is converted into a word, using a predetermined word list.

This means that part of our 24th word is actually a checksum so we can’t just choose any word, it has to be calculated. As this is almost impossible to do manually (it involves using the SHA-256 hash function) this tool has a “last word calculator”.

# How to use?
This tool is simply a single file web page using javascript for calculations, that can be downloaded and used offline. Now, since you have been really focused on maximum security so far you should keep that mindset for this step too.

I recommends booting any Linux Live from a USB stick, get the web page on the same or another USB stick and then NEVER connect this Linux Live to internet neither before nor after!

# References
[Create your own wallet seed using regular dice](https://en.bitcoin.se/articles/create-your-own-wallet-seed-using-regular-dice) 

[SeedPicker](https://seedpicker.net/calculator/last-word.html)



# Donations are welcome

bc1qzxvd55p0vxks6ffrrja65e4rcsd3ndhf8gme72
