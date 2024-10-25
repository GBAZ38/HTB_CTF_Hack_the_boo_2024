# LinkHands

You've infiltrated the secret meeting of the demonic cult - they want you to join their summoning circle. But who to link hands with?

---

# Supporting material:

This challege provided a .zip file titled rev_linkhands. the .zip archive contains the folder rev_linkhands. The folder contains an aplication file named link. 

# Methods:

Attempting to examine the binary code of `link` in Visual Studio Code gives us an error. Bypassing the error gives us a bunch of non legible text

![VS_Error](/Screenshots/VS_Error.png)

![Link_code1](/Screenshots/Link_code1.png)

The most interesting part of thise code is the plain text:

![Link_code2](/Screenshots/Link_code2.png)

It seems that we're meant to run the code we downloaded. To do so we use the terminal to change directory to the rev_linkhands folder. we do this by extracting the .zip file to our documents directory, and using the `cd` command to access our new `rev_linkhands` folder containing the `link` binary.

![Parrot_terminal](/Screenshots/Parrot_terminal.png)

We then use the `./link` command to execute the binary. this returns the text `The cultists look expectantly to you - who will you link hands with?`

It seems we need some key to get the flag. The frst thing that came to mind was `tcp`, but this gave me the output `You fail to grasp their hands - they look at you with suspicious...`

Then i thought maybe i needed to finish the sentence so i tried `eyes` to no avail.

Potentially need to use a tool like https://github.com/icsharpcode/ILSpy?tab=readme-ov-file to further analyze code.
