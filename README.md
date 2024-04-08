# Admin-HackPack-CTF-Contextual-Decipher
Admin Repo to be used for HackPack challenge deployment

# Challenge Explained (Admin Only):
- The theme of this challenge is Contextual Decipher targeting the use of LLMs to understand texts.
- Any LLM of their choice is allowed.
- Theme follows that a company follows a new security approach of encryption to protect their documents and keep them safe i.e. contextual ciphering.
- They share the protected file paired with additional files of large texts that are the `key` to the protected file `file containing the flag` which are then changed with every transmission.
- We have successfully caught one of the secure transmissions, and they have to unlock the secret file `capture the flag`.
- The `key` files may be completely unrelated to the protected file but they do hide the key in the context of the containing texts.
- We have captured the link to the _Participant_ Repository (`https://github.com/aadiltajani/decrypttheenigma` or something else) containing  `Most Rated Quarterly Featured Articles - All That Matters.pdf` which has 10 articles, each having a hidden main/central idea _(to be extracted using LLMs)_, and `Quarterly Government Directorate of Cybersecurity Directives Appendix.pdf` consisting of 26`[A-Z] indexed` directorates among which 10 directives are based on those 10 articles, where each directive uniquely relates to one article only _(to be semantically matched by LLMs)_.
- Brute forcing all the articles together won't work so they'll have to do it one by one or more if the model they selected has enough input_limit. Tested on GPT3.5/4 and Gemini 1.5 Pro.
- This has to be worked out by the participants and eventually, they have 10 non-repeated `[A-Z]` letters which have to be arranged in an ascending order of the dates of respective articles to form the password `QUEXOTIDAS`.
- This password then unlocks the protected file `Obvious Secret Message.pdf` revealing the flag `flag{ context_mogged }`.




_________________________________________________________________  
_________________________________________________________________


# Participant Challenge Title and Instructions:



## Title: Decrypt the Enigma
You've intercepted a transmission from CryptoCraft, a secretive organization renowned for their innovative encryption methods. This transmission revolves around their latest breakthrough in contextual encryption, a technique designed to render traditional methods useless. Your task is to decipher the encrypted message hidden within the transmission and uncover the flag. Good luck!
