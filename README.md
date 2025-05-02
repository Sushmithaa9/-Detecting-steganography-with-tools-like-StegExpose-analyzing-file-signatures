# Detecting-steganography-with-tools-like-StegExpose-analyzing-file-signatures
## AIM:
To detect hidden data using steganography detection tools like StegExpose and analyze file signatures for authenticity and manipulation.

## DESIGN STEPS:
### Step 1:
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROCEDURE:
### Step 1: Download Image and Create Secret Message File
  •	Download a .jpeg image (e.g., praveen.jpeg) from a trusted website or use own image.
  
  ![WhatsApp Image 2025-04-26 at 11 30 02_c84ed103](https://github.com/user-attachments/assets/85bfe533-03d0-482c-8e78-cb6b93ffc102)

  •	Create a text file named secret with a confidential message:
  
 ![Screenshot 2025-05-02 212408](https://github.com/user-attachments/assets/478b2a5f-2713-4933-9ed6-c3f421cb19ce)


### Step 2: Install and Verify Steghide Tool
  •	Install Steghide on Kali linux and confirm the installation by checking its version:
  
  ![image](https://github.com/user-attachments/assets/32c9a635-9f76-4b05-933e-a009f48aad68)

 
### Step 3: Embed the Secret Message into the Image
  •	Use the following command to embed secret into praveen.jpeg:

  ![WhatsApp Image 2025-04-26 at 11 38 44_d5298f40](https://github.com/user-attachments/assets/49e85201-32a7-42a9-be85-e4308872a5fa)


### Step 4: Delete the Original Secret File
  •	After embedding, delete the plaintext file:
  
  ![WhatsApp Image 2025-04-26 at 11 59 13_eee03eec](https://github.com/user-attachments/assets/616ffdc0-a613-493c-8b31-2cccba0b840b)


## OUTPUT:
### Step 1: Extract the Embedded Secret from the Image
  •	To retrieve the hidden file:
  
  ![WhatsApp Image 2025-04-26 at 12 00 02_68532d25](https://github.com/user-attachments/assets/6c1c52c5-2a7b-4c5f-8963-11436815d249)


  •	Enter the same passphrase used during embedding.
  
 ![Screenshot 2025-05-02 212408](https://github.com/user-attachments/assets/55006a16-e200-4478-a2b7-861a8355c1f7)




### Step 2: Verify the Extracted Message

  •	Display the extracted file content to verify:
  
![Screenshot 2025-05-02 213616-fotor-2025050221440](https://github.com/user-attachments/assets/a3fe2afc-cc51-4956-abcd-c4deb3894294)


  
  •	Ensure the message matches the original secret content.

  •	Another command to see the same secret message is
  
  ![WhatsApp Image 2025-04-26 at 12 01 44_cdf9505d](https://github.com/user-attachments/assets/f194a241-cc96-4c18-8271-38ced3b2005b)


 
### Step 3: Retrieve Information About the Embedded Data
  •	To gather details about embedded content in the image:
  
  ![WhatsApp Image 2025-04-26 at 12 02 38_52c10b06](https://github.com/user-attachments/assets/f07b1691-da22-4848-b2a0-1744792d839d)
   
  •	This will display file type, size, and whether data is embedded.


## RESULT:
Hidden data was successfully detected and file signatures were analyzed for irregularities.
