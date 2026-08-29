
USB Forensic Acquisition Using FTK Imager
Student Information

Student Name: Idriss Muhammad Abdullahi

Registration Number: fwsd2511475

Course: CIP-B102 Digital Forensics

Lab Title: USB Forensic Acquisition

Date:29/08/2026

1. Introduction

Digital forensic investigations require investigators to create exact copies of storage devices while preserving the integrity of the original evidence. This process is referred to as forensic acquisition or forensic imaging.

The purpose of this laboratory exercise was to create a forensically sound image of a USB storage device using FTK Imager, verify the integrity of the acquired image using hash values, and validate that the expected evidence files were successfully captured within the forensic image.

2. Objectives

The objectives of this laboratory were:

1. Prepare a USB device with sample evidence.
2. Document evidence acquisition information.
3. Acquire a forensic image using FTK Imager.
4. Verify image integrity using cryptographic hashes.
5. Validate that the image contains the expected evidence file.
6. Produce a professional forensic acquisition report.

3. Evidence Preparation

A folder named:
CIP-B102-Lab4-Evidence

was created on the USB device.

The following files were stored inside the folder:

Idriss_Muhammad.txt
my passport.jpg
Idriss Muhammed Abdullahi undertaking.pdf

Contents of firstname_lastname.txt:
Full Name: Idriss Muhammad Abdullahi
Registration Number: fwsd2511475
Date:28/August/2026

Statement:
I confirm that this USB device was prepared for a controlled forensic acquisition laboratory exercise for CIP-B102 Lab 4. The files stored on this device were intentionally added for forensic imaging and validation purposes.
Show more lines
Evidence Preparation Screenshots

4. Evidence Acquisition Information
Item	InformationCase/Lab ID	CIP-B102-Lab4
Student Name	Idriss Muhammad Abdullahi
USB Brand	__________________
USB Capacity	__________________
Date Prepared	__________________
Acquisition Method	FTK Imager
Tool Version	__________________
Image Filename	CIPB102_Lab4_Idriss_Abdullahi_USB.dd
Image Storage Location	C:\CIP-B102-Lab4
Hash Algorithms	MD5 and SHA1
5. Acquisition Procedure
Step 1: Launch FTK Imager

FTK Imager was launched in administrator mode.

Screenshot 04

Step 2: Select Source Device

The USB device was selected as a Physical Drive.

The correct device was identified based on:

Capacity
Device description
Drive number

Screenshot 05

Step 3: Evidence Information

Evidence details were entered into FTK Imager.

Included:

Case Number
Evidence Number
Examiner Name
Description
Notes

Screenshot 06

Step 4: Configure Destination

The image destination was configured.

Image format selected:

Plain Text
1
Raw (dd)
Show more lines

Image filename:

Plain Text
1
CIPB102_Lab4_Idriss_Abdullahi_USB.dd
Show more lines

Screenshot 07

Step 5: Verification Configuration

The verification option was enabled to verify the image after creation.

Screenshot 08

Step 6: Image Acquisition

The acquisition process was started and allowed to complete successfully.

Screenshot 09

Screenshot 10

6. Hash Verification

After successful imaging, FTK Imager generated verification hashes.

Source Device Hashes

MD5:
computed Hashes: fe910286ef8406aab8374e9cf2b83055
reported Hashes: fe910286ef8406aab8374e9cf2b83055
Verified Results: MAtch
SHA1:
Computed HAshes: 1b5795173fbd769222f870ecfd5aa72a55035608
reported Hashes: 1b5795173fbd769222f870ecfd5aa72a55035608
verified results: Match

The generated hash values matched successfully, confirming that the acquired image is an exact forensic copy of the source USB device.

7. Validation of Forensic Image

The acquired .dd image was added back into FTK Imager as an evidence item.

Navigation path:

Plain Text
1
Image File
2
└── Partition
3
└── File System
4
└── CIP-B102-Lab4-Evidence
Show more lines

The file

Plain Text
1
firstname_lastname.txt
Show more lines

was successfully located and examined within the forensic image.

Contents matched the original source file.

Screenshot 12

Screenshot 13

Screenshot 14

8. Results

The forensic acquisition process was completed successfully.

Findings include:

USB device successfully identified.
Forensic image successfully created.
Verification completed without errors.
Hash values matched.
Evidence file located within image.
Evidence integrity maintained.
9. Reflection

This laboratory exercise provided practical experience in forensic imaging and evidence preservation. The use of FTK Imager demonstrated how storage devices can be acquired without altering the original evidence. Through hash verification, I learned how investigators confirm the authenticity and integrity of digital evidence. The exercise also reinforced the importance of maintaining proper documentation throughout the acquisition process. Overall, the practical enhanced my understanding of digital forensic procedures and evidence handling techniques.

10. Conclusion

The forensic acquisition of the USB device was completed successfully using FTK Imager. A Raw/DD forensic image was created and verified using cryptographic hash functions. The verification process confirmed that the forensic image accurately represented the original USB device. Validation further confirmed the presence of the expected evidence file within the image. Therefore, the acquisition process maintained evidence integrity and complied with accepted forensic best practices.
