# Read-PDFs-from-directory-using-Tika-and-Parser-libraries
Read PDFs from a directory or a path using Tika and Parser libraries
# install os
pip install os

# import parser from tika
from tika import parser

# import os
import os

#path of pdf files
path = r"/content/Test_Files"

# list to store the path files name
file_list=[] 

# read the files in path
file_list = os.listdir(path)

#print the name of each file in the path
print(file_list)

#for loop to read each file in the dir. path
for i in range(len(file_list)):
    
  # Message to tell the result of each file 
  print("The content of "+file_list[i])
  #Read each line in the pdf file
  raw = parser.from_file('''/content/Test_Files/'''+file_list[i])
  # Read content of each page in the file
  txt=raw['content']
  # print the content of pdf file
  print(txt)  
  # New line to begin a new iteration   
  print("")
  
  #Python code
  
    # install os
    pip install os

    # import parser from tika
    from tika import parser

    # import os
    import os

    #path of pdf files
    path = r"/content/Test_Files"

    # list to store the path files name
    file_list=[] 

    # read the files in path
    file_list = os.listdir(path)

    #print the name of each file in the path
    print(file_list)

    #for loop to read each file in the dir. path
    for i in range(len(file_list)):

      # Message to tell the result of each file 
      print("The content of "+file_list[i])
      #Read each line in the pdf file
      raw = parser.from_file('''/content/Test_Files/'''+file_list[i])
      # Read content of each page in the file
      txt=raw['content']
      # print the content of pdf file
      print(txt)  
      # New line to begin a new iteration   
      print("")
