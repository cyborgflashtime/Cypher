#Cypher

Cypher is a proof of concept ransomware which implements the PyCrpto module and uses gmail(Currently) as a simple command and control server. It is a work in progress as of yet and i will be releasing updates periodically depending on the amount of time i have to work on the project.

#Operation

Cypher operates by generating a unique client ID for each box that has been infected. The client ID and encryption key will sent via email to a gmail adress by leveraging python's SMTP lib. After Cypher has enumerated the files we wish to encrypt the multiprocessing and PyCrypto libs are employed to do the actual encrypting. I opted to use the multiprocessing lib to speed up the encryption process.

Finally Cypher will write out a README note and the client ID which would have to be relayed to the operator in orer to retrieve the proper decrypting binary and key respectively.

#To do

[+]Extensive and multi-platform testing.
[+]Write decrypting module.
[+]Designing and developing a more secure C&C mechanism.

#Want to contribute?

I'd be more than willing to collaborate on this and if you wish to contribute feel free to open an issue and we may discuss the details and/or ideas you might have to offer.



