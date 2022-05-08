# UpKnight 
🕵️ A File Integrity Monitoring (FIM) tooling to ensure consistency and trustworthiness of user data. If data is modified within a file, then an alert is raised for the security analyst to investigate the change. Tools used: Powershell

## How it works
A user is prompted to upload their text files, which are saved locally. The script will look into the folder, associate each file with a hash, and store them in a digitial footprint text file. The digitial footprint text file is where the script will constantly reference to see if anything has changed. The digitial footprint text file has filename path and its corresponding hash using SHA-256 encryption. Next, the script references the digitial footprint text file and stores the data into a dictionary. The key is the filename path and the value is the hash. The script will continously loops through each orginal target file and makes sure the hashes matches the hashes in the digitial footprint file. If there is a difference between the original target files and the digitial footprint file, then the program will display a notification alerting the user that a file has been changed!

![image](https://user-images.githubusercontent.com/56704620/167319061-9ab451fd-36b7-4c3d-8468-e37d5bef10f4.png)


## Inspiration
💫Learning to gain a better understanding of integrity, as part of the principles of the CIA Triad that is essential to any cybersecurity infrastructure. As well as Hashing Algorithms to encypt and secure senstive data when 

## Future Additions 
Ability for user to select the type of Hash they want to use
Integrate features from AWS, have the data be populated/updated
Enhance for code for more usuability

## Takeaways
Exposure to Powershell syntax, Data Structures
