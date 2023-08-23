# eT3-Technical-Challenge
**The challenge was solved using Python and Google Colab.**

### How to run:
1- Upload the data to Google Drive, making sure it's in the "My Drive" section and that it's in the same form that was sent with the challenge. <br>
2- Upload and run notebooks in Google Colab and make sure that the paths of the data files match those in the code. <br>
3- The CSV and JSON files generated will appear on Google Drive in the path specified in the code  <br>

## Problem one:
- The problem was solved by first creating a new folder in the same directory as the data and copying all the images to it.
- Then, the prefix assumed to be everything before the word milk, for example, "Arla-Ecological-Medium-Fat-Milk_001.jpg" was renamed to "Milk_001.jpg". However, this would mean that the image "Garant-Ecological-Medium-Fat-Milk_001.jpg" would also become "Milk_001.jpg", which is not only redundant but also isn't quite descriptive. Therefore, the prefix to be removed was eventually assumed to be only the brand name like "Garant" or "Arla".
- After removing the brand names from all image names, the images in the folder were all renamed.
- Then, the info of each image (the new name, the size in bytes, and the date it was last modified) was extracted from Google Drive and saved into a CSV file.
- Finally, the CSV file was saved to Google Drive in the path specified in the code.

## Problem two:
- The image txt file was imported from Google Drive.
- Then, a structure for the required JSON form was made using a dictionary.
- The txt file was split into lines and the data for the X, Y, width, and length values were extracted and appended to the dictionary.
- After all the data had been converted, the JSON data was saved in a new file on google drive in the directory specified in the code.
