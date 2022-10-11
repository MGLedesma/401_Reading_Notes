# Applying The CIA triad to Enterprise File Transfer

## The CIA Triad refers to the three basic principles/objectives in information security
- Confidentiality 
    - refers to the principle of restricting access to or knowledge of certain pieces of information to certain individuals.
    - MitM attack to eavesdroop on transmission or hack directly, imperative to mitigate unauthorized access and disclosures.
- Integrity
    - pertains to the principle of preventing datat from being tampered.
    - MitM attacks during data transfers or direct hack
- Availability
    - data access available anytime

## Technical solutions for achieving enterprise file transfers
- Confidentiality in file transfers
    - Encryption - renders data unreadable, decryption to render data readable again
        - solution grouped into two categories
            - encrypt data-at-rest
            - decrypt data-in-transit 
        - data-in-transit encryption achieved through SSL or SSH
        - data-at-rest encryption is achieved through OpenPGP of disk-level or file-level encryption solutions.
        - encrypting data 
            - before (while in sender's server)
            - during (while traversing the network)
            - after (upon arrival at the recipient's server)
        - another method is authentication, can help restrict access to data to authorized individuals with multi-factor authentication
- I