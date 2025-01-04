![Image_1A](https://github.com/user-attachments/assets/0662984f-5a15-4410-ab1b-d0cbf220f8ed)
![Image_1B](https://github.com/user-attachments/assets/ab5b9cd7-1b99-4eb4-a91c-b2cb9e4bab54)
# Introduction
I have gotten into creating custom PCBs recently for a lot of my projects and I wanted to craft a small PCB with my information instead of a business card. I also wanted to incorporate an NFC tag to include my contact info as a quick way of sharing it with others. For these reasons, this project exists.
# EasyEDA
This project was created using EasyEDA, which is a PCB designing website. You can access it by going to: https://easyeda.com/

I highly recommend creating an account with Google, so it is easier to access later. After you have logged in, click on "Online Editor(Std Edition)." My current project looks like this:
![Image_2](https://github.com/user-attachments/assets/56d33924-dcb1-450c-96b9-7b57eb98293f)
When you open up the diagram, this is what you will see on my end:
![Image_3](https://github.com/user-attachments/assets/c1c175f7-895d-43a2-b9b8-416eb3fe3341)
Please note that, for some of these symbols, I went to user contributed symbols; to access these, go to Place then Symbol and search for the relevant symbol.

After I had created the circuit, I clicked on Design, then Convert Schematic to PCB. I moved around the components and clicked on Route and then Auto Route. I placed the NFC component on the back on purpose as well as the "Power" connection. The result is the following:
![Image_4](https://github.com/user-attachments/assets/fcf13c26-45eb-41a4-a2bf-af9358fd2908)
When I was ready to get my PCB created, I clicked on Fabrication then PCB Fabrication File (Gerber). You will get the following screen:
![Image_5](https://github.com/user-attachments/assets/84e913ee-8c45-444f-8f8b-cb427358a185)

Click on "Generate Gerber." This example is included in this project as well. You can then go to EasyEDA's partner website, https://jlcpcb.com/?href=easyeda-home, to order your PCB. Here, upload your .zip Gerber file and select additional customizations, like color. It usually ships within a few days and, hopefully, you will have your PCB in no time!

The next step is programming your NFC tag to include your specific details.
## NFC Tag
I have previously used these NFC tags for several projects, so I continue to rely on them.
![Image_4](https://github.com/user-attachments/assets/c1b4d1c5-4d13-4bfa-ba43-939e600c45c2)
The NFC tag is pretty simple to program using an Android phone and I’m sure you can use an iPhone as well.
# Initialization & Material(s)
Below you will find how I programmed the NFC tag and where it was purchased from.
## Initialization
I downloaded an app on the Play Store called NFC Tools; it is by wakdev. This app is incredibly useful and easy to use. When you first boot it up, this is what you’ll likely see:
![Image_5](https://github.com/user-attachments/assets/709e5967-18a4-4f82-8129-4af43c3fc6cd)
From here, tap your NFC tag; the following menu will appear.
![Image_6](https://github.com/user-attachments/assets/3fd644d4-7bb9-46e7-9eba-37c86f9be996)
Go to Write -> Add a record -> Contact. Enter your details.
![Image_7](https://github.com/user-attachments/assets/0435b498-c2f5-4c3b-ba01-dca678454fff)
The last thing left is the most critical: Make sure to press the “Write” button and then step away from your NFC tag and approach it again. Once it is completed, you should see this:
![Image_8](https://github.com/user-attachments/assets/204e200d-8ab7-4fe7-98e1-7b3b482a2dfd)
Now, the next time someone approaches this NFC, they will be prompted to add the contact.
## Material(s)
10pcs NFC Stickers Black NFC Tags NTAG215 NFC Sticker Tags 25MM Black NFC Stickers 504 Bytes Memory Programmable NFC Tags Compatible with Android iOS and NFC Enabled Phones Devices – this can be purchased for $7.96 at the following link:
https://www.amazon.com/Stickers-NTAG215-Programmable-Compatible-Android/dp/B091FCDPDR/ref=sxin_16_pa_sp_search_thematic_sspa?content-id=amzn1.sym.27b41115-b206-47c3-8621-713097e8442c%3Aamzn1.sym.27b41115-b206-47c3-8621-713097e8442c&crid=2CUK9W8I3L1WZ&cv_ct_cx=nfc%2Btags%2Bk%2Blakey&keywords=nfc%2Btags%2Bk%2Blakey&pd_rd_i=B091FCFJT9&pd_rd_r=1cfacf3c-cea7-49fc-9283-38dc8e35ebf4&pd_rd_w=3jGhz&pd_rd_wg=fOWr0&pf_rd_p=27b41115-b206-47c3-8621-713097e8442c&pf_rd_r=T2JE71K6VYQHEHNZ605T&qid=1735842929&sbo=RZvfv%2F%2FHxDF%2BO5021pAnSA%3D%3D&sprefix=nfc%2Btags%2Bk%2Blakey%2Caps%2C74&sr=1-1-6024b2a3-78e4-4fed-8fed-e1613be3bcce-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9zZWFyY2hfdGhlbWF0aWM&th=1
# Tips
You might want to get the surface-mounted components to fully complete this PCB, but it is not necessary. If you do, however, I recommend using a heat gun to help out with soldering the connections since it can be a bit tricky.

You may have an issue ensuring that your phone can read the NFC tag. I recommend, for at least Android and the process is likely similar for iOS, going to Settings -> Connected Devices -> Connection Preferences -> NFC (and turn this on).

People trying to read the NFC tag may also have issues if their phone has a thick case or if they are not tapping the correct part of the phone to the NFC tag. Removing the case and moving the phone around until it reads the tag helps with this, but this is easier for some than others.
