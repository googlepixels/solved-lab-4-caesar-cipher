Download Link: https://assignmentchef.com/product/solved-lab-4-caesar-cipher
<br>
Since you are now familiar with sub routines (procedures) lets use them to create a cipher.

<strong>Encryption and Decryption  </strong>

You want to be able to hang out with the cool kids that use the Caesar Cipher ( <a href="https://en.wikipedia.org/wiki/Caesar_cipher">http://en.wikipedia.org/wiki/Caesar_cipher</a> ) to tell jokes on the internet so you decide to write a program to help you convert jokes into and out of any Caesar Cipher format (ROT-13 is an example of one). Your task is:

<ol>

 <li>Create a 2×200 array. You will be able to store one string in normal text mode and the encrypted string for it.</li>

 <li>Print a prompt that asks to either encrypt or decrypt a string.</li>

 <li>Print a prompt that ask the user for a number between 1 and 25 or ‘x’ to quit.</li>

 <li>Print a prompt that asks for the string to encrypt or decrypt.</li>

 <li>Using either row major or column major form store the string entered into your 2D array in row</li>

 <li>Either encrypt or decrypt the string entered and store it into your 2D array in row 1. Print out your 2D array.</li>

 <li>Repeat.</li>

</ol>

You need to also make a flowchart for this program.

<strong>The Caesar Cipher Algorithm  </strong>

The Caesar Cipher is an encoding method that works like this (example is for a shift amount of 13, which is a ROT-13).

<strong>if ( character is in alphabet ) </strong>

<strong>{ </strong>

<strong>if ( character is in top half of alphabet [A-M|a-m] ) </strong> <strong>character = character + 13; </strong> <strong>else ( character is in bottom half [N-Z|n-z] ) </strong> <strong>character = character – 13; </strong>

<strong>} </strong>

<strong>print (character); </strong>

<strong>Notes:  </strong>

<ul>

 <li>Non-alphabetic characters such as numbers (1,2,3), punctuation (,.?!), and other weird stuff (&amp;#$[}|, etc) should not be altered before output. That is to say, if I enter ‘@’, I should get ‘@’ back.</li>

 <li>To get some test input do an internet search for “rot13 jokes”, this will be for Caesar Cipher’s of 13 only though.</li>

 <li>You can also search the internet for other Caesar Cipher examples.</li>

</ul>

<strong>Requirements  </strong>

You are required to use a 2D array structure with either <strong>Row Major </strong>or <strong>Column Major </strong>ordering that was covered in class. Be sure to put which one you use in your README and in your code comments. You need to make use of a few sub routines:

<ul>

 <li>Encrypt: It takes a character and a cipher as an input and returns the encrypted value</li>

 <li>Decrypt: It takes an encrypted character and a cipher and returns the decrypted value</li>

 <li>Print Array: It prints the 2D array out</li>

 <li>Store: Takes coordinates (Ri, Ci) and byte of data and stores into the 2D array</li>

 <li>Load: Takes coordinates (Ri, Ci) and loads a byte of data from the 2D array</li>

</ul>




<strong>The Encrypt, Decrypt, and Print Array sub routines will call the Store and Load sub routines.  </strong>

<strong>Example of possible output for Part B:  </strong>

<strong>Hello, welcome to my Caesar Cipher program </strong> <strong>Do you want to (E)ncrypt or D(ecrypt) or e(X)it? </strong>

<strong>&gt; D </strong>

<strong>What is the cipher (1-25)? </strong>

<strong>&gt; 13 </strong>

<strong>What is the string (up to 200 characters)? </strong>

<strong>&gt; Fpubby vf sha!! </strong>

<strong>Here is your string and the decrypted result </strong> <strong>&lt;Encrypted&gt; Fpubby vf sha!! </strong>

<strong>&lt;Decrypted&gt; School is fun!! </strong>

<strong>&gt; Do you want to (E)ncrypt or D(ecrypt) or e(x)it? </strong> <strong>&gt; X </strong>

<strong>Goodbye!! </strong>





