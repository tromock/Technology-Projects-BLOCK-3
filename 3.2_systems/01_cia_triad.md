# Exploring the CIA Triad

## Objective

Understand the **Confidentiality, Integrity and Availability (CIA)** principles using practical tasks on a Raspberry Pi.

---

# Part 1 – Confidentiality

1. Create a confidential file.

    ```bash
    nano secrets.txt
    ```

1. Write some confidential information.

1. Save the file.

1. Now restrict access:
    ```bash
    chmod 600 secrets.txt
    ```
1. Check permissions:
    ```bash
    ls -l secrets.txt
    ```

**Questions**
- Who can read this file? - admin
- How does file permission protect confidentiality? - unables the access to the data

## Part 2 – Integrity

1. Create a hash of the file.
    ```bash
    sha256sum secrets.txt
    ```
    _What does "hash" do?

1. Save the output. - 0d77482a3b516f1cc50ada879b19df6578e114d5ba6e7c293b9802e5a03a9f30  secrets.txt

1. Modify the file. - 
    ```bash
    nano secrets.txt
    ```

1. Run the hash again.
2c8e9cef379420c027282f8d9381c1126bd2dbde1cdd7e4da1244377ba55936a  secrets.txt

** Questions**
- Did the hash change? - Yes
- Why do security systems use hashing? - to secure the data


# Part 3 – Availability

1. Check system uptime:
    ```bash
    uptime
    ```

1. List running processes:
    ```bash
    top
    ```

**Questions**
- Why is system uptime important? - to be up the date
- What happens if a system is unavailable? - User cannot access services or data.

## Deliverables
Include:
- Screenshot of file permissions
- Screenshot of hash results
- Answers to questions
- Reflection
    >Explain how this activity demonstrated the CIA triad.
uptime
