# Stokvels in Algorand Blockchain 

A stokvel is a type of credit union in which a group of people enter into an agreement to contribute a fixed amount of money to a common pool weekly, fortnightly or monthly. Universally, such a system is known as a rotating savings and credit association which is a group of individuals who agree to meet for a defined period to save together, with each member receiving a periodic payout.

This is a development of a stokvel application (CLI) on the Algorand blockchain to demonstrate how to run a decentralised stokvel amongst 5 participants. 

The constitution of the stokvel is as follows:
-  On day t of each month, each participating member deposits 5 Algos from their account into the joint stokvel account. The stokvel account should be implemented as a multisignature (multisig) account.
- On day t + 1 of each month, 15 Algos (i.e. 60% of the current month’s deposits) are transferred to a randomly selected member who hasn’t been paid in previous rounds. For this payment to happen from the stokvel account, 80% of members must sign the payout transaction i.e. the stokvel account is a multisig account that requires a 4-of-5 quorum for payments to happen – i.e. 4 of the 5 members are required to sign the transaction on the stokvel account.
- The stokvel continues indefinitely unless a member elects to opt out at the end of the 5-month cycle (i.e. once everybody has been paid)

